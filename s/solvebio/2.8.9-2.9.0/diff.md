# Comparing `tmp/solvebio-2.8.9.tar.gz` & `tmp/solvebio-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/solvebio-2.8.9.tar", last modified: Thu Sep 19 17:45:00 2019, max compression
+gzip compressed data, was "dist/solvebio-2.9.0.tar", last modified: Thu Nov  7 21:51:36 2019, max compression
```

## Comparing `solvebio-2.8.9.tar` & `solvebio-2.9.0.tar`

### file list

```diff
@@ -1,1957 +1,1957 @@
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3788 2019-09-19 17:45:00.000000 solvebio-2.8.9/PKG-INFO
--rw-rw-r--   0 davecap   (1000) davecap   (1000)     1100 2016-05-02 13:03:38.000000 solvebio-2.8.9/LICENSE
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2413 2019-03-25 17:11:43.000000 solvebio-2.8.9/README.md
--rw-rw-r--   0 davecap   (1000) davecap   (1000)       64 2016-05-02 13:03:38.000000 solvebio-2.8.9/AUTHORS
--rw-rw-r--   0 davecap   (1000) davecap   (1000)       79 2019-09-19 17:45:00.000000 solvebio-2.8.9/setup.cfg
--rw-r--r--   0 davecap   (1000) davecap   (1000)      260 2017-11-13 22:59:28.000000 solvebio-2.8.9/MANIFEST.in
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio.egg-info/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3788 2019-09-19 17:44:58.000000 solvebio-2.8.9/solvebio.egg-info/PKG-INFO
--rw-r--r--   0 davecap   (1000) davecap   (1000)       53 2019-09-19 17:44:58.000000 solvebio-2.8.9/solvebio.egg-info/entry_points.txt
--rw-r--r--   0 davecap   (1000) davecap   (1000)        1 2019-09-19 17:44:58.000000 solvebio-2.8.9/solvebio.egg-info/dependency_links.txt
--rw-r--r--   0 davecap   (1000) davecap   (1000)        9 2019-09-19 17:44:58.000000 solvebio-2.8.9/solvebio.egg-info/top_level.txt
--rw-r--r--   0 davecap   (1000) davecap   (1000)       28 2019-09-19 17:44:58.000000 solvebio-2.8.9/solvebio.egg-info/requires.txt
--rw-r--r--   0 davecap   (1000) davecap   (1000)    72709 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio.egg-info/SOURCES.txt
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2086 2018-10-29 16:51:26.000000 solvebio-2.8.9/setup.py
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2822 2018-09-07 17:09:45.000000 solvebio-2.8.9/solvebio/annotate.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)      200 2019-09-19 17:43:06.000000 solvebio-2.8.9/solvebio/version.py
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/utils/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      372 2018-02-01 19:54:40.000000 solvebio-2.8.9/solvebio/utils/files.py
--rw-rw-r--   0 davecap   (1000) davecap   (1000)     2718 2016-05-02 13:03:38.000000 solvebio-2.8.9/solvebio/utils/humanize.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1140 2016-05-30 18:03:16.000000 solvebio-2.8.9/solvebio/utils/md5sum.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)      665 2019-03-25 17:11:43.000000 solvebio-2.8.9/solvebio/utils/validators.py
--rw-rw-r--   0 davecap   (1000) davecap   (1000)     3111 2016-05-02 13:03:38.000000 solvebio-2.8.9/solvebio/utils/printing.py
--rw-rw-r--   0 davecap   (1000) davecap   (1000)        0 2016-05-02 13:03:38.000000 solvebio-2.8.9/solvebio/utils/__init__.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    20738 2017-07-28 21:05:17.000000 solvebio-2.8.9/solvebio/utils/tabulate.py
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/test/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7021 2018-04-25 13:53:54.000000 solvebio-2.8.9/solvebio/test/test_filter.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6720 2018-09-11 16:02:27.000000 solvebio-2.8.9/solvebio/test/test_shortcuts.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2093 2017-11-22 14:20:14.000000 solvebio-2.8.9/solvebio/test/test_dataset_migrations.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6883 2018-04-25 13:53:54.000000 solvebio-2.8.9/solvebio/test/test_dataset.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1435 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/test/helper.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1415 2017-10-03 20:58:42.000000 solvebio-2.8.9/solvebio/test/test_ratelimit.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1221 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/test/test_beacon.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2794 2018-02-01 19:54:40.000000 solvebio-2.8.9/solvebio/test/test_vault.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)      611 2018-07-13 17:43:13.000000 solvebio-2.8.9/solvebio/test/test_apiresource.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4513 2017-07-28 21:05:17.000000 solvebio-2.8.9/solvebio/test/test_tabulate.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1334 2018-09-07 17:09:44.000000 solvebio-2.8.9/solvebio/test/test_exports.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1883 2016-09-23 18:26:15.000000 solvebio-2.8.9/solvebio/test/test_vcfparser.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2608 2018-09-11 16:02:27.000000 solvebio-2.8.9/solvebio/test/test_credentials.py
--rw-rw-r--   0 davecap   (1000) davecap   (1000)      437 2016-05-02 13:03:38.000000 solvebio-2.8.9/solvebio/test/test_conversion.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)      744 2016-12-13 15:48:47.000000 solvebio-2.8.9/solvebio/test/test_utils.py
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/test/data/
--rw-rw-r--   0 davecap   (1000) davecap   (1000)      104 2016-05-02 13:03:38.000000 solvebio-2.8.9/solvebio/test/data/test_creds
--rw-r--r--   0 davecap   (1000) davecap   (1000)      462 2017-04-18 13:10:06.000000 solvebio-2.8.9/solvebio/test/data/template.json
--rw-r--r--   0 davecap   (1000) davecap   (1000)      590 2016-08-25 19:19:42.000000 solvebio-2.8.9/solvebio/test/data/sample.vcf.gz
--rw-rw-r--   0 davecap   (1000) davecap   (1000)      243 2016-05-02 13:03:38.000000 solvebio-2.8.9/solvebio/test/data/sample2.vcf
--rw-r--r--   0 davecap   (1000) davecap   (1000)       18 2017-06-15 15:20:01.000000 solvebio-2.8.9/solvebio/test/data/test_export.csv
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5321 2016-12-12 15:08:56.000000 solvebio-2.8.9/solvebio/test/data/test_export.xlsx
--rw-r--r--   0 davecap   (1000) davecap   (1000)       62 2016-12-13 15:48:47.000000 solvebio-2.8.9/solvebio/test/data/some_export.json.gz
--rw-r--r--   0 davecap   (1000) davecap   (1000)       25 2016-12-12 15:08:56.000000 solvebio-2.8.9/solvebio/test/data/test_export.json
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1194 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/test/test_query_batch.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4898 2018-02-23 20:39:13.000000 solvebio-2.8.9/solvebio/test/client_mocks.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1725 2018-09-11 16:02:27.000000 solvebio-2.8.9/solvebio/test/test_login.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)      861 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/test/test_annotate.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)      936 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/test/test_client.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4387 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/test/test_lookup.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9995 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/test/test_query.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)        0 2018-09-11 16:02:27.000000 solvebio-2.8.9/solvebio/test/__init__.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3708 2018-02-01 19:54:40.000000 solvebio-2.8.9/solvebio/test/test_object.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9250 2019-09-19 16:04:54.000000 solvebio-2.8.9/solvebio/client.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)      442 2019-03-25 17:11:43.000000 solvebio-2.8.9/solvebio/help.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    26199 2019-09-19 16:04:54.000000 solvebio-2.8.9/solvebio/query.py
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/resource/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1462 2019-09-19 16:04:54.000000 solvebio-2.8.9/solvebio/resource/savedquery.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2306 2018-07-13 17:43:13.000000 solvebio-2.8.9/solvebio/resource/group.py
--rw-rw-r--   0 davecap   (1000) davecap   (1000)      596 2016-05-02 13:03:38.000000 solvebio-2.8.9/solvebio/resource/util.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1214 2017-11-22 14:20:14.000000 solvebio-2.8.9/solvebio/resource/beacon.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1331 2019-09-19 16:04:54.000000 solvebio-2.8.9/solvebio/resource/vault_sync_task.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1503 2019-09-19 16:04:54.000000 solvebio-2.8.9/solvebio/resource/object_copy_task.py
--rw-rw-r--   0 davecap   (1000) davecap   (1000)      115 2016-05-02 13:03:38.000000 solvebio-2.8.9/solvebio/resource/user.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2980 2019-09-19 16:04:54.000000 solvebio-2.8.9/solvebio/resource/datasetcommit.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2543 2019-03-25 17:11:43.000000 solvebio-2.8.9/solvebio/resource/manifest.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)      581 2017-11-22 14:20:14.000000 solvebio-2.8.9/solvebio/resource/datasettemplate.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)      689 2018-02-01 19:54:40.000000 solvebio-2.8.9/solvebio/resource/application.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)      876 2017-11-22 14:20:14.000000 solvebio-2.8.9/solvebio/resource/datasetfield.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2106 2017-11-22 14:20:14.000000 solvebio-2.8.9/solvebio/resource/datasetexport.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3113 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/resource/solveobject.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1424 2017-11-22 14:20:14.000000 solvebio-2.8.9/solvebio/resource/beaconset.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2811 2019-09-19 16:04:54.000000 solvebio-2.8.9/solvebio/resource/datasetmigration.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2948 2019-09-19 16:04:54.000000 solvebio-2.8.9/solvebio/resource/datasetimport.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1273 2019-09-19 16:04:54.000000 solvebio-2.8.9/solvebio/resource/task.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    12877 2019-09-19 17:43:06.000000 solvebio-2.8.9/solvebio/resource/dataset.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1332 2018-07-13 17:43:13.000000 solvebio-2.8.9/solvebio/resource/__init__.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7796 2018-07-10 20:05:39.000000 solvebio-2.8.9/solvebio/resource/vault.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10597 2018-07-13 17:43:13.000000 solvebio-2.8.9/solvebio/resource/apiresource.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9324 2019-03-05 20:23:42.000000 solvebio-2.8.9/solvebio/resource/object.py
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      249 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/contrib/dash/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2032 2018-02-01 18:13:16.000000 solvebio-2.8.9/solvebio/contrib/dash/usage.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)  1285869 2018-05-14 19:28:44.000000 solvebio-2.8.9/solvebio/contrib/dash/oauth-redirect.js
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      116 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asap/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10089 2016-01-04 02:27:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asap/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2697 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asap/CHANGES.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1083 2016-01-04 02:27:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asap/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-rsa/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      383 2016-02-25 22:57:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-rsa/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hoek/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    17309 2015-09-16 18:29:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hoek/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      105 2015-09-11 16:17:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hoek/CONTRIBUTING.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asn1/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1201 2014-06-05 15:13:40.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asn1/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-decorators/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1173 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-decorators/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shelljs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    21587 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shelljs/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    60297 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shelljs/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/abbrev/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      499 2010-10-04 18:52:26.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/abbrev/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/npmlog/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5983 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/npmlog/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1415 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/npmlog/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9813 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    13405 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2878 2013-01-24 02:15:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/graphviz.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4756 2013-01-24 02:15:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/pretty_gyp.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     5099 2015-07-10 13:00:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/pretty_sln.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     9586 2013-01-24 02:15:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/pretty_vcproj.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     8019 2015-07-10 13:00:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/gyptest.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)      447 2015-11-15 03:49:58.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/gyp_main.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3662 2015-11-15 03:49:58.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/PRESUBMIT.py
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1970 2013-11-26 08:32:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/common_test.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)   116086 2017-01-10 01:30:41.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/input.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)    23354 2015-11-15 03:49:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/mac_tool.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3270 2013-01-24 02:15:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/easy_xml_test.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    20063 2016-02-12 02:50:43.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/common.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10366 2014-02-24 15:39:19.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/ordered_dict.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    65086 2016-02-12 02:50:43.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xcode_emulation.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)    65937 2015-11-15 03:49:58.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings_test.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)    12751 2015-11-15 03:49:58.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/win_tool.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3207 2015-07-10 13:00:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/input_test.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4945 2015-07-10 13:00:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/easy_xml.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1804 2013-01-24 02:15:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSToolFile.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1247 2015-07-10 13:00:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/simple_copy.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    45045 2015-11-15 03:49:58.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)   120842 2016-02-12 02:50:43.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xcodeproj_file.py
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/
--rw-r--r--   0 davecap   (1000) davecap   (1000)   132681 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    45344 2016-06-15 10:31:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/android.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)      645 2013-11-26 08:32:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode_test.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    30567 2016-02-12 02:50:43.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/analyzer.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)   100329 2016-02-12 02:50:43.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    91092 2016-06-15 10:31:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1018 2013-01-24 02:15:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs_test.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    44604 2016-02-12 02:50:43.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/cmake.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    58344 2016-02-12 02:50:43.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    17014 2015-07-10 13:00:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/eclipse.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1665 2013-01-24 02:15:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/gypsh.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1786 2015-07-10 13:00:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja_test.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3426 2015-11-15 03:49:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/dump_dependency_json.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3474 2015-07-10 13:00:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/gypd.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)        0 2013-01-24 02:15:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/__init__.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5536 2013-11-26 08:32:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/ninja_syntax.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    12124 2015-07-10 13:00:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSNew.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1748 2015-07-10 13:00:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/flock_tool.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9537 2015-07-10 13:00:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSUtil.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10585 2015-07-10 13:00:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xcode_ninja.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2174 2013-01-24 02:15:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xml_fix.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    17165 2015-11-15 03:49:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSVersion.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6387 2013-01-24 02:15:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSProject.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5094 2013-01-24 02:15:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSUserFile.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)    22178 2015-11-15 03:49:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/__init__.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    47697 2015-11-15 03:49:58.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/msvs_emulation.py
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)      536 2013-11-26 08:32:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/setup.py
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/buildbot/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4228 2015-11-15 03:49:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/buildbot/buildbot_run.py
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/console-control-strings/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4475 2016-06-15 23:28:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/console-control-strings/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    16567 2016-12-06 15:47:48.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/faye-websocket/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    12372 2015-07-08 19:28:20.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/faye-websocket/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2893 2015-07-08 20:09:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/faye-websocket/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compressible/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1865 2017-03-24 04:39:24.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compressible/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1193 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compressible/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/async-foreach/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4977 2013-04-29 12:54:57.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/async-foreach/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx-self/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      683 2016-12-08 15:43:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx-self/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-deceiver/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1363 2015-11-16 22:23:56.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-deceiver/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/parse-asn1/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      421 2016-11-28 20:06:19.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/parse-asn1/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-sticky-regex/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      529 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-sticky-regex/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-svg/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      828 2016-11-04 14:28:29.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-svg/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regenerate/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    12583 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regenerate/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esrecurse/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esrecurse/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esrecurse/node_modules/estraverse/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4161 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esrecurse/node_modules/estraverse/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/base64-js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1005 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/base64-js/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mixin-object/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2824 2015-07-05 05:54:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mixin-object/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mixin-object/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mixin-object/node_modules/for-in/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3112 2016-03-27 14:56:29.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mixin-object/node_modules/for-in/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/for-own/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3465 2016-03-27 15:06:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/for-own/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-shorthand-properties/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      807 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-shorthand-properties/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/alphanum-sort/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      808 2015-10-03 19:46:39.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/alphanum-sort/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-builtin-module/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      625 2015-05-04 15:46:42.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-builtin-module/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cookie-signature/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1490 2014-06-19 01:26:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cookie-signature/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      695 2015-02-03 22:10:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cookie-signature/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cookie/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8208 2016-05-27 04:01:25.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cookie/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2626 2016-05-27 04:21:40.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cookie/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/indent-string/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      988 2015-07-25 19:15:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/indent-string/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babylon/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5894 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babylon/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    32311 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babylon/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tough-cookie/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    26050 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tough-cookie/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/coa/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    22636 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/coa/README.ru.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    12006 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/coa/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cssesc/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6289 2013-08-09 13:21:42.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cssesc/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hosted-git-info/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4070 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hosted-git-info/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/user-home/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      724 2015-06-13 12:36:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/user-home/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-callable/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1978 2015-08-12 19:17:54.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-callable/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1815 2016-02-28 00:49:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-callable/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shallow-clone/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2592 2015-10-17 17:57:53.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shallow-clone/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/kind-of/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6177 2015-05-31 20:29:42.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/kind-of/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/lazy-cache/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2944 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/lazy-cache/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/combined-stream/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4551 2015-06-14 15:08:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/combined-stream/Readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/right-align/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2066 2015-06-09 05:57:37.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/right-align/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/string-width/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1156 2016-08-13 20:30:48.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/string-width/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-async-to-generator/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      837 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-async-to-generator/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-date-object/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1751 2015-08-12 05:57:54.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-date-object/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      421 2015-09-27 13:14:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-date-object/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/elliptic/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6593 2017-02-06 23:08:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/elliptic/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-remap-async-to-generator/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       56 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-remap-async-to-generator/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/watchpack/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3092 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/watchpack/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/timers-browserify/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1197 2015-02-23 16:03:54.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/timers-browserify/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2039 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/timers-browserify/CHANGELOG.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2505 2012-05-26 02:27:10.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/timers-browserify/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/finalhandler/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3968 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/finalhandler/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3317 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/finalhandler/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/assert/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2307 2016-05-06 19:07:33.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/assert/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/source-list-map/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2437 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/source-list-map/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/camelcase-keys/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/camelcase-keys/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/camelcase-keys/node_modules/camelcase/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1045 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/camelcase-keys/node_modules/camelcase/readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      847 2016-03-15 14:20:09.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/camelcase-keys/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/natural-compare/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3352 2016-07-22 20:48:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/natural-compare/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/url/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3604 2015-08-27 15:36:24.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/url/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/url/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/url/node_modules/punycode/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5988 2014-08-31 16:09:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/url/node_modules/punycode/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-spread/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      654 2016-12-08 15:43:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-spread/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/buffer/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    16577 2016-08-09 00:59:55.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/buffer/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1529 2016-08-18 03:46:30.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/buffer/AUTHORS.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prop-types/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5268 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prop-types/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    16921 2017-03-02 23:05:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/is-extglob/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3469 2016-09-03 19:12:15.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/is-extglob/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/is-glob/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5219 2016-09-03 19:14:26.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/is-glob/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5358 2017-03-02 23:02:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json-loader/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      379 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json-loader/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/read-pkg-up/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1710 2015-09-03 05:22:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/read-pkg-up/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-types/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    40446 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-types/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-export-extensions/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      474 2016-03-21 23:00:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-export-extensions/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-calc/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3201 2016-07-11 04:52:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-calc/README.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2183 2016-08-22 08:58:37.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-calc/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pluralize/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2228 2015-09-17 03:34:01.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pluralize/Readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-call-delegate/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       45 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-call-delegate/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/builtin-status-codes/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      610 2015-11-17 22:20:35.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/builtin-status-codes/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ripemd160/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1894 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ripemd160/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      897 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ripemd160/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/camelcase/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1045 2015-11-12 18:54:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/camelcase/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-messages/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      272 2017-01-20 05:35:55.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-messages/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-get-function-arity/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       50 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-get-function-arity/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/find-cache-dir/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2827 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/find-cache-dir/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/which-module/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1933 2016-06-06 05:50:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/which-module/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      331 2016-06-06 05:53:30.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/which-module/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/enhanced-resolve/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3168 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/enhanced-resolve/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/set-blocking/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1538 2016-05-17 22:57:19.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/set-blocking/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      718 2016-05-17 22:58:30.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/set-blocking/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack-dev-middleware/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6697 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack-dev-middleware/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/merge-descriptors/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1213 2015-05-22 03:38:01.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/merge-descriptors/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      363 2016-01-17 23:41:34.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/merge-descriptors/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esutils/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6655 2015-03-11 15:11:56.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esutils/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-commonjs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2741 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-commonjs/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fstream/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2345 2015-09-09 23:40:40.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fstream/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-reduce-idents/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5078 2017-01-04 18:09:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-reduce-idents/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      943 2017-01-04 18:11:15.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-reduce-idents/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-primitive/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1055 2015-03-17 03:56:35.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-primitive/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-regenerator/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1239 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-regenerator/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/stdout-stream/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1009 2015-06-23 06:32:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/stdout-stream/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/react/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      849 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/react/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-equal-shallow/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2775 2015-06-23 03:39:48.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-equal-shallow/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/extsprintf/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1169 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/extsprintf/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/emojis-list/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1893 2016-10-03 14:00:23.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/emojis-list/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3027 2016-10-03 14:00:58.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/emojis-list/CHANGELOG.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1084 2015-04-19 20:40:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/emojis-list/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-react/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1241 2017-04-01 14:50:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-react/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-svgo/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5298 2016-12-17 15:02:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-svgo/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1246 2016-12-17 15:15:25.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-svgo/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ms/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1832 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ms/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1077 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ms/LICENSE.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1721 2017-05-16 12:24:53.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ms/readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1077 2017-05-16 12:22:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ms/license.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-duplicates/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3281 2017-02-26 19:18:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-duplicates/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1492 2017-02-26 19:17:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-duplicates/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-type/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      728 2015-09-04 08:27:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-type/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/to-arraybuffer/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      940 2016-01-13 04:01:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/to-arraybuffer/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pinkie-promise/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      751 2016-04-10 17:37:01.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pinkie-promise/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-code-frame/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1204 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-code-frame/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-colormin/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1363 2016-03-01 21:02:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-colormin/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2416 2017-02-06 17:36:39.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-colormin/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7504 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5646 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/node_modules/ms/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      933 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/node_modules/ms/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1307 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/node_modules/ms/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/node_modules/debug/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6310 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/node_modules/debug/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5611 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/node_modules/debug/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fastparse/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3265 2015-05-24 18:14:54.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fastparse/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/parse-json/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1273 2015-08-31 16:21:26.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/parse-json/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-plain-obj/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      631 2015-07-11 11:06:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-plain-obj/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/on-headers/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1929 2015-02-15 19:58:54.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/on-headers/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      296 2015-09-30 03:43:50.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/on-headers/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cli-width/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1814 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cli-width/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fbjs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2903 2017-03-29 23:45:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fbjs/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fbjs/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fbjs/node_modules/core-js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    22838 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fbjs/node_modules/core-js/CHANGELOG.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4577 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fbjs/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-define-map/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       42 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-define-map/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2897 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1443 2017-03-10 13:04:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/CONTRIBUTING.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/doc/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/doc/wg-meetings/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2280 2016-09-29 06:59:25.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/doc/wg-meetings/2015-01-30.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/node_modules/string_decoder/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1113 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/node_modules/string_decoder/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5550 2017-03-10 13:04:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/GOVERNANCE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/querystring/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1081 2012-10-23 20:34:36.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/querystring/License.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      331 2013-03-05 21:31:48.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/querystring/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      357 2013-03-05 21:32:31.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/querystring/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.memoize/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      460 2016-08-13 17:33:14.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.memoize/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/supports-color/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1491 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/supports-color/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/del/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2422 2016-08-13 00:03:37.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/del/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ua-parser-js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10381 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ua-parser-js/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-libs-browser/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4015 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-libs-browser/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/aws4/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    16755 2016-10-11 22:34:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/aws4/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-dynamic-import/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      452 2016-10-24 19:15:50.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-dynamic-import/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/har-schema/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2117 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/har-schema/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/randombytes/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      575 2016-01-13 13:14:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/randombytes/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uniq/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1221 2013-03-31 02:52:01.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uniq/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esquery/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2048 2017-03-10 23:08:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esquery/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-reduce-transforms/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1269 2015-10-05 19:19:01.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-reduce-transforms/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      373 2016-11-01 14:47:14.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-reduce-transforms/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdx-license-ids/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1598 2015-08-17 06:36:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdx-license-ids/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/trim-newlines/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      953 2015-09-29 09:22:47.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/trim-newlines/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/reduce-css-calc/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1531 2016-02-22 06:29:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/reduce-css-calc/README.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2389 2016-08-26 11:03:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/reduce-css-calc/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pinkie/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2691 2016-02-01 10:28:24.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pinkie/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nopt/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7690 2015-11-12 21:18:50.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nopt/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/icss-replace-symbols/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      988 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/icss-replace-symbols/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sshpk/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    21169 2017-04-13 01:18:41.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sshpk/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/wide-align/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1551 2015-12-16 05:57:07.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/wide-align/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/stream-http/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6509 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/stream-http/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/aws-sign2/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      130 2013-04-22 05:13:39.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/aws-sign2/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-loader/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    13163 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-loader/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-loader/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-loader/node_modules/css-selector-tokenizer/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2405 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-loader/node_modules/css-selector-tokenizer/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1641 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-loader/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/run-async/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1266 2014-08-11 01:10:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/run-async/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ansi-styles/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1448 2016-03-28 20:32:20.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ansi-styles/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-signature/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    13849 2016-01-25 22:01:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-signature/http_signing.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1594 2015-10-14 21:20:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-signature/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1350 2016-01-25 22:03:07.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-signature/CHANGES.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-signature/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-signature/node_modules/assert-plus/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4618 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-signature/node_modules/assert-plus/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      219 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-signature/node_modules/assert-plus/CHANGES.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/util-deprecate/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1666 2014-11-25 20:05:41.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/util-deprecate/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      282 2015-10-07 18:37:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/util-deprecate/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/write/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2851 2015-07-29 19:13:56.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/write/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/safe-buffer/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    19324 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/safe-buffer/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack-dev-server/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2681 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack-dev-server/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-to-regexp/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1102 2015-07-28 02:27:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-to-regexp/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      694 2015-07-28 03:06:47.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-to-regexp/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fill-range/
--rwxr--r--   0 davecap   (1000) davecap   (1000)     6701 2015-04-07 08:50:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fill-range/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fill-range/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fill-range/node_modules/isobject/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2999 2016-04-25 21:03:56.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fill-range/node_modules/isobject/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/qs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    13292 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/qs/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10370 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/qs/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/clap/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      662 2015-08-30 19:25:57.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/clap/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      491 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/clap/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color-convert/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2853 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color-convert/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1417 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color-convert/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/normalize-url/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3344 2017-01-09 17:47:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/normalize-url/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-extglob/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1912 2015-03-06 21:00:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-extglob/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-gradients/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3091 2016-10-19 14:08:11.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-gradients/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      524 2016-11-01 00:02:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-gradients/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cssnano/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2449 2016-11-25 21:24:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cssnano/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    11849 2017-01-03 22:22:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cssnano/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)      920 2017-02-28 21:46:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/node_modules/acorn/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    16810 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/node_modules/acorn/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6233 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/node_modules/acorn/CHANGELOG.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      233 2017-02-28 21:46:54.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/rechoir/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2018 2015-07-22 12:11:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/rechoir/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/convert-source-map/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4419 2017-03-28 09:07:55.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/convert-source-map/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/opn/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2224 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/opn/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/crypto-browserify/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1604 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/crypto-browserify/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strip-ansi/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      801 2016-02-21 12:14:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strip-ansi/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/co/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5382 2015-07-09 22:27:26.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/co/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3629 2015-07-09 22:29:39.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/co/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/brace-expansion/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3657 2017-04-07 08:13:12.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/brace-expansion/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/range-parser/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1996 2016-06-01 16:06:29.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/range-parser/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      832 2016-06-01 16:47:14.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/range-parser/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-typedarray/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      558 2014-06-01 19:09:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-typedarray/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1073 2014-06-01 19:08:03.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-typedarray/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/domain-browser/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7869 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/domain-browser/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1381 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/domain-browser/HISTORY.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1348 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/domain-browser/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-map/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2238 2017-01-13 10:33:18.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-map/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/source-map/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    23480 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/source-map/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7884 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/source-map/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/query-string/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4955 2017-04-17 05:51:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/query-string/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hpack.js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1860 2016-03-24 16:14:30.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hpack.js/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-decorators/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      432 2016-03-21 23:00:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-decorators/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/center-align/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1950 2015-10-27 09:26:20.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/center-align/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/builtin-modules/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      957 2015-09-01 17:27:52.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/builtin-modules/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-replace-supers/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       46 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-replace-supers/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/braces/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6629 2016-05-21 15:12:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/braces/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/table/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    15847 2016-09-17 20:02:56.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/table/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/table/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/table/node_modules/string-width/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1156 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/table/node_modules/string-width/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/table/node_modules/is-fullwidth-code-point/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      836 2016-09-22 06:35:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/table/node_modules/is-fullwidth-code-point/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-font-values/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1748 2016-02-08 01:16:37.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-font-values/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-jsx/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      369 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-jsx/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-flatten/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1245 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-flatten/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserslist/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8921 2017-03-03 09:54:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserslist/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3169 2017-03-21 08:08:33.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserslist/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object.omit/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4646 2016-10-27 06:23:10.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object.omit/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-flow/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      675 2017-02-13 02:45:24.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-flow/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loose-envify/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1071 2016-05-15 03:29:30.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loose-envify/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/minimalistic-crypto-utils/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1882 2017-02-22 21:12:33.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/minimalistic-crypto-utils/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/batch/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1822 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/batch/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1271 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/batch/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-reduce-initial/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2722 2016-12-22 16:40:07.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-reduce-initial/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      105 2016-12-22 16:40:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-reduce-initial/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-hoist-variables/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       47 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-hoist-variables/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/delegates/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1768 2015-12-14 19:55:23.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/delegates/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      336 2015-12-14 19:55:48.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/delegates/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-empty/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1149 2015-08-13 11:22:07.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-empty/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      427 2016-04-26 15:55:50.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-empty/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-convert-values/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5380 2017-02-03 18:57:50.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-convert-values/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3319 2017-02-03 19:01:26.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-convert-values/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/create-ecdh/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      669 2015-10-29 12:49:13.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/create-ecdh/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-overridden/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2603 2016-04-27 03:21:30.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-overridden/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)        0 2016-04-26 10:57:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-overridden/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-traverse/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       17 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-traverse/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/glob-parent/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1518 2015-09-18 14:58:10.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/glob-parent/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/events/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      371 2016-06-22 15:53:40.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/events/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      760 2016-06-22 16:09:10.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/events/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs-client/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    15712 2017-01-22 19:46:46.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs-client/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8717 2017-01-23 23:43:09.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs-client/Changelog.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/faye-websocket/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    12576 2017-01-22 19:44:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/faye-websocket/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      162 2015-11-08 12:15:20.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/faye-websocket/CODE_OF_CONDUCT.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3140 2017-01-22 19:45:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/faye-websocket/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-optimise-call-expression/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       56 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-optimise-call-expression/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-computed-properties/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1816 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-computed-properties/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mime/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2119 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mime/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/reduce-function-call/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1651 2016-11-28 07:19:41.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/reduce-function-call/README.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)      265 2016-11-28 07:22:17.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/reduce-function-call/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/evp_bytestokey/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1770 2017-09-05 10:20:26.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/evp_bytestokey/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      383 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/evp_bytestokey/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-des/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       39 2015-09-27 17:30:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-des/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/minimatch/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6336 2016-02-20 22:10:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/minimatch/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-es2015/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      865 2017-04-01 14:50:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-es2015/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-jsx/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2751 2016-05-02 16:02:15.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-jsx/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-jsx/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-jsx/node_modules/acorn/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    16680 2016-06-07 11:28:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-jsx/node_modules/acorn/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3444 2016-07-25 21:22:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-jsx/node_modules/acorn/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-aes/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      802 2017-10-10 12:30:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-aes/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      780 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-aes/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-path-in-cwd/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      523 2014-06-20 22:20:41.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-path-in-cwd/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/preserve/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1335 2015-01-10 12:25:52.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/preserve/.verb.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2230 2015-01-10 22:21:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/preserve/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-for-of/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2406 2017-01-20 05:35:55.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-for-of/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-block-scoped-functions/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      604 2016-12-08 15:43:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-block-scoped-functions/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/repeat-string/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5057 2016-10-23 08:00:31.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/repeat-string/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-plain-object/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2598 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-plain-object/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.uniq/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      439 2016-08-13 17:34:12.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.uniq/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-stream/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      664 2016-04-12 07:19:14.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-stream/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caller-path/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      726 2014-04-19 10:18:24.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caller-path/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pako/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5340 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pako/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1537 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pako/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color-name/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      384 2017-03-14 02:54:03.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color-name/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-property/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      625 2013-07-18 14:04:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-property/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/binary-extensions/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      759 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/binary-extensions/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/parseurl/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3463 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/parseurl/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      832 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/parseurl/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-unused/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4345 2016-11-21 17:51:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-unused/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      809 2016-11-21 17:51:07.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-unused/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/destroy/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2185 2016-01-13 16:29:37.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/destroy/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/unpipe/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1250 2015-06-14 20:29:42.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/unpipe/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)       59 2015-06-14 20:29:42.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/unpipe/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/indexes-of/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      320 2013-11-16 09:01:14.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/indexes-of/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/negotiator/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4811 2016-05-03 04:32:15.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/negotiator/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2296 2016-05-03 04:43:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/negotiator/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/to-fast-properties/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      733 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/to-fast-properties/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-regex/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1624 2017-01-10 22:24:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-regex/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1109 2017-02-18 08:12:31.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-regex/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readline2/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1541 2015-07-17 06:53:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readline2/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/decamelize/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      781 2016-03-05 08:48:07.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/decamelize/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hash.js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1255 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hash.js/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/async-each/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1122 2016-08-24 23:21:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/async-each/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      593 2016-08-24 23:17:25.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/async-each/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1054 2016-08-06 16:40:01.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    12535 2017-02-23 18:05:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/API.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4632 2017-02-23 18:21:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-params/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      663 2016-09-30 16:51:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-params/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      580 2016-12-28 10:45:12.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-params/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/vendors/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      964 2016-08-11 10:41:50.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/vendors/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/errno/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4415 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/errno/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/core-util-is/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       67 2015-11-20 00:23:19.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/core-util-is/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ajv/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    65968 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ajv/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ajv/lib/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ajv/lib/dotjs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      149 2017-04-06 18:04:40.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ajv/lib/dotjs/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ee-first/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2617 2015-05-25 18:17:03.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ee-first/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdy-transport/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2246 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdy-transport/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/yargs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    53446 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/yargs/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    63371 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/yargs/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/slice-ansi/
--rwxr--r--   0 davecap   (1000) davecap   (1000)     1176 2015-09-26 07:54:33.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/slice-ansi/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint-plugin-react/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)    12746 2017-03-19 16:25:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint-plugin-react/README.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)    77312 2017-03-20 21:46:54.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint-plugin-react/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fast-levenshtein/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3414 2016-09-07 04:51:17.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fast-levenshtein/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1100 2014-12-06 02:56:29.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fast-levenshtein/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/optionator/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    14932 2016-09-21 19:42:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/optionator/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1771 2016-09-21 19:42:25.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/optionator/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/wbuf/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1127 2016-05-04 20:27:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/wbuf/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isstream/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2424 2015-03-07 00:14:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isstream/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1125 2015-03-07 00:14:31.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isstream/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/error-ex/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4143 2016-11-24 18:33:26.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/error-ex/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/util/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      409 2013-11-22 18:19:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/util/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/util/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/util/node_modules/inherits/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1625 2013-05-16 14:24:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/util/node_modules/inherits/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/micromatch/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    19913 2016-07-15 17:13:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/micromatch/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-path-cwd/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      474 2014-06-19 10:18:10.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-path-cwd/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-object-rest-spread/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1441 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-object-rest-spread/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esprima/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2333 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esprima/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/balanced-match/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3308 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/balanced-match/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1096 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/balanced-match/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-stage-0/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      391 2017-04-01 14:50:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-stage-0/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/y18n/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2365 2016-03-17 05:01:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/y18n/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/style-loader/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6258 2017-03-22 13:43:50.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/style-loader/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2519 2017-03-28 13:28:42.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/style-loader/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/style-loader/.github/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      716 2017-02-24 16:02:11.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/style-loader/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      733 2017-02-24 16:02:11.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/style-loader/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/constants-browserify/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1668 2015-07-13 18:14:07.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/constants-browserify/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/get-stdin/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      571 2014-08-17 19:16:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/get-stdin/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-classes/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1778 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-classes/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3523 2016-03-28 18:13:37.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/graceful-fs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4454 2016-09-26 21:37:48.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/graceful-fs/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-glob/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3218 2015-10-02 04:34:15.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-glob/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-filter-plugins/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3821 2016-07-12 14:03:47.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-filter-plugins/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      296 2016-10-03 16:27:35.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-filter-plugins/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/html-entities/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2364 2017-04-24 11:44:25.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/html-entities/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/encodeurl/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3613 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/encodeurl/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      159 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/encodeurl/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/imurmurhash/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4763 2013-08-11 11:48:48.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/imurmurhash/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-async-generators/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      477 2016-03-21 23:00:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-async-generators/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/portfinder/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1333 2017-01-31 14:42:41.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/portfinder/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/portfinder/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/portfinder/node_modules/async/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    60782 2016-01-07 23:18:07.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/portfinder/node_modules/async/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5398 2016-01-08 00:03:29.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/portfinder/node_modules/async/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ramda/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6695 2017-06-02 04:46:26.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ramda/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      117 2017-05-05 18:02:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ramda/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/rx-lite/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8938 2015-08-14 19:47:34.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/rx-lite/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hawk/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)    31409 2016-01-21 18:20:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hawk/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/promise/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9295 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/promise/Readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ecc-jsbn/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      402 2014-08-24 04:10:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ecc-jsbn/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-value-parser/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7650 2016-02-18 17:35:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-value-parser/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/autoprefixer/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    17201 2017-03-11 11:27:20.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/autoprefixer/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    21804 2017-03-11 11:27:20.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/autoprefixer/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/escape-html/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      707 2015-09-01 04:46:01.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/escape-html/Readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    14669 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/docs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3188 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/docs/source-maps.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7916 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/docs/syntax.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/docs/guidelines/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4489 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/docs/guidelines/runner.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5994 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/docs/guidelines/plugin.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    15274 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/get-caller-file/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      316 2016-08-09 00:43:20.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/get-caller-file/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caseless/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1173 2014-10-29 18:52:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caseless/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strip-json-comments/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1493 2015-11-18 14:02:54.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strip-json-comments/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/currently-unhandled/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1501 2016-06-02 10:38:24.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/currently-unhandled/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-literals/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      859 2016-12-08 15:43:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-literals/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caniuse-db/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      833 2017-04-12 02:49:09.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caniuse-db/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7081 2017-04-23 22:33:55.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caniuse-db/CONTRIBUTING.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/os-homedir/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      735 2016-09-30 04:57:23.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/os-homedir/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack-sources/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5131 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack-sources/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack-sources/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack-sources/node_modules/source-list-map/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2554 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack-sources/node_modules/source-list-map/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prelude-ls/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      613 2014-10-01 01:42:58.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prelude-ls/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3989 2015-05-15 02:39:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prelude-ls/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-loader/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9822 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-loader/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6585 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-loader/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/form-data/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6437 2017-04-09 15:09:56.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/form-data/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-function-bind/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      450 2016-03-21 23:00:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-function-bind/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/original/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1787 2014-11-08 16:04:46.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/original/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/original/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/original/node_modules/url-parse/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5159 2015-10-30 14:42:40.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/original/node_modules/url-parse/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.mergewith/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      474 2016-08-13 17:34:37.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.mergewith/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loud-rejection/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1719 2016-07-03 22:00:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loud-rejection/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/react-dom/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      897 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/react-dom/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tar/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1298 2015-09-10 01:47:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tar/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cross-spawn/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2605 2016-05-18 13:23:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cross-spawn/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.assign/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      453 2016-08-13 17:33:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.assign/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-do-expressions/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      456 2016-03-21 23:00:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-do-expressions/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json-schema/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      405 2016-09-03 02:53:20.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json-schema/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asynckit/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7640 2016-06-14 18:28:19.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asynckit/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-async-functions/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      462 2016-03-21 23:00:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-async-functions/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object-assign/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1502 2016-11-04 02:19:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object-assign/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-binary-path/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      696 2015-04-07 08:14:18.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-binary-path/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regenerator-transform/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      719 2016-05-30 19:47:37.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regenerator-transform/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/progress/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2365 2014-03-30 13:46:56.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/progress/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2017 2014-07-01 02:16:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/progress/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/setprototypeof/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      401 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/setprototypeof/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/yargs-parser/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6665 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/yargs-parser/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6054 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/yargs-parser/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-tokens/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6522 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-tokens/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3725 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-tokens/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-bindify-decorators/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       50 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-bindify-decorators/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-unique-selectors/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1156 2015-08-25 12:53:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-unique-selectors/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      248 2016-02-07 00:32:46.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-unique-selectors/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    12111 2017-03-31 19:56:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint/node_modules/doctrine/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6470 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint/node_modules/doctrine/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3076 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint/node_modules/doctrine/CHANGELOG.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)   273638 2017-03-31 20:05:15.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/slash/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      890 2014-08-13 10:14:42.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/slash/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/performance-now/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1985 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/performance-now/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-sign/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      857 2016-05-12 14:30:13.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-sign/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-extendable/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2546 2015-07-04 22:50:02.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-extendable/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-zindex/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2462 2016-11-25 16:47:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-zindex/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1117 2016-11-25 16:53:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-zindex/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-my-json-valid/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4962 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-my-json-valid/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-static/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7508 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-static/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8185 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-static/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tunnel-agent/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      113 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tunnel-agent/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/require-uncached/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      833 2016-11-03 06:59:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/require-uncached/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/argparse/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8172 2016-03-17 14:49:34.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/argparse/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3341 2016-09-29 19:26:03.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/argparse/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    16810 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7033 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/create-hmac/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1083 2017-04-27 14:33:47.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/create-hmac/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      720 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/create-hmac/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ansi-regex/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1749 2017-01-14 03:03:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ansi-regex/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-comments/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2796 2016-02-10 16:59:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-comments/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1727 2016-02-10 16:59:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-comments/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-utf8/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      397 2015-12-19 03:59:50.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-utf8/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uniqs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1204 2014-06-03 08:27:53.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uniqs/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/utils-merge/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      634 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/utils-merge/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-selectors/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1147 2016-01-11 11:31:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-selectors/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2541 2016-12-31 12:39:58.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-selectors/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-idents/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1649 2016-02-07 00:48:47.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-idents/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1079 2016-08-16 19:46:39.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-idents/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/globule/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6460 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/globule/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/globule/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/globule/node_modules/lodash/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1120 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/globule/node_modules/lodash/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/d/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2724 2015-06-25 13:18:23.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/d/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    43529 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    53650 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs-parser/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5614 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs-parser/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1960 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs-parser/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/window-size/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1783 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/window-size/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1934 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/CHANGELOG.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2598 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/block-stream/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      369 2011-10-07 03:09:34.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/block-stream/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strip-indent/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      957 2014-08-13 13:44:37.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strip-indent/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regex-cache/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5314 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regex-cache/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/dashdash/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    18164 2016-01-18 19:18:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/dashdash/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10912 2016-11-22 22:33:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/dashdash/CHANGES.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regjsparser/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      440 2015-02-27 23:46:17.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regjsparser/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regjsparser/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regjsparser/node_modules/jsesc/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    12447 2014-05-25 09:18:35.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regjsparser/node_modules/jsesc/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/bcrypt-pbkdf/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1359 2017-02-02 03:51:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/bcrypt-pbkdf/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ignore/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     6666 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ignore/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-values/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1175 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-values/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/html-comment-regex/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      974 2015-05-21 08:08:52.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/html-comment-regex/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/process/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1359 2015-09-08 15:14:50.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/process/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/content-disposition/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5148 2016-12-09 01:01:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/content-disposition/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      866 2016-12-09 01:16:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/content-disposition/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/exit-hook/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      676 2014-08-31 23:27:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/exit-hook/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/delayed-stream/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3871 2015-04-27 18:43:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/delayed-stream/Readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/extglob/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3242 2015-08-01 20:11:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/extglob/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/requires-port/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1814 2014-11-08 15:59:03.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/requires-port/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sort-keys/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1002 2016-05-18 04:43:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sort-keys/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tapable/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4813 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tapable/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hmac-drbg/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1723 2017-02-22 21:41:57.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hmac-drbg/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-template-literals/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1116 2016-12-08 15:43:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-template-literals/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/invert-kv/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      480 2014-06-26 20:07:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/invert-kv/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/media-typer/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2371 2014-09-08 04:06:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/media-typer/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      461 2014-09-08 04:30:34.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/media-typer/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/etag/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4208 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/etag/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1640 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/etag/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-zlib/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      722 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-zlib/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/gauge/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    15073 2016-11-03 21:33:48.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/gauge/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6376 2017-04-21 23:05:55.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/gauge/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/on-finished/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4886 2015-05-26 02:27:15.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/on-finished/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1694 2015-05-27 01:18:07.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/on-finished/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-resolvable/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2206 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-resolvable/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fs.realpath/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      881 2016-06-15 18:27:25.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fs.realpath/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/forever-agent/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      163 2015-03-21 11:48:42.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/forever-agent/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    14123 2017-01-29 18:01:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/README.ru.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10540 2017-01-29 17:57:33.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/node_modules/esprima/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2006 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/node_modules/esprima/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/node_modules/js-yaml/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9283 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/node_modules/js-yaml/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9054 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/node_modules/js-yaml/CHANGELOG.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    31474 2017-01-29 17:57:33.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-yaml/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9709 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-yaml/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9619 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-yaml/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-posix-bracket/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3212 2016-04-05 05:30:30.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-posix-bracket/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/anymatch/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3884 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/anymatch/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/has-ansi/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      856 2015-06-30 16:13:09.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/has-ansi/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-systemjs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1013 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-systemjs/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/math-expression-evaluator/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3562 2017-02-02 07:48:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/math-expression-evaluator/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-path-inside/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      514 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-path-inside/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json3/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9293 2014-06-22 21:15:11.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json3/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/chokidar/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    13069 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/chokidar/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9832 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/chokidar/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/define-properties/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2725 2015-10-14 22:16:36.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/define-properties/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      972 2015-10-14 22:22:54.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/define-properties/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-buffer/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1504 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-buffer/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/load-json-file/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/load-json-file/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/load-json-file/node_modules/strip-bom/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      902 2015-06-29 13:11:39.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/load-json-file/node_modules/strip-bom/readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      951 2015-11-08 13:46:23.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/load-json-file/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.clonedeep/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      474 2016-08-13 17:34:12.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.clonedeep/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/callsites/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1896 2014-04-19 10:11:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/callsites/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-export-extensions/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1082 2016-12-08 15:43:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-export-extensions/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsbn/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1623 2017-02-12 07:42:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsbn/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/statuses/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2746 2016-11-12 02:35:26.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/statuses/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      887 2016-11-12 04:00:10.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/statuses/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/code-point-at/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      617 2016-11-03 10:06:35.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/code-point-at/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/aproba/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2594 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/aproba/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx-source/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      636 2016-12-08 15:43:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx-source/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-umd/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4581 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-umd/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/has-flag/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      927 2015-07-07 22:30:14.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/has-flag/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs/examples/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs/examples/echo/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      355 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs/examples/echo/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs/examples/multiplex/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      697 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs/examples/multiplex/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    16405 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs/tests/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs/tests/test_server/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      737 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs/tests/test_server/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color-string/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1274 2015-02-19 06:58:18.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color-string/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      386 2015-02-19 07:21:40.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color-string/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-generator/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4200 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-generator/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/circular-json/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4371 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/circular-json/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/type-is/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4161 2017-03-25 04:58:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/type-is/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3923 2017-04-01 03:15:33.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/type-is/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsprim/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    11023 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsprim/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      895 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsprim/CHANGES.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-function-name/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      531 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-function-name/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es5-ext/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    38986 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es5-ext/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/console-browserify/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      544 2014-04-08 02:54:18.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/console-browserify/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/private/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7958 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/private/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-driver/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    13736 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-driver/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      162 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-driver/CODE_OF_CONDUCT.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2966 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-driver/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/depd/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10142 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/depd/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1839 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/depd/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/remove-trailing-separator/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      236 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/remove-trailing-separator/history.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1789 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/remove-trailing-separator/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-builder-react-jsx/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      709 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-builder-react-jsx/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/espree/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7931 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/espree/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    15373 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/espree/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sprintf-js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4855 2015-07-10 13:33:43.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sprintf-js/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/encoding/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1392 2015-12-23 09:05:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/encoding/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-exists/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1217 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-exists/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/whet.extend/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      507 2012-05-24 15:14:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/whet.extend/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      513 2013-01-27 21:37:52.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/whet.extend/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cryptiles/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      599 2015-09-09 06:08:12.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cryptiles/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/which/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1154 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/which/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2339 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/which/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-set/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1940 2017-01-12 15:43:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-set/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-check-es2015-constants/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1068 2017-01-07 22:18:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-check-es2015-constants/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regenerator-runtime/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      758 2016-05-02 15:31:09.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regenerator-runtime/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-class-properties/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      468 2016-03-21 23:00:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-class-properties/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ansi-html/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1395 2015-11-21 10:15:48.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ansi-html/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-cipher/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      302 2015-09-27 18:34:58.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-cipher/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/date-now/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      824 2013-02-09 03:02:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/date-now/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prepend-http/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      577 2016-05-10 05:18:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prepend-http/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isarray/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1890 2015-12-10 10:04:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isarray/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/inherits/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1625 2013-05-16 14:24:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/inherits/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-runtime/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       17 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-runtime/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array.prototype.find/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1327 2016-11-08 08:33:50.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array.prototype.find/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1210 2017-03-30 18:50:57.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array.prototype.find/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-selector-tokenizer/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2405 2015-06-12 03:43:48.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-selector-tokenizer/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/oauth-sign/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      107 2016-05-04 21:10:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/oauth-sign/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/has-unicode/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1388 2015-11-26 00:54:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/has-unicode/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/arr-flatten/
--rwxr--r--   0 davecap   (1000) davecap   (1000)     3549 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/arr-flatten/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-template/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1233 2017-04-01 14:50:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-template/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-arrayish/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      704 2015-08-25 17:01:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-arrayish/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-class-constructor-call/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2324 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-class-constructor-call/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/electron-to-chromium/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5320 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/electron-to-chromium/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      296 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/electron-to-chromium/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uniqid/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3406 2017-01-07 17:52:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uniqid/Readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/os-tmpdir/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      693 2016-09-30 04:50:25.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/os-tmpdir/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/gaze/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8132 2016-09-27 19:30:42.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/gaze/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    41777 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/camelcase/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      889 2015-07-30 15:11:13.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/camelcase/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/yargs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    22253 2015-05-29 04:23:14.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/yargs/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    37151 2015-05-29 04:30:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/yargs/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/cliui/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2019 2015-04-24 22:33:35.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/cliui/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/debug/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    17918 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/debug/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/debug/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/debug/node_modules/ms/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1832 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/debug/node_modules/ms/readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1077 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/debug/node_modules/ms/license.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10988 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/debug/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/csso/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    15039 2017-03-10 21:36:14.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/csso/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    13476 2017-03-10 21:43:33.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/csso/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ajv-keywords/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    12462 2017-01-22 17:51:02.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ajv-keywords/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ajv-keywords/keywords/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ajv-keywords/keywords/dotjs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      158 2016-12-22 20:46:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ajv-keywords/keywords/dotjs/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/string_decoder/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      498 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/string_decoder/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/interpret/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3612 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/interpret/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-flow-strip-types/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      962 2016-12-08 15:43:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-flow-strip-types/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-explode-class/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       45 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-explode-class/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/invariant/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1613 2016-11-15 11:07:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/invariant/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      684 2016-11-15 11:07:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/invariant/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.tail/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      439 2016-08-13 17:33:11.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.tail/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asn1.js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2480 2015-10-23 21:46:19.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asn1.js/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-register/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2846 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-register/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/concat-stream/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3505 2016-12-19 15:43:58.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/concat-stream/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-arrow-functions/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2403 2016-12-08 15:43:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-arrow-functions/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/clone/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3585 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/clone/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    26687 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/tools/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      456 2017-04-05 22:07:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/tools/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2362 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/scopes.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1900 2017-04-05 22:07:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/string_bytes.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10837 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/persistent.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2121 2017-04-05 22:07:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/buffers.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1513 2017-04-05 22:07:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/callback.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1950 2017-04-05 22:07:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/converters.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7404 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/errors.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2240 2017-04-05 22:07:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/node_misc.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2914 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/v8_misc.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4859 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/new.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7389 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/v8_internals.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3255 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/asyncworker.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8204 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/object_wrappers.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1279 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/script.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    27016 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/methods.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1941 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/json.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    21167 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/maybe_types.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    17639 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/CHANGELOG.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1216 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/event-emitter/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3335 2017-01-10 11:39:53.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/event-emitter/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-base64/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1282 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-base64/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1480 2014-12-06 20:50:57.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-base64/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-extract-imports/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1623 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-extract-imports/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lcid/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      826 2015-03-16 06:56:30.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lcid/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/minimalistic-assert/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       58 2015-01-12 16:19:40.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/minimalistic-assert/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/wrap-ansi/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2026 2016-11-29 17:14:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/wrap-ansi/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-regex/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       37 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-regex/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/public-encrypt/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      195 2015-02-12 13:26:13.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/public-encrypt/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-destructuring/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      513 2017-01-20 05:35:55.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-destructuring/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/flatten/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      460 2016-01-20 00:43:29.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/flatten/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-stage-3/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1181 2017-04-01 14:50:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-stage-3/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/align-text/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5507 2016-02-02 01:50:23.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/align-text/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readdirp/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readdirp/examples/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1076 2014-12-12 21:18:57.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readdirp/examples/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8824 2014-12-12 21:18:57.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readdirp/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/onetime/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      892 2015-12-18 00:17:29.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/onetime/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pkg-dir/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1109 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pkg-dir/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-extensions/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    14241 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-extensions/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-extensions/lib/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-extensions/lib/pipeline/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    24700 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-extensions/lib/pipeline/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      244 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-extensions/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/xtend/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      725 2015-11-02 22:19:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/xtend/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-is-absolute/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1153 2016-09-30 04:41:17.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-is-absolute/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/window-size/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      624 2014-02-15 03:41:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/window-size/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strict-uri-encode/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      666 2016-01-04 06:59:39.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strict-uri-encode/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      854 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/node_modules/regexpu-core/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2808 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/node_modules/regexpu-core/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-normalize-charset/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      805 2016-09-30 16:50:14.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-normalize-charset/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      306 2016-11-08 15:31:25.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-normalize-charset/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-amd/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      900 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-amd/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/signal-exit/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1497 2016-12-02 21:10:47.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/signal-exit/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1071 2016-12-02 21:10:47.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/signal-exit/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/q/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    25386 2017-03-22 02:09:48.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/q/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    29828 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/q/CHANGES.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sha.js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1287 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sha.js/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/connect-history-api-fallback/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4727 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/connect-history-api-fallback/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      935 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/connect-history-api-fallback/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eventemitter3/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3685 2015-06-14 14:05:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eventemitter3/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/buffer-shims/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      497 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/buffer-shims/readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1064 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/buffer-shims/license.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/globby/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2197 2016-06-11 06:17:12.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/globby/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/in-publish/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1130 2015-07-07 19:00:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/in-publish/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdx-correct/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      225 2015-10-26 16:53:56.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdx-correct/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-rules/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1585 2015-10-18 19:27:53.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-rules/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3538 2017-02-20 11:09:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-rules/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-builder-binary-assignment-operator-visitor/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       74 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-builder-binary-assignment-operator-visitor/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-fetch/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6177 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-fetch/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1232 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-fetch/ERROR-HANDLING.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4439 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-fetch/CHANGELOG.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1079 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-fetch/LICENSE.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1341 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-fetch/LIMITS.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-class-properties/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1778 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-class-properties/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-errors/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4640 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-errors/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2120 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-errors/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-errors/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-errors/node_modules/setprototypeof/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      401 2016-02-06 23:38:42.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-errors/node_modules/setprototypeof/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object-keys/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2460 2015-10-14 22:01:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object-keys/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6992 2016-07-05 17:14:10.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object-keys/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pseudomap/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2163 2015-11-28 22:25:20.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pseudomap/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-parameters/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      899 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-parameters/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/find-up/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1271 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/find-up/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8656 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10068 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/node_modules/debug/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8483 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/node_modules/debug/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10364 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/node_modules/debug/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/node_modules/http-errors/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4803 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/node_modules/http-errors/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2548 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/node_modules/http-errors/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/parse-glob/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4017 2015-09-22 15:16:36.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/parse-glob/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/expand-range/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4391 2016-05-05 09:25:14.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/expand-range/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-finite/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      544 2016-09-30 07:42:48.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-finite/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/restore-cursor/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      359 2014-08-31 23:29:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/restore-cursor/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-ordered-values/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3355 2016-06-23 22:41:47.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-ordered-values/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1293 2017-01-10 11:43:09.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-ordered-values/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/express/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4540 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/express/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)   102583 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/express/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/express/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/express/node_modules/debug/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8483 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/express/node_modules/debug/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10364 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/express/node_modules/debug/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/meow/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3845 2016-01-04 14:11:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/meow/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/handle-thing/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1382 2016-03-02 06:31:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/handle-thing/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fresh/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3236 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fresh/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1220 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fresh/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mime-types/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3104 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mime-types/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3994 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mime-types/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mime-db/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2991 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mime-db/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    11272 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mime-db/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-typeof-symbol/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      960 2017-01-20 05:35:55.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-typeof-symbol/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/are-we-there-yet/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6302 2017-04-21 07:41:17.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/are-we-there-yet/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1107 2017-04-21 07:46:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/are-we-there-yet/CHANGES.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/redent/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      750 2015-09-29 10:53:48.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/redent/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/extend/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2360 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/extend/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2162 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/extend/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-exponentiation-operator/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      514 2016-03-21 23:00:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-exponentiation-operator/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-strict-mode/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1041 2017-04-01 14:50:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-strict-mode/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/map-obj/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      555 2015-05-02 18:02:23.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/map-obj/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es-abstract/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1812 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es-abstract/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4096 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es-abstract/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mute-stream/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1653 2013-07-15 01:14:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mute-stream/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1832 2017-04-01 14:50:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/figures/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4016 2016-05-17 16:58:13.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/figures/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/har-validator/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2891 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/har-validator/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/randomatic/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6151 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/randomatic/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/generate-function/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1748 2014-07-30 17:29:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/generate-function/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uuid/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6393 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uuid/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uuid/benchmark/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2031 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uuid/benchmark/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      100 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uuid/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-longhand/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1326 2015-08-17 15:37:35.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-longhand/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      455 2017-01-13 15:32:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-longhand/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/macaddress/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2793 2015-04-26 11:57:23.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/macaddress/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/repeat-element/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1439 2015-05-07 03:15:50.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/repeat-element/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/clone-deep/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3001 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/clone-deep/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regexpu-core/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2808 2016-01-11 16:21:10.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regexpu-core/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lru-cache/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4910 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lru-cache/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/wrappy/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      685 2016-05-17 23:15:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/wrappy/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/home-or-tmp/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      647 2015-05-17 22:13:12.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/home-or-tmp/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/inquirer/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    11124 2015-12-31 23:28:34.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/inquirer/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sntp/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1898 2014-09-05 19:49:55.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sntp/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/miller-rabin/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1135 2015-10-28 20:20:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/miller-rabin/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/stringstream/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1062 2013-01-21 10:47:30.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/stringstream/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/resolve-from/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      992 2015-10-05 14:28:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/resolve-from/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-local-by-default/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1965 2015-06-10 09:55:43.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-local-by-default/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2692 2015-09-19 14:47:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-local-by-default/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-color-names/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      787 2015-09-04 16:30:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-color-names/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/querystring-es3/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1081 2014-10-13 18:58:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/querystring-es3/License.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      367 2014-10-13 18:58:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/querystring-es3/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      357 2014-10-13 18:58:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/querystring-es3/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/methods/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1694 2016-01-18 01:17:30.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/methods/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      427 2016-01-18 02:40:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/methods/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/longest/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2204 2015-03-31 11:37:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/longest/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/detect-indent/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2361 2015-09-07 09:14:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/detect-indent/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cliui/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2355 2016-04-11 02:03:36.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cliui/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      510 2016-04-11 02:46:52.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cliui/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/validate-npm-package-license/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2561 2015-08-23 23:32:29.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/validate-npm-package-license/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/escope/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3269 2016-03-10 21:49:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/escope/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      402 2015-03-08 02:09:55.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/escope/CONTRIBUTING.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ieee754/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1413 2016-10-03 07:50:52.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ieee754/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/filename-regex/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1025 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/filename-regex/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ipaddr.js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7541 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ipaddr.js/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-exponentiation-operator/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      944 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-exponentiation-operator/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/big.js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7943 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/big.js/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/rimraf/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3600 2015-12-23 18:43:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/rimraf/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/process-nextick-args/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      451 2015-09-09 18:40:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/process-nextick-args/readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1064 2015-09-09 18:40:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/process-nextick-args/license.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/bytes/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3130 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/bytes/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1225 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/bytes/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/source-map-support/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8559 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/source-map-support/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1079 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/source-map-support/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-absolute-url/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      632 2016-10-25 18:44:53.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-absolute-url/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdy/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8098 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdy/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-function-bind/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3656 2017-01-07 22:18:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-function-bind/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cipher-base/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      726 2017-07-06 12:04:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cipher-base/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      726 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cipher-base/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-symbol/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2129 2016-11-11 20:09:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-symbol/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-class-constructor-call/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      509 2016-10-21 15:29:24.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-class-constructor-call/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/brorand/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1130 2016-09-06 14:17:10.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/brorand/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    23750 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2800 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2031 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-autotools.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4359 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-importer.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4253 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/custom-functions-internal.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3436 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-mingw.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1281 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-on-gentoo.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1118 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-context-example.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4855 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1596 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/README.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     7760 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/dev-ast-memory.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3471 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-function.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1273 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-value-internal.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2947 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-visual-studio.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4813 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-on-windows.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2149 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-function-example.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)      421 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-importer-internal.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3965 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/unicode.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3512 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-context-internal.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)      164 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-function-internal.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3653 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-importer-example.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1405 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-value-example.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2325 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/source-map-internals.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1915 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/plugins.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1418 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-shared-library.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1600 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-makefiles.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1773 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/triage.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)      792 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-on-darwin.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1622 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/implementations.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     6137 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-value.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1405 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/contributing.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2899 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/compatibility-plan.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)    11063 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-context.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     7725 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-doc.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)      892 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/trace.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2457 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/setup-environment.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4351 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/Readme.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)      370 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/SECURITY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/.github/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3723 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/.github/CONTRIBUTING.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)      448 2018-05-14 19:25:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-object-rest-spread/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      480 2016-03-21 23:00:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-object-rest-spread/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object.assign/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6303 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object.assign/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-duplicate-keys/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1066 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-duplicate-keys/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/repeating/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1282 2016-04-11 17:31:47.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/repeating/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/kind-of/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8177 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/kind-of/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/num2fraction/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2594 2015-09-14 01:50:23.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/num2fraction/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/expand-brackets/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3765 2016-04-01 23:34:57.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/expand-brackets/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/indexof/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      141 2012-08-16 23:38:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/indexof/Readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-loader/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7639 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-loader/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4934 2017-04-21 20:11:39.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-loader/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loader-runner/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1191 2016-09-14 22:08:13.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loader-runner/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tryit/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1601 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tryit/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regjsgen/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1181 2014-09-02 04:33:52.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regjsgen/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/async/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1261 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/async/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    16868 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/async/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-to-browserify/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      574 2014-02-05 12:40:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-to-browserify/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/create-hash/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      691 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/create-hash/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-union/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      513 2016-06-16 12:14:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-union/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/glob/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    14664 2016-09-20 18:27:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/glob/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1430 2016-02-11 06:23:26.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/glob/changelog.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/globals/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1411 2016-10-25 18:34:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/globals/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/arrify/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      519 2015-12-09 17:46:03.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/arrify/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es-to-primitive/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2174 2015-11-01 03:25:26.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es-to-primitive/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1201 2016-01-04 01:34:54.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es-to-primitive/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/diffie-hellman/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      518 2015-01-27 14:00:29.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/diffie-hellman/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lazy-cache/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3721 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lazy-cache/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loader-utils/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8364 2017-03-16 14:00:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loader-utils/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      736 2017-03-16 14:04:12.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loader-utils/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/core-js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    37340 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/core-js/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pify/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2579 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pify/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-dotfile/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1977 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-dotfile/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-trailing-function-commas/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2617 2016-12-08 15:43:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-trailing-function-commas/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/foreach/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      593 2014-09-22 06:18:56.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/foreach/Readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-fullwidth-code-point/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      833 2015-07-16 21:59:20.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-fullwidth-code-point/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-explode-assignable-expression/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       61 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-explode-assignable-expression/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strip-bom/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      913 2016-04-30 15:51:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strip-bom/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/getpass/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      774 2016-04-21 21:51:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/getpass/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-object-super/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      507 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-object-super/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/require-main-filename/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1064 2016-02-01 05:31:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/require-main-filename/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/punycode/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6115 2015-02-24 22:04:57.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/punycode/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/buffer-xor/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1014 2015-09-25 07:13:39.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/buffer-xor/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-weak-map/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1808 2015-06-25 13:26:46.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-weak-map/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/content-type/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2796 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/content-type/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      265 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/content-type/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/request/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    43747 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/request/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/request/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4644 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      626 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/HISTORY.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1109 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/LICENSE.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)    65653 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/request/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eventsource/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2381 2014-12-26 09:41:57.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eventsource/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      234 2015-02-08 23:43:58.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eventsource/CONTRIBUTING.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5137 2015-02-09 08:21:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eventsource/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/select-hose/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1373 2015-07-14 04:36:13.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/select-hose/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/arr-diff/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2194 2015-12-06 04:25:40.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/arr-diff/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/osenv/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1468 2012-06-18 00:50:18.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/osenv/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jodid25519/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2705 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jodid25519/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      162 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jodid25519/AUTHORS.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/file-entry-cache/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4856 2016-08-01 09:48:42.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/file-entry-cache/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3616 2016-08-16 20:48:13.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/file-entry-cache/changelog.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cli-cursor/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      666 2015-09-18 13:45:53.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cli-cursor/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-symbol/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1469 2015-01-24 21:07:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-symbol/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      121 2015-01-26 09:43:10.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-symbol/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ansi-escapes/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3394 2016-04-17 20:33:57.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ansi-escapes/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caniuse-api/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2668 2017-04-06 15:04:56.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caniuse-api/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2107 2017-04-07 07:42:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caniuse-api/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-core/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7547 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-core/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/os-browserify/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      212 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/os-browserify/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-scope/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2305 2015-10-20 07:54:40.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-scope/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/iconv-lite/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6796 2017-04-21 09:01:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/iconv-lite/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3012 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/iconv-lite/Changelog.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/number-is-nan/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      559 2016-09-30 05:10:34.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/number-is-nan/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-normalize-url/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1577 2015-08-13 10:42:53.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-normalize-url/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2026 2016-12-30 22:04:08.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-normalize-url/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/normalize-range/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4013 2015-09-12 06:23:53.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/normalize-range/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-unique/
--rwxr--r--   0 davecap   (1000) davecap   (1000)     1965 2015-03-25 03:46:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-unique/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/read-pkg/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1710 2015-09-03 04:54:53.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/read-pkg/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json-stringify-safe/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1261 2015-05-19 01:41:30.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json-stringify-safe/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      734 2015-05-19 01:41:30.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json-stringify-safe/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/type-check/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10168 2015-12-29 05:40:34.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/type-check/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/normalize-package-data/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7223 2017-04-21 00:27:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/normalize-package-data/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/vary/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2716 2017-03-20 18:45:24.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/vary/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      707 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/vary/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/trim-right/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      673 2015-02-17 03:45:01.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/trim-right/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/boom/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)    16600 2015-10-30 19:11:45.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/boom/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      105 2014-09-23 13:15:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/boom/CONTRIBUTING.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.camelcase/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      474 2016-08-13 17:33:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash.camelcase/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/assert-plus/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4791 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/assert-plus/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      428 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/assert-plus/CHANGES.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-message-helpers/
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2295 2014-11-24 19:32:43.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-message-helpers/README.md
--rwxr-xr-x   0 davecap   (1000) davecap   (1000)      359 2015-01-26 07:14:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-message-helpers/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-do-expressions/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4191 2016-12-08 15:43:16.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-do-expressions/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-async-generator-functions/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2611 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-async-generator-functions/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/generate-object-property/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      473 2015-03-27 14:09:55.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/generate-object-property/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sax/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8381 2016-03-19 03:03:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sax/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/set-immediate-shim/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      558 2014-12-29 09:38:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/set-immediate-shim/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-stage-2/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1248 2017-04-01 14:50:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-stage-2/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helpers/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      326 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helpers/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-function-name/
--rw-r--r--   0 davecap   (1000) davecap   (1000)       45 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-function-name/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-block-scoping/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1162 2017-04-01 14:50:05.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-block-scoping/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/for-in/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3452 2016-03-27 14:56:29.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/for-in/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/inflight/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      991 2014-05-05 03:32:51.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/inflight/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8575 2017-04-15 15:46:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1758 2017-04-19 18:40:31.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/CHANGELOG.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1077 2016-06-15 17:48:01.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/once/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1772 2016-09-06 21:07:04.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/once/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tweetnacl/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    13166 2016-12-13 11:07:18.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tweetnacl/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      875 2016-12-13 10:02:34.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tweetnacl/AUTHORS.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1040 2016-12-13 10:02:34.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tweetnacl/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5904 2016-12-13 10:58:09.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tweetnacl/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-display-name/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      649 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-display-name/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pbkdf2/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1439 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pbkdf2/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/doctrine/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7263 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/doctrine/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2903 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/doctrine/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isobject/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2568 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isobject/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/whatwg-fetch/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8628 2017-03-02 17:49:23.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/whatwg-fetch/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/semver/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    13336 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/semver/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-stage-1/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1406 2017-04-01 14:50:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-stage-1/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/function-bind/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1488 2016-02-14 07:31:07.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/function-bind/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/forwarded/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1432 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/forwarded/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)       59 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/forwarded/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isexe/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1395 2017-03-23 00:52:07.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isexe/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsonpointer/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1103 2016-12-21 13:04:09.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsonpointer/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1152 2016-05-19 07:21:41.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsonpointer/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/colormin/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1340 2016-03-01 20:55:20.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/colormin/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)      599 2016-08-16 17:36:12.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/colormin/CHANGELOG.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/proxy-addr/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4202 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/proxy-addr/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2087 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/proxy-addr/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/os-locale/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1027 2015-09-08 06:02:17.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/os-locale/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/flat-cache/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2683 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/flat-cache/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7143 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/flat-cache/changelog.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/colors/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3473 2015-06-17 12:57:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/colors/ReadMe.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1120 2016-12-31 22:32:40.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/accepts/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3838 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/accepts/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4542 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/accepts/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-flow/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      374 2016-10-17 22:44:21.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-flow/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-find-index/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      686 2016-09-30 08:34:35.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-find-index/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-uniq/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      671 2016-06-16 12:16:36.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-uniq/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-parse/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      912 2015-04-21 15:25:22.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-parse/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-number/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3439 2015-05-02 07:52:39.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-number/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4737 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5971 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/HISTORY.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/ms/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      933 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/ms/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1307 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/ms/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/debug/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6310 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/debug/Readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5611 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/debug/History.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/glob-base/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4690 2015-09-18 17:59:28.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/glob-base/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdx-expression-parse/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3608 2016-10-05 20:10:06.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdx-expression-parse/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json5/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8894 2016-10-07 18:59:57.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json5/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6335 2016-11-27 20:33:32.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json5/CHANGELOG.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1136 2016-09-28 01:11:56.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json5/LICENSE.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prr/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1680 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prr/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/memory-fs/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      786 2016-12-05 18:47:38.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/memory-fs/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/yallist/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4717 2015-12-19 19:51:30.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/yallist/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/chalk/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/chalk/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/chalk/node_modules/supports-color/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      823 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/chalk/node_modules/supports-color/readme.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     6136 2016-03-29 00:14:01.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/chalk/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-iterator/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4274 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-iterator/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    46737 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack/node_modules/
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack/node_modules/loader-utils/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7555 2017-02-20 18:01:27.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack/node_modules/loader-utils/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isomorphic-fetch/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1218 2015-01-23 11:55:10.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isomorphic-fetch/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/levn/
--rw-r--r--   0 davecap   (1000) davecap   (1000)    10468 2015-12-29 05:52:40.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/levn/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/bn.js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7075 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/bn.js/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/normalize-path/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     5085 2017-03-29 18:19:49.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/normalize-path/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/escape-string-regexp/
--rw-r--r--   0 davecap   (1000) davecap   (1000)      552 2016-02-21 12:17:12.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/escape-string-regexp/readme.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/des.js/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1127 2015-09-06 18:26:19.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/des.js/README.md
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/verror/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4522 2018-05-14 19:25:44.000000 solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/verror/README.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)   880118 2018-05-25 18:14:57.000000 solvebio-2.8.9/solvebio/contrib/dash/login.js
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/tmp/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8081 2018-05-14 18:58:33.000000 solvebio-2.8.9/solvebio/contrib/dash/tmp/oauth.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     7140 2019-07-09 19:29:10.000000 solvebio-2.8.9/solvebio/contrib/dash/solvebio_auth.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)      147 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/contrib/dash/__init__.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2316 2019-07-09 19:29:10.000000 solvebio-2.8.9/solvebio/contrib/dash/solvebio_dash.py
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/dash/tests/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3339 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/contrib/dash/tests/test_solvebio_auth_integration.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)      371 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/contrib/dash/tests/credentials.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4374 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/contrib/dash/tests/IntegrationTests.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2365 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/contrib/dash/tests/utils.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8528 2018-09-11 16:02:27.000000 solvebio-2.8.9/solvebio/contrib/dash/tests/test_solvebio_auth.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)       91 2018-05-22 15:35:20.000000 solvebio-2.8.9/solvebio/contrib/dash/tests/credentials_local.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)        0 2017-11-13 22:59:28.000000 solvebio-2.8.9/solvebio/contrib/dash/tests/__init__.py
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:45:00.000000 solvebio-2.8.9/solvebio/contrib/vcf_parser/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     8983 2017-11-14 14:35:18.000000 solvebio-2.8.9/solvebio/contrib/vcf_parser/vcf_parser.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)        0 2016-06-30 15:13:33.000000 solvebio-2.8.9/solvebio/contrib/vcf_parser/__init__.py
--rw-rw-r--   0 davecap   (1000) davecap   (1000)        0 2016-05-02 13:03:38.000000 solvebio-2.8.9/solvebio/contrib/__init__.py
-drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-09-19 17:44:59.000000 solvebio-2.8.9/solvebio/cli/
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3480 2019-03-25 17:11:43.000000 solvebio-2.8.9/solvebio/cli/credentials.py
--rw-rw-r--   0 davecap   (1000) davecap   (1000)      212 2016-05-02 13:03:38.000000 solvebio-2.8.9/solvebio/cli/tutorial.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4801 2017-07-28 21:05:17.000000 solvebio-2.8.9/solvebio/cli/tutorial.md
--rw-r--r--   0 davecap   (1000) davecap   (1000)     9005 2018-02-23 20:39:13.000000 solvebio-2.8.9/solvebio/cli/data.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)    11794 2018-10-10 17:18:54.000000 solvebio-2.8.9/solvebio/cli/main.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1612 2018-09-11 16:02:27.000000 solvebio-2.8.9/solvebio/cli/ipython_init.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     3926 2018-09-11 16:02:27.000000 solvebio-2.8.9/solvebio/cli/auth.py
--rw-rw-r--   0 davecap   (1000) davecap   (1000)        0 2016-05-02 13:03:38.000000 solvebio-2.8.9/solvebio/cli/__init__.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     2974 2018-07-13 17:43:13.000000 solvebio-2.8.9/solvebio/cli/ipython.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     1930 2018-02-12 23:39:53.000000 solvebio-2.8.9/solvebio/errors.py
--rw-r--r--   0 davecap   (1000) davecap   (1000)     4871 2019-09-19 16:04:54.000000 solvebio-2.8.9/solvebio/__init__.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3788 2019-11-07 21:51:36.000000 solvebio-2.9.0/PKG-INFO
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)     1100 2016-05-02 13:03:38.000000 solvebio-2.9.0/LICENSE
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2413 2019-03-25 17:11:43.000000 solvebio-2.9.0/README.md
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)       64 2016-05-02 13:03:38.000000 solvebio-2.9.0/AUTHORS
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)       79 2019-11-07 21:51:36.000000 solvebio-2.9.0/setup.cfg
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      260 2017-11-13 22:59:28.000000 solvebio-2.9.0/MANIFEST.in
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio.egg-info/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3788 2019-11-07 21:51:35.000000 solvebio-2.9.0/solvebio.egg-info/PKG-INFO
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       53 2019-11-07 21:51:35.000000 solvebio-2.9.0/solvebio.egg-info/entry_points.txt
+-rw-r--r--   0 davecap   (1000) davecap   (1000)        1 2019-11-07 21:51:35.000000 solvebio-2.9.0/solvebio.egg-info/dependency_links.txt
+-rw-r--r--   0 davecap   (1000) davecap   (1000)        9 2019-11-07 21:51:35.000000 solvebio-2.9.0/solvebio.egg-info/top_level.txt
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       28 2019-11-07 21:51:35.000000 solvebio-2.9.0/solvebio.egg-info/requires.txt
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    72709 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio.egg-info/SOURCES.txt
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2086 2018-10-29 16:51:26.000000 solvebio-2.9.0/setup.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2822 2018-09-07 17:09:45.000000 solvebio-2.9.0/solvebio/annotate.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      200 2019-11-07 21:49:23.000000 solvebio-2.9.0/solvebio/version.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/utils/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      372 2018-02-01 19:54:40.000000 solvebio-2.9.0/solvebio/utils/files.py
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)     2718 2016-05-02 13:03:38.000000 solvebio-2.9.0/solvebio/utils/humanize.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1140 2016-05-30 18:03:16.000000 solvebio-2.9.0/solvebio/utils/md5sum.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      665 2019-03-25 17:11:43.000000 solvebio-2.9.0/solvebio/utils/validators.py
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)     3111 2016-05-02 13:03:38.000000 solvebio-2.9.0/solvebio/utils/printing.py
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)        0 2016-05-02 13:03:38.000000 solvebio-2.9.0/solvebio/utils/__init__.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    20738 2017-07-28 21:05:17.000000 solvebio-2.9.0/solvebio/utils/tabulate.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/test/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7021 2018-04-25 13:53:54.000000 solvebio-2.9.0/solvebio/test/test_filter.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    12290 2019-11-07 21:47:01.000000 solvebio-2.9.0/solvebio/test/test_shortcuts.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2093 2017-11-22 14:20:14.000000 solvebio-2.9.0/solvebio/test/test_dataset_migrations.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3474 2019-11-06 16:26:19.000000 solvebio-2.9.0/solvebio/test/test_dataset.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1444 2019-11-06 16:26:19.000000 solvebio-2.9.0/solvebio/test/helper.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1415 2017-10-03 20:58:42.000000 solvebio-2.9.0/solvebio/test/test_ratelimit.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1200 2019-11-06 16:26:19.000000 solvebio-2.9.0/solvebio/test/test_beacon.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2794 2018-02-01 19:54:40.000000 solvebio-2.9.0/solvebio/test/test_vault.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      611 2018-07-13 17:43:13.000000 solvebio-2.9.0/solvebio/test/test_apiresource.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4513 2017-07-28 21:05:17.000000 solvebio-2.9.0/solvebio/test/test_tabulate.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1334 2018-09-07 17:09:44.000000 solvebio-2.9.0/solvebio/test/test_exports.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1883 2016-09-23 18:26:15.000000 solvebio-2.9.0/solvebio/test/test_vcfparser.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2608 2018-09-11 16:02:27.000000 solvebio-2.9.0/solvebio/test/test_credentials.py
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)      437 2016-05-02 13:03:38.000000 solvebio-2.9.0/solvebio/test/test_conversion.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      744 2016-12-13 15:48:47.000000 solvebio-2.9.0/solvebio/test/test_utils.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/test/data/
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)      104 2016-05-02 13:03:38.000000 solvebio-2.9.0/solvebio/test/data/test_creds
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      462 2017-04-18 13:10:06.000000 solvebio-2.9.0/solvebio/test/data/template.json
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      590 2016-08-25 19:19:42.000000 solvebio-2.9.0/solvebio/test/data/sample.vcf.gz
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)      243 2016-05-02 13:03:38.000000 solvebio-2.9.0/solvebio/test/data/sample2.vcf
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       18 2017-06-15 15:20:01.000000 solvebio-2.9.0/solvebio/test/data/test_export.csv
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5321 2016-12-12 15:08:56.000000 solvebio-2.9.0/solvebio/test/data/test_export.xlsx
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       62 2016-12-13 15:48:47.000000 solvebio-2.9.0/solvebio/test/data/some_export.json.gz
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       25 2016-12-12 15:08:56.000000 solvebio-2.9.0/solvebio/test/data/test_export.json
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1197 2019-11-06 16:26:19.000000 solvebio-2.9.0/solvebio/test/test_query_batch.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5296 2019-11-07 21:47:01.000000 solvebio-2.9.0/solvebio/test/client_mocks.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1725 2018-09-11 16:02:27.000000 solvebio-2.9.0/solvebio/test/test_login.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      861 2017-11-13 22:59:28.000000 solvebio-2.9.0/solvebio/test/test_annotate.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      936 2017-11-13 22:59:28.000000 solvebio-2.9.0/solvebio/test/test_client.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1303 2019-11-06 16:26:19.000000 solvebio-2.9.0/solvebio/test/test_lookup.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10237 2019-11-06 16:26:19.000000 solvebio-2.9.0/solvebio/test/test_query.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)        0 2018-09-11 16:02:27.000000 solvebio-2.9.0/solvebio/test/__init__.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4406 2019-11-07 21:47:01.000000 solvebio-2.9.0/solvebio/test/test_object.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     9193 2019-11-07 21:47:01.000000 solvebio-2.9.0/solvebio/client.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      442 2019-03-25 17:11:43.000000 solvebio-2.9.0/solvebio/help.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    26199 2019-09-19 16:04:54.000000 solvebio-2.9.0/solvebio/query.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/resource/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1462 2019-09-19 16:04:54.000000 solvebio-2.9.0/solvebio/resource/savedquery.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2306 2018-07-13 17:43:13.000000 solvebio-2.9.0/solvebio/resource/group.py
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)      596 2016-05-02 13:03:38.000000 solvebio-2.9.0/solvebio/resource/util.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1214 2017-11-22 14:20:14.000000 solvebio-2.9.0/solvebio/resource/beacon.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1331 2019-09-19 16:04:54.000000 solvebio-2.9.0/solvebio/resource/vault_sync_task.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1503 2019-09-19 16:04:54.000000 solvebio-2.9.0/solvebio/resource/object_copy_task.py
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)      115 2016-05-02 13:03:38.000000 solvebio-2.9.0/solvebio/resource/user.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2980 2019-09-19 16:04:54.000000 solvebio-2.9.0/solvebio/resource/datasetcommit.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2543 2019-03-25 17:11:43.000000 solvebio-2.9.0/solvebio/resource/manifest.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      581 2017-11-22 14:20:14.000000 solvebio-2.9.0/solvebio/resource/datasettemplate.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      689 2018-02-01 19:54:40.000000 solvebio-2.9.0/solvebio/resource/application.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      876 2017-11-22 14:20:14.000000 solvebio-2.9.0/solvebio/resource/datasetfield.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2106 2017-11-22 14:20:14.000000 solvebio-2.9.0/solvebio/resource/datasetexport.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3113 2017-11-13 22:59:28.000000 solvebio-2.9.0/solvebio/resource/solveobject.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1424 2017-11-22 14:20:14.000000 solvebio-2.9.0/solvebio/resource/beaconset.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2811 2019-09-19 16:04:54.000000 solvebio-2.9.0/solvebio/resource/datasetmigration.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2948 2019-09-19 16:04:54.000000 solvebio-2.9.0/solvebio/resource/datasetimport.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1273 2019-09-19 16:04:54.000000 solvebio-2.9.0/solvebio/resource/task.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    12877 2019-09-19 17:43:06.000000 solvebio-2.9.0/solvebio/resource/dataset.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1332 2018-07-13 17:43:13.000000 solvebio-2.9.0/solvebio/resource/__init__.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7796 2018-07-10 20:05:39.000000 solvebio-2.9.0/solvebio/resource/vault.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10597 2018-07-13 17:43:13.000000 solvebio-2.9.0/solvebio/resource/apiresource.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    14610 2019-11-07 21:47:01.000000 solvebio-2.9.0/solvebio/resource/object.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      249 2017-11-13 22:59:28.000000 solvebio-2.9.0/solvebio/contrib/dash/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2032 2018-02-01 18:13:16.000000 solvebio-2.9.0/solvebio/contrib/dash/usage.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)  1285869 2018-05-14 19:28:44.000000 solvebio-2.9.0/solvebio/contrib/dash/oauth-redirect.js
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      116 2017-11-13 22:59:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asap/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10089 2016-01-04 02:27:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asap/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2697 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asap/CHANGES.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1083 2016-01-04 02:27:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asap/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-rsa/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      383 2016-02-25 22:57:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-rsa/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hoek/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    17309 2015-09-16 18:29:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hoek/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      105 2015-09-11 16:17:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hoek/CONTRIBUTING.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asn1/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1201 2014-06-05 15:13:40.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asn1/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-decorators/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1173 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-decorators/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shelljs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    21587 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shelljs/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    60297 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shelljs/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/abbrev/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      499 2010-10-04 18:52:26.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/abbrev/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/npmlog/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5983 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/npmlog/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1415 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/npmlog/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     9813 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    13405 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2878 2013-01-24 02:15:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/graphviz.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4756 2013-01-24 02:15:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/pretty_gyp.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     5099 2015-07-10 13:00:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/pretty_sln.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     9586 2013-01-24 02:15:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/pretty_vcproj.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     8019 2015-07-10 13:00:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/gyptest.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)      447 2015-11-15 03:49:58.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/gyp_main.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3662 2015-11-15 03:49:58.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/PRESUBMIT.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1970 2013-11-26 08:32:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/common_test.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)   116086 2017-01-10 01:30:41.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/input.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)    23354 2015-11-15 03:49:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/mac_tool.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3270 2013-01-24 02:15:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/easy_xml_test.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    20063 2016-02-12 02:50:43.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/common.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10366 2014-02-24 15:39:19.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/ordered_dict.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    65086 2016-02-12 02:50:43.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xcode_emulation.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)    65937 2015-11-15 03:49:58.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings_test.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)    12751 2015-11-15 03:49:58.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/win_tool.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3207 2015-07-10 13:00:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/input_test.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4945 2015-07-10 13:00:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/easy_xml.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1804 2013-01-24 02:15:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSToolFile.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1247 2015-07-10 13:00:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/simple_copy.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    45045 2015-11-15 03:49:58.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)   120842 2016-02-12 02:50:43.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xcodeproj_file.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)   132681 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    45344 2016-06-15 10:31:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/android.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      645 2013-11-26 08:32:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode_test.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    30567 2016-02-12 02:50:43.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/analyzer.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)   100329 2016-02-12 02:50:43.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    91092 2016-06-15 10:31:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1018 2013-01-24 02:15:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs_test.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    44604 2016-02-12 02:50:43.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/cmake.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    58344 2016-02-12 02:50:43.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    17014 2015-07-10 13:00:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/eclipse.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1665 2013-01-24 02:15:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/gypsh.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1786 2015-07-10 13:00:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja_test.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3426 2015-11-15 03:49:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/dump_dependency_json.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3474 2015-07-10 13:00:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/gypd.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)        0 2013-01-24 02:15:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/__init__.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5536 2013-11-26 08:32:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/ninja_syntax.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    12124 2015-07-10 13:00:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSNew.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1748 2015-07-10 13:00:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/flock_tool.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     9537 2015-07-10 13:00:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSUtil.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10585 2015-07-10 13:00:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xcode_ninja.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2174 2013-01-24 02:15:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xml_fix.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    17165 2015-11-15 03:49:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSVersion.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6387 2013-01-24 02:15:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSProject.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5094 2013-01-24 02:15:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSUserFile.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)    22178 2015-11-15 03:49:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/__init__.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    47697 2015-11-15 03:49:58.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/msvs_emulation.py
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)      536 2013-11-26 08:32:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/setup.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/buildbot/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4228 2015-11-15 03:49:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/buildbot/buildbot_run.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/console-control-strings/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4475 2016-06-15 23:28:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/console-control-strings/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    16567 2016-12-06 15:47:48.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/faye-websocket/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    12372 2015-07-08 19:28:20.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/faye-websocket/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2893 2015-07-08 20:09:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/faye-websocket/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compressible/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1865 2017-03-24 04:39:24.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compressible/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1193 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compressible/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/async-foreach/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4977 2013-04-29 12:54:57.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/async-foreach/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx-self/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      683 2016-12-08 15:43:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx-self/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-deceiver/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1363 2015-11-16 22:23:56.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-deceiver/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/parse-asn1/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      421 2016-11-28 20:06:19.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/parse-asn1/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-sticky-regex/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      529 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-sticky-regex/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-svg/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      828 2016-11-04 14:28:29.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-svg/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regenerate/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    12583 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regenerate/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esrecurse/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esrecurse/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esrecurse/node_modules/estraverse/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4161 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esrecurse/node_modules/estraverse/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/base64-js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1005 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/base64-js/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mixin-object/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2824 2015-07-05 05:54:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mixin-object/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mixin-object/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mixin-object/node_modules/for-in/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3112 2016-03-27 14:56:29.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mixin-object/node_modules/for-in/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/for-own/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3465 2016-03-27 15:06:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/for-own/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-shorthand-properties/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      807 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-shorthand-properties/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/alphanum-sort/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      808 2015-10-03 19:46:39.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/alphanum-sort/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-builtin-module/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      625 2015-05-04 15:46:42.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-builtin-module/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cookie-signature/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1490 2014-06-19 01:26:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cookie-signature/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      695 2015-02-03 22:10:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cookie-signature/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cookie/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8208 2016-05-27 04:01:25.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cookie/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2626 2016-05-27 04:21:40.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cookie/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/indent-string/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      988 2015-07-25 19:15:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/indent-string/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babylon/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5894 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babylon/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    32311 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babylon/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tough-cookie/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    26050 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tough-cookie/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/coa/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    22636 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/coa/README.ru.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    12006 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/coa/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cssesc/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6289 2013-08-09 13:21:42.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cssesc/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hosted-git-info/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4070 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hosted-git-info/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/user-home/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      724 2015-06-13 12:36:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/user-home/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-callable/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1978 2015-08-12 19:17:54.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-callable/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1815 2016-02-28 00:49:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-callable/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shallow-clone/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2592 2015-10-17 17:57:53.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shallow-clone/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/kind-of/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6177 2015-05-31 20:29:42.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/kind-of/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/lazy-cache/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2944 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/lazy-cache/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/combined-stream/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4551 2015-06-14 15:08:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/combined-stream/Readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/right-align/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2066 2015-06-09 05:57:37.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/right-align/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/string-width/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1156 2016-08-13 20:30:48.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/string-width/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-async-to-generator/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      837 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-async-to-generator/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-date-object/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1751 2015-08-12 05:57:54.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-date-object/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      421 2015-09-27 13:14:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-date-object/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/elliptic/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6593 2017-02-06 23:08:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/elliptic/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-remap-async-to-generator/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       56 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-remap-async-to-generator/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/watchpack/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3092 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/watchpack/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/timers-browserify/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1197 2015-02-23 16:03:54.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/timers-browserify/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2039 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/timers-browserify/CHANGELOG.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2505 2012-05-26 02:27:10.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/timers-browserify/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/finalhandler/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3968 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/finalhandler/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3317 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/finalhandler/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/assert/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2307 2016-05-06 19:07:33.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/assert/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/source-list-map/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2437 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/source-list-map/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/camelcase-keys/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/camelcase-keys/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/camelcase-keys/node_modules/camelcase/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1045 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/camelcase-keys/node_modules/camelcase/readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      847 2016-03-15 14:20:09.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/camelcase-keys/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/natural-compare/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3352 2016-07-22 20:48:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/natural-compare/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/url/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3604 2015-08-27 15:36:24.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/url/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/url/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/url/node_modules/punycode/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5988 2014-08-31 16:09:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/url/node_modules/punycode/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-spread/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      654 2016-12-08 15:43:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-spread/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/buffer/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    16577 2016-08-09 00:59:55.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/buffer/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1529 2016-08-18 03:46:30.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/buffer/AUTHORS.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prop-types/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5268 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prop-types/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    16921 2017-03-02 23:05:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/is-extglob/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3469 2016-09-03 19:12:15.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/is-extglob/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/is-glob/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5219 2016-09-03 19:14:26.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/is-glob/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5358 2017-03-02 23:02:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json-loader/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      379 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json-loader/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/read-pkg-up/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1710 2015-09-03 05:22:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/read-pkg-up/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-types/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    40446 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-types/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-export-extensions/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      474 2016-03-21 23:00:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-export-extensions/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-calc/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3201 2016-07-11 04:52:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-calc/README.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2183 2016-08-22 08:58:37.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-calc/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pluralize/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2228 2015-09-17 03:34:01.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pluralize/Readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-call-delegate/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       45 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-call-delegate/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/builtin-status-codes/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      610 2015-11-17 22:20:35.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/builtin-status-codes/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ripemd160/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1894 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ripemd160/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      897 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ripemd160/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/camelcase/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1045 2015-11-12 18:54:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/camelcase/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-messages/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      272 2017-01-20 05:35:55.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-messages/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-get-function-arity/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       50 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-get-function-arity/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/find-cache-dir/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2827 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/find-cache-dir/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/which-module/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1933 2016-06-06 05:50:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/which-module/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      331 2016-06-06 05:53:30.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/which-module/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/enhanced-resolve/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3168 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/enhanced-resolve/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/set-blocking/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1538 2016-05-17 22:57:19.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/set-blocking/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      718 2016-05-17 22:58:30.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/set-blocking/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack-dev-middleware/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6697 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack-dev-middleware/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/merge-descriptors/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1213 2015-05-22 03:38:01.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/merge-descriptors/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      363 2016-01-17 23:41:34.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/merge-descriptors/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esutils/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6655 2015-03-11 15:11:56.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esutils/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-commonjs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2741 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-commonjs/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fstream/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2345 2015-09-09 23:40:40.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fstream/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-reduce-idents/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5078 2017-01-04 18:09:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-reduce-idents/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      943 2017-01-04 18:11:15.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-reduce-idents/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-primitive/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1055 2015-03-17 03:56:35.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-primitive/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-regenerator/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1239 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-regenerator/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/stdout-stream/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1009 2015-06-23 06:32:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/stdout-stream/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/react/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      849 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/react/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-equal-shallow/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2775 2015-06-23 03:39:48.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-equal-shallow/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/extsprintf/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1169 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/extsprintf/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/emojis-list/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1893 2016-10-03 14:00:23.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/emojis-list/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3027 2016-10-03 14:00:58.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/emojis-list/CHANGELOG.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1084 2015-04-19 20:40:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/emojis-list/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-react/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1241 2017-04-01 14:50:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-react/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-svgo/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5298 2016-12-17 15:02:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-svgo/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1246 2016-12-17 15:15:25.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-svgo/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ms/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1832 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ms/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1077 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ms/LICENSE.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1721 2017-05-16 12:24:53.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ms/readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1077 2017-05-16 12:22:00.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ms/license.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-duplicates/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3281 2017-02-26 19:18:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-duplicates/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1492 2017-02-26 19:17:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-duplicates/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-type/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      728 2015-09-04 08:27:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-type/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/to-arraybuffer/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      940 2016-01-13 04:01:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/to-arraybuffer/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pinkie-promise/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      751 2016-04-10 17:37:01.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pinkie-promise/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-code-frame/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1204 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-code-frame/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-colormin/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1363 2016-03-01 21:02:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-colormin/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2416 2017-02-06 17:36:39.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-colormin/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7504 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5646 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/node_modules/ms/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      933 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/node_modules/ms/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1307 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/node_modules/ms/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/node_modules/debug/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6310 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/node_modules/debug/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5611 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/node_modules/debug/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fastparse/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3265 2015-05-24 18:14:54.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fastparse/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/parse-json/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1273 2015-08-31 16:21:26.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/parse-json/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-plain-obj/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      631 2015-07-11 11:06:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-plain-obj/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/on-headers/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1929 2015-02-15 19:58:54.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/on-headers/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      296 2015-09-30 03:43:50.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/on-headers/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cli-width/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1814 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cli-width/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fbjs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2903 2017-03-29 23:45:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fbjs/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fbjs/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fbjs/node_modules/core-js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    22838 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fbjs/node_modules/core-js/CHANGELOG.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4577 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fbjs/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-define-map/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       42 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-define-map/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2897 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1443 2017-03-10 13:04:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/CONTRIBUTING.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/doc/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/doc/wg-meetings/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2280 2016-09-29 06:59:25.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/doc/wg-meetings/2015-01-30.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/node_modules/string_decoder/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1113 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/node_modules/string_decoder/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5550 2017-03-10 13:04:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/GOVERNANCE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/querystring/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1081 2012-10-23 20:34:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/querystring/License.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      331 2013-03-05 21:31:48.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/querystring/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      357 2013-03-05 21:32:31.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/querystring/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.memoize/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      460 2016-08-13 17:33:14.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.memoize/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/supports-color/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1491 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/supports-color/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/del/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2422 2016-08-13 00:03:37.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/del/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ua-parser-js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10381 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ua-parser-js/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-libs-browser/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4015 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-libs-browser/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/aws4/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    16755 2016-10-11 22:34:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/aws4/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-dynamic-import/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      452 2016-10-24 19:15:50.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-dynamic-import/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/har-schema/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2117 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/har-schema/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/randombytes/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      575 2016-01-13 13:14:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/randombytes/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uniq/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1221 2013-03-31 02:52:01.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uniq/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esquery/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2048 2017-03-10 23:08:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esquery/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-reduce-transforms/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1269 2015-10-05 19:19:01.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-reduce-transforms/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      373 2016-11-01 14:47:14.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-reduce-transforms/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdx-license-ids/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1598 2015-08-17 06:36:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdx-license-ids/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/trim-newlines/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      953 2015-09-29 09:22:47.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/trim-newlines/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/reduce-css-calc/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1531 2016-02-22 06:29:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/reduce-css-calc/README.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2389 2016-08-26 11:03:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/reduce-css-calc/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pinkie/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2691 2016-02-01 10:28:24.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pinkie/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nopt/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7690 2015-11-12 21:18:50.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nopt/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/icss-replace-symbols/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      988 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/icss-replace-symbols/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sshpk/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    21169 2017-04-13 01:18:41.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sshpk/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/wide-align/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1551 2015-12-16 05:57:07.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/wide-align/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/stream-http/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6509 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/stream-http/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/aws-sign2/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      130 2013-04-22 05:13:39.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/aws-sign2/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-loader/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    13163 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-loader/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-loader/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-loader/node_modules/css-selector-tokenizer/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2405 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-loader/node_modules/css-selector-tokenizer/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1641 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-loader/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/run-async/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1266 2014-08-11 01:10:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/run-async/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ansi-styles/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1448 2016-03-28 20:32:20.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ansi-styles/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-signature/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    13849 2016-01-25 22:01:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-signature/http_signing.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1594 2015-10-14 21:20:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-signature/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1350 2016-01-25 22:03:07.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-signature/CHANGES.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-signature/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-signature/node_modules/assert-plus/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4618 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-signature/node_modules/assert-plus/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      219 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-signature/node_modules/assert-plus/CHANGES.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/util-deprecate/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1666 2014-11-25 20:05:41.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/util-deprecate/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      282 2015-10-07 18:37:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/util-deprecate/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/write/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2851 2015-07-29 19:13:56.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/write/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/safe-buffer/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    19324 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/safe-buffer/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack-dev-server/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2681 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack-dev-server/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-to-regexp/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1102 2015-07-28 02:27:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-to-regexp/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      694 2015-07-28 03:06:47.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-to-regexp/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fill-range/
+-rwxr--r--   0 davecap   (1000) davecap   (1000)     6701 2015-04-07 08:50:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fill-range/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fill-range/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fill-range/node_modules/isobject/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2999 2016-04-25 21:03:56.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fill-range/node_modules/isobject/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/qs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    13292 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/qs/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10370 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/qs/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/clap/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      662 2015-08-30 19:25:57.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/clap/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      491 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/clap/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color-convert/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2853 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color-convert/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1417 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color-convert/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/normalize-url/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3344 2017-01-09 17:47:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/normalize-url/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-extglob/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1912 2015-03-06 21:00:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-extglob/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-gradients/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3091 2016-10-19 14:08:11.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-gradients/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      524 2016-11-01 00:02:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-gradients/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cssnano/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2449 2016-11-25 21:24:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cssnano/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    11849 2017-01-03 22:22:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cssnano/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)      920 2017-02-28 21:46:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/node_modules/acorn/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    16810 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/node_modules/acorn/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6233 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/node_modules/acorn/CHANGELOG.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      233 2017-02-28 21:46:54.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/rechoir/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2018 2015-07-22 12:11:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/rechoir/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/convert-source-map/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4419 2017-03-28 09:07:55.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/convert-source-map/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/opn/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2224 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/opn/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/crypto-browserify/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1604 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/crypto-browserify/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strip-ansi/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      801 2016-02-21 12:14:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strip-ansi/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/co/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5382 2015-07-09 22:27:26.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/co/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3629 2015-07-09 22:29:39.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/co/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/brace-expansion/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3657 2017-04-07 08:13:12.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/brace-expansion/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/range-parser/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1996 2016-06-01 16:06:29.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/range-parser/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      832 2016-06-01 16:47:14.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/range-parser/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-typedarray/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      558 2014-06-01 19:09:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-typedarray/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1073 2014-06-01 19:08:03.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-typedarray/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/domain-browser/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7869 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/domain-browser/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1381 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/domain-browser/HISTORY.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1348 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/domain-browser/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-map/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2238 2017-01-13 10:33:18.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-map/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/source-map/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    23480 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/source-map/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7884 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/source-map/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/query-string/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4955 2017-04-17 05:51:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/query-string/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hpack.js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1860 2016-03-24 16:14:30.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hpack.js/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-decorators/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      432 2016-03-21 23:00:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-decorators/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/center-align/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1950 2015-10-27 09:26:20.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/center-align/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/builtin-modules/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      957 2015-09-01 17:27:52.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/builtin-modules/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-replace-supers/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       46 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-replace-supers/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/braces/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6629 2016-05-21 15:12:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/braces/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/table/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    15847 2016-09-17 20:02:56.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/table/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/table/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/table/node_modules/string-width/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1156 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/table/node_modules/string-width/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/table/node_modules/is-fullwidth-code-point/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      836 2016-09-22 06:35:00.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/table/node_modules/is-fullwidth-code-point/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-font-values/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1748 2016-02-08 01:16:37.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-font-values/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-jsx/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      369 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-jsx/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-flatten/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1245 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-flatten/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserslist/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8921 2017-03-03 09:54:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserslist/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3169 2017-03-21 08:08:33.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserslist/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object.omit/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4646 2016-10-27 06:23:10.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object.omit/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-flow/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      675 2017-02-13 02:45:24.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-flow/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loose-envify/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1071 2016-05-15 03:29:30.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loose-envify/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/minimalistic-crypto-utils/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1882 2017-02-22 21:12:33.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/minimalistic-crypto-utils/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/batch/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1822 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/batch/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1271 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/batch/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-reduce-initial/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2722 2016-12-22 16:40:07.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-reduce-initial/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      105 2016-12-22 16:40:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-reduce-initial/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-hoist-variables/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       47 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-hoist-variables/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/delegates/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1768 2015-12-14 19:55:23.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/delegates/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      336 2015-12-14 19:55:48.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/delegates/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-empty/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1149 2015-08-13 11:22:07.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-empty/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      427 2016-04-26 15:55:50.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-empty/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-convert-values/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5380 2017-02-03 18:57:50.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-convert-values/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3319 2017-02-03 19:01:26.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-convert-values/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/create-ecdh/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      669 2015-10-29 12:49:13.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/create-ecdh/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-overridden/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2603 2016-04-27 03:21:30.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-overridden/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)        0 2016-04-26 10:57:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-overridden/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-traverse/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       17 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-traverse/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/glob-parent/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1518 2015-09-18 14:58:10.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/glob-parent/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/events/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      371 2016-06-22 15:53:40.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/events/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      760 2016-06-22 16:09:10.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/events/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs-client/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    15712 2017-01-22 19:46:46.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs-client/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8717 2017-01-23 23:43:09.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs-client/Changelog.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/faye-websocket/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    12576 2017-01-22 19:44:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/faye-websocket/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      162 2015-11-08 12:15:20.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/faye-websocket/CODE_OF_CONDUCT.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3140 2017-01-22 19:45:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/faye-websocket/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-optimise-call-expression/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       56 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-optimise-call-expression/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-computed-properties/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1816 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-computed-properties/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mime/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2119 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mime/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/reduce-function-call/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1651 2016-11-28 07:19:41.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/reduce-function-call/README.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)      265 2016-11-28 07:22:17.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/reduce-function-call/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/evp_bytestokey/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1770 2017-09-05 10:20:26.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/evp_bytestokey/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      383 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/evp_bytestokey/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-des/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       39 2015-09-27 17:30:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-des/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/minimatch/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6336 2016-02-20 22:10:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/minimatch/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-es2015/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      865 2017-04-01 14:50:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-es2015/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-jsx/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2751 2016-05-02 16:02:15.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-jsx/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-jsx/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-jsx/node_modules/acorn/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    16680 2016-06-07 11:28:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-jsx/node_modules/acorn/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3444 2016-07-25 21:22:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-jsx/node_modules/acorn/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-aes/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      802 2017-10-10 12:30:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-aes/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      780 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-aes/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-path-in-cwd/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      523 2014-06-20 22:20:41.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-path-in-cwd/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/preserve/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1335 2015-01-10 12:25:52.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/preserve/.verb.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2230 2015-01-10 22:21:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/preserve/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-for-of/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2406 2017-01-20 05:35:55.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-for-of/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-block-scoped-functions/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      604 2016-12-08 15:43:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-block-scoped-functions/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/repeat-string/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5057 2016-10-23 08:00:31.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/repeat-string/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-plain-object/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2598 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-plain-object/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.uniq/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      439 2016-08-13 17:34:12.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.uniq/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-stream/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      664 2016-04-12 07:19:14.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-stream/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caller-path/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      726 2014-04-19 10:18:24.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caller-path/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pako/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5340 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pako/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1537 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pako/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color-name/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      384 2017-03-14 02:54:03.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color-name/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-property/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      625 2013-07-18 14:04:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-property/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/binary-extensions/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      759 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/binary-extensions/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/parseurl/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3463 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/parseurl/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      832 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/parseurl/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-unused/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4345 2016-11-21 17:51:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-unused/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      809 2016-11-21 17:51:07.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-unused/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/destroy/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2185 2016-01-13 16:29:37.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/destroy/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/unpipe/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1250 2015-06-14 20:29:42.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/unpipe/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       59 2015-06-14 20:29:42.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/unpipe/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/indexes-of/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      320 2013-11-16 09:01:14.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/indexes-of/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/negotiator/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4811 2016-05-03 04:32:15.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/negotiator/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2296 2016-05-03 04:43:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/negotiator/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/to-fast-properties/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      733 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/to-fast-properties/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-regex/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1624 2017-01-10 22:24:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-regex/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1109 2017-02-18 08:12:31.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-regex/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readline2/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1541 2015-07-17 06:53:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readline2/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/decamelize/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      781 2016-03-05 08:48:07.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/decamelize/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hash.js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1255 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hash.js/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/async-each/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1122 2016-08-24 23:21:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/async-each/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      593 2016-08-24 23:17:25.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/async-each/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1054 2016-08-06 16:40:01.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    12535 2017-02-23 18:05:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/API.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4632 2017-02-23 18:21:00.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-params/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      663 2016-09-30 16:51:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-params/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      580 2016-12-28 10:45:12.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-params/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/vendors/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      964 2016-08-11 10:41:50.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/vendors/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/errno/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4415 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/errno/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/core-util-is/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       67 2015-11-20 00:23:19.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/core-util-is/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ajv/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    65968 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ajv/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ajv/lib/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ajv/lib/dotjs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      149 2017-04-06 18:04:40.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ajv/lib/dotjs/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ee-first/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2617 2015-05-25 18:17:03.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ee-first/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdy-transport/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2246 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdy-transport/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/yargs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    53446 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/yargs/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    63371 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/yargs/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/slice-ansi/
+-rwxr--r--   0 davecap   (1000) davecap   (1000)     1176 2015-09-26 07:54:33.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/slice-ansi/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint-plugin-react/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)    12746 2017-03-19 16:25:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint-plugin-react/README.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)    77312 2017-03-20 21:46:54.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint-plugin-react/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fast-levenshtein/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3414 2016-09-07 04:51:17.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fast-levenshtein/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1100 2014-12-06 02:56:29.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fast-levenshtein/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/optionator/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    14932 2016-09-21 19:42:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/optionator/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1771 2016-09-21 19:42:25.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/optionator/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/wbuf/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1127 2016-05-04 20:27:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/wbuf/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isstream/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2424 2015-03-07 00:14:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isstream/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1125 2015-03-07 00:14:31.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isstream/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/error-ex/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4143 2016-11-24 18:33:26.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/error-ex/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/util/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      409 2013-11-22 18:19:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/util/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/util/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/util/node_modules/inherits/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1625 2013-05-16 14:24:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/util/node_modules/inherits/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/micromatch/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    19913 2016-07-15 17:13:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/micromatch/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-path-cwd/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      474 2014-06-19 10:18:10.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-path-cwd/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-object-rest-spread/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1441 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-object-rest-spread/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esprima/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2333 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esprima/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/balanced-match/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3308 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/balanced-match/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1096 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/balanced-match/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-stage-0/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      391 2017-04-01 14:50:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-stage-0/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/y18n/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2365 2016-03-17 05:01:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/y18n/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/style-loader/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6258 2017-03-22 13:43:50.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/style-loader/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2519 2017-03-28 13:28:42.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/style-loader/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/style-loader/.github/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      716 2017-02-24 16:02:11.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/style-loader/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      733 2017-02-24 16:02:11.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/style-loader/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/constants-browserify/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1668 2015-07-13 18:14:07.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/constants-browserify/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/get-stdin/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      571 2014-08-17 19:16:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/get-stdin/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-classes/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1778 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-classes/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3523 2016-03-28 18:13:37.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/graceful-fs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4454 2016-09-26 21:37:48.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/graceful-fs/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-glob/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3218 2015-10-02 04:34:15.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-glob/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-filter-plugins/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3821 2016-07-12 14:03:47.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-filter-plugins/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      296 2016-10-03 16:27:35.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-filter-plugins/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/html-entities/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2364 2017-04-24 11:44:25.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/html-entities/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/encodeurl/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3613 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/encodeurl/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      159 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/encodeurl/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/imurmurhash/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4763 2013-08-11 11:48:48.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/imurmurhash/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-async-generators/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      477 2016-03-21 23:00:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-async-generators/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/portfinder/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1333 2017-01-31 14:42:41.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/portfinder/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/portfinder/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/portfinder/node_modules/async/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    60782 2016-01-07 23:18:07.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/portfinder/node_modules/async/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5398 2016-01-08 00:03:29.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/portfinder/node_modules/async/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ramda/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6695 2017-06-02 04:46:26.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ramda/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      117 2017-05-05 18:02:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ramda/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/rx-lite/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8938 2015-08-14 19:47:34.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/rx-lite/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hawk/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)    31409 2016-01-21 18:20:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hawk/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/promise/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     9295 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/promise/Readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ecc-jsbn/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      402 2014-08-24 04:10:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ecc-jsbn/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-value-parser/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7650 2016-02-18 17:35:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-value-parser/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/autoprefixer/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    17201 2017-03-11 11:27:20.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/autoprefixer/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    21804 2017-03-11 11:27:20.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/autoprefixer/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/escape-html/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      707 2015-09-01 04:46:01.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/escape-html/Readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    14669 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/docs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3188 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/docs/source-maps.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7916 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/docs/syntax.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/docs/guidelines/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4489 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/docs/guidelines/runner.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5994 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/docs/guidelines/plugin.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    15274 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/get-caller-file/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      316 2016-08-09 00:43:20.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/get-caller-file/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caseless/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1173 2014-10-29 18:52:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caseless/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strip-json-comments/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1493 2015-11-18 14:02:54.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strip-json-comments/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/currently-unhandled/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1501 2016-06-02 10:38:24.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/currently-unhandled/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-literals/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      859 2016-12-08 15:43:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-literals/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caniuse-db/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      833 2017-04-12 02:49:09.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caniuse-db/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7081 2017-04-23 22:33:55.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caniuse-db/CONTRIBUTING.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/os-homedir/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      735 2016-09-30 04:57:23.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/os-homedir/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack-sources/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5131 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack-sources/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack-sources/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack-sources/node_modules/source-list-map/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2554 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack-sources/node_modules/source-list-map/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prelude-ls/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      613 2014-10-01 01:42:58.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prelude-ls/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3989 2015-05-15 02:39:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prelude-ls/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-loader/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     9822 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-loader/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6585 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-loader/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/form-data/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6437 2017-04-09 15:09:56.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/form-data/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-function-bind/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      450 2016-03-21 23:00:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-function-bind/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/original/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1787 2014-11-08 16:04:46.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/original/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/original/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/original/node_modules/url-parse/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5159 2015-10-30 14:42:40.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/original/node_modules/url-parse/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.mergewith/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      474 2016-08-13 17:34:37.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.mergewith/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loud-rejection/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1719 2016-07-03 22:00:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loud-rejection/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/react-dom/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      897 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/react-dom/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tar/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1298 2015-09-10 01:47:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tar/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cross-spawn/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2605 2016-05-18 13:23:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cross-spawn/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.assign/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      453 2016-08-13 17:33:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.assign/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-do-expressions/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      456 2016-03-21 23:00:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-do-expressions/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json-schema/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      405 2016-09-03 02:53:20.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json-schema/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asynckit/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7640 2016-06-14 18:28:19.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asynckit/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-async-functions/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      462 2016-03-21 23:00:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-async-functions/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object-assign/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1502 2016-11-04 02:19:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object-assign/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-binary-path/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      696 2015-04-07 08:14:18.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-binary-path/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regenerator-transform/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      719 2016-05-30 19:47:37.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regenerator-transform/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/progress/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2365 2014-03-30 13:46:56.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/progress/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2017 2014-07-01 02:16:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/progress/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/setprototypeof/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      401 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/setprototypeof/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/yargs-parser/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6665 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/yargs-parser/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6054 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/yargs-parser/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-tokens/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6522 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-tokens/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3725 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-tokens/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-bindify-decorators/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       50 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-bindify-decorators/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-unique-selectors/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1156 2015-08-25 12:53:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-unique-selectors/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      248 2016-02-07 00:32:46.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-unique-selectors/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    12111 2017-03-31 19:56:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint/node_modules/doctrine/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6470 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint/node_modules/doctrine/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3076 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint/node_modules/doctrine/CHANGELOG.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)   273638 2017-03-31 20:05:15.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/slash/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      890 2014-08-13 10:14:42.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/slash/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/performance-now/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1985 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/performance-now/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-sign/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      857 2016-05-12 14:30:13.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-sign/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-extendable/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2546 2015-07-04 22:50:02.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-extendable/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-zindex/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2462 2016-11-25 16:47:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-zindex/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1117 2016-11-25 16:53:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-zindex/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-my-json-valid/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4962 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-my-json-valid/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-static/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7508 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-static/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8185 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-static/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tunnel-agent/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      113 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tunnel-agent/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/require-uncached/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      833 2016-11-03 06:59:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/require-uncached/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/argparse/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8172 2016-03-17 14:49:34.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/argparse/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3341 2016-09-29 19:26:03.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/argparse/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    16810 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7033 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/create-hmac/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1083 2017-04-27 14:33:47.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/create-hmac/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      720 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/create-hmac/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ansi-regex/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1749 2017-01-14 03:03:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ansi-regex/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-comments/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2796 2016-02-10 16:59:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-comments/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1727 2016-02-10 16:59:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-comments/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-utf8/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      397 2015-12-19 03:59:50.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-utf8/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uniqs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1204 2014-06-03 08:27:53.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uniqs/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/utils-merge/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      634 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/utils-merge/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-selectors/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1147 2016-01-11 11:31:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-selectors/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2541 2016-12-31 12:39:58.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-selectors/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-idents/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1649 2016-02-07 00:48:47.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-idents/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1079 2016-08-16 19:46:39.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-idents/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/globule/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6460 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/globule/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/globule/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/globule/node_modules/lodash/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1120 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/globule/node_modules/lodash/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/d/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2724 2015-06-25 13:18:23.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/d/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    43529 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    53650 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs-parser/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5614 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs-parser/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1960 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs-parser/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/window-size/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1783 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/window-size/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1934 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/CHANGELOG.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2598 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/block-stream/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      369 2011-10-07 03:09:34.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/block-stream/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strip-indent/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      957 2014-08-13 13:44:37.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strip-indent/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regex-cache/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5314 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regex-cache/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/dashdash/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    18164 2016-01-18 19:18:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/dashdash/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10912 2016-11-22 22:33:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/dashdash/CHANGES.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regjsparser/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      440 2015-02-27 23:46:17.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regjsparser/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regjsparser/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regjsparser/node_modules/jsesc/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    12447 2014-05-25 09:18:35.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regjsparser/node_modules/jsesc/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/bcrypt-pbkdf/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1359 2017-02-02 03:51:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/bcrypt-pbkdf/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ignore/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     6666 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ignore/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-values/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1175 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-values/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/html-comment-regex/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      974 2015-05-21 08:08:52.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/html-comment-regex/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/process/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1359 2015-09-08 15:14:50.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/process/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/content-disposition/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5148 2016-12-09 01:01:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/content-disposition/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      866 2016-12-09 01:16:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/content-disposition/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/exit-hook/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      676 2014-08-31 23:27:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/exit-hook/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/delayed-stream/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3871 2015-04-27 18:43:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/delayed-stream/Readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/extglob/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3242 2015-08-01 20:11:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/extglob/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/requires-port/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1814 2014-11-08 15:59:03.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/requires-port/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sort-keys/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1002 2016-05-18 04:43:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sort-keys/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tapable/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4813 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tapable/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hmac-drbg/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1723 2017-02-22 21:41:57.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hmac-drbg/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-template-literals/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1116 2016-12-08 15:43:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-template-literals/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/invert-kv/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      480 2014-06-26 20:07:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/invert-kv/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/media-typer/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2371 2014-09-08 04:06:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/media-typer/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      461 2014-09-08 04:30:34.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/media-typer/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/etag/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4208 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/etag/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1640 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/etag/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-zlib/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      722 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-zlib/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/gauge/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    15073 2016-11-03 21:33:48.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/gauge/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6376 2017-04-21 23:05:55.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/gauge/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/on-finished/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4886 2015-05-26 02:27:15.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/on-finished/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1694 2015-05-27 01:18:07.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/on-finished/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-resolvable/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2206 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-resolvable/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fs.realpath/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      881 2016-06-15 18:27:25.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fs.realpath/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/forever-agent/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      163 2015-03-21 11:48:42.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/forever-agent/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    14123 2017-01-29 18:01:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/README.ru.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10540 2017-01-29 17:57:33.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/node_modules/esprima/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2006 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/node_modules/esprima/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/node_modules/js-yaml/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     9283 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/node_modules/js-yaml/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     9054 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/node_modules/js-yaml/CHANGELOG.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    31474 2017-01-29 17:57:33.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-yaml/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     9709 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-yaml/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     9619 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-yaml/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-posix-bracket/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3212 2016-04-05 05:30:30.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-posix-bracket/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/anymatch/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3884 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/anymatch/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/has-ansi/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      856 2015-06-30 16:13:09.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/has-ansi/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-systemjs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1013 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-systemjs/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/math-expression-evaluator/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3562 2017-02-02 07:48:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/math-expression-evaluator/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-path-inside/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      514 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-path-inside/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json3/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     9293 2014-06-22 21:15:11.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json3/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/chokidar/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    13069 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/chokidar/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     9832 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/chokidar/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/define-properties/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2725 2015-10-14 22:16:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/define-properties/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      972 2015-10-14 22:22:54.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/define-properties/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-buffer/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1504 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-buffer/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/load-json-file/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/load-json-file/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/load-json-file/node_modules/strip-bom/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      902 2015-06-29 13:11:39.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/load-json-file/node_modules/strip-bom/readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      951 2015-11-08 13:46:23.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/load-json-file/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.clonedeep/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      474 2016-08-13 17:34:12.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.clonedeep/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/callsites/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1896 2014-04-19 10:11:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/callsites/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-export-extensions/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1082 2016-12-08 15:43:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-export-extensions/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsbn/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1623 2017-02-12 07:42:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsbn/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/statuses/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2746 2016-11-12 02:35:26.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/statuses/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      887 2016-11-12 04:00:10.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/statuses/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/code-point-at/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      617 2016-11-03 10:06:35.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/code-point-at/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/aproba/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2594 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/aproba/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx-source/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      636 2016-12-08 15:43:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx-source/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-umd/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4581 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-umd/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/has-flag/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      927 2015-07-07 22:30:14.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/has-flag/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs/examples/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs/examples/echo/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      355 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs/examples/echo/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs/examples/multiplex/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      697 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs/examples/multiplex/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    16405 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs/tests/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs/tests/test_server/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      737 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs/tests/test_server/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color-string/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1274 2015-02-19 06:58:18.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color-string/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      386 2015-02-19 07:21:40.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color-string/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-generator/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4200 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-generator/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/circular-json/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4371 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/circular-json/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/type-is/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4161 2017-03-25 04:58:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/type-is/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3923 2017-04-01 03:15:33.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/type-is/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsprim/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    11023 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsprim/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      895 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsprim/CHANGES.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-function-name/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      531 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-function-name/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es5-ext/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    38986 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es5-ext/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/console-browserify/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      544 2014-04-08 02:54:18.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/console-browserify/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/private/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7958 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/private/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-driver/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    13736 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-driver/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      162 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-driver/CODE_OF_CONDUCT.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2966 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-driver/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/depd/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10142 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/depd/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1839 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/depd/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/remove-trailing-separator/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      236 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/remove-trailing-separator/history.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1789 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/remove-trailing-separator/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-builder-react-jsx/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      709 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-builder-react-jsx/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/espree/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7931 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/espree/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    15373 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/espree/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sprintf-js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4855 2015-07-10 13:33:43.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sprintf-js/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/encoding/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1392 2015-12-23 09:05:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/encoding/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-exists/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1217 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-exists/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/whet.extend/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      507 2012-05-24 15:14:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/whet.extend/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      513 2013-01-27 21:37:52.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/whet.extend/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cryptiles/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      599 2015-09-09 06:08:12.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cryptiles/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/which/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1154 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/which/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2339 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/which/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-set/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1940 2017-01-12 15:43:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-set/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-check-es2015-constants/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1068 2017-01-07 22:18:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-check-es2015-constants/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regenerator-runtime/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      758 2016-05-02 15:31:09.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regenerator-runtime/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-class-properties/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      468 2016-03-21 23:00:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-class-properties/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ansi-html/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1395 2015-11-21 10:15:48.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ansi-html/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-cipher/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      302 2015-09-27 18:34:58.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-cipher/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/date-now/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      824 2013-02-09 03:02:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/date-now/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prepend-http/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      577 2016-05-10 05:18:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prepend-http/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isarray/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1890 2015-12-10 10:04:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isarray/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/inherits/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1625 2013-05-16 14:24:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/inherits/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-runtime/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       17 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-runtime/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array.prototype.find/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1327 2016-11-08 08:33:50.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array.prototype.find/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1210 2017-03-30 18:50:57.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array.prototype.find/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-selector-tokenizer/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2405 2015-06-12 03:43:48.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-selector-tokenizer/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/oauth-sign/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      107 2016-05-04 21:10:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/oauth-sign/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/has-unicode/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1388 2015-11-26 00:54:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/has-unicode/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/arr-flatten/
+-rwxr--r--   0 davecap   (1000) davecap   (1000)     3549 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/arr-flatten/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-template/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1233 2017-04-01 14:50:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-template/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-arrayish/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      704 2015-08-25 17:01:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-arrayish/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-class-constructor-call/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2324 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-class-constructor-call/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/electron-to-chromium/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5320 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/electron-to-chromium/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      296 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/electron-to-chromium/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uniqid/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3406 2017-01-07 17:52:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uniqid/Readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/os-tmpdir/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      693 2016-09-30 04:50:25.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/os-tmpdir/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/gaze/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8132 2016-09-27 19:30:42.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/gaze/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    41777 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/camelcase/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      889 2015-07-30 15:11:13.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/camelcase/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/yargs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    22253 2015-05-29 04:23:14.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/yargs/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    37151 2015-05-29 04:30:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/yargs/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/cliui/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2019 2015-04-24 22:33:35.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/cliui/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/debug/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    17918 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/debug/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/debug/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/debug/node_modules/ms/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1832 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/debug/node_modules/ms/readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1077 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/debug/node_modules/ms/license.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10988 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/debug/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/csso/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    15039 2017-03-10 21:36:14.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/csso/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    13476 2017-03-10 21:43:33.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/csso/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ajv-keywords/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    12462 2017-01-22 17:51:02.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ajv-keywords/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ajv-keywords/keywords/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ajv-keywords/keywords/dotjs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      158 2016-12-22 20:46:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ajv-keywords/keywords/dotjs/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/string_decoder/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      498 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/string_decoder/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/interpret/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3612 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/interpret/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-flow-strip-types/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      962 2016-12-08 15:43:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-flow-strip-types/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-explode-class/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       45 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-explode-class/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/invariant/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1613 2016-11-15 11:07:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/invariant/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      684 2016-11-15 11:07:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/invariant/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.tail/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      439 2016-08-13 17:33:11.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.tail/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asn1.js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2480 2015-10-23 21:46:19.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asn1.js/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-register/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2846 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-register/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/concat-stream/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3505 2016-12-19 15:43:58.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/concat-stream/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-arrow-functions/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2403 2016-12-08 15:43:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-arrow-functions/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/clone/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3585 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/clone/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    26687 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/tools/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      456 2017-04-05 22:07:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/tools/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2362 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/scopes.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1900 2017-04-05 22:07:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/string_bytes.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10837 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/persistent.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2121 2017-04-05 22:07:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/buffers.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1513 2017-04-05 22:07:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/callback.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1950 2017-04-05 22:07:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/converters.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7404 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/errors.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2240 2017-04-05 22:07:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/node_misc.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2914 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/v8_misc.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4859 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/new.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7389 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/v8_internals.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3255 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/asyncworker.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8204 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/object_wrappers.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1279 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/script.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    27016 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/methods.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1941 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/json.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    21167 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/maybe_types.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    17639 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/CHANGELOG.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1216 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/event-emitter/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3335 2017-01-10 11:39:53.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/event-emitter/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-base64/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1282 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-base64/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1480 2014-12-06 20:50:57.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-base64/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-extract-imports/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1623 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-extract-imports/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lcid/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      826 2015-03-16 06:56:30.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lcid/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/minimalistic-assert/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       58 2015-01-12 16:19:40.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/minimalistic-assert/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/wrap-ansi/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2026 2016-11-29 17:14:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/wrap-ansi/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-regex/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       37 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-regex/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/public-encrypt/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      195 2015-02-12 13:26:13.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/public-encrypt/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-destructuring/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      513 2017-01-20 05:35:55.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-destructuring/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/flatten/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      460 2016-01-20 00:43:29.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/flatten/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-stage-3/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1181 2017-04-01 14:50:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-stage-3/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/align-text/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5507 2016-02-02 01:50:23.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/align-text/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readdirp/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readdirp/examples/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1076 2014-12-12 21:18:57.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readdirp/examples/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8824 2014-12-12 21:18:57.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readdirp/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/onetime/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      892 2015-12-18 00:17:29.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/onetime/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pkg-dir/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1109 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pkg-dir/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-extensions/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    14241 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-extensions/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-extensions/lib/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-extensions/lib/pipeline/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    24700 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-extensions/lib/pipeline/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      244 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-extensions/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/xtend/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      725 2015-11-02 22:19:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/xtend/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-is-absolute/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1153 2016-09-30 04:41:17.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-is-absolute/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/window-size/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      624 2014-02-15 03:41:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/window-size/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strict-uri-encode/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      666 2016-01-04 06:59:39.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strict-uri-encode/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      854 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/node_modules/regexpu-core/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2808 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/node_modules/regexpu-core/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-normalize-charset/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      805 2016-09-30 16:50:14.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-normalize-charset/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      306 2016-11-08 15:31:25.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-normalize-charset/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-amd/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      900 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-amd/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/signal-exit/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1497 2016-12-02 21:10:47.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/signal-exit/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1071 2016-12-02 21:10:47.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/signal-exit/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/q/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    25386 2017-03-22 02:09:48.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/q/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    29828 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/q/CHANGES.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sha.js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1287 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sha.js/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/connect-history-api-fallback/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4727 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/connect-history-api-fallback/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      935 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/connect-history-api-fallback/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eventemitter3/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3685 2015-06-14 14:05:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eventemitter3/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/buffer-shims/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      497 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/buffer-shims/readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1064 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/buffer-shims/license.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/globby/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2197 2016-06-11 06:17:12.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/globby/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/in-publish/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1130 2015-07-07 19:00:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/in-publish/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdx-correct/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      225 2015-10-26 16:53:56.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdx-correct/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-rules/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1585 2015-10-18 19:27:53.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-rules/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3538 2017-02-20 11:09:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-rules/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-builder-binary-assignment-operator-visitor/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       74 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-builder-binary-assignment-operator-visitor/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-fetch/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6177 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-fetch/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1232 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-fetch/ERROR-HANDLING.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4439 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-fetch/CHANGELOG.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1079 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-fetch/LICENSE.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1341 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-fetch/LIMITS.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-class-properties/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1778 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-class-properties/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-errors/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4640 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-errors/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2120 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-errors/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-errors/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-errors/node_modules/setprototypeof/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      401 2016-02-06 23:38:42.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-errors/node_modules/setprototypeof/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object-keys/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2460 2015-10-14 22:01:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object-keys/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6992 2016-07-05 17:14:10.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object-keys/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pseudomap/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2163 2015-11-28 22:25:20.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pseudomap/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-parameters/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      899 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-parameters/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/find-up/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1271 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/find-up/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8656 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10068 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/node_modules/debug/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8483 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/node_modules/debug/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10364 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/node_modules/debug/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/node_modules/http-errors/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4803 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/node_modules/http-errors/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2548 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/node_modules/http-errors/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/parse-glob/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4017 2015-09-22 15:16:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/parse-glob/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/expand-range/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4391 2016-05-05 09:25:14.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/expand-range/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-finite/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      544 2016-09-30 07:42:48.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-finite/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/restore-cursor/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      359 2014-08-31 23:29:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/restore-cursor/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-ordered-values/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3355 2016-06-23 22:41:47.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-ordered-values/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1293 2017-01-10 11:43:09.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-ordered-values/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/express/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4540 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/express/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)   102583 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/express/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/express/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/express/node_modules/debug/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8483 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/express/node_modules/debug/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10364 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/express/node_modules/debug/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/meow/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3845 2016-01-04 14:11:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/meow/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/handle-thing/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1382 2016-03-02 06:31:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/handle-thing/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fresh/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3236 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fresh/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1220 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fresh/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mime-types/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3104 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mime-types/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3994 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mime-types/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mime-db/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2991 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mime-db/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    11272 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mime-db/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-typeof-symbol/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      960 2017-01-20 05:35:55.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-typeof-symbol/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/are-we-there-yet/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6302 2017-04-21 07:41:17.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/are-we-there-yet/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1107 2017-04-21 07:46:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/are-we-there-yet/CHANGES.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/redent/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      750 2015-09-29 10:53:48.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/redent/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/extend/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2360 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/extend/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2162 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/extend/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-exponentiation-operator/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      514 2016-03-21 23:00:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-exponentiation-operator/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-strict-mode/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1041 2017-04-01 14:50:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-strict-mode/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/map-obj/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      555 2015-05-02 18:02:23.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/map-obj/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es-abstract/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1812 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es-abstract/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4096 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es-abstract/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mute-stream/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1653 2013-07-15 01:14:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mute-stream/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1832 2017-04-01 14:50:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/figures/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4016 2016-05-17 16:58:13.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/figures/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/har-validator/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2891 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/har-validator/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/randomatic/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6151 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/randomatic/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/generate-function/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1748 2014-07-30 17:29:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/generate-function/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uuid/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6393 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uuid/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uuid/benchmark/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2031 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uuid/benchmark/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      100 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uuid/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-longhand/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1326 2015-08-17 15:37:35.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-longhand/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      455 2017-01-13 15:32:00.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-longhand/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/macaddress/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2793 2015-04-26 11:57:23.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/macaddress/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/repeat-element/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1439 2015-05-07 03:15:50.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/repeat-element/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/clone-deep/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3001 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/clone-deep/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regexpu-core/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2808 2016-01-11 16:21:10.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regexpu-core/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lru-cache/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4910 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lru-cache/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/wrappy/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      685 2016-05-17 23:15:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/wrappy/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/home-or-tmp/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      647 2015-05-17 22:13:12.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/home-or-tmp/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/inquirer/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    11124 2015-12-31 23:28:34.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/inquirer/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sntp/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1898 2014-09-05 19:49:55.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sntp/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/miller-rabin/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1135 2015-10-28 20:20:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/miller-rabin/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/stringstream/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1062 2013-01-21 10:47:30.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/stringstream/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/resolve-from/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      992 2015-10-05 14:28:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/resolve-from/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-local-by-default/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1965 2015-06-10 09:55:43.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-local-by-default/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2692 2015-09-19 14:47:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-local-by-default/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-color-names/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      787 2015-09-04 16:30:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-color-names/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/querystring-es3/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1081 2014-10-13 18:58:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/querystring-es3/License.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      367 2014-10-13 18:58:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/querystring-es3/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      357 2014-10-13 18:58:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/querystring-es3/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/methods/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1694 2016-01-18 01:17:30.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/methods/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      427 2016-01-18 02:40:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/methods/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/longest/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2204 2015-03-31 11:37:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/longest/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/detect-indent/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2361 2015-09-07 09:14:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/detect-indent/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cliui/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2355 2016-04-11 02:03:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cliui/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      510 2016-04-11 02:46:52.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cliui/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/validate-npm-package-license/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2561 2015-08-23 23:32:29.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/validate-npm-package-license/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/escope/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3269 2016-03-10 21:49:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/escope/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      402 2015-03-08 02:09:55.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/escope/CONTRIBUTING.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ieee754/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1413 2016-10-03 07:50:52.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ieee754/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/filename-regex/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1025 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/filename-regex/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ipaddr.js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7541 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ipaddr.js/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-exponentiation-operator/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      944 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-exponentiation-operator/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/big.js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7943 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/big.js/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/rimraf/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3600 2015-12-23 18:43:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/rimraf/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/process-nextick-args/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      451 2015-09-09 18:40:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/process-nextick-args/readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1064 2015-09-09 18:40:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/process-nextick-args/license.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/bytes/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3130 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/bytes/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1225 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/bytes/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/source-map-support/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8559 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/source-map-support/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1079 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/source-map-support/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-absolute-url/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      632 2016-10-25 18:44:53.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-absolute-url/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdy/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8098 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdy/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-function-bind/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3656 2017-01-07 22:18:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-function-bind/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cipher-base/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      726 2017-07-06 12:04:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cipher-base/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      726 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cipher-base/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-symbol/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2129 2016-11-11 20:09:00.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-symbol/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-class-constructor-call/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      509 2016-10-21 15:29:24.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-class-constructor-call/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/brorand/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1130 2016-09-06 14:17:10.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/brorand/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    23750 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2800 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2031 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-autotools.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4359 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-importer.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4253 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/custom-functions-internal.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3436 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-mingw.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1281 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-on-gentoo.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1118 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-context-example.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4855 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1596 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/README.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     7760 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/dev-ast-memory.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3471 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-function.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1273 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-value-internal.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2947 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-visual-studio.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4813 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-on-windows.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2149 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-function-example.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)      421 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-importer-internal.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3965 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/unicode.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3512 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-context-internal.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)      164 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-function-internal.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3653 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-importer-example.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1405 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-value-example.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2325 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/source-map-internals.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1915 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/plugins.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1418 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-shared-library.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1600 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-makefiles.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1773 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/triage.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)      792 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-on-darwin.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1622 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/implementations.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     6137 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-value.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     1405 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/contributing.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2899 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/compatibility-plan.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)    11063 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-context.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     7725 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-doc.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)      892 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/trace.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2457 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/setup-environment.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     4351 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/Readme.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)      370 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/SECURITY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/.github/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     3723 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/.github/CONTRIBUTING.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)      448 2018-05-14 19:25:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-object-rest-spread/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      480 2016-03-21 23:00:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-object-rest-spread/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object.assign/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6303 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object.assign/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-duplicate-keys/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1066 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-duplicate-keys/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/repeating/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1282 2016-04-11 17:31:47.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/repeating/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/kind-of/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8177 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/kind-of/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/num2fraction/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2594 2015-09-14 01:50:23.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/num2fraction/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/expand-brackets/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3765 2016-04-01 23:34:57.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/expand-brackets/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/indexof/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      141 2012-08-16 23:38:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/indexof/Readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-loader/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7639 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-loader/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4934 2017-04-21 20:11:39.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-loader/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loader-runner/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1191 2016-09-14 22:08:13.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loader-runner/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tryit/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1601 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tryit/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regjsgen/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1181 2014-09-02 04:33:52.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regjsgen/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/async/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1261 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/async/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    16868 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/async/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-to-browserify/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      574 2014-02-05 12:40:00.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-to-browserify/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/create-hash/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      691 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/create-hash/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-union/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      513 2016-06-16 12:14:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-union/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/glob/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    14664 2016-09-20 18:27:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/glob/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1430 2016-02-11 06:23:26.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/glob/changelog.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/globals/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1411 2016-10-25 18:34:00.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/globals/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/arrify/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      519 2015-12-09 17:46:03.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/arrify/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es-to-primitive/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2174 2015-11-01 03:25:26.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es-to-primitive/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1201 2016-01-04 01:34:54.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es-to-primitive/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/diffie-hellman/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      518 2015-01-27 14:00:29.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/diffie-hellman/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lazy-cache/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3721 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lazy-cache/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loader-utils/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8364 2017-03-16 14:00:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loader-utils/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      736 2017-03-16 14:04:12.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loader-utils/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/core-js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    37340 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/core-js/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pify/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2579 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pify/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-dotfile/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1977 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-dotfile/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-trailing-function-commas/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2617 2016-12-08 15:43:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-trailing-function-commas/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/foreach/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      593 2014-09-22 06:18:56.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/foreach/Readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-fullwidth-code-point/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      833 2015-07-16 21:59:20.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-fullwidth-code-point/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-explode-assignable-expression/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       61 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-explode-assignable-expression/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strip-bom/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      913 2016-04-30 15:51:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strip-bom/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/getpass/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      774 2016-04-21 21:51:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/getpass/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-object-super/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      507 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-object-super/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/require-main-filename/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1064 2016-02-01 05:31:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/require-main-filename/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/punycode/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6115 2015-02-24 22:04:57.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/punycode/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/buffer-xor/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1014 2015-09-25 07:13:39.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/buffer-xor/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-weak-map/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1808 2015-06-25 13:26:46.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-weak-map/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/content-type/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2796 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/content-type/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      265 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/content-type/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/request/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    43747 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/request/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/request/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4644 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      626 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/HISTORY.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1109 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/LICENSE.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    65653 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/request/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eventsource/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2381 2014-12-26 09:41:57.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eventsource/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      234 2015-02-08 23:43:58.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eventsource/CONTRIBUTING.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5137 2015-02-09 08:21:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eventsource/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/select-hose/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1373 2015-07-14 04:36:13.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/select-hose/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/arr-diff/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2194 2015-12-06 04:25:40.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/arr-diff/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/osenv/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1468 2012-06-18 00:50:18.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/osenv/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jodid25519/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2705 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jodid25519/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      162 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jodid25519/AUTHORS.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/file-entry-cache/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4856 2016-08-01 09:48:42.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/file-entry-cache/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3616 2016-08-16 20:48:13.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/file-entry-cache/changelog.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cli-cursor/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      666 2015-09-18 13:45:53.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cli-cursor/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-symbol/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1469 2015-01-24 21:07:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-symbol/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      121 2015-01-26 09:43:10.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-symbol/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ansi-escapes/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3394 2016-04-17 20:33:57.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ansi-escapes/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caniuse-api/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2668 2017-04-06 15:04:56.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caniuse-api/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2107 2017-04-07 07:42:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caniuse-api/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-core/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7547 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-core/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/os-browserify/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      212 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/os-browserify/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-scope/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2305 2015-10-20 07:54:40.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-scope/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/iconv-lite/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6796 2017-04-21 09:01:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/iconv-lite/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3012 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/iconv-lite/Changelog.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/number-is-nan/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      559 2016-09-30 05:10:34.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/number-is-nan/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-normalize-url/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1577 2015-08-13 10:42:53.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-normalize-url/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2026 2016-12-30 22:04:08.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-normalize-url/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/normalize-range/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4013 2015-09-12 06:23:53.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/normalize-range/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-unique/
+-rwxr--r--   0 davecap   (1000) davecap   (1000)     1965 2015-03-25 03:46:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-unique/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/read-pkg/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1710 2015-09-03 04:54:53.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/read-pkg/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json-stringify-safe/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1261 2015-05-19 01:41:30.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json-stringify-safe/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      734 2015-05-19 01:41:30.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json-stringify-safe/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/type-check/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10168 2015-12-29 05:40:34.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/type-check/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/normalize-package-data/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7223 2017-04-21 00:27:59.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/normalize-package-data/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/vary/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2716 2017-03-20 18:45:24.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/vary/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      707 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/vary/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/trim-right/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      673 2015-02-17 03:45:01.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/trim-right/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/boom/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)    16600 2015-10-30 19:11:45.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/boom/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      105 2014-09-23 13:15:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/boom/CONTRIBUTING.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.camelcase/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      474 2016-08-13 17:33:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash.camelcase/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/assert-plus/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4791 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/assert-plus/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      428 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/assert-plus/CHANGES.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-message-helpers/
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)     2295 2014-11-24 19:32:43.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-message-helpers/README.md
+-rwxr-xr-x   0 davecap   (1000) davecap   (1000)      359 2015-01-26 07:14:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-message-helpers/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-do-expressions/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4191 2016-12-08 15:43:16.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-do-expressions/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-async-generator-functions/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2611 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-async-generator-functions/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/generate-object-property/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      473 2015-03-27 14:09:55.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/generate-object-property/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sax/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8381 2016-03-19 03:03:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sax/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/set-immediate-shim/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      558 2014-12-29 09:38:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/set-immediate-shim/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-stage-2/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1248 2017-04-01 14:50:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-stage-2/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helpers/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      326 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helpers/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-function-name/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       45 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-function-name/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-block-scoping/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1162 2017-04-01 14:50:05.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-block-scoping/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/for-in/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3452 2016-03-27 14:56:29.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/for-in/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/inflight/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      991 2014-05-05 03:32:51.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/inflight/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8575 2017-04-15 15:46:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1758 2017-04-19 18:40:31.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/CHANGELOG.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1077 2016-06-15 17:48:01.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/once/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1772 2016-09-06 21:07:04.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/once/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tweetnacl/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    13166 2016-12-13 11:07:18.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tweetnacl/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      875 2016-12-13 10:02:34.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tweetnacl/AUTHORS.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1040 2016-12-13 10:02:34.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tweetnacl/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5904 2016-12-13 10:58:09.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tweetnacl/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-display-name/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      649 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-display-name/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pbkdf2/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1439 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pbkdf2/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/doctrine/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7263 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/doctrine/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2903 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/doctrine/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isobject/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2568 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isobject/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/whatwg-fetch/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8628 2017-03-02 17:49:23.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/whatwg-fetch/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/semver/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    13336 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/semver/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-stage-1/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1406 2017-04-01 14:50:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-stage-1/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/function-bind/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1488 2016-02-14 07:31:07.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/function-bind/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/forwarded/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1432 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/forwarded/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       59 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/forwarded/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isexe/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1395 2017-03-23 00:52:07.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isexe/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsonpointer/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1103 2016-12-21 13:04:09.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsonpointer/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1152 2016-05-19 07:21:41.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsonpointer/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/colormin/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1340 2016-03-01 20:55:20.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/colormin/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      599 2016-08-16 17:36:12.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/colormin/CHANGELOG.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/proxy-addr/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4202 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/proxy-addr/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2087 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/proxy-addr/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/os-locale/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1027 2015-09-08 06:02:17.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/os-locale/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/flat-cache/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2683 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/flat-cache/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7143 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/flat-cache/changelog.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/colors/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3473 2015-06-17 12:57:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/colors/ReadMe.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1120 2016-12-31 22:32:40.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/accepts/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3838 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/accepts/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4542 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/accepts/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-flow/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      374 2016-10-17 22:44:21.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-flow/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-find-index/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      686 2016-09-30 08:34:35.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-find-index/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-uniq/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      671 2016-06-16 12:16:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-uniq/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-parse/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      912 2015-04-21 15:25:22.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-parse/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-number/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3439 2015-05-02 07:52:39.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-number/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4737 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5971 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/HISTORY.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/ms/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      933 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/ms/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1307 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/ms/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/debug/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6310 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/debug/Readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5611 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/debug/History.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/glob-base/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4690 2015-09-18 17:59:28.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/glob-base/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdx-expression-parse/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3608 2016-10-05 20:10:06.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdx-expression-parse/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json5/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8894 2016-10-07 18:59:57.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json5/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6335 2016-11-27 20:33:32.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json5/CHANGELOG.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1136 2016-09-28 01:11:56.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json5/LICENSE.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prr/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1680 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prr/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/memory-fs/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      786 2016-12-05 18:47:38.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/memory-fs/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/yallist/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4717 2015-12-19 19:51:30.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/yallist/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/chalk/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/chalk/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/chalk/node_modules/supports-color/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      823 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/chalk/node_modules/supports-color/readme.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     6136 2016-03-29 00:14:01.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/chalk/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-iterator/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4274 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-iterator/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    46737 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack/node_modules/
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack/node_modules/loader-utils/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7555 2017-02-20 18:01:27.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack/node_modules/loader-utils/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isomorphic-fetch/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1218 2015-01-23 11:55:10.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isomorphic-fetch/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/levn/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    10468 2015-12-29 05:52:40.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/levn/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/bn.js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7075 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/bn.js/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/normalize-path/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     5085 2017-03-29 18:19:49.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/normalize-path/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/escape-string-regexp/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      552 2016-02-21 12:17:12.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/escape-string-regexp/readme.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/des.js/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1127 2015-09-06 18:26:19.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/des.js/README.md
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/verror/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4522 2018-05-14 19:25:44.000000 solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/verror/README.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)   880118 2018-05-25 18:14:57.000000 solvebio-2.9.0/solvebio/contrib/dash/login.js
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/tmp/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8081 2018-05-14 18:58:33.000000 solvebio-2.9.0/solvebio/contrib/dash/tmp/oauth.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     7140 2019-07-09 19:29:10.000000 solvebio-2.9.0/solvebio/contrib/dash/solvebio_auth.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      147 2017-11-13 22:59:28.000000 solvebio-2.9.0/solvebio/contrib/dash/__init__.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2316 2019-07-09 19:29:10.000000 solvebio-2.9.0/solvebio/contrib/dash/solvebio_dash.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/dash/tests/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3339 2017-11-13 22:59:28.000000 solvebio-2.9.0/solvebio/contrib/dash/tests/test_solvebio_auth_integration.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)      371 2017-11-13 22:59:28.000000 solvebio-2.9.0/solvebio/contrib/dash/tests/credentials.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4374 2017-11-13 22:59:28.000000 solvebio-2.9.0/solvebio/contrib/dash/tests/IntegrationTests.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2365 2017-11-13 22:59:28.000000 solvebio-2.9.0/solvebio/contrib/dash/tests/utils.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8529 2019-11-07 21:47:01.000000 solvebio-2.9.0/solvebio/contrib/dash/tests/test_solvebio_auth.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)       91 2018-05-22 15:35:20.000000 solvebio-2.9.0/solvebio/contrib/dash/tests/credentials_local.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)        0 2017-11-13 22:59:28.000000 solvebio-2.9.0/solvebio/contrib/dash/tests/__init__.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/contrib/vcf_parser/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     8983 2017-11-14 14:35:18.000000 solvebio-2.9.0/solvebio/contrib/vcf_parser/vcf_parser.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)        0 2016-06-30 15:13:33.000000 solvebio-2.9.0/solvebio/contrib/vcf_parser/__init__.py
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)        0 2016-05-02 13:03:38.000000 solvebio-2.9.0/solvebio/contrib/__init__.py
+drwxr-xr-x   0 davecap   (1000) davecap   (1000)        0 2019-11-07 21:51:36.000000 solvebio-2.9.0/solvebio/cli/
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3480 2019-03-25 17:11:43.000000 solvebio-2.9.0/solvebio/cli/credentials.py
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)      212 2016-05-02 13:03:38.000000 solvebio-2.9.0/solvebio/cli/tutorial.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4801 2017-07-28 21:05:17.000000 solvebio-2.9.0/solvebio/cli/tutorial.md
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    14655 2019-11-07 21:47:01.000000 solvebio-2.9.0/solvebio/cli/data.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)    14498 2019-11-07 21:47:01.000000 solvebio-2.9.0/solvebio/cli/main.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1612 2018-09-11 16:02:27.000000 solvebio-2.9.0/solvebio/cli/ipython_init.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     3924 2019-11-07 21:47:01.000000 solvebio-2.9.0/solvebio/cli/auth.py
+-rw-rw-r--   0 davecap   (1000) davecap   (1000)        0 2016-05-02 13:03:38.000000 solvebio-2.9.0/solvebio/cli/__init__.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     2974 2018-07-13 17:43:13.000000 solvebio-2.9.0/solvebio/cli/ipython.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     1975 2019-11-06 16:26:19.000000 solvebio-2.9.0/solvebio/errors.py
+-rw-r--r--   0 davecap   (1000) davecap   (1000)     4871 2019-09-19 16:04:54.000000 solvebio-2.9.0/solvebio/__init__.py
```

### Comparing `solvebio-2.8.9/PKG-INFO` & `solvebio-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvebio
-Version: 2.8.9
+Version: 2.9.0
 Summary: The SolveBio Python client
 Home-page: https://github.com/solvebio/solvebio-python
 Author: Solve, Inc.
 Author-email: contact@solvebio.com
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/solvebio/solvebio-python.svg?branch=master)](http://travis-ci.org/solvebio/solvebio-python)
```

### Comparing `solvebio-2.8.9/LICENSE` & `solvebio-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/README.md` & `solvebio-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio.egg-info/PKG-INFO` & `solvebio-2.9.0/solvebio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvebio
-Version: 2.8.9
+Version: 2.9.0
 Summary: The SolveBio Python client
 Home-page: https://github.com/solvebio/solvebio-python
 Author: Solve, Inc.
 Author-email: contact@solvebio.com
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/solvebio/solvebio-python.svg?branch=master)](http://travis-ci.org/solvebio/solvebio-python)
```

### Comparing `solvebio-2.8.9/solvebio.egg-info/SOURCES.txt` & `solvebio-2.9.0/solvebio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/setup.py` & `solvebio-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/annotate.py` & `solvebio-2.9.0/solvebio/annotate.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/utils/humanize.py` & `solvebio-2.9.0/solvebio/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/utils/md5sum.py` & `solvebio-2.9.0/solvebio/utils/md5sum.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/utils/validators.py` & `solvebio-2.9.0/solvebio/utils/validators.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/utils/printing.py` & `solvebio-2.9.0/solvebio/utils/printing.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/utils/tabulate.py` & `solvebio-2.9.0/solvebio/utils/tabulate.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/test_filter.py` & `solvebio-2.9.0/solvebio/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/test_dataset_migrations.py` & `solvebio-2.9.0/solvebio/test/test_dataset_migrations.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/helper.py` & `solvebio-2.9.0/solvebio/test/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 else:
     import unittest2 as unittest  # NOQA
 
 import solvebio
 
 
 class SolveBioTestCase(unittest.TestCase):
-    TEST_DATASET_FULL_PATH = 'solvebio:public:/HGNC/1.0.0-1/HGNC'
+    TEST_DATASET_FULL_PATH = 'solvebio:public:/HGNC/3.3.0-2019-07-22/HGNC'
 
     def setUp(self):
         super(SolveBioTestCase, self).setUp()
         api_key = os.environ.get('SOLVEBIO_API_KEY', None)
         api_host = os.environ.get('SOLVEBIO_API_HOST', None)
         self.client = solvebio.SolveClient(host=api_host, token=api_key)
```

### Comparing `solvebio-2.8.9/solvebio/test/test_ratelimit.py` & `solvebio-2.9.0/solvebio/test/test_ratelimit.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/test_vault.py` & `solvebio-2.9.0/solvebio/test/test_vault.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/test_apiresource.py` & `solvebio-2.9.0/solvebio/test/test_apiresource.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/test_tabulate.py` & `solvebio-2.9.0/solvebio/test/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/test_exports.py` & `solvebio-2.9.0/solvebio/test/test_exports.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/test_vcfparser.py` & `solvebio-2.9.0/solvebio/test/test_vcfparser.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/test_credentials.py` & `solvebio-2.9.0/solvebio/test/test_credentials.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/test_utils.py` & `solvebio-2.9.0/solvebio/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/data/sample.vcf.gz` & `solvebio-2.9.0/solvebio/test/data/sample.vcf.gz`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/data/test_export.xlsx` & `solvebio-2.9.0/solvebio/test/data/test_export.xlsx`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/test_query_batch.py` & `solvebio-2.9.0/solvebio/test/test_query_batch.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.assertEqual(len(results), 2)
         self.assertEqual(results[0]['status_code'], 400)
         self.assertEqual(results[1]['status_code'], 400)
 
     def test_batch_query(self):
         queries = [
             self.dataset.query(limit=1),
-            self.dataset.query(limit=10).filter(hgnc_id__gt=100),
+            self.dataset.query(limit=10).filter(mamit_trnadb__gt=1),
             self.dataset.query(limit=100),
         ]
         results = self.client.BatchQuery(queries).execute()
         self.assertEqual(len(results), 3)
         self.assertEqual(len(results[0]['results']), 1)
         self.assertEqual(len(results[1]['results']), 10)
         self.assertEqual(len(results[2]['results']), 100)
```

### Comparing `solvebio-2.8.9/solvebio/test/client_mocks.py` & `solvebio-2.9.0/solvebio/test/client_mocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,36 @@
 class Fake201Response(object):
     status_code = 201
     class_name = None
 
     def __init__(self, data):
         self.object = {
             'id': 100,
-            'class_name': self.class_name,
+            'class_name': self.class_name
         }
 
     def json(self):
         return self.object
 
     def create(self, *args, **kwargs):
         return convert_to_solve_object(self.object)
 
     def retrieve(self, r_id, *args, **kwargs):
         obj = self.create()
         obj.id = r_id
         return obj
 
+    def _retrieve_helper(self, model_name, field_name, error_value,
+                         *args, **kwargs):
+        obj = self.create()
+        for k, v in kwargs.items():
+            obj[k] = v
+
+        return obj
+
     def all(self, *args, **kwargs):
         class ExtendedList(list):
             def solve_objects(self):
                 return convert_to_solve_object(self)
 
         return ExtendedList([self.create()])
 
@@ -86,15 +94,16 @@
             'id': 100,
             'parent_object_id': 99,
             'path': None,
             'full_path': None,
             'upload_url': None,
             'size': None,
             'md5': None,
-            'filename': 'file.json.gz'
+            'filename': 'file.json.gz',
+            'object_type': 'folder'
         }
 
 
 class FakeDatasetResponse(Fake201Response):
 
     class_name = 'Dataset'
 
