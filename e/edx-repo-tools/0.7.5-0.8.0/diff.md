# Comparing `tmp/edx-repo-tools-0.7.5.tar.gz` & `tmp/edx-repo-tools-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-repo-tools-0.7.5.tar", last modified: Thu May 11 16:29:42 2023, max compression
+gzip compressed data, was "edx-repo-tools-0.8.0.tar", last modified: Mon Jun 12 12:49:40 2023, max compression
```

## Comparing `edx-repo-tools-0.7.5.tar` & `edx-repo-tools-0.8.0.tar`

### file list

```diff
@@ -1,100 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.245565 edx-repo-tools-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-05-11 16:29:42.245565 edx-repo-tools-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.237565 edx-repo-tools-0.7.5/edx_repo_tools/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/add_common_constraint.py
--rw-r--r--   0 runner    (1001) docker     (122)     7051 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.237565 edx-repo-tools-0.7.5/edx_repo_tools/codemods/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.237565 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django2/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django2/auth_anonymous_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django2/foreignkey_on_delete_mod.py
--rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django2/widget_add_renderer_mod.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.241565 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3125 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/add_new_django32_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/github_actions_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3830 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/github_actions_modernizer_django.py
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/remove_python2_unicode_compatible.py
--rw-r--r--   0 runner    (1001) docker     (122)     1372 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/replace_render_to_response.py
--rw-r--r--   0 runner    (1001) docker     (122)      500 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/replace_static.py
--rw-r--r--   0 runner    (1001) docker     (122)      814 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/replace_unicode_with_str.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/setup_file_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4132 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/tox_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4613 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/travis_modernizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.241565 edx-repo-tools-0.7.5/edx_repo_tools/codemods/node16/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/node16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2913 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/node16/gha_ci_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/codemods/node16/gha_release_workflow_modernizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.241565 edx-repo-tools-0.7.5/edx_repo_tools/conventional_commits/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/conventional_commits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6830 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/conventional_commits/commitstats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2626 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/dependabot_yml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.241565 edx-repo-tools-0.7.5/edx_repo_tools/dev/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2390 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/dev/clone_org.py
--rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/dev/get_org_repo_urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/dev/show_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.241565 edx-repo-tools-0.7.5/edx_repo_tools/find_dependencies/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/find_dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10833 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/find_dependencies/find_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.241565 edx-repo-tools-0.7.5/edx_repo_tools/gitgraft/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/gitgraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22365 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/gitgraft/gitgraft.py
--rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      977 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/modernize_openedx_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.241565 edx-repo-tools-0.7.5/edx_repo_tools/oep2/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/oep2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.241565 edx-repo-tools-0.7.5/edx_repo_tools/oep2/checks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/oep2/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/oep2/checks/check_explicit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6240 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/oep2/checks/check_oep10.py
--rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/oep2/checks/check_oep2.py
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/oep2/explode_repos_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.241565 edx-repo-tools-0.7.5/edx_repo_tools/oep2/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/oep2/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/oep2/report/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/oep2/report/oep2-report.ini
--rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/oep2/report/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.241565 edx-repo-tools-0.7.5/edx_repo_tools/ospr/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/ospr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/ospr/no_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.245565 edx-repo-tools-0.7.5/edx_repo_tools/release/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28778 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/release/tag_release.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.245565 edx-repo-tools-0.7.5/edx_repo_tools/repo_access_scraper/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/repo_access_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6613 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/repo_access_scraper/repo_access_scraper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/edx_repo_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.237565 edx-repo-tools-0.7.5/edx_repo_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-05-11 16:29:42.000000 edx-repo-tools-0.7.5/edx_repo_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-05-11 16:29:42.000000 edx-repo-tools-0.7.5/edx_repo_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 16:29:42.000000 edx-repo-tools-0.7.5/edx_repo_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-05-11 16:29:42.000000 edx-repo-tools-0.7.5/edx_repo_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-05-11 16:29:42.000000 edx-repo-tools-0.7.5/edx_repo_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-11 16:29:42.000000 edx-repo-tools-0.7.5/edx_repo_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.245565 edx-repo-tools-0.7.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 16:29:42.245565 edx-repo-tools-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4674 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:42.245565 edx-repo-tools-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/tests/test_actions_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/tests/test_actions_modernizer_django.py
--rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/tests/test_add_new_django32_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/tests/test_gha_release_workflow_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/tests/test_modernize_openedx_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/tests/test_node_ci_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/tests/test_remove_python2_unicode_compatible.py
--rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/tests/test_replace_render_to_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/tests/test_setup_file_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)    16510 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/tests/test_tag_release.py
--rw-r--r--   0 runner    (1001) docker     (122)     4131 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/tests/test_tox_modernizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3517 2023-05-11 16:29:37.000000 edx-repo-tools-0.7.5/tests/test_travis_modernizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.636682 edx-repo-tools-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3179 2023-06-12 12:49:40.636682 edx-repo-tools-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.628682 edx-repo-tools-0.8.0/edx_repo_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/add_common_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7051 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.628682 edx-repo-tools-0.8.0/edx_repo_tools/codemods/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.628682 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django2/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django2/auth_anonymous_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django2/foreignkey_on_delete_mod.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django2/widget_add_renderer_mod.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.628682 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3125 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/add_new_django32_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/github_actions_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3830 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/github_actions_modernizer_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/remove_python2_unicode_compatible.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1372 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/replace_render_to_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)      500 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/replace_static.py
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/replace_unicode_with_str.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/setup_file_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4132 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/tox_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4613 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/travis_modernizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.628682 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django42/
+-rw-r--r--   0 runner    (1001) docker     (122)     4308 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/django42/tox_moderniser_django42.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.628682 edx-repo-tools-0.8.0/edx_repo_tools/codemods/node16/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/node16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2913 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/node16/gha_ci_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/codemods/node16/gha_release_workflow_modernizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.628682 edx-repo-tools-0.8.0/edx_repo_tools/conventional_commits/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/conventional_commits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6830 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/conventional_commits/commitstats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2626 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/dependabot_yml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.632682 edx-repo-tools-0.8.0/edx_repo_tools/dev/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2390 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/dev/clone_org.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/dev/get_org_repo_urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/dev/show_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.632682 edx-repo-tools-0.8.0/edx_repo_tools/find_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/find_dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10833 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/find_dependencies/find_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.632682 edx-repo-tools-0.8.0/edx_repo_tools/gitgraft/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/gitgraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22365 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/gitgraft/gitgraft.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/modernize_openedx_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.632682 edx-repo-tools-0.8.0/edx_repo_tools/oep2/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/oep2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.632682 edx-repo-tools-0.8.0/edx_repo_tools/oep2/checks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/oep2/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/oep2/checks/check_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6240 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/oep2/checks/check_oep10.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/oep2/checks/check_oep2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/oep2/explode_repos_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.632682 edx-repo-tools-0.8.0/edx_repo_tools/oep2/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/oep2/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/oep2/report/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/oep2/report/oep2-report.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/oep2/report/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.632682 edx-repo-tools-0.8.0/edx_repo_tools/ospr/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/ospr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/ospr/no_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.632682 edx-repo-tools-0.8.0/edx_repo_tools/release/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28778 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/release/tag_release.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.632682 edx-repo-tools-0.8.0/edx_repo_tools/repo_access_scraper/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/repo_access_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6613 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/repo_access_scraper/repo_access_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.632682 edx-repo-tools-0.8.0/edx_repo_tools/repo_checks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/repo_checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6306 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/repo_checks/labels.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    35545 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/repo_checks/repo_checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/edx_repo_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.628682 edx-repo-tools-0.8.0/edx_repo_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3179 2023-06-12 12:49:40.000000 edx-repo-tools-0.8.0/edx_repo_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3329 2023-06-12 12:49:40.000000 edx-repo-tools-0.8.0/edx_repo_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 12:49:40.000000 edx-repo-tools-0.8.0/edx_repo_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-06-12 12:49:40.000000 edx-repo-tools-0.8.0/edx_repo_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4801 2023-06-12 12:49:40.000000 edx-repo-tools-0.8.0/edx_repo_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-12 12:49:40.000000 edx-repo-tools-0.8.0/edx_repo_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.632682 edx-repo-tools-0.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-12 12:49:40.636682 edx-repo-tools-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5333 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:40.636682 edx-repo-tools-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/test_actions_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/test_actions_modernizer_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/test_add_new_django32_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/test_gha_release_workflow_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/test_modernize_openedx_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/test_node_ci_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/test_remove_python2_unicode_compatible.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/test_replace_render_to_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2814 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/test_repo_checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/test_setup_file_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16510 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/test_tag_release.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4131 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/test_tox_modernizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3517 2023-06-12 12:49:35.000000 edx-repo-tools-0.8.0/tests/test_travis_modernizer.py
```

### Comparing `edx-repo-tools-0.7.5/LICENSE.txt` & `edx-repo-tools-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/NOTICE.txt` & `edx-repo-tools-0.8.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/PKG-INFO` & `edx-repo-tools-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: edx-repo-tools
-Version: 0.7.5
+Version: 0.8.0
 Summary: This repo contains a number of tools Open edX uses for working with GitHub repositories.
 Home-page: https://github.com/openedx/repo-tools
 Author: edX
 Author-email: oscm@edx.org
 License: Apache
 Keywords: edx repo tools
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Provides-Extra: find_dependencies
 Provides-Extra: repo_access_scraper
+Provides-Extra: repo_checks
 Provides-Extra: conventional_commits
+Provides-Extra: dev
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 ###################
 Open edX Repo Tools
 ###################
```

### Comparing `edx-repo-tools-0.7.5/README.rst` & `edx-repo-tools-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/add_common_constraint.py` & `edx-repo-tools-0.8.0/edx_repo_tools/add_common_constraint.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/auth.py` & `edx-repo-tools-0.8.0/edx_repo_tools/auth.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/django2/auth_anonymous_update.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/django2/auth_anonymous_update.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/django2/foreignkey_on_delete_mod.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/django2/foreignkey_on_delete_mod.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/django2/widget_add_renderer_mod.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/django2/widget_add_renderer_mod.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/add_new_django32_settings.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/add_new_django32_settings.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/github_actions_modernizer.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/github_actions_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/github_actions_modernizer_django.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/github_actions_modernizer_django.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/remove_python2_unicode_compatible.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/remove_python2_unicode_compatible.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/replace_render_to_response.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/replace_render_to_response.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/replace_unicode_with_str.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/replace_unicode_with_str.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/setup_file_modernizer.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/setup_file_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/tox_modernizer.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/tox_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/django3/travis_modernizer.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/django3/travis_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/node16/gha_ci_modernizer.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/node16/gha_ci_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/codemods/node16/gha_release_workflow_modernizer.py` & `edx-repo-tools-0.8.0/edx_repo_tools/codemods/node16/gha_release_workflow_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/conventional_commits/commitstats.py` & `edx-repo-tools-0.8.0/edx_repo_tools/conventional_commits/commitstats.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/data.py` & `edx-repo-tools-0.8.0/edx_repo_tools/data.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/dependabot_yml.py` & `edx-repo-tools-0.8.0/edx_repo_tools/dependabot_yml.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/dev/clone_org.py` & `edx-repo-tools-0.8.0/edx_repo_tools/dev/clone_org.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/dev/get_org_repo_urls.py` & `edx-repo-tools-0.8.0/edx_repo_tools/dev/get_org_repo_urls.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/dev/show_hooks.py` & `edx-repo-tools-0.8.0/edx_repo_tools/dev/show_hooks.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/find_dependencies/find_dependencies.py` & `edx-repo-tools-0.8.0/edx_repo_tools/find_dependencies/find_dependencies.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/gitgraft/gitgraft.py` & `edx-repo-tools-0.8.0/edx_repo_tools/gitgraft/gitgraft.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/helpers.py` & `edx-repo-tools-0.8.0/edx_repo_tools/helpers.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/modernize_openedx_yaml.py` & `edx-repo-tools-0.8.0/edx_repo_tools/modernize_openedx_yaml.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/oep2/checks/check_explicit.py` & `edx-repo-tools-0.8.0/edx_repo_tools/oep2/checks/check_explicit.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/oep2/checks/check_oep10.py` & `edx-repo-tools-0.8.0/edx_repo_tools/oep2/checks/check_oep10.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/oep2/checks/check_oep2.py` & `edx-repo-tools-0.8.0/edx_repo_tools/oep2/checks/check_oep2.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/oep2/explode_repos_yaml.py` & `edx-repo-tools-0.8.0/edx_repo_tools/oep2/explode_repos_yaml.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/oep2/report/cli.py` & `edx-repo-tools-0.8.0/edx_repo_tools/oep2/report/cli.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/oep2/report/plugin.py` & `edx-repo-tools-0.8.0/edx_repo_tools/oep2/report/plugin.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/ospr/no_yaml.py` & `edx-repo-tools-0.8.0/edx_repo_tools/ospr/no_yaml.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/release/tag_release.py` & `edx-repo-tools-0.8.0/edx_repo_tools/release/tag_release.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/repo_access_scraper/repo_access_scraper.py` & `edx-repo-tools-0.8.0/edx_repo_tools/repo_access_scraper/repo_access_scraper.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools/utils.py` & `edx-repo-tools-0.8.0/edx_repo_tools/utils.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools.egg-info/PKG-INFO` & `edx-repo-tools-0.8.0/edx_repo_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: edx-repo-tools
-Version: 0.7.5
+Version: 0.8.0
 Summary: This repo contains a number of tools Open edX uses for working with GitHub repositories.
 Home-page: https://github.com/openedx/repo-tools
 Author: edX
 Author-email: oscm@edx.org
 License: Apache
 Keywords: edx repo tools
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Provides-Extra: find_dependencies
 Provides-Extra: repo_access_scraper