@@ -173,14 +182,19 @@
     return FakeObjectResponse(kwargs).all()
 
 
 def fake_object_create(*args, **kwargs):
     return FakeObjectResponse(kwargs).create()
 
 
+def fake_object_retrieve(*args, **kwargs):
+    return FakeObjectResponse(kwargs)._retrieve_helper(
+        'LogicalObject', *args, **kwargs)
+
+
 def fake_dataset_create(*args, **kwargs):
     return FakeDatasetResponse(kwargs).create()
 
 
 def fake_dataset_import_create(*args, **kwargs):
     return FakeDatasetImport(kwargs).create()
```

### Comparing `solvebio-2.8.9/solvebio/test/test_login.py` & `solvebio-2.9.0/solvebio/test/test_login.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/test_annotate.py` & `solvebio-2.9.0/solvebio/test/test_annotate.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/test_client.py` & `solvebio-2.9.0/solvebio/test/test_client.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/test/test_query.py` & `solvebio-2.9.0/solvebio/test/test_query.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,18 @@
     def setUp(self):
         super(BaseQueryTest, self).setUp()
         self.dataset = self.client.Dataset.get_by_full_path(
             self.TEST_DATASET_FULL_PATH)
 
     def test_basic(self):
         results = self.dataset.query().filter(
-            omim_ids__in=[123631, 123670, 123690, 306250])
+            omim_id__in=['OMIM:123631',
+                         'OMIM:123670',
+                         'OMIM:123690',
+                         'OMIM:306250'])
         self.assertEqual(results.total, 4)
         self.assertEqual(len(results), results.total)
 
         # Test that iteration returns the correct number of results.
         # Test iterating through result-sets that are smaller than
         # the page size.
         self.assertEqual(len(results), len([r for r in results]))