+Provides-Extra: repo_checks
 Provides-Extra: conventional_commits
+Provides-Extra: dev
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 ###################
 Open edX Repo Tools
 ###################
```

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools.egg-info/SOURCES.txt` & `edx-repo-tools-0.8.0/edx_repo_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 edx_repo_tools/codemods/django3/remove_python2_unicode_compatible.py
 edx_repo_tools/codemods/django3/replace_render_to_response.py
 edx_repo_tools/codemods/django3/replace_static.py
 edx_repo_tools/codemods/django3/replace_unicode_with_str.py
 edx_repo_tools/codemods/django3/setup_file_modernizer.py
 edx_repo_tools/codemods/django3/tox_modernizer.py
 edx_repo_tools/codemods/django3/travis_modernizer.py
+edx_repo_tools/codemods/django42/tox_moderniser_django42.py
 edx_repo_tools/codemods/node16/__init__.py
 edx_repo_tools/codemods/node16/gha_ci_modernizer.py
 edx_repo_tools/codemods/node16/gha_release_workflow_modernizer.py
 edx_repo_tools/conventional_commits/__init__.py
 edx_repo_tools/conventional_commits/commitstats.py
 edx_repo_tools/dev/__init__.py
 edx_repo_tools/dev/clone_org.py
@@ -58,22 +59,26 @@
 edx_repo_tools/oep2/report/plugin.py
 edx_repo_tools/ospr/__init__.py
 edx_repo_tools/ospr/no_yaml.py
 edx_repo_tools/release/__init__.py
 edx_repo_tools/release/tag_release.py
 edx_repo_tools/repo_access_scraper/__init__.py
 edx_repo_tools/repo_access_scraper/repo_access_scraper.py
+edx_repo_tools/repo_checks/__init__.py
+edx_repo_tools/repo_checks/labels.yaml
+edx_repo_tools/repo_checks/repo_checks.py
 requirements/base.in
 requirements/constraints.txt
 tests/__init__.py
 tests/test_actions_modernizer.py
 tests/test_actions_modernizer_django.py
 tests/test_add_new_django32_settings.py
 tests/test_gha_release_workflow_modernizer.py
 tests/test_modernize_openedx_yaml.py
 tests/test_node_ci_modernizer.py
 tests/test_remove_python2_unicode_compatible.py
 tests/test_replace_render_to_response.py
+tests/test_repo_checks.py
 tests/test_setup_file_modernizer.py
 tests/test_tag_release.py
 tests/test_tox_modernizer.py
 tests/test_travis_modernizer.py
```

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools.egg-info/entry_points.txt` & `edx-repo-tools-0.8.0/edx_repo_tools.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 modernize_github_actions = edx_repo_tools.codemods.django3.github_actions_modernizer:main
 modernize_github_actions_django = edx_repo_tools.codemods.django3.github_actions_modernizer_django:main
 modernize_node_release_workflow = edx_repo_tools.codemods.node16.gha_release_workflow_modernizer:main
 modernize_node_workflow = edx_repo_tools.codemods.node16.gha_ci_modernizer:main
 modernize_openedx_yaml = edx_repo_tools.modernize_openedx_yaml:main
 modernize_setup_file = edx_repo_tools.codemods.django3.setup_file_modernizer:main
 modernize_tox = edx_repo_tools.codemods.django3.tox_modernizer:main