@@ -36,115 +39,115 @@
 
     def test_count(self):
         q = self.dataset.query()
         total = q.count()
         self.assertGreater(total, 0)
 
         # with a filter
-        q = self.dataset.query().filter(omim_ids=123631)
+        q = self.dataset.query().filter(omim_id='OMIM:123631')
         self.assertEqual(q.count(), 1)
 
         # with a bogus filter
-        q = self.dataset.query().filter(omim_ids=999999)
+        q = self.dataset.query().filter(omim_id='OMIM:99999')
         self.assertEqual(q.count(), 0)
 
     def test_count_with_limit(self):
         q = self.dataset.query()
         total = q.count()
         self.assertGreater(total, 0)
 
         for limit in [0, 10, 1000]:
             # with a filter
-            q = self.dataset.query(limit=limit).filter(omim_ids=123631)
+            q = self.dataset.query(limit=limit).filter(omim_id='OMIM:123631')
             self.assertEqual(q.count(), 1)
 
             # with a bogus filter
-            q = self.dataset.query(limit=limit).filter(omim_ids=999999)
+            q = self.dataset.query(limit=limit).filter(omim_id='OMIM:99999')
             self.assertEqual(q.count(), 0)
 
     def test_len(self):
         q = self.dataset.query()
         total = q.count()
         self.assertGreater(total, 0)
         self.assertEqual(len(q), total)
 
         # with a filter