+modernize_tox_django42 = edx_repo_tools.codemods.django42.tox_moderniser_django42:main
 modernize_travis = edx_repo_tools.codemods.django3.travis_modernizer:main
 no_yaml = edx_repo_tools.ospr.no_yaml:no_yaml
 oep2 = edx_repo_tools.oep2:_cli
 remove_python2_unicode_compatible = edx_repo_tools.codemods.django3.remove_python2_unicode_compatible:main
 replace_render_to_response = edx_repo_tools.codemods.django3.replace_render_to_response:main
 replace_static = edx_repo_tools.codemods.django3.replace_static:main
 replace_unicode_with_str = edx_repo_tools.codemods.django3.replace_unicode_with_str:main
 repo_access_scraper = edx_repo_tools.repo_access_scraper.repo_access_scraper:main
+repo_checks = edx_repo_tools.repo_checks.repo_checks:main
 show_hooks = edx_repo_tools.dev.show_hooks:main
 tag_release = edx_repo_tools.release.tag_release:main
```

### Comparing `edx-repo-tools-0.7.5/edx_repo_tools.egg-info/requires.txt` & `edx-repo-tools-0.8.0/edx_repo_tools.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,129 +1,284 @@
-virtualenv==20.23.0
-scrapy==2.8.0
-filelock==3.12.0
-pluggy==1.0.0
-cssselect==1.2.0
-urllib3==1.26.15
-constantly==15.1.0
-idna==3.4
-numpy==1.24.3
-pyyaml==6.0
-iniconfig==2.0.0
-typing-extensions==4.5.0
-six==1.16.0
-docutils==0.19
-appdirs==1.4.4
-requests-toolbelt==1.0.0
-gitdb==4.0.10
-python-dotenv==1.0.0
-tqdm==4.65.0
-service-identity==21.1.0
-click==8.1.3
-statistics==1.0.3.5
-smmap==5.0.0
-ruamel-yaml==0.17.22
-pyopenssl==23.1.1
-w3lib==2.1.1
+packaging==23.1
+cffi==1.15.1
 gitpython==3.1.31
+platformdirs==3.5.1
+fissix==21.11.13
+statistics==1.0.3.5
+six==1.16.0
 lockfile==0.12.2
-volatile==2.1.0
-itemloaders==1.1.0
-path==16.6.0
-lazy==1.5
-pyasn1==0.5.0
-twisted==22.10.0
-protego==0.2.1
-cffi==1.15.1
-hyperlink==21.0.0
-oauthlib==3.2.2
+appdirs==1.4.4
+filelock==3.12.0
+virtualenv==20.23.0
 exceptiongroup==1.1.1
-packaging==23.1
-ruamel-yaml-clib==0.2.7
-pyjwt[crypto]==2.6.0
-execnet==1.9.0
+bowler==0.9.0
+volatile==2.1.0
+tomli==2.0.1
+pyjwt[crypto]==2.7.0
+distlib==0.3.6
+queuelib==1.6.2
+pyyaml==6.0
+urllib3==2.0.3
 parsel==1.8.1
-pycparser==2.21
+smmap==5.0.0
+click==8.1.3
 path-py==12.5.0
-zope-interface==6.0
-github3-py==4.0.1
-itemadapter==0.8.0
-distlib==0.3.6
-tlslite==0.4.9
-cachecontrol==0.12.11
-pytest==7.3.1
+python-dotenv==1.0.0
+twisted==22.10.0
+pyopenssl==23.2.0
 requests-oauthlib==1.3.1
-charset-normalizer==3.1.0
-bowler==0.9.0
-moreorless==0.4.0
-msgpack==1.0.5
+pluggy==1.0.0
+py==1.11.0
+execnet==1.9.0
 pydispatcher==2.0.7
-requests==2.29.0
-tldextract==3.4.1
-pytest-xdist==3.2.1
-pyasn1-modules==0.3.0
-platformdirs==3.5.0
-python-dateutil==2.8.2
+scrapy==2.9.0
+attrs==23.1.0
+certifi==2023.5.7
+idna==3.4
+jmespath==1.0.1
+msgpack==1.0.5
+requests-file==1.5.1
+path==16.6.0
+tlslite==0.4.9
+lxml==4.9.2
 tox==3.28.0
-automat==22.10.0
+cssselect==1.2.0
+w3lib==2.1.1
+hyperlink==21.0.0
+itemloaders==1.1.0
+charset-normalizer==3.1.0
+typing-extensions==4.6.3
+zope-interface==6.0
+docutils==0.20.1
+tqdm==4.65.0
+cryptography==41.0.1
+ruamel-yaml==0.17.31
+backports-csv==1.0.7
 more-itertools==9.1.0