-        q = self.dataset.query().filter(omim_ids=123631)
+        q = self.dataset.query().filter(omim_id='OMIM:123631')
         self.assertEqual(len(q), 1)
 
         # with a bogus filter
-        q = self.dataset.query().filter(omim_ids=999999)
+        q = self.dataset.query().filter(omim_id='OMIM:999999')
         self.assertEqual(len(q), 0)
 
     def test_len_with_limit(self):
         q = self.dataset.query()
         total = q.count()
         self.assertGreater(total, 0)
         self.assertEqual(len(q), total)
 
         for limit in [0, 10, 1000]:
             # with a filter
-            q = self.dataset.query(limit=limit).filter(omim_ids=123631)
+            q = self.dataset.query(limit=limit).filter(omim_id='OMIM:123631')
             self.assertEqual(len(q), 1 if limit > 0 else 0)
 
             # with a bogus filter
-            q = self.dataset.query(limit=limit).filter(omim_ids=999999)
+            q = self.dataset.query(limit=limit).filter(omim_id='OMIM:999999')
             self.assertEqual(len(q), 0)
 
     def test_empty(self):
         """
         test Query when limit is specified and is GREATER THAN total available
         results.
         """
         # bogus filter
-        results = self.dataset.query().filter(omim_ids=999999)
+        results = self.dataset.query().filter(omim_id='OMIM:99999')
         self.assertEqual(len(results), 0)
         self.assertEqual(results[:]._buffer, [])
         self.assertRaises(IndexError, lambda: results[0])
 
     def test_empty_with_limit(self):
         """
         test Query when limit is specified and is GREATER THAN total available
         results.
         """
         limit = 100
         # bogus filter
         results = self.dataset.query(limit=limit) \