-queuelib==1.6.2
-fissix==21.11.13
-jmespath==1.0.1
-tomli==2.0.1
+numpy==1.24.3
+pyasn1-modules==0.3.0
+ruamel-yaml-clib==0.2.7
+service-identity==21.1.0
+uritemplate==4.1.1
+lazy==1.5
 incremental==22.10.0
-py==1.11.0
+python-dateutil==2.8.2
 jira==1.0.3
-cryptography==40.0.2
-attrs==23.1.0
-pytest-logging==2015.11.4
+requests-toolbelt==1.0.0
+iniconfig==2.0.0
+requests==2.31.0
+pytest==7.3.1
+constantly==15.1.0
 urlobject==2.4.3
-lxml==4.9.2
-certifi==2022.12.7
-requests-file==1.5.1
-uritemplate==4.1.1
-backports-csv==1.0.7
+pytest-logging==2015.11.4
+protego==0.2.1
+tldextract==3.4.4
+itemadapter==0.8.0
+pycparser==2.21
+automat==22.10.0
+pyasn1==0.5.0
+oauthlib==3.2.2
+pytest-xdist==3.3.1
+github3-py==4.0.1
+gitdb==4.0.10
+cachecontrol==0.13.0
+moreorless==0.4.0
 
 [conventional_commits]
-sqlalchemy==1.4.48
-cycler==0.11.0
 packaging==23.1
-python-dateutil==2.8.2
-pandas==2.0.1
-pillow==9.5.0
-alembic==1.10.4
-dataset==1.6.0
-pyparsing==3.0.9
-fonttools==4.39.3
-banal==1.0.6
+typing-extensions==4.6.3
 importlib-metadata==6.6.0
+greenlet==2.0.2
+banal==1.0.6
 tzdata==2023.3
+cycler==0.11.0
+contourpy==1.0.7
+six==1.16.0
 numpy==1.24.3
+markupsafe==2.1.3
+mako==1.2.4
+pandas==2.0.2
+zipp==3.15.0
+importlib-resources==5.12.0
+alembic==1.11.1
+pyparsing==3.0.9
+python-dateutil==2.8.2
 kiwisolver==1.4.4
+dataset==1.6.0
+sqlalchemy==1.4.48
 matplotlib==3.7.1
+pillow==9.5.0
+fonttools==4.39.4
+pytz==2023.3
+
+[dev]
+alembic==1.11.1
+appdirs==1.4.4
+astroid==2.15.5
+attrs==23.1.0
+automat==22.10.0
+backports-csv==1.0.7
+banal==1.0.6
+bowler==0.9.0
+build==0.10.0
+cache-to-disk==2.0.0
+cachecontrol==0.13.0
+certifi==2023.5.7
+cffi==1.15.1
+charset-normalizer==3.1.0
+click-log==0.4.0
+click==8.1.3
+code-annotations==1.3.0
+constantly==15.1.0
+contourpy==1.0.7
+cryptography==41.0.1
+cssselect==1.2.0
+cycler==0.11.0
+dataset==1.6.0
+dill==0.3.6
+distlib==0.3.6
+docutils==0.20.1
+edx-lint==5.3.4
+exceptiongroup==1.1.1
+execnet==1.9.0
+fastcore==1.5.29
+filelock==3.12.0
+fissix==21.11.13
+fonttools==4.39.4
+ghapi==1.0.3
+gitdb==4.0.10
+github3-py==4.0.1
+gitpython==3.1.31
 greenlet==2.0.2
-zipp==3.15.0
+hyperlink==21.0.0
+idna==3.4
+importlib-metadata==6.6.0
 importlib-resources==5.12.0