-            .filter(omim_ids=999999)
+            .filter(omim_id='OMIM:99999')
         self.assertEqual(len(results), 0)
         self.assertEqual(results[:]._buffer, [])
         self.assertRaises(IndexError, lambda: results[0])
 
     def test_filter(self):
         """
         test Filtered Query in which limit is specified but is GREATER THAN
         the number of total available results
         """
         num_filters = 4
         filters = \
-            Filter(omim_ids=123631) | \
-            Filter(omim_ids=123670) | \
-            Filter(omim_ids=123690) | \
-            Filter(omim_ids=306250)
+            Filter(omim_id='OMIM:123631') | \
+            Filter(omim_id='OMIM:123670') | \
+            Filter(omim_id='OMIM:123690') | \
+            Filter(omim_id='OMIM:306250')
         results = self.dataset.query(filters=filters)
         self.assertEqual(len(results), num_filters)
         self.assertRaises(IndexError, lambda: results[num_filters])
 
     def test_filter_with_limit(self):
         """
         test Filtered Query in which limit is specified but is GREATER THAN
         the number of total available results
         """
         limit = 10
         num_filters = 4
         filters = \
-            Filter(omim_ids=123631) | \
-            Filter(omim_ids=123670) | \
-            Filter(omim_ids=123690) | \
-            Filter(omim_ids=306250)
+            Filter(omim_id='OMIM:123631') | \
+            Filter(omim_id='OMIM:123670') | \
+            Filter(omim_id='OMIM:123690') | \
+            Filter(omim_id='OMIM:306250')
         results = self.dataset.query(
             limit=limit, filters=filters)
         self.assertEqual(len(results), num_filters)
         self.assertRaises(IndexError, lambda: results[num_filters])
 
     def test_paging(self):
         page_size = 10
@@ -190,15 +193,15 @@
         self.assertEqual(len(results[:limit]), limit)
 
         results = self.dataset.query(limit=limit)
         self.assertEqual(len(results[limit:]), limit)
 
         r0 = self.dataset.query(limit=limit)[0:limit][limit - 1]
         r1 = self.dataset.query(limit=limit)[limit - 1:][0]
-        self.assertEqual(r0['hgnc_id'], r1['hgnc_id'])
+        self.assertEqual(r0['entrez_id'], r1['entrez_id'])
 
     def test_slice_ranges_with_paging(self):
         limit = 50
         page_size = 10
 
         results = self.dataset.query(limit=limit, page_size=page_size)
         self.assertEqual(len(results[0:limit]), limit)
@@ -207,68 +210,69 @@
         self.assertEqual(len(results[:limit]), limit)
 
         results = self.dataset.query(limit=limit, page_size=page_size)
         self.assertEqual(len(results[limit:]), limit)
 
         r0 = self.dataset.query(limit=limit)[0:limit][limit - 1]
         r1 = self.dataset.query(limit=limit)[limit - 1:][0]
-        self.assertEqual(r0['hgnc_id'], r1['hgnc_id'])
+        self.assertEqual(r0['entrez_id'], r1['entrez_id'])
 
     def test_slice_offsets(self):
         zero_two = self.dataset.query()[0:2]
         one_three = self.dataset.query()[1:3]
 
         # Ensure that the repr for [0:1] != [1:2]
         self.assertNotEqual(repr(zero_two), repr(one_three))
 
         # Ensure that the second repr for [0:2] == [1:3]
         self.assertEqual(repr(zero_two[1]), repr(one_three[0]))
 
     def test_slice_ranges_with_small_limit(self):
         # Test slices larger than 'limit'
+        # query returns 6
         limit = 1
         results = self.dataset.query(limit=limit) \
-            .filter(hgnc_id__range=(1000, 2000))[0:4]
+            .filter(mamit_trnadb__range=(2, 12))[0:4]
         self.assertEqual(len(results), limit)
 
     def test_paging_and_slice_equivalence(self):
         idx0 = 3
         idx1 = 5
 
         def _query():
             return self.dataset.query(limit=10) \
-                .filter(hgnc_id__range=(1000, 5000))
+                .filter(mamit_trnadb__range=(2, 12))
 
         results_slice = _query()[idx0:idx1]
         results_paging = []
 
         for (i, r) in enumerate(_query()):
             if i == idx1:
                 break
             elif i >= idx0:
                 results_paging.append(r)
 
         self.assertEqual(len(results_paging), len(results_slice))
 
         for i in range(0, len(results_slice)):
-            id_a = results_paging[i]['hgnc_id']
-            id_b = results_slice[i]['hgnc_id']
+            id_a = results_paging[i]['entrez_id']
+            id_b = results_slice[i]['entrez_id']
             self.assertEqual(id_a, id_b)
 
     def test_caching(self):
         idx0 = 60
         idx1 = 81
 
         q = self.dataset.query(limit=100)
         results_slice = q[idx0:idx1]
         results_cached = q[idx0:idx1]
         self.assertEqual(len(results_slice), len(results_cached))
         for i in range(0, len(results_slice)):
-            id_a = results_slice[i]['chromosome']
-            id_b = results_cached[i]['chromosome']
+            id_a = results_slice[i]['status']
+            id_b = results_cached[i]['status']
             self.assertEqual(id_a, id_b)
 
     def test_get_by_index(self):
         limit = 100
         page_size = 10
         idxs = [0, 1, 10, 20, 50, 99]
         q = self.dataset.query(limit=limit, page_size=page_size)