-typing-extensions==4.5.0
-markupsafe==2.1.2
+incremental==22.10.0
+iniconfig==2.0.0
+isort==5.12.0
+itemadapter==0.8.0
+itemloaders==1.1.0
+jinja2==3.1.2
+jira==1.0.3
+jmespath==1.0.1
+kiwisolver==1.4.4
+lazy-object-proxy==1.9.0
+lazy==1.5
+lockfile==0.12.2
+lxml==4.9.2
+mako==1.2.4
+markdown-it-py==2.2.0
+markupsafe==2.1.3
+matplotlib==3.7.1
+mccabe==0.7.0
+mdurl==0.1.2
+more-itertools==9.1.0
+moreorless==0.4.0
+msgpack==1.0.5
+numpy==1.24.3
+oauthlib==3.2.2
+packaging==23.1
+pandas==2.0.2
+parsel==1.8.1
+path-py==12.5.0
+path==16.6.0
+pbr==5.11.1
+pep8==1.7.1
+pillow==9.5.0
+pip-tools==6.13.0
+platformdirs==3.5.1
+playwright==1.34.0
+pluggy==1.0.0
+protego==0.2.1
+py==1.11.0
+pyasn1-modules==0.3.0
+pyasn1==0.5.0
+pycparser==2.21
+pydispatcher==2.0.7
+pyee==9.0.4
+pygments==2.15.1
+pyjwt[crypto]==2.7.0
+pylint-celery==0.3
+pylint-django==2.5.3
+pylint-plugin-utils==0.8.2
+pylint==2.17.4
+pyopenssl==23.2.0
+pyparsing==3.0.9
+pyproject-hooks==1.0.0
+pytest-logging==2015.11.4
+pytest-mock==3.10.0
+pytest-xdist==3.3.1
+pytest==7.3.1
+python-dateutil==2.8.2
+python-dotenv==1.0.0
+python-slugify==8.0.1
 pytz==2023.3
+pyyaml==6.0
+queuelib==1.6.2
+requests-file==1.5.1
+requests-oauthlib==1.3.1
+requests-toolbelt==1.0.0
+requests==2.31.0
+responses==0.23.1
+rich==13.4.1
+ruamel-yaml-clib==0.2.7
+ruamel-yaml==0.17.31
+scrapy==2.9.0
+service-identity==21.1.0
 six==1.16.0
-contourpy==1.0.7
-mako==1.2.4
+smmap==5.0.0
+sqlalchemy==1.4.48
+statistics==1.0.3.5
+stevedore==5.1.0
+text-unidecode==1.3
+tldextract==3.4.4
+tlslite==0.4.9
+tomli==2.0.1
+tomlkit==0.11.8
+tox==3.28.0
+tqdm==4.65.0
+twisted==22.10.0
+types-pyyaml==6.0.12.10
+typing-extensions==4.6.3
+tzdata==2023.3
+uritemplate==4.1.1
+urllib3==2.0.3
+urlobject==2.4.3
+virtualenv==20.23.0
+volatile==2.1.0
+w3lib==2.1.1
+wheel==0.40.0
+wrapt==1.15.0
+zipp==3.15.0
+zope-interface==6.0
 
 [find_dependencies]
-typing-extensions==4.5.0
-certifi==2022.12.7
-urllib3==1.26.15
-requests==2.29.0
 charset-normalizer==3.1.0
+pygments==2.15.1
 idna==3.4
-rich==13.3.5
-mdurl==0.1.2
+typing-extensions==4.6.3
+urllib3==2.0.3
 markdown-it-py==2.2.0
-pygments==2.15.1
+certifi==2023.5.7
+rich==13.4.1
+mdurl==0.1.2
+requests==2.31.0
 
 [repo_access_scraper]
-greenlet==2.0.1
-typing-extensions==4.5.0
-playwright==1.33.0
+typing-extensions==4.6.3
+playwright==1.34.0
+greenlet==2.0.2
 pyee==9.0.4
+
+[repo_checks]
+packaging==23.1
+fastcore==1.5.29
+click==8.1.3
+charset-normalizer==3.1.0
+urllib3==2.0.3
+cache-to-disk==2.0.0
+certifi==2023.5.7
+idna==3.4
+ghapi==1.0.3
+pyyaml==6.0
+requests==2.31.0
```

### Comparing `edx-repo-tools-0.7.5/setup.py` & `edx-repo-tools-0.8.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,23 @@
 # extra.in file. It will be pip-compiled to extra.txt.  Here we find them all
 # and register them as extras.
 EXTRAS_REQUIRE = {}
 for fextra in glob.glob("edx_repo_tools/*/extra.txt"):
     slug = fextra.split("/")[1]
     EXTRAS_REQUIRE[slug] = load_requirements(fextra)
 
+# To run tests & linting across the entire repo, we need to install the union
+# of *all* extra requirements lists *plus* the dev-specific requirements.
+# If this list contains conflicting pins, then installing it will fail;
+# that is intentional. 
+EXTRAS_REQUIRE["dev"] = sorted({
+    *load_requirements("requirements/development.txt"),
+    *(extra_pin for extra_reqs in EXTRAS_REQUIRE.values() for extra_pin in extra_reqs),
+})
+
 setup(
     name='edx-repo-tools',
     version=VERSION,
     description="This repo contains a number of tools Open edX uses for working with GitHub repositories.",
     long_description=long_description,
     license='Apache',
     keywords='edx repo tools',
@@ -72,14 +81,15 @@
     ],
     packages=setuptools.find_packages(),
     install_requires=load_requirements("requirements/base.txt"),
     extras_require=EXTRAS_REQUIRE,
     entry_points={
         'console_scripts': [
             'add_common_constraint = edx_repo_tools.add_common_constraint:main',
+            'add_dependabot_ecosystem = edx_repo_tools.dependabot_yml:main',
             'add_django32_settings = edx_repo_tools.codemods.django3.add_new_django32_settings:main',
             'clone_org = edx_repo_tools.dev.clone_org:main',
             'conventional_commits = edx_repo_tools.conventional_commits.commitstats:main',
             'find_dependencies = edx_repo_tools.find_dependencies.find_dependencies:main',
             'get_org_repo_urls = edx_repo_tools.dev.get_org_repo_urls:main',
             'modernize_github_actions = edx_repo_tools.codemods.django3.github_actions_modernizer:main',
             'modernize_github_actions_django = edx_repo_tools.codemods.django3.github_actions_modernizer_django:main',
@@ -92,16 +102,18 @@
             'no_yaml = edx_repo_tools.ospr.no_yaml:no_yaml',
             'oep2 = edx_repo_tools.oep2:_cli',
             'remove_python2_unicode_compatible = edx_repo_tools.codemods.django3.remove_python2_unicode_compatible:main',
             'replace_render_to_response = edx_repo_tools.codemods.django3.replace_render_to_response:main',
             'replace_static = edx_repo_tools.codemods.django3.replace_static:main',
             'replace_unicode_with_str = edx_repo_tools.codemods.django3.replace_unicode_with_str:main',
             'repo_access_scraper = edx_repo_tools.repo_access_scraper.repo_access_scraper:main',
+            'repo_checks = edx_repo_tools.repo_checks.repo_checks:main',
             'show_hooks = edx_repo_tools.dev.show_hooks:main',
             'tag_release = edx_repo_tools.release.tag_release:main',
-            'add_dependabot_ecosystem = edx_repo_tools.dependabot_yml:main',
+            'modernize_tox_django42 = edx_repo_tools.codemods.django42.tox_moderniser_django42:main',
         ],
     },
     package_data={
         'edx_repo_tools.oep2.report': ['oep2-report.ini'],
+        'edx_repo_tools.repo_checks': ['labels.yaml'],
     },
 )
```

### Comparing `edx-repo-tools-0.7.5/tests/test_actions_modernizer.py` & `edx-repo-tools-0.8.0/tests/test_actions_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/tests/test_actions_modernizer_django.py` & `edx-repo-tools-0.8.0/tests/test_actions_modernizer_django.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/tests/test_add_new_django32_settings.py` & `edx-repo-tools-0.8.0/tests/test_add_new_django32_settings.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/tests/test_gha_release_workflow_modernizer.py` & `edx-repo-tools-0.8.0/tests/test_gha_release_workflow_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/tests/test_modernize_openedx_yaml.py` & `edx-repo-tools-0.8.0/tests/test_modernize_openedx_yaml.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/tests/test_node_ci_modernizer.py` & `edx-repo-tools-0.8.0/tests/test_node_ci_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/tests/test_remove_python2_unicode_compatible.py` & `edx-repo-tools-0.8.0/tests/test_remove_python2_unicode_compatible.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/tests/test_replace_render_to_response.py` & `edx-repo-tools-0.8.0/tests/test_replace_render_to_response.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/tests/test_setup_file_modernizer.py` & `edx-repo-tools-0.8.0/tests/test_setup_file_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/tests/test_tag_release.py` & `edx-repo-tools-0.8.0/tests/test_tag_release.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/tests/test_tox_modernizer.py` & `edx-repo-tools-0.8.0/tests/test_tox_modernizer.py`

 * *Files identical despite different names*

### Comparing `edx-repo-tools-0.7.5/tests/test_travis_modernizer.py` & `edx-repo-tools-0.8.0/tests/test_travis_modernizer.py`

 * *Files identical despite different names*