@@ -283,21 +287,21 @@
         # backwards
         for (i, idx) in reversed(list(enumerate(idxs))):
             self.assertEqual(cached[i], q[idx])
 
     def test_field_filters(self):
         limit = 1
         results = self.dataset.query(limit=limit)
-        self.assertEqual(len(results[0].keys()), 41)
+        self.assertEqual(len(results[0].keys()), 54)
 
-        results = self.dataset.query(limit=limit, fields=['hgnc_id'])
+        results = self.dataset.query(limit=limit, fields=['entrez_id'])
         self.assertEqual(len(results[0].keys()), 1)
 
         results = self.dataset.query(
-            limit=limit, exclude_fields=['hgnc_id'])
-        self.assertEqual(len(results[0].keys()), 40)
-        self.assertTrue('hgnc_id' not in results[0].keys())
+            limit=limit, exclude_fields=['entrez_id'])
+        self.assertEqual(len(results[0].keys()), 53)
+        self.assertTrue('entrez_id' not in results[0].keys())
 
     def test_entity_filters(self):
         entities = [('gene', 'BRCA2')]
         query = self.dataset.query(entities=entities)
         self.assertEqual(query.count(), 1)
```

### Comparing `solvebio-2.8.9/solvebio/test/test_object.py` & `solvebio-2.9.0/solvebio/test/test_object.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import absolute_import
-# from solvebio.resource import Vault
 
 from .helper import SolveBioTestCase
 
 
 class ObjectTests(SolveBioTestCase):
 
     def test_object_paths(self):
@@ -16,14 +15,30 @@
 
                 # assert path is gettable
                 self.client.Object.get_by_full_path(o_path)
 
         with self.assertRaises(Exception):
             self.client.Object.get_by_full_path('what/is/this')
 
+    def test_object_output(self):
+
+        case = 'acme:myVault/uploads_folder'
+        expected = 'acme:myVault:/uploads_folder'
+        p, path_dict = self.client.Object.validate_full_path(case)
+
+        self.assertEqual(p, expected)
+        self.assertEqual(path_dict['full_path'], expected)
+        self.assertEqual(path_dict['path'], '/uploads_folder')
+        self.assertEqual(path_dict['parent_path'], '/')
+        self.assertEqual(path_dict['parent_full_path'], 'acme:myVault:/')
+        self.assertEqual(path_dict['filename'], 'uploads_folder')
+        self.assertEqual(path_dict['domain'], 'acme')
+        self.assertEqual(path_dict['vault'], 'myVault')
+        self.assertEqual(path_dict['vault_full_path'], 'acme:myVault')
+
     def test_object_path_cases(self):
 
         user = self.client.User.retrieve()
         domain = user.account.domain
         user_vault = '{0}:user-{1}'.format(domain, user.id)
         test_cases = [
             ['acme:myVault:/uploads_folder', 'acme:myVault:/uploads_folder'],
```

### Comparing `solvebio-2.8.9/solvebio/client.py` & `solvebio-2.9.0/solvebio/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,18 +149,15 @@
                 ua = '{}/{} {}'.format(name, version, ua)
             else:
                 ua = '{} {}'.format(name, ua)
 
         self._headers['User-Agent'] = ua
 
     def whoami(self):
-        try:
-            return self.get('/v1/user', {})
-        except:
-            return None
+        return self.get('/v1/user', {})
 
     def get(self, url, params, **kwargs):
         """Issues an HTTP GET across the wire via the Python requests
         library. See *request()* for information on keyword args."""
         kwargs['params'] = params
         return self.request('GET', url, **kwargs)
```

### Comparing `solvebio-2.8.9/solvebio/query.py` & `solvebio-2.9.0/solvebio/query.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/savedquery.py` & `solvebio-2.9.0/solvebio/resource/savedquery.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/group.py` & `solvebio-2.9.0/solvebio/resource/group.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/util.py` & `solvebio-2.9.0/solvebio/resource/util.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/beacon.py` & `solvebio-2.9.0/solvebio/resource/beacon.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/vault_sync_task.py` & `solvebio-2.9.0/solvebio/resource/vault_sync_task.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/object_copy_task.py` & `solvebio-2.9.0/solvebio/resource/object_copy_task.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/datasetcommit.py` & `solvebio-2.9.0/solvebio/resource/datasetcommit.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/manifest.py` & `solvebio-2.9.0/solvebio/resource/manifest.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/datasettemplate.py` & `solvebio-2.9.0/solvebio/resource/datasettemplate.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/application.py` & `solvebio-2.9.0/solvebio/resource/application.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/datasetfield.py` & `solvebio-2.9.0/solvebio/resource/datasetfield.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/datasetexport.py` & `solvebio-2.9.0/solvebio/resource/datasetexport.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/solveobject.py` & `solvebio-2.9.0/solvebio/resource/solveobject.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/beaconset.py` & `solvebio-2.9.0/solvebio/resource/beaconset.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/datasetmigration.py` & `solvebio-2.9.0/solvebio/resource/datasetmigration.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/datasetimport.py` & `solvebio-2.9.0/solvebio/resource/datasetimport.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/task.py` & `solvebio-2.9.0/solvebio/resource/task.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/dataset.py` & `solvebio-2.9.0/solvebio/resource/dataset.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/__init__.py` & `solvebio-2.9.0/solvebio/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/vault.py` & `solvebio-2.9.0/solvebio/resource/vault.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/apiresource.py` & `solvebio-2.9.0/solvebio/resource/apiresource.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/resource/object.py` & `solvebio-2.9.0/solvebio/resource/object.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import os
 import re
 import base64
 import binascii
 import mimetypes
 
 import requests
+from requests.packages.urllib3.util.retry import Retry
 
-from solvebio import SolveError
+from solvebio.errors import SolveError
+from solvebio.errors import NotFoundError
+from solvebio.errors import FileUploadError
 from solvebio.utils.md5sum import md5sum
 
 from ..client import client
 
 from .apiresource import CreateableAPIResource
 from .apiresource import ListableAPIResource
 from .apiresource import SearchableAPIResource
@@ -58,14 +61,15 @@
             * The validated full_path
             * A dictionary with the components:
                 * domain: the domain of the vault
                 * vault: the name of the vault, without domain
                 * vault_full_path: domain:vault
                 * path: the object path within the vault
                 * parent_path: the parent path to the object
+                * parent_full_path: the parent full path to the object
                 * filename: the object's filename (if any)
                 * full_path: the validated full path
 
         The following components may be overridden using kwargs:
 
             * vault
             * path
@@ -125,18 +129,25 @@
         # Remove double slashes
         object_path = re.sub('//+', '/', object_path)
         if object_path != '/':
             # Remove trailing slash
             object_path = object_path.rstrip('/')
 
         path_dict['path'] = object_path
-        # TODO: parent_path and filename
-        full_path = '{domain}:{vault}:{path}'.format(**path_dict)
-        path_dict['full_path'] = full_path
-        return full_path, path_dict
+        path_dict['full_path'] = '{domain}:{vault}:{path}'.format(**path_dict)
+
+        # Assumes no trailing slash, will be '' if is a vault root
+        path_dict['filename'] = os.path.basename(object_path)
+
+        # Will be / if parent is vault root
+        path_dict['parent_path'] = os.path.dirname(object_path)
+        path_dict['parent_full_path'] = '{vault_full_path}:{parent_path}' \
+            .format(**path_dict)
+
+        return path_dict['full_path'], path_dict
 
     @classmethod
     def get_by_full_path(cls, full_path, **params):
         # Don't pop client from params since **params is used below
         _client = params.get('client', None) or cls._client or client
         full_path, _ = cls.validate_full_path(full_path, client=_client)
         assert_type = params.pop('assert_type', None)
@@ -174,84 +185,214 @@
             print('Notice: Cannot upload empty file {0}'.format(local_path))
             return
 
         # Get vault
         vault = Vault.get_by_full_path(vault_full_path, client=_client)
 
         # Get MD5, mimetype, and file size for the object
-        md5, _ = md5sum(local_path, multipart_threshold=None)
+        local_md5, _ = md5sum(local_path, multipart_threshold=None)
         _, mimetype = mimetypes.guess_type(local_path)
         size = os.path.getsize(local_path)
 
+        # Check if object exists already and compare md5sums
+        full_path, path_dict = Object.validate_full_path(
+            os.path.join('{}:{}'.format(vault.full_path, remote_path),
+                         os.path.basename(local_path)))
+        try:
+            obj = cls.get_by_full_path(full_path)
+            if not obj.is_file:
+                print('WARNING: A {} currently exists at {}'
+                      .format(obj.object_type, full_path))
+            else:
+                # Check against md5sum of remote file
+                if obj.md5 == local_md5:
+                    print('WARNING: File {} (md5sum {}) already exists, '
+                          'not uploading'.format(full_path, local_md5))
+                    return obj
+                else:
+                    print('WARNING: File {} exists on SolveBio with different '
+                          'md5sum (local: {} vs remote: {}) Uploading anyway, '
+                          'but not overwriting.'
+                          .format(full_path, local_md5, obj.md5))
+        except NotFoundError:
+            pass
+
         # Lookup parent object
-        if remote_path == '/':
+        if path_dict['parent_path'] == '/':
             parent_object_id = None
         else:
             parent_obj = Object.get_by_full_path(
-                ':'.join([vault.full_path, remote_path]),
-                assert_type='folder', client=_client)
+                path_dict['parent_full_path'], assert_type='folder',
+                client=_client
+            )
             parent_object_id = parent_obj.id
 
-        description = kwargs.get(
-            'description',
-            'File uploaded via python client'
-        )
+        description = kwargs.get('description')
 
         # Create the file, and upload it to the Upload URL
         obj = Object.create(
             vault_id=vault.id,
             parent_object_id=parent_object_id,
             object_type='file',
             filename=os.path.basename(local_path),
-            md5=md5,
+            md5=local_md5,
             mimetype=mimetype,
             size=size,
             description=description,
+            tags=kwargs.get('tags', []) or [],
             client=_client
         )
 
         print('Notice: File created for {0} at {1}'.format(local_path,
                                                            obj.path))
         print('Notice: Upload initialized')
 
         upload_url = obj.upload_url
 
         headers = {
-            'Content-MD5': base64.b64encode(binascii.unhexlify(md5)),
+            'Content-MD5': base64.b64encode(binascii.unhexlify(local_md5)),
             'Content-Type': mimetype,
             'Content-Length': str(size),
         }
 
         # Use a session with a retry policy to handle connection errors.
         session = requests.Session()
-        session.mount('https://', requests.adapters.HTTPAdapter(max_retries=5))
+        max_retries = 5
+        retry = Retry(
+            total=max_retries,
+            read=max_retries,
+            connect=max_retries,
+            backoff_factor=0.3,
+            status_forcelist=(500, 502, 504, 400),
+        )
+        session.mount(
+            'https://', requests.adapters.HTTPAdapter(max_retries=retry))
         upload_resp = session.put(upload_url,
                                   data=open(local_path, 'rb'),
                                   headers=headers)
 
         if upload_resp.status_code != 200:
-            print('Notice: Upload status code for {0} was {1}'.format(
+            print('WARNING: Upload status code for {0} was {1}'.format(
                 local_path, upload_resp.status_code
             ))
-            print('See error message below:')
-            print(upload_resp.content)
             # Clean up the failed upload
             obj.delete(force=True)
+            raise FileUploadError(upload_resp.content)
         else:
             print('Notice: Successfully uploaded {0} to {1}'.format(local_path,
                                                                     obj.path))
 
         return obj
 
+    def _object_list_helper(self, **params):
+        """Helper method to get objects within"""
+
+        if not self.is_folder:
+            raise SolveError(
+                "Only folders contain child objects. This is a {}"
+                .format(self.object_type))
+
+        params['vault_id'] = self.vault_id
+        if 'recursive' in params:
+            params['ancestor_id'] = self.id
+            params['limit'] = 1000
+        else:
+            params['parent_object_id'] = self.id
+
+        items = self.all(client=self._client, **params)
+        return items
+
+    def files(self, **params):
+        return self._object_list_helper(object_type='file', **params)
+
+    def folders(self, **params):
+        return self._object_list_helper(object_type='folder', **params)
+
+    def datasets(self, **params):
+        return self._object_list_helper(object_type='dataset', **params)
+
+    def objects(self, **params):
+        return self._object_list_helper(**params)
+
+    def ls(self, **params):
+        return self.objects(**params)
+
+    def query(self, query=None, **params):
+        """Shortcut to query the underlying Dataset object"""
+        from solvebio import Dataset
+
+        if not self.is_dataset:
+            raise SolveError(
+                "The query method can only be used by a dataset. Found a {}"
+                .format(self.object_type))
+
+        return Dataset(self.dataset_id).query(query=query, **params)
+
     @property
     def parent(self):
         """ Returns the parent object """
         if self['parent_object_id']:
             return self.retrieve(self['parent_object_id'], client=self._client)
 
         return None
 
     @property
     def vault(self):
         """ Returns the vault object """
         from . import Vault
         return Vault.retrieve(self['vault_id'], client=self._client)
+
+    @property
+    def is_dataset(self):
+        return self.object_type == 'dataset'
+
+    @property
+    def is_folder(self):
+        return self.object_type == 'folder'
+
+    @property
+    def is_file(self):
+        return self.object_type == 'file'
+
+    def tag(self, tags, remove=False, dry_run=False, apply_save=False):
+        """Add or remove tags on an object"""
+
+        def lowercase(x):
+            return x.lower()
+
+        existing_tags = map(lowercase, self.tags)
+
+        if remove:
+            removal_tags = [tag for tag in tags
+                            if lowercase(tag) in existing_tags]
+            if removal_tags:
+                print('{}Notice: Removing tags: {} from object: {}'
+                      .format('[Dry Run] ' if dry_run else '',
+                              ', '.join(removal_tags), self.full_path))
+
+                updated_tags = [tag for tag in existing_tags
+                                if tag not in removal_tags]
+            else:
+                print('{}Notice: Object {} does not contain any of the '
+                      'following tags: {}'.format(
+                          '[Dry Run] ' if dry_run else '',
+                          self.full_path, ', '.join(tags)))
+                return False
+        else:
+            new_tags = [tag for tag in tags
+                        if lowercase(tag) not in existing_tags]
+            if new_tags:
+                print('{}Notice: Adding tags: {} to object: {}'
+                      .format('[Dry Run] ' if dry_run else '',
+                              ', '.join(new_tags), self.full_path))
+                updated_tags = self.tags + new_tags
+            else:
+                print('{}Notice: Object {} already contains these tags: {}'
+                      .format('[Dry Run] ' if dry_run else '',
+                              self.full_path, ', '.join(tags)))
+                return False
+
+        if not dry_run and apply_save:
+            self.tags = updated_tags
+            self.save()
+
+        return True
```

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/usage.py` & `solvebio-2.9.0/solvebio/contrib/dash/usage.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/oauth-redirect.js` & `solvebio-2.9.0/solvebio/contrib/dash/oauth-redirect.js`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asap/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asap/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asap/CHANGES.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asap/CHANGES.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asap/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asap/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hoek/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hoek/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asn1/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asn1/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-decorators/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-decorators/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shelljs/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shelljs/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shelljs/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shelljs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/npmlog/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/npmlog/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/npmlog/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/npmlog/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/graphviz.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/graphviz.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/pretty_gyp.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/pretty_gyp.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/pretty_sln.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/pretty_sln.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/pretty_vcproj.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/tools/pretty_vcproj.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/gyptest.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/gyptest.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/PRESUBMIT.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/PRESUBMIT.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/common_test.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/common_test.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/input.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/input.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/mac_tool.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/mac_tool.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/easy_xml_test.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/easy_xml_test.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/common.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/common.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/ordered_dict.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/ordered_dict.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xcode_emulation.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xcode_emulation.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings_test.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings_test.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/win_tool.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/win_tool.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/input_test.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/input_test.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/easy_xml.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/easy_xml.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSToolFile.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSToolFile.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/simple_copy.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/simple_copy.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xcodeproj_file.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xcodeproj_file.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/android.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/android.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode_test.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode_test.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/analyzer.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/analyzer.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs_test.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs_test.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/cmake.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/cmake.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/eclipse.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/eclipse.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/gypsh.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/gypsh.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja_test.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja_test.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/dump_dependency_json.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/dump_dependency_json.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/gypd.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/generator/gypd.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/ninja_syntax.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/ninja_syntax.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSNew.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSNew.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/flock_tool.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/flock_tool.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSUtil.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSUtil.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xcode_ninja.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xcode_ninja.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xml_fix.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/xml_fix.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSVersion.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSVersion.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSProject.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSProject.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSUserFile.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/MSVSUserFile.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/__init__.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/__init__.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/msvs_emulation.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/pylib/gyp/msvs_emulation.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/setup.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/setup.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/buildbot/buildbot_run.py` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-gyp/gyp/buildbot/buildbot_run.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/console-control-strings/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/console-control-strings/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/faye-websocket/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/faye-websocket/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/faye-websocket/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/faye-websocket/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compressible/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compressible/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compressible/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compressible/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/async-foreach/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/async-foreach/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx-self/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx-self/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-deceiver/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-deceiver/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-sticky-regex/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-sticky-regex/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-svg/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-svg/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regenerate/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regenerate/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esrecurse/node_modules/estraverse/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esrecurse/node_modules/estraverse/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/base64-js/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/base64-js/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mixin-object/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mixin-object/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mixin-object/node_modules/for-in/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mixin-object/node_modules/for-in/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/for-own/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/for-own/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-shorthand-properties/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-shorthand-properties/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/alphanum-sort/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/alphanum-sort/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-builtin-module/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-builtin-module/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cookie-signature/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cookie-signature/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cookie-signature/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cookie-signature/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cookie/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cookie/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cookie/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cookie/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/indent-string/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/indent-string/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babylon/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babylon/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babylon/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babylon/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tough-cookie/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tough-cookie/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/coa/README.ru.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/coa/README.ru.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/coa/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/coa/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cssesc/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cssesc/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hosted-git-info/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hosted-git-info/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/user-home/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/user-home/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-callable/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-callable/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-callable/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-callable/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shallow-clone/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shallow-clone/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/kind-of/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/kind-of/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/lazy-cache/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/shallow-clone/node_modules/lazy-cache/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/combined-stream/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/combined-stream/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/right-align/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/right-align/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/string-width/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/string-width/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-async-to-generator/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-async-to-generator/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-date-object/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-date-object/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/elliptic/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/elliptic/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/watchpack/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/watchpack/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/timers-browserify/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/timers-browserify/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/timers-browserify/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/timers-browserify/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/timers-browserify/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/timers-browserify/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/finalhandler/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/finalhandler/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/finalhandler/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/finalhandler/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/assert/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/assert/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/source-list-map/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/source-list-map/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/camelcase-keys/node_modules/camelcase/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/camelcase-keys/node_modules/camelcase/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/camelcase-keys/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/camelcase-keys/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/natural-compare/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/natural-compare/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/url/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/url/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/url/node_modules/punycode/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/url/node_modules/punycode/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-spread/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-spread/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/buffer/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/buffer/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/buffer/AUTHORS.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/buffer/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prop-types/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prop-types/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/is-extglob/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/is-extglob/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/is-glob/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/node_modules/is-glob/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-proxy-middleware/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/read-pkg-up/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/read-pkg-up/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-types/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-types/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-calc/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-calc/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-calc/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-calc/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pluralize/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pluralize/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/builtin-status-codes/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/builtin-status-codes/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ripemd160/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ripemd160/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ripemd160/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ripemd160/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/camelcase/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/camelcase/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/find-cache-dir/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/find-cache-dir/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/which-module/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/which-module/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/enhanced-resolve/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/enhanced-resolve/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/set-blocking/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/set-blocking/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/set-blocking/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/set-blocking/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack-dev-middleware/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack-dev-middleware/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/merge-descriptors/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/merge-descriptors/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esutils/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esutils/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-commonjs/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-commonjs/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fstream/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fstream/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-reduce-idents/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-reduce-idents/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-reduce-idents/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-reduce-idents/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-primitive/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-primitive/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-regenerator/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-regenerator/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/stdout-stream/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/stdout-stream/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/react/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/react/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-equal-shallow/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-equal-shallow/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/extsprintf/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/extsprintf/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/emojis-list/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/emojis-list/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/emojis-list/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/emojis-list/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/emojis-list/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/emojis-list/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-react/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-react/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-svgo/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-svgo/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-svgo/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-svgo/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ms/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ms/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ms/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ms/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ms/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ms/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ms/license.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ms/license.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-duplicates/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-duplicates/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-duplicates/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-duplicates/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-type/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-type/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/to-arraybuffer/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/to-arraybuffer/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pinkie-promise/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pinkie-promise/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-code-frame/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-code-frame/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-colormin/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-colormin/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-colormin/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-colormin/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/node_modules/ms/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/node_modules/ms/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/node_modules/ms/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/node_modules/ms/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/node_modules/debug/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/node_modules/debug/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/compression/node_modules/debug/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/compression/node_modules/debug/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fastparse/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fastparse/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/parse-json/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/parse-json/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-plain-obj/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-plain-obj/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/on-headers/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/on-headers/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cli-width/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cli-width/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fbjs/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fbjs/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fbjs/node_modules/core-js/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fbjs/node_modules/core-js/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fbjs/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fbjs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/CONTRIBUTING.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/doc/wg-meetings/2015-01-30.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/doc/wg-meetings/2015-01-30.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/node_modules/string_decoder/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/node_modules/string_decoder/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readable-stream/GOVERNANCE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readable-stream/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/querystring/License.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/querystring/License.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/supports-color/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/supports-color/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/del/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/del/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ua-parser-js/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ua-parser-js/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-libs-browser/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-libs-browser/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/aws4/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/aws4/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/har-schema/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/har-schema/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/randombytes/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/randombytes/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uniq/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uniq/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esquery/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esquery/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-reduce-transforms/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-reduce-transforms/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdx-license-ids/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdx-license-ids/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/trim-newlines/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/trim-newlines/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/reduce-css-calc/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/reduce-css-calc/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/reduce-css-calc/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/reduce-css-calc/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pinkie/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pinkie/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nopt/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nopt/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/icss-replace-symbols/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/icss-replace-symbols/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sshpk/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sshpk/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/wide-align/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/wide-align/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/stream-http/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/stream-http/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-loader/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-loader/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-loader/node_modules/css-selector-tokenizer/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-loader/node_modules/css-selector-tokenizer/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-loader/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-loader/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/run-async/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/run-async/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ansi-styles/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ansi-styles/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-signature/http_signing.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-signature/http_signing.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-signature/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-signature/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-signature/CHANGES.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-signature/CHANGES.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-signature/node_modules/assert-plus/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-signature/node_modules/assert-plus/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/util-deprecate/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/util-deprecate/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/write/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/write/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/safe-buffer/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/safe-buffer/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack-dev-server/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack-dev-server/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-to-regexp/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-to-regexp/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-to-regexp/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-to-regexp/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fill-range/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fill-range/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fill-range/node_modules/isobject/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fill-range/node_modules/isobject/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/qs/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/qs/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/qs/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/qs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/clap/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/clap/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color-convert/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color-convert/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color-convert/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color-convert/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/normalize-url/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/normalize-url/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-extglob/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-extglob/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-gradients/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-gradients/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-gradients/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-gradients/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cssnano/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cssnano/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cssnano/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cssnano/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/node_modules/acorn/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/node_modules/acorn/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/node_modules/acorn/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-dynamic-import/node_modules/acorn/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/rechoir/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/rechoir/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/convert-source-map/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/convert-source-map/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/opn/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/opn/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/crypto-browserify/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/crypto-browserify/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strip-ansi/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strip-ansi/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/co/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/co/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/co/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/co/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/brace-expansion/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/brace-expansion/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/range-parser/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/range-parser/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/range-parser/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/range-parser/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-typedarray/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-typedarray/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-typedarray/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-typedarray/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/domain-browser/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/domain-browser/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/domain-browser/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/domain-browser/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/domain-browser/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/domain-browser/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-map/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-map/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/source-map/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/source-map/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/source-map/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/source-map/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/query-string/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/query-string/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hpack.js/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hpack.js/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/center-align/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/center-align/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/builtin-modules/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/builtin-modules/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/braces/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/braces/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/table/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/table/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/table/node_modules/string-width/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/table/node_modules/string-width/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/table/node_modules/is-fullwidth-code-point/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/table/node_modules/is-fullwidth-code-point/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-font-values/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-font-values/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-flatten/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-flatten/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserslist/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserslist/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserslist/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserslist/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object.omit/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object.omit/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-flow/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-flow/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loose-envify/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loose-envify/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/minimalistic-crypto-utils/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/minimalistic-crypto-utils/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/batch/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/batch/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/batch/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/batch/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-reduce-initial/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-reduce-initial/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/delegates/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/delegates/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-empty/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-empty/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-convert-values/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-convert-values/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-convert-values/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-convert-values/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/create-ecdh/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/create-ecdh/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-overridden/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-overridden/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/glob-parent/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/glob-parent/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/events/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/events/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs-client/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs-client/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs-client/Changelog.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs-client/Changelog.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/faye-websocket/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/faye-websocket/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/faye-websocket/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs-client/node_modules/faye-websocket/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-computed-properties/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-computed-properties/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mime/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mime/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/reduce-function-call/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/reduce-function-call/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/evp_bytestokey/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/evp_bytestokey/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/minimatch/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/minimatch/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-es2015/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-es2015/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-jsx/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-jsx/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-jsx/node_modules/acorn/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-jsx/node_modules/acorn/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn-jsx/node_modules/acorn/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn-jsx/node_modules/acorn/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-aes/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-aes/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-aes/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-aes/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-path-in-cwd/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-path-in-cwd/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/preserve/.verb.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/preserve/.verb.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/preserve/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/preserve/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-for-of/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-for-of/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-block-scoped-functions/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-block-scoped-functions/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/repeat-string/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/repeat-string/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-plain-object/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-plain-object/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-stream/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-stream/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caller-path/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caller-path/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pako/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pako/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pako/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pako/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-property/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-property/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/binary-extensions/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/binary-extensions/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/parseurl/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/parseurl/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/parseurl/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/parseurl/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-unused/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-unused/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-unused/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-unused/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/destroy/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/destroy/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/unpipe/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/unpipe/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/negotiator/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/negotiator/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/negotiator/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/negotiator/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/to-fast-properties/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/to-fast-properties/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-regex/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-regex/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-regex/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-regex/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readline2/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readline2/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/decamelize/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/decamelize/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hash.js/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hash.js/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/async-each/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/async-each/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/async-each/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/async-each/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/API.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/API.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-selector-parser/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-params/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-params/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-params/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-params/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/vendors/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/vendors/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/errno/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/errno/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ajv/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ajv/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ee-first/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ee-first/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdy-transport/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdy-transport/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/yargs/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/yargs/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/yargs/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/yargs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/slice-ansi/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/slice-ansi/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint-plugin-react/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint-plugin-react/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint-plugin-react/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint-plugin-react/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fast-levenshtein/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fast-levenshtein/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fast-levenshtein/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fast-levenshtein/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/optionator/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/optionator/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/optionator/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/optionator/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/wbuf/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/wbuf/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isstream/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isstream/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isstream/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isstream/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/error-ex/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/error-ex/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/util/node_modules/inherits/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/util/node_modules/inherits/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/micromatch/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/micromatch/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-object-rest-spread/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-object-rest-spread/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/esprima/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/esprima/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/balanced-match/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/balanced-match/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/balanced-match/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/balanced-match/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/y18n/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/y18n/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/style-loader/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/style-loader/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/style-loader/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/style-loader/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/style-loader/.github/PULL_REQUEST_TEMPLATE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/style-loader/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/style-loader/.github/ISSUE_TEMPLATE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/style-loader/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/constants-browserify/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/constants-browserify/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/get-stdin/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/get-stdin/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-classes/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-classes/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/graceful-fs/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/graceful-fs/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-glob/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-glob/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-filter-plugins/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-filter-plugins/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/html-entities/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/html-entities/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/encodeurl/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/encodeurl/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/imurmurhash/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/imurmurhash/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/portfinder/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/portfinder/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/portfinder/node_modules/async/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/portfinder/node_modules/async/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/portfinder/node_modules/async/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/portfinder/node_modules/async/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ramda/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ramda/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/rx-lite/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/rx-lite/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hawk/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hawk/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/promise/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/promise/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-value-parser/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-value-parser/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/autoprefixer/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/autoprefixer/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/autoprefixer/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/autoprefixer/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/escape-html/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/escape-html/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/docs/source-maps.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/docs/source-maps.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/docs/syntax.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/docs/syntax.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/docs/guidelines/runner.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/docs/guidelines/runner.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/docs/guidelines/plugin.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/docs/guidelines/plugin.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caseless/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caseless/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strip-json-comments/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strip-json-comments/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/currently-unhandled/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/currently-unhandled/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-literals/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-literals/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caniuse-db/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caniuse-db/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caniuse-db/CONTRIBUTING.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caniuse-db/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/os-homedir/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/os-homedir/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack-sources/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack-sources/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack-sources/node_modules/source-list-map/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack-sources/node_modules/source-list-map/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prelude-ls/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prelude-ls/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prelude-ls/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prelude-ls/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-loader/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-loader/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-loader/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-loader/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/form-data/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/form-data/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/original/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/original/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/original/node_modules/url-parse/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/original/node_modules/url-parse/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loud-rejection/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loud-rejection/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/react-dom/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/react-dom/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tar/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tar/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cross-spawn/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cross-spawn/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asynckit/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asynckit/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object-assign/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object-assign/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-binary-path/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-binary-path/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regenerator-transform/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regenerator-transform/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/progress/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/progress/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/progress/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/progress/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/yargs-parser/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/yargs-parser/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/yargs-parser/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/yargs-parser/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-tokens/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-tokens/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-tokens/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-tokens/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-unique-selectors/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-unique-selectors/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint/node_modules/doctrine/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint/node_modules/doctrine/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint/node_modules/doctrine/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint/node_modules/doctrine/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eslint/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eslint/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/slash/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/slash/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/performance-now/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/performance-now/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-sign/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-sign/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-extendable/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-extendable/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-zindex/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-zindex/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-zindex/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-zindex/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-my-json-valid/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-my-json-valid/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-static/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-static/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-static/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-static/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/require-uncached/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/require-uncached/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/argparse/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/argparse/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/argparse/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/argparse/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/acorn/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/acorn/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/create-hmac/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/create-hmac/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/create-hmac/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/create-hmac/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ansi-regex/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ansi-regex/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-comments/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-comments/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-discard-comments/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-discard-comments/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uniqs/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uniqs/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/utils-merge/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/utils-merge/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-selectors/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-selectors/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-minify-selectors/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-minify-selectors/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-idents/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-idents/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-idents/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-idents/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/globule/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/globule/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/globule/node_modules/lodash/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/globule/node_modules/lodash/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/d/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/d/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs-parser/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs-parser/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs-parser/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/yargs-parser/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/window-size/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/node_modules/window-size/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sass-graph/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sass-graph/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strip-indent/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strip-indent/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regex-cache/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regex-cache/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/dashdash/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/dashdash/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/dashdash/CHANGES.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/dashdash/CHANGES.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regjsparser/node_modules/jsesc/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regjsparser/node_modules/jsesc/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/bcrypt-pbkdf/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/bcrypt-pbkdf/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ignore/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ignore/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-values/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-values/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/html-comment-regex/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/html-comment-regex/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/process/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/process/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/content-disposition/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/content-disposition/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/content-disposition/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/content-disposition/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/exit-hook/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/exit-hook/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/delayed-stream/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/delayed-stream/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/extglob/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/extglob/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/requires-port/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/requires-port/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sort-keys/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sort-keys/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tapable/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tapable/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/hmac-drbg/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/hmac-drbg/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-template-literals/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-template-literals/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/media-typer/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/media-typer/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/etag/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/etag/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/etag/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/etag/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/browserify-zlib/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/browserify-zlib/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/gauge/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/gauge/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/gauge/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/gauge/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/on-finished/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/on-finished/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/on-finished/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/on-finished/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-resolvable/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-resolvable/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fs.realpath/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fs.realpath/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/README.ru.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/README.ru.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/node_modules/esprima/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/node_modules/esprima/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/node_modules/js-yaml/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/node_modules/js-yaml/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/node_modules/js-yaml/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/node_modules/js-yaml/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/svgo/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/svgo/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-yaml/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-yaml/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-yaml/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-yaml/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-posix-bracket/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-posix-bracket/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/anymatch/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/anymatch/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/has-ansi/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/has-ansi/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-systemjs/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-systemjs/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/math-expression-evaluator/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/math-expression-evaluator/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-path-inside/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-path-inside/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json3/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json3/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/chokidar/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/chokidar/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/chokidar/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/chokidar/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/define-properties/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/define-properties/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/define-properties/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/define-properties/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-buffer/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-buffer/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/load-json-file/node_modules/strip-bom/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/load-json-file/node_modules/strip-bom/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/load-json-file/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/load-json-file/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/callsites/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/callsites/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-export-extensions/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-export-extensions/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsbn/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsbn/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/statuses/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/statuses/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/statuses/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/statuses/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/code-point-at/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/code-point-at/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/aproba/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/aproba/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx-source/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx-source/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-umd/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-umd/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/has-flag/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/has-flag/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs/examples/multiplex/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs/examples/multiplex/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sockjs/tests/test_server/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sockjs/tests/test_server/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/color-string/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/color-string/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-generator/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-generator/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/circular-json/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/circular-json/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/type-is/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/type-is/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/type-is/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/type-is/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsprim/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsprim/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsprim/CHANGES.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsprim/CHANGES.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-function-name/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-function-name/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es5-ext/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es5-ext/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/console-browserify/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/console-browserify/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/private/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/private/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-driver/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-driver/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-driver/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-driver/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/depd/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/depd/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/depd/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/depd/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/remove-trailing-separator/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/remove-trailing-separator/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-helper-builder-react-jsx/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-helper-builder-react-jsx/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/espree/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/espree/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/espree/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/espree/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sprintf-js/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sprintf-js/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/encoding/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/encoding/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-exists/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-exists/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/whet.extend/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/whet.extend/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cryptiles/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cryptiles/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/which/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/which/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/which/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/which/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-set/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-set/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-check-es2015-constants/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-check-es2015-constants/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regenerator-runtime/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regenerator-runtime/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ansi-html/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ansi-html/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/date-now/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/date-now/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prepend-http/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prepend-http/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isarray/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isarray/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/inherits/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/inherits/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array.prototype.find/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array.prototype.find/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array.prototype.find/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array.prototype.find/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-selector-tokenizer/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-selector-tokenizer/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/has-unicode/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/has-unicode/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/arr-flatten/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/arr-flatten/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-template/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-template/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-arrayish/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-arrayish/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-class-constructor-call/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-class-constructor-call/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/electron-to-chromium/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/electron-to-chromium/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uniqid/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uniqid/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/os-tmpdir/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/os-tmpdir/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/gaze/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/gaze/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/camelcase/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/camelcase/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/yargs/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/yargs/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/yargs/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/yargs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/cliui/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-js/node_modules/cliui/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/debug/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/debug/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/debug/node_modules/ms/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/debug/node_modules/ms/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/debug/node_modules/ms/license.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/debug/node_modules/ms/license.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/debug/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/debug/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/csso/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/csso/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/csso/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/csso/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ajv-keywords/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ajv-keywords/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/interpret/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/interpret/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-flow-strip-types/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-flow-strip-types/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/invariant/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/invariant/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/invariant/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/invariant/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/asn1.js/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/asn1.js/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-register/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-register/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/concat-stream/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/concat-stream/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-arrow-functions/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-arrow-functions/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/clone/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/clone/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/scopes.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/scopes.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/string_bytes.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/string_bytes.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/persistent.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/persistent.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/buffers.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/buffers.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/callback.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/callback.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/converters.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/converters.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/errors.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/errors.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/node_misc.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/node_misc.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/v8_misc.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/v8_misc.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/new.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/new.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/v8_internals.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/v8_internals.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/asyncworker.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/asyncworker.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/object_wrappers.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/object_wrappers.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/script.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/script.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/methods.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/methods.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/json.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/json.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/doc/maybe_types.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/doc/maybe_types.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/nan/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/nan/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/event-emitter/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/event-emitter/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-base64/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-base64/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/js-base64/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/js-base64/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-extract-imports/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-extract-imports/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lcid/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lcid/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/wrap-ansi/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/wrap-ansi/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-destructuring/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-destructuring/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-stage-3/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-stage-3/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/align-text/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/align-text/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readdirp/examples/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readdirp/examples/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/readdirp/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/readdirp/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/onetime/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/onetime/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pkg-dir/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pkg-dir/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-extensions/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-extensions/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/websocket-extensions/lib/pipeline/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/websocket-extensions/lib/pipeline/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/xtend/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/xtend/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-is-absolute/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-is-absolute/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/window-size/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/window-size/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strict-uri-encode/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strict-uri-encode/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/node_modules/regexpu-core/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-unicode-regex/node_modules/regexpu-core/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-normalize-charset/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-normalize-charset/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-amd/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-modules-amd/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/signal-exit/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/signal-exit/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/signal-exit/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/signal-exit/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/q/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/q/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/q/CHANGES.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/q/CHANGES.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sha.js/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sha.js/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/connect-history-api-fallback/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/connect-history-api-fallback/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/connect-history-api-fallback/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/connect-history-api-fallback/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eventemitter3/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eventemitter3/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/buffer-shims/license.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/buffer-shims/license.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/globby/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/globby/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/in-publish/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/in-publish/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-rules/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-rules/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-rules/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-rules/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-fetch/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-fetch/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-fetch/ERROR-HANDLING.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-fetch/ERROR-HANDLING.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-fetch/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-fetch/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-fetch/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-fetch/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-fetch/LIMITS.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-fetch/LIMITS.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-class-properties/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-class-properties/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-errors/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-errors/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/http-errors/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/http-errors/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object-keys/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object-keys/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object-keys/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object-keys/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pseudomap/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pseudomap/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-parameters/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-parameters/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/find-up/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/find-up/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/node_modules/debug/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/node_modules/debug/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/node_modules/debug/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/node_modules/debug/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/node_modules/http-errors/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/node_modules/http-errors/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/send/node_modules/http-errors/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/send/node_modules/http-errors/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/parse-glob/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/parse-glob/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/expand-range/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/expand-range/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-finite/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-finite/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-ordered-values/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-ordered-values/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-ordered-values/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-ordered-values/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/express/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/express/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/express/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/express/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/express/node_modules/debug/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/express/node_modules/debug/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/express/node_modules/debug/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/express/node_modules/debug/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/meow/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/meow/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/handle-thing/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/handle-thing/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fresh/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fresh/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/fresh/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/fresh/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mime-types/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mime-types/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mime-types/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mime-types/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mime-db/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mime-db/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mime-db/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mime-db/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-typeof-symbol/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-typeof-symbol/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/are-we-there-yet/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/are-we-there-yet/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/are-we-there-yet/CHANGES.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/are-we-there-yet/CHANGES.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/redent/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/redent/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/extend/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/extend/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/extend/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/extend/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-exponentiation-operator/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-exponentiation-operator/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-strict-mode/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-strict-mode/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/map-obj/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/map-obj/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es-abstract/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es-abstract/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es-abstract/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es-abstract/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/mute-stream/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/mute-stream/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-jsx/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/figures/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/figures/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/har-validator/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/har-validator/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/randomatic/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/randomatic/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/generate-function/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/generate-function/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uuid/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uuid/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uuid/benchmark/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uuid/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-merge-longhand/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-merge-longhand/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/macaddress/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/macaddress/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/repeat-element/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/repeat-element/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/clone-deep/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/clone-deep/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regexpu-core/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regexpu-core/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lru-cache/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lru-cache/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/wrappy/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/wrappy/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/home-or-tmp/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/home-or-tmp/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/inquirer/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/inquirer/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sntp/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sntp/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/miller-rabin/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/miller-rabin/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/stringstream/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/stringstream/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/resolve-from/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/resolve-from/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-local-by-default/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-local-by-default/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-local-by-default/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-local-by-default/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/css-color-names/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/css-color-names/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/querystring-es3/License.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/querystring-es3/License.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/methods/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/methods/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/longest/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/longest/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/detect-indent/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/detect-indent/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cliui/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cliui/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/validate-npm-package-license/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/validate-npm-package-license/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/escope/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/escope/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ieee754/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ieee754/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/filename-regex/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/filename-regex/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ipaddr.js/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ipaddr.js/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-exponentiation-operator/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-exponentiation-operator/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/big.js/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/big.js/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/rimraf/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/rimraf/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/process-nextick-args/license.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/process-nextick-args/license.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/bytes/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/bytes/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/bytes/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/bytes/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/source-map-support/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/source-map-support/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/source-map-support/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/source-map-support/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-absolute-url/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-absolute-url/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdy/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdy/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-function-bind/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-function-bind/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cipher-base/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cipher-base/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cipher-base/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cipher-base/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-symbol/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-symbol/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/brorand/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/brorand/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-autotools.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-autotools.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-importer.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-importer.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/custom-functions-internal.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/custom-functions-internal.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-mingw.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-mingw.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-on-gentoo.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-on-gentoo.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-context-example.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-context-example.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/dev-ast-memory.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/dev-ast-memory.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-function.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-function.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-value-internal.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-value-internal.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-visual-studio.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-visual-studio.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-on-windows.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-on-windows.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-function-example.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-function-example.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/unicode.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/unicode.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-context-internal.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-context-internal.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-importer-example.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-importer-example.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-value-example.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-value-example.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/source-map-internals.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/source-map-internals.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/plugins.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-shared-library.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-shared-library.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-makefiles.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-with-makefiles.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/triage.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/triage.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-on-darwin.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/build-on-darwin.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/implementations.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/implementations.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-value.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-value.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/contributing.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/compatibility-plan.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/compatibility-plan.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-context.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-context.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-doc.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/api-doc.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/trace.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/trace.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/setup-environment.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/docs/setup-environment.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/.github/CONTRIBUTING.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/node-sass/src/libsass/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/object.assign/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/object.assign/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-duplicate-keys/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-duplicate-keys/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/repeating/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/repeating/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/kind-of/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/kind-of/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/num2fraction/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/num2fraction/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/expand-brackets/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/expand-brackets/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-loader/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-loader/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-loader/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-loader/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loader-runner/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loader-runner/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tryit/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tryit/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/regjsgen/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/regjsgen/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/async/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/async/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/async/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/async/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/uglify-to-browserify/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/uglify-to-browserify/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/create-hash/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/create-hash/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-union/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-union/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/glob/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/glob/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/glob/changelog.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/glob/changelog.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/globals/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/globals/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/arrify/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/arrify/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es-to-primitive/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es-to-primitive/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es-to-primitive/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es-to-primitive/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/diffie-hellman/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/diffie-hellman/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lazy-cache/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lazy-cache/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loader-utils/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loader-utils/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/loader-utils/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/loader-utils/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/core-js/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/core-js/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pify/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pify/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-dotfile/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-dotfile/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-trailing-function-commas/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-syntax-trailing-function-commas/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/foreach/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/foreach/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-fullwidth-code-point/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-fullwidth-code-point/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/strip-bom/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/strip-bom/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/getpass/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/getpass/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/require-main-filename/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/require-main-filename/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/punycode/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/punycode/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/buffer-xor/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/buffer-xor/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-weak-map/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-weak-map/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/content-type/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/content-type/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/request/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/request/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/request/node_modules/uuid/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/request/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/request/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eventsource/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eventsource/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/eventsource/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/eventsource/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/select-hose/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/select-hose/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/arr-diff/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/arr-diff/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/osenv/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/osenv/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jodid25519/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jodid25519/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/file-entry-cache/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/file-entry-cache/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/file-entry-cache/changelog.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/file-entry-cache/changelog.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/cli-cursor/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/cli-cursor/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-symbol/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-symbol/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/ansi-escapes/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/ansi-escapes/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caniuse-api/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caniuse-api/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/caniuse-api/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/caniuse-api/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-core/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-core/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-modules-scope/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-modules-scope/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/iconv-lite/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/iconv-lite/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/iconv-lite/Changelog.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/iconv-lite/Changelog.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/number-is-nan/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/number-is-nan/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-normalize-url/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-normalize-url/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-normalize-url/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-normalize-url/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/normalize-range/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/normalize-range/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-unique/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-unique/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/read-pkg/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/read-pkg/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json-stringify-safe/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json-stringify-safe/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json-stringify-safe/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json-stringify-safe/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/type-check/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/type-check/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/normalize-package-data/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/normalize-package-data/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/vary/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/vary/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/vary/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/vary/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/trim-right/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/trim-right/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/boom/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/boom/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/assert-plus/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/assert-plus/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/postcss-message-helpers/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/postcss-message-helpers/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-do-expressions/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-do-expressions/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-async-generator-functions/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-async-generator-functions/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/sax/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/sax/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/set-immediate-shim/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/set-immediate-shim/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-stage-2/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-stage-2/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-block-scoping/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-es2015-block-scoping/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/for-in/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/for-in/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/inflight/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/inflight/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsx-ast-utils/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/once/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/once/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tweetnacl/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tweetnacl/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tweetnacl/AUTHORS.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tweetnacl/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tweetnacl/PULL_REQUEST_TEMPLATE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tweetnacl/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/tweetnacl/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/tweetnacl/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-display-name/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-plugin-transform-react-display-name/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/pbkdf2/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/pbkdf2/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/doctrine/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/doctrine/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/doctrine/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/doctrine/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isobject/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isobject/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/whatwg-fetch/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/whatwg-fetch/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/semver/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/semver/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/babel-preset-stage-1/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/babel-preset-stage-1/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/function-bind/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/function-bind/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/forwarded/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/forwarded/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isexe/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isexe/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsonpointer/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsonpointer/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/jsonpointer/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/jsonpointer/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/colormin/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/colormin/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/colormin/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/colormin/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/proxy-addr/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/proxy-addr/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/proxy-addr/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/proxy-addr/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/os-locale/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/os-locale/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/flat-cache/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/flat-cache/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/flat-cache/changelog.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/flat-cache/changelog.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/colors/ReadMe.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/colors/ReadMe.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/lodash/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/lodash/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/accepts/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/accepts/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/accepts/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/accepts/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-find-index/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-find-index/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/array-uniq/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/array-uniq/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/path-parse/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/path-parse/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/is-number/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/is-number/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/HISTORY.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/HISTORY.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/ms/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/ms/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/ms/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/ms/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/debug/Readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/debug/Readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/debug/History.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/serve-index/node_modules/debug/History.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/glob-base/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/glob-base/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/spdx-expression-parse/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/spdx-expression-parse/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json5/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json5/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json5/CHANGELOG.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/json5/LICENSE.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/json5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/prr/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/prr/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/memory-fs/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/memory-fs/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/yallist/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/yallist/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/chalk/node_modules/supports-color/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/chalk/node_modules/supports-color/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/chalk/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/chalk/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/es6-iterator/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/es6-iterator/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/webpack/node_modules/loader-utils/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/webpack/node_modules/loader-utils/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/isomorphic-fetch/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/isomorphic-fetch/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/levn/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/levn/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/bn.js/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/bn.js/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/normalize-path/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/normalize-path/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/escape-string-regexp/readme.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/escape-string-regexp/readme.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/des.js/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/des.js/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/js/node_modules/verror/README.md` & `solvebio-2.9.0/solvebio/contrib/dash/js/node_modules/verror/README.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/login.js` & `solvebio-2.9.0/solvebio/contrib/dash/login.js`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/tmp/oauth.py` & `solvebio-2.9.0/solvebio/contrib/dash/tmp/oauth.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/solvebio_auth.py` & `solvebio-2.9.0/solvebio/contrib/dash/solvebio_auth.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/solvebio_dash.py` & `solvebio-2.9.0/solvebio/contrib/dash/solvebio_dash.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/tests/test_solvebio_auth_integration.py` & `solvebio-2.9.0/solvebio/contrib/dash/tests/test_solvebio_auth_integration.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/tests/IntegrationTests.py` & `solvebio-2.9.0/solvebio/contrib/dash/tests/IntegrationTests.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/tests/utils.py` & `solvebio-2.9.0/solvebio/contrib/dash/tests/utils.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/contrib/dash/tests/test_solvebio_auth.py` & `solvebio-2.9.0/solvebio/contrib/dash/tests/test_solvebio_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             self._oauth_client_id,
             secret_key='test-secret-key',
             salt='test-salt'
         )
         app.layout = html.Div()
 
         creator = self._oauth_token
-        f = 'solvebio.contrib.dash.solvebio_auth.SolveBioAuth.check_view_access' # noqa
+        f = 'solvebio.contrib.dash.solvebio_auth.SolveBioAuth.check_view_access'  # noqa
         with mock.patch(f, wraps=auth.check_view_access) as wrapped:
             self.check_endpoints(auth, app, creator)
             res = self.check_endpoints(auth, app, creator)
 
             n_endpoints = (
                 len(endpoints['protected']['get']) +
                 len(endpoints['unprotected']['get']))
```

### Comparing `solvebio-2.8.9/solvebio/contrib/vcf_parser/vcf_parser.py` & `solvebio-2.9.0/solvebio/contrib/vcf_parser/vcf_parser.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/cli/credentials.py` & `solvebio-2.9.0/solvebio/cli/credentials.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/cli/tutorial.md` & `solvebio-2.9.0/solvebio/cli/tutorial.md`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/cli/main.py` & `solvebio-2.9.0/solvebio/cli/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -179,40 +179,107 @@
         },
         'upload': {
             'func': data.upload,
             'help': 'Upload a file or directory to a SolveBio Vault',
             'arguments': [
                 {
                     'flags': '--full-path',
-                    'required': True,
                     'help': 'The full path where the files and folders should '
                     'be created, defaults to the root of your personal vault',
-                    'action': TildeFixStoreAction
+                    'action': TildeFixStoreAction,
+                    'default': '~/'
                 },
                 {
-                    'flags': '--vault',
-                    'help': 'The vault where the files will be uploaded. '
-                    'Defaults to your personal vault. '
-                    'Overrides the vault component of --full-path',
-                    'action': TildeFixStoreAction
+                    'flags': '--create-full-path',
+                    'help': 'Creates --full-path location if it does '
+                    'not exist. NOTE: This will not create new vaults.',
+                    'action': 'store_true',
                 },
                 {
-                    'flags': '--path',
-                    'help': 'The path (relative to a vault) '
-                    'where the files will be uploaded. '
-                    'Overrides the path component of --full-path'
+                    'flags': '--exclude',
+                    'help': 'Paths to files or folder to be excluded from '
+                    'upload. Unix shell-style wildcards are supported.',
+                    'action': 'append'
+                },
+                {
+                    'flags': '--dry-run',
+                    'help': 'Dry run mode will not upload any files or '
+                    'create any folders.',
+                    'action': 'store_true'
                 },
                 {
                     'name': 'local_path',
                     'help': 'The path to the local file or directory '
                             'to upload',
                     'nargs': '+'
                 }
             ]
         },
+        'tag': {
+            'func': data.tag,
+            'help': 'Apply tags or remove tags on objects',
+            'arguments': [
+                {
+                    'flags': 'full_path',
+                    'help': 'The full path of the files, '
+                    'folders or datasets to apply the tag updates. '
+                    'Unix shell-style wildcards are supported. ',
+                    'nargs': '+'
+                },
+                {
+                    'name': '--tag',
+                    'help': 'A tag to be added/removed. '
+                    'Files, folders and datasets can be tagged. '
+                    'Tags are case insensitive strings. Example tags: '
+                    '--tag GRCh38 --tag Tissue --tag "Foundation Medicine"',
+                    'action': 'append',
+                    'required': True
+                },
+                {
+                    'flags': '--remove',
+                    'help': 'Will remove tags instead of adding them.',
+                    'action': 'store_true'
+                },
+                {
+                    'flags': '--exclude',
+                    'help': 'Paths to files or folder to be excluded from '
+                    'tagging. Unix shell-style wildcards are supported.',
+                    'action': 'append'
+                },
+                {
+                    'flags': '--tag-folders-only',
+                    'help': 'Will only apply tags to folders (tags '
+                    'all objects by default). ',
+                    'action': 'store_true'
+                },
+                {
+                    'flags': '--tag-files-only',
+                    'help': 'Will only apply tags to files (tags '
+                    'all objects by default). ',
+                    'action': 'store_true'
+                },
+                {
+                    'flags': '--tag-datasets-only',
+                    'help': 'Will only apply tags to datasets (tags '
+                    'all objects by default). ',
+                    'action': 'store_true'
+                },
+                {
+                    'flags': '--dry-run',
+                    'help': 'Dry run mode will not save tags.',
+                    'action': 'store_true'
+                },
+                {
+                    'flags': '--no-input',
+                    'help': 'Automatically accept changes (overrides '
+                    'user prompt)',
+                    'action': 'store_true'
+                },
+            ]
+        },
     }
 
     def __init__(self, *args, **kwargs):
         super(SolveArgumentParser, self).__init__(*args, **kwargs)
         self._optionals.title = 'SolveBio Options'
         self.add_argument(
             '--version',
```

### Comparing `solvebio-2.8.9/solvebio/cli/ipython_init.py` & `solvebio-2.9.0/solvebio/cli/ipython_init.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/cli/auth.py` & `solvebio-2.9.0/solvebio/cli/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,24 +59,24 @@
         # Run the global login() if kwargs are provided
         # or local credentials are found.
         solvebio.login(**kwargs)
     else:
         interactive_login()
 
     # Print information about the current user
-    user = client.whoami()
-
-    if user:
+    try:
+        user = client.whoami()
+    except Exception as e:
+        _print_msg(e.message)
+        return False
+    else:
         print_user(user)
         save_credentials(user['email'].lower(), solvebio.api_key)
         _print_msg('Updated local credentials.')
         return True
-    else:
-        _print_msg('Invalid credentials. You may not be logged-in.')
-        return False
 
 
 def interactive_login():
     """
     Force an interactive login via the command line.
     Sets the global API key and updates the client auth.
     """
@@ -114,20 +114,20 @@
 
 
 def whoami(*args, **kwargs):
     """
     Prints information about the current user.
     Assumes the user is already logged-in.
     """
-    user = client.whoami()
-
-    if user:
-        print_user(user)
+    try:
+        user = client.whoami()
+    except Exception as e:
+        print(e.message)
     else:
-        print('You are not logged-in.')
+        print_user(user)
 
 
 def print_user(user):
     """
     Prints information about the current user.
     """
     email = user['email']
```

### Comparing `solvebio-2.8.9/solvebio/cli/ipython.py` & `solvebio-2.9.0/solvebio/cli/ipython.py`

 * *Files identical despite different names*

### Comparing `solvebio-2.8.9/solvebio/errors.py` & `solvebio-2.9.0/solvebio/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 logger = logging.getLogger('solvebio')
 
 
 class NotFoundError(Exception):
     pass
 
 
+class FileUploadError(Exception):
+    pass
+
+
 class SolveError(Exception):
     """Exceptions tailored to the kinds of errors from a SolveBio API
     request"""
     default_message = ('Unexpected error communicating with SolveBio. '
                        'If this problem persists, let us know at '
                        'support@solvebio.com.')
```

### Comparing `solvebio-2.8.9/solvebio/__init__.py` & `solvebio-2.9.0/solvebio/__init__.py`

 * *Files identical despite different names*

