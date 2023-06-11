# Comparing `tmp/pythonce-0.0.4.tar.gz` & `tmp/pythonce-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonce-0.0.4.tar", last modified: Sun Jun 11 21:32:48 2023, max compression
+gzip compressed data, was "pythonce-0.0.5.tar", last modified: Sun Jun 11 23:35:58 2023, max compression
```

## Comparing `pythonce-0.0.4.tar` & `pythonce-0.0.5.tar`

### file list

```diff
@@ -1,1142 +1,1145 @@
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.969871 pythonce-0.0.4/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      300 2023-06-11 21:32:37.000000 pythonce-0.0.4/CHANGELOG.txt
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1059 2023-06-11 19:56:54.000000 pythonce-0.0.4/LINCENCE.txt
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       31 2023-06-11 19:56:54.000000 pythonce-0.0.4/MANIFEST.in
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      823 2023-06-11 21:32:48.969871 pythonce-0.0.4/PKG-INFO
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       45 2023-06-11 19:56:54.000000 pythonce-0.0.4/README.txt
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.765867 pythonce-0.0.4/env/
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.757867 pythonce-0.0.4/env/lib/
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.757867 pythonce-0.0.4/env/lib/python3.13/
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.757867 pythonce-0.0.4/env/lib/python3.13/site-packages/
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.773867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      357 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1198 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/__main__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1444 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/__pip-runner__.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.777867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      573 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10243 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/build_env.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9661 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cache.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.777867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      132 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6676 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/autocompletion.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8176 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/base_command.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30030 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/cmdoptions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      774 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/command_context.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2816 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/main.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4338 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/main_parser.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10817 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/parser.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1968 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/progress_bars.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18328 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/req_command.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5118 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/spinners.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      116 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/status_codes.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.781867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3882 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7581 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/cache.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1684 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/check.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4129 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/completion.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9815 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/configuration.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6591 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/debug.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5182 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/download.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2951 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/freeze.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1703 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/hash.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1132 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/help.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4793 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/index.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3188 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/inspect.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    28722 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/install.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12343 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/list.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5697 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/search.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6419 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/show.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3886 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/uninstall.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6324 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/wheel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13529 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/configuration.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.781867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/distributions/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      858 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/distributions/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1221 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/distributions/base.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      729 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/distributions/installed.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6494 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/distributions/sdist.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1164 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/distributions/wheel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23741 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/exceptions.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.785867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/index/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       30 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/index/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    16504 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/index/collector.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    37873 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/index/package_finder.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6556 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/index/sources.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.785867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/locations/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    15365 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/locations/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6100 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/locations/_distutils.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7680 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/locations/_sysconfig.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2556 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/locations/base.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      340 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/main.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.785867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4280 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2595 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/_json.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    25277 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/base.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.785867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      107 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1882 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8181 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7457 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9773 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.789867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       63 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      990 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/candidate.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6931 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/direct_url.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2520 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/format_control.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1030 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/index.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2619 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/installation_report.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18817 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/link.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      738 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/scheme.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4643 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/search_scope.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1907 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/selection_prefs.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3858 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/target_python.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3600 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/wheel.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.789867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       50 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20435 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/auth.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2145 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/cache.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6096 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/download.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7638 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/lazy_wheel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18442 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/session.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4073 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/utils.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1791 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/xmlrpc.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.789867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/__init__.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.793867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4133 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1422 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/metadata.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1474 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2198 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1075 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/wheel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1417 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3064 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5122 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/check.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9816 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/freeze.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.793867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/install/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       51 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/install/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1282 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27475 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/install/wheel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27696 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/prepare.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7161 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/pyproject.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.793867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/req/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2738 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/req/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    16610 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/req/constructors.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17872 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/req/req_file.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    32782 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/req/req_install.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2858 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/req/req_set.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    24678 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/req/req_uninstall.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.793867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      583 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/base.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.793867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/legacy/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    24128 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.797867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5220 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18864 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27845 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5705 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9824 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3094 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5454 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11538 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8167 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/self_outdated_check.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.801868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3351 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1015 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/_log.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1665 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/appdirs.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1884 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5377 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      242 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/datetime.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3627 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/deprecation.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3206 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2118 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/egg_link.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1169 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/encoding.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3064 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/entrypoints.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5122 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/filesystem.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      716 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/filetypes.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3110 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/glibc.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5118 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/hashes.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      795 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11632 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/logging.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22216 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/misc.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1193 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/models.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2108 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/packaging.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4435 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/setuptools_build.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9200 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/subprocess.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7702 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/temp_dir.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8821 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/unpacking.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1759 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/urls.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3456 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/virtualenv.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4549 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/wheel.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.805868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/vcs/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      596 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/vcs/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3519 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/vcs/bazaar.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18116 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/vcs/git.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5238 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/vcs/mercurial.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11729 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/vcs/subversion.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22811 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11842 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/wheel_builder.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.805868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4966 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/__init__.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.805868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      465 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1379 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5033 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1535 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.805868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/caches/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      242 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5271 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1033 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      778 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    16416 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3946 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4154 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7105 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      774 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.805868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       94 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/certifi/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      255 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/certifi/__main__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4279 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/certifi/core.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.817868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4797 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    31274 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/big5freq.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1763 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/big5prober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10032 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3915 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5420 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.817868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/cli/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3242 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3732 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      542 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1860 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1683 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/enums.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4006 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/escprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12176 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/escsm.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3934 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13566 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1753 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    36913 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1753 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20735 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1759 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14537 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    25796 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    42498 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1752 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/johabprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27055 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   104562 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    98484 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    98196 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   101363 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   128035 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   102774 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    95372 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5380 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6077 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3715 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2131 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30391 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.817868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/metadata/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13560 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      402 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/resultdict.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6400 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4137 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4007 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14848 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8505 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2812 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      244 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/version.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.817868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      266 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2522 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/ansi.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11128 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3325 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/initialise.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.821868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       75 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2839 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10678 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6741 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1866 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1079 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3709 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6181 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/win32.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7134 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/winterm.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.825868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      581 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    41259 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    51697 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/database.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20834 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/index.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    51991 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/locators.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14811 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/manifest.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5058 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/markers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39801 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/metadata.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10820 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/resources.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18102 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/scripts.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    66262 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/util.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23513 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/version.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    43898 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/wheel.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.825868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distro/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      981 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distro/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       64 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distro/__main__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    49330 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distro/distro.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.825868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      849 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3374 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/codec.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      321 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12950 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/core.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    44375 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/idnadata.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1881 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/intranges.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       21 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/package_data.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   206539 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/uts46data.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.829868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/msgpack/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1132 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/msgpack/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1081 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6079 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/msgpack/ext.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34544 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/msgpack/fallback.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.829868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      661 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/__about__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      497 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11488 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4378 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1431 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/_structures.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8487 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/markers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4676 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/requirements.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30110 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/specifiers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    15699 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/tags.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4200 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/utils.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14665 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/version.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.829868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pkg_resources/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   109388 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pkg_resources/__init__.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.833868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18003 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1198 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4303 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/android.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5706 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/api.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2800 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/macos.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7448 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/unix.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      160 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/version.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7098 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/windows.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.833868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2999 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      353 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/__main__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23685 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/cmdline.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1697 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/console.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1938 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/filter.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.833868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/filters/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    40386 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2917 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatter.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.837868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4800 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4104 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3314 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5086 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35601 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    21938 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4981 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    19351 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5073 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2212 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5014 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7335 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4674 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11753 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    32064 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexer.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.837868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11164 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    71556 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    53572 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      986 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/modeline.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2591 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/plugin.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3072 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/regexopt.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3092 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/scanner.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6882 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6257 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/style.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.837868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/styles/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3419 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6184 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/token.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    63187 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/unistring.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9110 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/util.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.841868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9171 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6426 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/actions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12936 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/common.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   213344 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/core.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.841868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/diagram/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23685 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9023 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39129 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    25341 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/results.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13402 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/testing.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10787 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6805 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/util.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.841868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      491 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      138 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11920 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_impl.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.841868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      546 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10927 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.845868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5178 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      435 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/__version__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1397 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    21443 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/adapters.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6377 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/api.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10187 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/auth.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      575 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/certs.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1286 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18560 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/cookies.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3823 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/exceptions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3879 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/help.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      733 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/hooks.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35288 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/models.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      695 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/packages.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30180 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/sessions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4235 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/status_codes.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2912 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/structures.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    33240 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/utils.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.849868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      537 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.849868 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/compat/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      156 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5871 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/providers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1601 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20511 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4963 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/structs.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.865869 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6090 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8478 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/__main__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10096 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   140235 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1064 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2100 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_export_format.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      265 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_extension.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      799 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_fileno.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9695 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_inspect.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3225 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_log_render.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1236 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_loop.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1387 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_null_file.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7063 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_palettes.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      423 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_pick.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5472 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_ratio.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    19919 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_spinners.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      351 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_stack.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      417 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_timer.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22820 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_win32_console.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1926 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_windows.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2783 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1840 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_wrap.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      890 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/abc.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10368 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/align.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6906 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/ansi.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3264 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/bar.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9842 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/box.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4509 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/cells.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18224 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/color.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1054 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/color_triplet.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7131 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/columns.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    99195 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/console.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1288 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/constrain.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5497 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/containers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6630 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/control.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8082 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/default_styles.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      972 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/diagnose.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2501 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/emoji.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      642 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/errors.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1683 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/file_proxy.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2508 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/filesize.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9584 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/highlighter.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5032 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/json.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3252 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/jupyter.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14007 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/layout.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14273 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/live.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3667 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/live_render.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11903 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/logging.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8198 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/markup.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5305 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/measure.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4970 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/padding.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      828 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/pager.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3396 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/palette.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10574 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/panel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35852 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/pretty.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    59706 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/progress.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8165 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/progress_bar.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11303 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/prompt.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1391 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/protocol.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      166 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/region.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4431 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/repr.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4602 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/rule.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2843 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/scope.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1591 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/screen.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    24247 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/segment.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4339 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/spinner.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4425 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/status.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27073 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/style.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1258 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/styled.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35153 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/syntax.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39684 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/table.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3370 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    45525 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/text.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3777 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/theme.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      102 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/themes.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    29604 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/traceback.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9169 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/tree.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34549 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/six.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.865869 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20493 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3551 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2179 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/_utils.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1682 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/after.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1562 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/before.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2372 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1383 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/nap.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8746 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/retry.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3086 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/stop.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2142 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8024 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/wait.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.865869 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tomli/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      396 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tomli/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22633 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tomli/_parser.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2943 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tomli/_re.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      254 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tomli/_types.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    84101 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/typing_extensions.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.869869 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3333 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10811 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/_collections.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       64 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/_version.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20300 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/connection.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39128 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.869869 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      957 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.869869 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17632 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13922 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11036 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4528 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17081 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34448 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7097 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8217 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8579 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/fields.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2440 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/filepost.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.869869 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.869869 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1417 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34665 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    19786 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5985 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/request.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30641 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/response.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.873869 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1155 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4901 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1605 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      498 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3997 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/request.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3510 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/response.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22003 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17177 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5758 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6895 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10168 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14296 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/url.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5403 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      476 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/vendor.txt
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.873869 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/webencodings/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10579 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/webencodings/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8979 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/webencodings/labels.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1305 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6563 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/webencodings/tests.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4307 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.773867 pythonce-0.0.4/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9953 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1093 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/LICENSE.txt
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      125 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/entry_points.txt
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        4 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/top_level.txt
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.765867 pythonce-0.0.4/env/lib64/
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.765867 pythonce-0.0.4/env/lib64/python3.13/
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.765867 pythonce-0.0.4/env/lib64/python3.13/site-packages/
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.873869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      357 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1198 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/__main__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1444 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/__pip-runner__.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.877869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      573 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10243 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/build_env.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9661 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cache.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.877869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      132 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6676 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/autocompletion.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8176 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/base_command.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30030 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/cmdoptions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      774 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/command_context.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2816 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/main.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4338 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/main_parser.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10817 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/parser.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1968 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/progress_bars.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18328 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/req_command.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5118 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/spinners.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      116 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/status_codes.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.881869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3882 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7581 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/cache.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1684 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/check.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4129 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/completion.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9815 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/configuration.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6591 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/debug.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5182 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/download.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2951 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/freeze.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1703 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/hash.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1132 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/help.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4793 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/index.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3188 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/inspect.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    28722 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/install.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12343 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/list.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5697 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/search.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6419 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/show.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3886 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/uninstall.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6324 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/wheel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13529 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/configuration.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.881869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/distributions/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      858 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/distributions/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1221 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/distributions/base.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      729 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/distributions/installed.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6494 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/distributions/sdist.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1164 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/distributions/wheel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23741 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/exceptions.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.885869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/index/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       30 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/index/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    16504 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/index/collector.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    37873 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/index/package_finder.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6556 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/index/sources.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.885869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/locations/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    15365 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/locations/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6100 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/locations/_distutils.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7680 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/locations/_sysconfig.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2556 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/locations/base.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      340 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/main.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.885869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4280 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2595 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/_json.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    25277 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/base.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.885869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      107 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1882 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8181 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7457 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9773 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.885869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       63 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      990 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/candidate.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6931 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/direct_url.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2520 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/format_control.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1030 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/index.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2619 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/installation_report.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18817 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/link.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      738 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/scheme.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4643 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/search_scope.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1907 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/selection_prefs.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3858 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/target_python.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3600 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/wheel.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.889869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       50 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20435 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/auth.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2145 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/cache.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6096 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/download.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7638 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/lazy_wheel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18442 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/session.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4073 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/utils.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1791 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/xmlrpc.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.889869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/__init__.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.889869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4133 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1422 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/metadata.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1474 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2198 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1075 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/wheel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1417 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3064 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5122 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/check.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9816 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/freeze.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.889869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/install/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       51 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/install/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1282 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27475 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/install/wheel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27696 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/prepare.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7161 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/pyproject.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.893869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/req/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2738 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/req/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    16610 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/req/constructors.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17872 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/req/req_file.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    32782 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/req/req_install.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2858 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/req/req_set.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    24678 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/req/req_uninstall.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.893869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      583 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/base.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.893869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/legacy/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    24128 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.893869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5220 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18864 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27845 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5705 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9824 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3094 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5454 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11538 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8167 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/self_outdated_check.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.897869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3351 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1015 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/_log.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1665 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/appdirs.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1884 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5377 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      242 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/datetime.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3627 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/deprecation.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3206 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2118 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/egg_link.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1169 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/encoding.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3064 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/entrypoints.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5122 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/filesystem.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      716 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/filetypes.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3110 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/glibc.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5118 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/hashes.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      795 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11632 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/logging.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22216 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/misc.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1193 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/models.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2108 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/packaging.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4435 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/setuptools_build.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9200 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/subprocess.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7702 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/temp_dir.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8821 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/unpacking.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1759 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/urls.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3456 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/virtualenv.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4549 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/wheel.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.901869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/vcs/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      596 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/vcs/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3519 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/vcs/bazaar.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18116 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/vcs/git.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5238 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/vcs/mercurial.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11729 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/vcs/subversion.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22811 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11842 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/wheel_builder.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.901869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4966 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/__init__.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.901869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      465 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1379 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5033 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1535 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.901869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/caches/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      242 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5271 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1033 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      778 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    16416 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3946 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4154 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7105 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      774 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.905870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       94 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/certifi/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      255 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/certifi/__main__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4279 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/certifi/core.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.913870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4797 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    31274 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/big5freq.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1763 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/big5prober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10032 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3915 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5420 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.913870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/cli/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3242 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3732 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      542 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1860 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1683 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/enums.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4006 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/escprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12176 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/escsm.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3934 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13566 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1753 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    36913 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1753 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20735 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1759 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14537 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    25796 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    42498 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1752 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/johabprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27055 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   104562 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    98484 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    98196 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   101363 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   128035 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   102774 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    95372 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5380 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6077 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3715 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2131 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30391 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.913870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/metadata/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13560 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      402 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/resultdict.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6400 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4137 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4007 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14848 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8505 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2812 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      244 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/version.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.913870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      266 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2522 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/ansi.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11128 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3325 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/initialise.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.917870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       75 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2839 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10678 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6741 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1866 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1079 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3709 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6181 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/win32.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7134 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/winterm.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.917870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      581 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    41259 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    51697 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/database.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20834 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/index.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    51991 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/locators.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14811 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/manifest.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5058 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/markers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39801 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/metadata.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10820 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/resources.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18102 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/scripts.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    66262 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/util.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23513 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/version.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    43898 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/wheel.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.921870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distro/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      981 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distro/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       64 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distro/__main__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    49330 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distro/distro.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.921870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      849 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3374 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/codec.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      321 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12950 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/core.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    44375 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/idnadata.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1881 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/intranges.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       21 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/package_data.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   206539 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/uts46data.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.921870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1132 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1081 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6079 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/ext.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34544 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/fallback.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.925870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      661 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/__about__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      497 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11488 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4378 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1431 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/_structures.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8487 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/markers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4676 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/requirements.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30110 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/specifiers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    15699 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/tags.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4200 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/utils.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14665 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/version.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.925870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pkg_resources/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   109388 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pkg_resources/__init__.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.925870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18003 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1198 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4303 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/android.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5706 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/api.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2800 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/macos.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7448 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/unix.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      160 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/version.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7098 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/windows.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.929870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2999 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      353 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/__main__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23685 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/cmdline.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1697 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/console.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1938 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/filter.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.929870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/filters/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    40386 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2917 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatter.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.933870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4800 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4104 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3314 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5086 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35601 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    21938 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4981 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    19351 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5073 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2212 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5014 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7335 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4674 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11753 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    32064 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexer.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.933870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11164 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    71556 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    53572 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      986 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/modeline.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2591 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/plugin.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3072 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/regexopt.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3092 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/scanner.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6882 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6257 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/style.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.933870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/styles/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3419 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6184 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/token.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    63187 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/unistring.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9110 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/util.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.937870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9171 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6426 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/actions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12936 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/common.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   213344 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/core.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.937870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/diagram/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23685 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9023 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39129 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    25341 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/results.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13402 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/testing.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10787 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6805 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/util.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.937870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      491 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      138 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11920 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_impl.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.937870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      546 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10927 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.941870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5178 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      435 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/__version__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1397 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    21443 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/adapters.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6377 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/api.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10187 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/auth.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      575 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/certs.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1286 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/compat.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18560 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/cookies.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3823 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/exceptions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3879 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/help.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      733 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/hooks.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35288 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/models.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      695 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/packages.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30180 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/sessions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4235 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/status_codes.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2912 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/structures.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    33240 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/utils.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.941870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      537 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.941870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/compat/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      156 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5871 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/providers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1601 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20511 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4963 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/structs.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.953870 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6090 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8478 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/__main__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10096 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   140235 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1064 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2100 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_export_format.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      265 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_extension.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      799 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_fileno.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9695 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_inspect.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3225 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_log_render.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1236 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_loop.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1387 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_null_file.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7063 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_palettes.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      423 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_pick.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5472 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_ratio.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    19919 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_spinners.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      351 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_stack.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      417 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_timer.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22820 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_win32_console.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1926 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_windows.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2783 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1840 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_wrap.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      890 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/abc.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10368 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/align.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6906 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/ansi.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3264 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/bar.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9842 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/box.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4509 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/cells.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18224 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/color.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1054 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/color_triplet.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7131 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/columns.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    99195 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/console.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1288 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/constrain.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5497 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/containers.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6630 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/control.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8082 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/default_styles.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      972 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/diagnose.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2501 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/emoji.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      642 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/errors.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1683 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/file_proxy.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2508 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/filesize.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9584 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/highlighter.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5032 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/json.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3252 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/jupyter.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14007 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/layout.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14273 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/live.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3667 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/live_render.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11903 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/logging.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8198 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/markup.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5305 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/measure.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4970 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/padding.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      828 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/pager.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3396 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/palette.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10574 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/panel.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35852 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/pretty.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    59706 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/progress.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8165 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/progress_bar.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11303 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/prompt.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1391 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/protocol.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      166 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/region.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4431 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/repr.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4602 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/rule.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2843 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/scope.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1591 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/screen.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    24247 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/segment.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4339 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/spinner.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4425 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/status.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27073 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/style.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1258 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/styled.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35153 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/syntax.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39684 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/table.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3370 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    45525 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/text.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3777 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/theme.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      102 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/themes.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    29604 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/traceback.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9169 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/tree.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34549 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/six.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.957871 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20493 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3551 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2179 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/_utils.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1682 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/after.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1562 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/before.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2372 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1383 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/nap.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8746 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/retry.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3086 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/stop.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2142 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8024 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/wait.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.957871 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tomli/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      396 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tomli/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22633 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tomli/_parser.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2943 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tomli/_re.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      254 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tomli/_types.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    84101 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/typing_extensions.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.961871 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3333 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10811 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/_collections.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       64 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/_version.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20300 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/connection.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39128 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.961871 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      957 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.961871 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17632 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13922 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11036 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4528 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17081 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34448 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7097 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8217 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8579 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/fields.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2440 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/filepost.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.961871 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.961871 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1417 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34665 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    19786 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5985 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/request.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30641 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/response.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.965871 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1155 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4901 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1605 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      498 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3997 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/request.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3510 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/response.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22003 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17177 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5758 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6895 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10168 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14296 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/url.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5403 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      476 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/vendor.txt
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.965871 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10579 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8979 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/labels.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1305 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6563 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/tests.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4307 2023-06-11 19:56:55.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.877869 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9953 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1093 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/LICENSE.txt
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      125 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/entry_points.txt
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        4 2023-06-11 19:56:54.000000 pythonce-0.0.4/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/top_level.txt
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.965871 pythonce-0.0.4/pythonce/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      100 2023-06-11 19:56:55.000000 pythonce-0.0.4/pythonce/OlaMi.c
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      214 2023-06-11 21:19:33.000000 pythonce-0.0.4/pythonce/OlaMi.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      542 2023-06-11 21:20:19.000000 pythonce-0.0.4/pythonce/__init__.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      369 2023-06-11 19:56:55.000000 pythonce-0.0.4/pythonce/c-teste.c
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1741 2023-06-11 20:46:01.000000 pythonce-0.0.4/pythonce/c-torrent.c
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      908 2023-06-11 19:56:55.000000 pythonce-0.0.4/pythonce/calculadora.c
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      277 2023-06-11 19:56:55.000000 pythonce-0.0.4/pythonce/count.c
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      289 2023-06-11 19:56:55.000000 pythonce-0.0.4/pythonce/count.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       78 2023-06-11 19:56:55.000000 pythonce-0.0.4/pythonce/ola.c
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       93 2023-06-11 19:56:55.000000 pythonce-0.0.4/pythonce/ola.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      370 2023-06-11 21:26:57.000000 pythonce-0.0.4/pythonce/soma.c
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      375 2023-06-11 21:30:08.000000 pythonce-0.0.4/pythonce/sub.c
-drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 21:32:48.969871 pythonce-0.0.4/pythonce.egg-info/
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      823 2023-06-11 21:32:48.000000 pythonce-0.0.4/pythonce.egg-info/PKG-INFO
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    68039 2023-06-11 21:32:48.000000 pythonce-0.0.4/pythonce.egg-info/SOURCES.txt
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        1 2023-06-11 21:32:48.000000 pythonce-0.0.4/pythonce.egg-info/dependency_links.txt
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        9 2023-06-11 21:32:48.000000 pythonce-0.0.4/pythonce.egg-info/top_level.txt
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       38 2023-06-11 21:32:48.969871 pythonce-0.0.4/setup.cfg
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      706 2023-06-11 21:32:46.000000 pythonce-0.0.4/setup.py
--rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       51 2023-06-11 19:56:55.000000 pythonce-0.0.4/teste.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.168919 pythonce-0.0.5/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      373 2023-06-11 23:35:25.000000 pythonce-0.0.5/CHANGELOG.txt
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1059 2023-06-10 04:27:15.000000 pythonce-0.0.5/LINCENCE.txt
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       32 2023-06-11 23:17:15.000000 pythonce-0.0.5/MANIFEST.in
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      896 2023-06-11 23:35:58.168919 pythonce-0.0.5/PKG-INFO
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       45 2023-06-10 04:27:15.000000 pythonce-0.0.5/README.txt
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.012918 pythonce-0.0.5/env/
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.004917 pythonce-0.0.5/env/lib/
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.004917 pythonce-0.0.5/env/lib/python3.13/
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.004917 pythonce-0.0.5/env/lib/python3.13/site-packages/
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.016918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      357 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1198 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/__main__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1444 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/__pip-runner__.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.020918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      573 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10243 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/build_env.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9661 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cache.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.020918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      132 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6676 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/autocompletion.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8176 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/base_command.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30030 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      774 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/command_context.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2816 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/main.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4338 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/main_parser.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10817 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/parser.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1968 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/progress_bars.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18328 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/req_command.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5118 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/spinners.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      116 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/status_codes.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.024918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3882 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7581 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/cache.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1684 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/check.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4129 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/completion.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9815 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6591 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/debug.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5182 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/download.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2951 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1703 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/hash.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1132 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/help.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4793 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/index.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3188 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/inspect.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    28722 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/install.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12343 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/list.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5697 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/search.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6419 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/show.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3886 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6324 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13529 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/configuration.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.024918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/distributions/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      858 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/distributions/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1221 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/distributions/base.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      729 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/distributions/installed.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6494 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/distributions/sdist.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1164 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/distributions/wheel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23741 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/exceptions.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.024918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/index/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       30 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/index/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    16504 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/index/collector.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    37873 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/index/package_finder.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6556 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/index/sources.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.024918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/locations/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    15365 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/locations/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6100 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/locations/_distutils.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7680 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2556 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/locations/base.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      340 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/main.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.024918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4280 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2595 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/_json.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    25277 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/base.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.028918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      107 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1882 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8181 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7457 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9773 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.028918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       63 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      990 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/candidate.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6931 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/direct_url.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2520 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/format_control.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1030 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/index.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2619 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/installation_report.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18817 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/link.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      738 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/scheme.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4643 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/search_scope.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1907 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/selection_prefs.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3858 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/target_python.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3600 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/wheel.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.028918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       50 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20435 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/auth.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2145 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/cache.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6096 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/download.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7638 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18442 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/session.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4073 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/utils.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1791 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/xmlrpc.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.032918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/__init__.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.032918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4133 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1422 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/metadata.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1474 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2198 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1075 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/wheel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1417 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3064 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5122 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/check.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9816 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/freeze.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.032918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/install/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       51 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/install/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1282 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27475 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/install/wheel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27696 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7161 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/pyproject.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.032918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/req/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2738 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/req/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    16610 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/req/constructors.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17872 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/req/req_file.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    32782 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/req/req_install.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2858 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/req/req_set.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    24678 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/req/req_uninstall.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.036918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      583 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/base.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.036918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/legacy/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    24128 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.036918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5220 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18864 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27845 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5705 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9824 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3094 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5454 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11538 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8167 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/self_outdated_check.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.040918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3351 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1015 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/_log.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1665 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1884 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5377 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      242 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/datetime.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3627 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3206 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2118 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/egg_link.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1169 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3064 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/entrypoints.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5122 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      716 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/filetypes.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3110 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5118 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      795 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11632 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/logging.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22216 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/misc.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1193 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/models.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2108 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4435 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9200 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/subprocess.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7702 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8821 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/unpacking.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1759 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/urls.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3456 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/virtualenv.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4549 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/wheel.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.040918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/vcs/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      596 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3519 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18116 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/vcs/git.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5238 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11729 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22811 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11842 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/wheel_builder.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.040918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4966 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/__init__.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.044918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      465 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1379 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5033 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1535 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.044918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      242 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5271 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1033 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      778 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    16416 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3946 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4154 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7105 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      774 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.044918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       94 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      255 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4279 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/certifi/core.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.052918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4797 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    31274 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1763 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10032 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3915 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5420 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.052918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/cli/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3242 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3732 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      542 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1860 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1683 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4006 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12176 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3934 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13566 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1753 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    36913 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1753 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20735 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1759 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14537 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    25796 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    42498 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1752 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27055 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   104562 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    98484 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    98196 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   101363 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   128035 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   102774 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    95372 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5380 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6077 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3715 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2131 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30391 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.052918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/metadata/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13560 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      402 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6400 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4137 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4007 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14848 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8505 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2812 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      244 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/version.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.052918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      266 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2522 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11128 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3325 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/initialise.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.052918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       75 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2839 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10678 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6741 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1866 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1079 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3709 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6181 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7134 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/winterm.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.056918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      581 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    41259 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    51697 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20834 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    51991 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14811 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5058 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39801 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10820 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18102 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    66262 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23513 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    43898 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/wheel.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.056918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distro/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      981 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distro/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       64 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distro/__main__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    49330 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distro/distro.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.056918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      849 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3374 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      321 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12950 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/core.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    44375 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1881 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       21 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   206539 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/uts46data.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.060918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/msgpack/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1132 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1081 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6079 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/msgpack/ext.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34544 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/msgpack/fallback.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.060918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      661 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      497 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11488 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4378 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1431 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8487 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4676 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30110 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    15699 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/tags.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4200 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14665 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/version.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.060918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pkg_resources/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   109388 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pkg_resources/__init__.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.060918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18003 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1198 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4303 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/android.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5706 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/api.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2800 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7448 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      160 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/version.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7098 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/windows.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.064918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2999 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      353 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/__main__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23685 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1697 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/console.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1938 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/filter.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.064918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/filters/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    40386 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2917 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatter.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.068918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4800 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4104 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3314 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5086 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35601 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    21938 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4981 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    19351 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5073 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2212 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5014 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7335 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4674 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11753 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    32064 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexer.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.068918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11164 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    71556 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    53572 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      986 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/modeline.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2591 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/plugin.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3072 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3092 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/scanner.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6882 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6257 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/style.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.068918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/styles/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3419 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6184 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/token.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    63187 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/unistring.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9110 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/util.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.068918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9171 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6426 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12936 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/common.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   213344 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/core.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.068918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23685 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9023 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39129 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    25341 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/results.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13402 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10787 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6805 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/util.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.068918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      491 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      138 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11920 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.068918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      546 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10927 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.072918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5178 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      435 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1397 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    21443 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6377 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/api.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10187 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      575 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1286 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18560 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3823 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3879 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/help.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      733 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35288 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/models.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      695 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30180 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4235 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2912 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    33240 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/utils.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.072918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      537 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.072918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/compat/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      156 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5871 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1601 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20511 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4963 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/structs.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.084918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6090 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8478 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/__main__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10096 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   140235 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1064 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2100 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_export_format.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      265 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_extension.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      799 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_fileno.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9695 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_inspect.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3225 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_log_render.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1236 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_loop.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1387 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_null_file.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7063 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_palettes.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      423 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_pick.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5472 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_ratio.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    19919 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_spinners.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      351 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_stack.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      417 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_timer.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22820 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1926 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_windows.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2783 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1840 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_wrap.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      890 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/abc.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10368 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/align.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6906 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/ansi.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3264 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/bar.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9842 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/box.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4509 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/cells.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18224 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/color.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1054 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7131 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/columns.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    99195 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/console.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1288 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/constrain.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5497 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/containers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6630 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/control.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8082 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/default_styles.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      972 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/diagnose.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2501 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/emoji.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      642 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/errors.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1683 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2508 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/filesize.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9584 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/highlighter.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5032 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/json.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3252 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/jupyter.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14007 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/layout.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14273 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/live.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3667 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/live_render.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11903 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/logging.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8198 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/markup.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5305 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/measure.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4970 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/padding.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      828 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/pager.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3396 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/palette.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10574 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/panel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35852 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/pretty.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    59706 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/progress.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8165 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11303 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/prompt.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1391 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/protocol.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      166 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/region.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4431 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/repr.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4602 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/rule.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2843 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/scope.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1591 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/screen.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    24247 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/segment.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4339 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/spinner.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4425 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/status.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27073 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/style.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1258 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/styled.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35153 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/syntax.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39684 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/table.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3370 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    45525 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/text.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3777 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/theme.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      102 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/themes.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    29604 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/traceback.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9169 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/tree.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34549 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/six.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.088919 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20493 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3551 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2179 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1682 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/after.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1562 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/before.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2372 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1383 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/nap.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8746 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/retry.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3086 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/stop.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2142 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8024 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/wait.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.088919 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tomli/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      396 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tomli/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22633 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tomli/_parser.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2943 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tomli/_re.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      254 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tomli/_types.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    84101 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/typing_extensions.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.088919 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3333 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10811 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       64 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/_version.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20300 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39128 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.088919 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      957 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.092918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17632 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13922 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11036 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4528 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17081 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34448 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7097 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8217 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8579 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2440 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/filepost.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.092918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.092918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1417 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34665 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    19786 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5985 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30641 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/response.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.092918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1155 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4901 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1605 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      498 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3997 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3510 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22003 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17177 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5758 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6895 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10168 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14296 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5403 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      476 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/vendor.txt
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.092918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/webencodings/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10579 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8979 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1305 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6563 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4307 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.020918 pythonce-0.0.5/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9953 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1093 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      125 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/entry_points.txt
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        4 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/top_level.txt
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.012918 pythonce-0.0.5/env/lib64/
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.012918 pythonce-0.0.5/env/lib64/python3.13/
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.012918 pythonce-0.0.5/env/lib64/python3.13/site-packages/
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.096918 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      357 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1198 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/__main__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1444 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/__pip-runner__.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.096918 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      573 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10243 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/build_env.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9661 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cache.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.096918 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      132 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6676 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/autocompletion.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8176 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/base_command.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30030 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      774 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/command_context.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2816 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/main.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4338 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/main_parser.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10817 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/parser.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1968 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/progress_bars.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18328 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/req_command.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5118 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/spinners.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      116 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/status_codes.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.100919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3882 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7581 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/cache.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1684 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/check.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4129 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/completion.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9815 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6591 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/debug.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5182 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/download.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2951 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1703 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/hash.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1132 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/help.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4793 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/index.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3188 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/inspect.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    28722 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/install.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12343 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/list.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5697 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/search.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6419 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/show.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3886 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6324 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13529 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/configuration.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.100919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/distributions/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      858 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/distributions/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1221 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/distributions/base.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      729 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/distributions/installed.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6494 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/distributions/sdist.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1164 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/distributions/wheel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23741 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/exceptions.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.100919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/index/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       30 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/index/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    16504 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/index/collector.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    37873 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/index/package_finder.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6556 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/index/sources.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.104919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/locations/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    15365 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/locations/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6100 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/locations/_distutils.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7680 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2556 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/locations/base.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      340 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/main.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.104919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4280 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2595 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/_json.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    25277 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/base.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.104919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      107 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1882 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8181 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7457 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9773 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.104919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       63 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      990 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/candidate.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6931 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/direct_url.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2520 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/format_control.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1030 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/index.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2619 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/installation_report.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18817 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/link.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      738 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/scheme.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4643 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/search_scope.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1907 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/selection_prefs.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3858 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/target_python.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3600 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/wheel.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.104919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       50 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20435 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/auth.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2145 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/cache.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6096 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/download.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7638 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18442 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/session.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4073 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/utils.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1791 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/xmlrpc.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.108919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/__init__.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.108919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4133 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1422 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/metadata.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1474 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2198 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1075 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/wheel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1417 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3064 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5122 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/check.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9816 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/freeze.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.108919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/install/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       51 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/install/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1282 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27475 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/install/wheel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27696 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7161 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/pyproject.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.108919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/req/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2738 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/req/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    16610 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/req/constructors.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17872 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/req/req_file.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    32782 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/req/req_install.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2858 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/req/req_set.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    24678 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/req/req_uninstall.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.108919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      583 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/base.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.108919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/legacy/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    24128 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.112919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5220 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18864 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27845 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5705 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9824 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3094 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5454 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11538 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8167 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/self_outdated_check.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.112919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3351 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1015 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/_log.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1665 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1884 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5377 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      242 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/datetime.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3627 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3206 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2118 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/egg_link.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1169 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3064 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/entrypoints.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5122 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      716 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/filetypes.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3110 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5118 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      795 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11632 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/logging.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22216 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/misc.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1193 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/models.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2108 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4435 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9200 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/subprocess.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7702 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8821 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/unpacking.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1759 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/urls.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3456 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/virtualenv.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4549 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/wheel.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.116919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/vcs/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      596 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3519 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18116 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/vcs/git.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5238 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11729 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22811 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11842 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/wheel_builder.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.116919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4966 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/__init__.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.116919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      465 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1379 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5033 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1535 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.116919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      242 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5271 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1033 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      778 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    16416 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3946 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4154 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7105 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      774 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.116919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       94 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      255 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4279 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/certifi/core.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.124919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4797 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    31274 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1763 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10032 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3915 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5420 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.124919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/cli/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3242 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3732 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      542 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1860 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1683 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4006 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12176 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3934 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13566 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1753 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    36913 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1753 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20735 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1759 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14537 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    25796 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    42498 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1752 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27055 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   104562 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    98484 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    98196 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   101363 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   128035 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   102774 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    95372 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5380 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6077 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3715 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2131 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30391 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.124919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/metadata/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13560 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      402 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6400 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4137 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4007 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14848 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8505 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2812 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      244 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/version.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.124919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      266 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2522 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11128 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3325 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/initialise.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.128919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       75 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2839 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10678 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6741 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1866 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1079 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3709 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6181 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7134 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/winterm.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.128919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      581 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    41259 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    51697 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20834 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    51991 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14811 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5058 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39801 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10820 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18102 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    66262 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23513 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    43898 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/wheel.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.128919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distro/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      981 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distro/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       64 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distro/__main__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    49330 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distro/distro.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.132919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      849 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3374 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      321 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12950 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/core.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    44375 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1881 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       21 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   206539 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/uts46data.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.132919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1132 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1081 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6079 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/ext.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34544 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/fallback.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.132919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      661 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      497 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11488 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4378 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1431 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8487 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4676 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30110 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    15699 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/tags.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4200 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14665 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/version.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.132919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pkg_resources/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   109388 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pkg_resources/__init__.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.136919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18003 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1198 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4303 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/android.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5706 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/api.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2800 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7448 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      160 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/version.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7098 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/windows.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.136919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2999 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      353 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/__main__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23685 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1697 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/console.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1938 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/filter.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.136919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/filters/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    40386 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2917 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatter.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.140919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4800 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4104 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3314 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5086 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35601 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    21938 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4981 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    19351 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5073 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2212 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5014 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7335 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4674 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11753 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    32064 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexer.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.140919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11164 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    71556 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    53572 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      986 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/modeline.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2591 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/plugin.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3072 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3092 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/scanner.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6882 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6257 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/style.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.140919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/styles/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3419 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6184 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/token.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    63187 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/unistring.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9110 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/util.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.140919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9171 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6426 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    12936 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/common.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   213344 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/core.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.140919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    23685 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9023 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39129 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    25341 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/results.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13402 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10787 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6805 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/util.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.140919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      491 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      138 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11920 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.140919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      546 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10927 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.144919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5178 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      435 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1397 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    21443 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6377 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/api.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10187 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      575 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1286 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18560 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3823 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3879 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/help.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      733 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35288 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/models.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      695 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30180 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4235 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2912 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    33240 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/utils.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.144919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      537 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.144919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/compat/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      156 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5871 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1601 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20511 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4963 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/structs.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.156919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6090 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8478 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/__main__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10096 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)   140235 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1064 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2100 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_export_format.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      265 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_extension.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      799 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_fileno.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9695 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_inspect.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3225 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_log_render.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1236 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_loop.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1387 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_null_file.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7063 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_palettes.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      423 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_pick.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5472 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_ratio.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    19919 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_spinners.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      351 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_stack.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      417 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_timer.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22820 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1926 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_windows.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2783 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1840 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_wrap.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      890 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/abc.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10368 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/align.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6906 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/ansi.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3264 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/bar.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9842 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/box.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4509 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/cells.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    18224 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/color.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1054 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7131 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/columns.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    99195 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/console.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1288 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/constrain.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5497 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/containers.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6630 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/control.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8082 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/default_styles.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      972 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/diagnose.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2501 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/emoji.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      642 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/errors.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1683 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2508 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/filesize.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9584 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/highlighter.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5032 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/json.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3252 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/jupyter.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14007 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/layout.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14273 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/live.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3667 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/live_render.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11903 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/logging.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8198 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/markup.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5305 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/measure.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4970 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/padding.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      828 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/pager.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3396 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/palette.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10574 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/panel.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35852 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/pretty.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    59706 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/progress.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8165 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11303 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/prompt.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1391 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/protocol.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      166 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/region.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4431 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/repr.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4602 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/rule.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2843 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/scope.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1591 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/screen.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    24247 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/segment.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4339 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/spinner.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4425 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/status.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    27073 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/style.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1258 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/styled.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    35153 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/syntax.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39684 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/table.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3370 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    45525 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/text.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3777 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/theme.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      102 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/themes.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    29604 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/traceback.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9169 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/tree.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34549 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/six.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.156919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20493 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3551 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2179 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1682 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/after.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1562 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/before.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2372 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1383 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/nap.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8746 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/retry.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3086 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/stop.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2142 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8024 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/wait.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.156919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tomli/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      396 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tomli/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22633 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tomli/_parser.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2943 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tomli/_re.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      254 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tomli/_types.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    84101 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/typing_extensions.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.160919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3333 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10811 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       64 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/_version.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    20300 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    39128 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.160919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      957 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.160919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17632 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    13922 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    11036 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4528 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17081 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34448 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     7097 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8217 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8579 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     2440 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/filepost.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.160919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.160919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1417 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    34665 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    19786 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5985 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    30641 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/response.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.164919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1155 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4901 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1605 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      498 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3997 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     3510 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    22003 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    17177 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5758 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6895 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10168 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    14296 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     5403 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      476 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/vendor.txt
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.164919 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    10579 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     8979 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1305 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     6563 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     4307 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.096918 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     9953 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1093 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      125 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/entry_points.txt
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        4 2023-06-10 04:27:15.000000 pythonce-0.0.5/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/top_level.txt
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.164919 pythonce-0.0.5/pythonce/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      100 2023-06-10 04:27:15.000000 pythonce-0.0.5/pythonce/OlaMi.c
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      214 2023-06-11 23:17:15.000000 pythonce-0.0.5/pythonce/OlaMi.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1130 2023-06-11 23:17:15.000000 pythonce-0.0.5/pythonce/__init__.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      369 2023-06-10 04:27:15.000000 pythonce-0.0.5/pythonce/c-teste.c
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1741 2023-06-11 23:17:15.000000 pythonce-0.0.5/pythonce/c-torrent.c
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1709 2023-06-11 23:17:15.000000 pythonce-0.0.5/pythonce/c_torrent.c
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      908 2023-06-10 05:19:37.000000 pythonce-0.0.5/pythonce/calculadora.c
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      277 2023-06-10 04:27:15.000000 pythonce-0.0.5/pythonce/count.c
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      289 2023-06-10 04:27:15.000000 pythonce-0.0.5/pythonce/count.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       78 2023-06-10 04:27:15.000000 pythonce-0.0.5/pythonce/ola.c
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       93 2023-06-10 04:27:15.000000 pythonce-0.0.5/pythonce/ola.py
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      370 2023-06-11 23:17:15.000000 pythonce-0.0.5/pythonce/soma.c
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      375 2023-06-11 23:17:15.000000 pythonce-0.0.5/pythonce/subtracao.c
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)     1402 2023-06-11 03:24:12.000000 pythonce-0.0.5/pythonce/wozidown.py
+drwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)        0 2023-06-11 23:35:58.164919 pythonce-0.0.5/pythonce.egg-info/
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      896 2023-06-11 23:35:57.000000 pythonce-0.0.5/pythonce.egg-info/PKG-INFO
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)    68092 2023-06-11 23:35:57.000000 pythonce-0.0.5/pythonce.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        1 2023-06-11 23:35:57.000000 pythonce-0.0.5/pythonce.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)        9 2023-06-11 23:35:57.000000 pythonce-0.0.5/pythonce.egg-info/top_level.txt
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       38 2023-06-11 23:35:58.168919 pythonce-0.0.5/setup.cfg
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)      968 2023-06-11 23:35:44.000000 pythonce-0.0.5/setup.py
+-rwxrwxr-x   0 carlinhoshk  (1000) carlinhoshk  (1000)    16032 2023-06-10 07:00:36.000000 pythonce-0.0.5/soma
+-rw-rw-r--   0 carlinhoshk  (1000) carlinhoshk  (1000)       51 2023-06-11 23:17:15.000000 pythonce-0.0.5/teste.py
```

### Comparing `pythonce-0.0.4/LINCENCE.txt` & `pythonce-0.0.5/LINCENCE.txt`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/PKG-INFO` & `pythonce-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonce
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Library writen in C 
 Home-page: UNKNOWN
 Author: carlinhoshk
 Author-email: carlosmdohk@gmail.com
 License: MIT
 Keywords: c
 Platform: UNKNOWN
@@ -25,18 +25,22 @@
 - Create sample code in C
 
 ## [0.0.2] - 07-06-2023
 
 - Release version 0.0.2
 - Fix C path issue
 
-## [0.0.3] - 11-06-2023
+## [0.0.3] Dev-Version - 11-06-2023
 
 - Release version 0.0.3
 - Release OlaMi 
 
-## [0.0.4] - 11-06-2023
+## [0.0.4] Dev-Version- 11-06-2023
 
 - Release version 0.0.4
 - Release Subtraction 
 
+## [0.0.5] - Dev-Version-
+
+- Fix 0.0.4 troubles 
+
```

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/__main__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/__pip-runner__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/build_env.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cache.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/autocompletion.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/base_command.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/cmdoptions.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/command_context.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/main.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/main_parser.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/parser.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/progress_bars.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/req_command.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/cli/spinners.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/cache.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/check.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/completion.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/configuration.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/debug.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/download.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/freeze.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/hash.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/help.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/index.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/inspect.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/install.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/list.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/search.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/show.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/uninstall.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/commands/wheel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/configuration.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/distributions/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/distributions/base.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/distributions/installed.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/distributions/sdist.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/distributions/wheel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/exceptions.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/index/collector.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/index/package_finder.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/index/sources.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/locations/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/locations/_distutils.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/locations/_sysconfig.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/locations/base.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/_json.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/base.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/_compat.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/_dists.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/_envs.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/metadata/pkg_resources.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/candidate.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/direct_url.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/format_control.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/index.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/installation_report.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/link.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/scheme.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/search_scope.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/selection_prefs.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/target_python.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/models/wheel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/auth.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/cache.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/download.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/lazy_wheel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/session.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/utils.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/network/xmlrpc.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/build_tracker.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/metadata.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/metadata_editable.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/wheel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/wheel_editable.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/check.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/freeze.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/install/editable_legacy.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/install/wheel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/operations/prepare.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/pyproject.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/req/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/req/constructors.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/req/req_file.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/req/req_install.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/req/req_set.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/req/req_uninstall.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/base.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/legacy/resolver.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/base.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/self_outdated_check.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/_jaraco_text.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/_log.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/appdirs.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/compat.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/compatibility_tags.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/deprecation.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/direct_url_helpers.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/egg_link.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/encoding.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/entrypoints.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/filesystem.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/filetypes.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/glibc.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/hashes.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/inject_securetransport.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/logging.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/misc.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/models.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/packaging.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/setuptools_build.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/subprocess.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/temp_dir.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/unpacking.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/urls.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/virtualenv.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/utils/wheel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/vcs/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/vcs/bazaar.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/vcs/git.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/vcs/mercurial.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/vcs/subversion.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/vcs/versioncontrol.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_internal/wheel_builder.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/adapter.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/cache.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/compat.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/controller.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/serialize.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/certifi/core.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/big5freq.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/big5prober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/chardistribution.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/charsetprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/cp949prober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/enums.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/escprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/escsm.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/eucjpprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/euckrfreq.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/euckrprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/euctwfreq.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/euctwprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/gb2312freq.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/gb2312prober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/hebrewprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/jisfreq.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/johabfreq.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/johabprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/jpcntx.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langthaimodel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/latin1prober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/macromanprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/mbcssm.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/metadata/languages.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/sjisprober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/universaldetector.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/utf1632prober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/chardet/utf8prober.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/ansi.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/ansitowin32.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/initialise.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/utils.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/win32.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/colorama/winterm.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/compat.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/database.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/index.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/locators.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/manifest.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/markers.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/metadata.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/resources.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/scripts.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/util.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/version.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distlib/wheel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distro/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/distro/distro.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/codec.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/core.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/idnadata.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/intranges.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/idna/uts46data.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/msgpack/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/msgpack/exceptions.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/msgpack/ext.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/msgpack/fallback.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/__about__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/_manylinux.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/_musllinux.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/_structures.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/markers.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/requirements.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/specifiers.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/tags.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/utils.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/packaging/version.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pkg_resources/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/__main__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/android.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/api.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/macos.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/unix.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/windows.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/cmdline.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/console.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/filter.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/filters/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatter.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/groff.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/html.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/img.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/irc.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/latex.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/other.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/svg.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexer.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/python.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/modeline.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/plugin.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/regexopt.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/scanner.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/sphinxext.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/style.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/styles/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/token.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/unistring.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pygments/util.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/actions.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/common.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/core.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/exceptions.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/helpers.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/results.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/testing.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/unicode.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/util.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/_internal_utils.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/adapters.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/api.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/auth.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/certs.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/compat.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/cookies.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/exceptions.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/help.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/hooks.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/models.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/packages.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/sessions.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/status_codes.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/structures.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/requests/utils.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/providers.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/reporters.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/resolvers.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/structs.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/__main__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_cell_widths.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_emoji_codes.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_emoji_replace.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_export_format.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_fileno.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_inspect.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_log_render.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_loop.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_null_file.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_palettes.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_ratio.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_spinners.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_win32_console.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_windows.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_windows_renderer.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/_wrap.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/abc.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/align.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/ansi.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/bar.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/box.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/cells.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/color.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/color_triplet.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/columns.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/console.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/constrain.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/containers.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/control.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/default_styles.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/diagnose.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/emoji.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/errors.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/file_proxy.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/filesize.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/highlighter.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/json.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/jupyter.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/layout.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/live.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/live_render.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/logging.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/markup.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/measure.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/padding.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/pager.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/palette.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/panel.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/pretty.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/progress.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/progress_bar.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/prompt.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/protocol.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/repr.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/rule.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/scope.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/screen.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/segment.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/spinner.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/status.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/style.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/styled.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/syntax.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/table.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/terminal_theme.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/text.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/theme.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/traceback.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/rich/tree.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/six.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/_asyncio.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/_utils.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/after.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/before.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/before_sleep.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/nap.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/retry.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/stop.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tenacity/wait.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tomli/_parser.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/tomli/_re.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/typing_extensions.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/_collections.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/connection.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/connectionpool.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/exceptions.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/fields.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/filepost.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/six.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/poolmanager.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/request.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/response.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/connection.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/proxy.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/request.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/response.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/retry.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/timeout.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/url.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/wait.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/webencodings/__init__.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/webencodings/labels.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/webencodings/mklabels.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/webencodings/tests.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/AUTHORS.txt` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/LICENSE.txt` & `pythonce-0.0.5/env/lib/python3.13/site-packages/pip-23.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/__main__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/__pip-runner__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/build_env.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cache.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/autocompletion.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/base_command.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/cmdoptions.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/command_context.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/main.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/main_parser.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/parser.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/progress_bars.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/req_command.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/cli/spinners.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/cache.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/check.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/completion.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/configuration.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/debug.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/download.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/freeze.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/hash.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/help.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/index.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/inspect.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/install.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/list.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/search.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/show.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/uninstall.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/commands/wheel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/configuration.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/distributions/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/distributions/base.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/distributions/installed.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/distributions/sdist.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/distributions/wheel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/exceptions.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/index/collector.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/index/package_finder.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/index/sources.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/locations/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/locations/_distutils.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/locations/_sysconfig.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/locations/base.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/_json.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/base.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/_compat.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/_dists.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/_envs.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/metadata/pkg_resources.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/candidate.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/direct_url.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/format_control.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/index.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/installation_report.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/link.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/scheme.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/search_scope.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/selection_prefs.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/target_python.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/models/wheel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/auth.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/cache.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/download.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/lazy_wheel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/session.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/utils.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/network/xmlrpc.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/build_tracker.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/metadata.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/metadata_editable.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/wheel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/wheel_editable.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/check.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/freeze.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/install/editable_legacy.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/install/wheel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/operations/prepare.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/pyproject.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/req/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/req/constructors.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/req/req_file.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/req/req_install.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/req/req_set.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/req/req_uninstall.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/base.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/legacy/resolver.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/base.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/self_outdated_check.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/_jaraco_text.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/_log.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/appdirs.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/compat.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/compatibility_tags.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/deprecation.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/direct_url_helpers.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/egg_link.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/encoding.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/entrypoints.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/filesystem.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/filetypes.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/glibc.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/hashes.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/inject_securetransport.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/logging.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/misc.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/models.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/packaging.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/setuptools_build.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/subprocess.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/temp_dir.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/unpacking.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/urls.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/virtualenv.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/utils/wheel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/vcs/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/vcs/bazaar.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/vcs/git.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/vcs/mercurial.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/vcs/subversion.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/vcs/versioncontrol.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_internal/wheel_builder.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/adapter.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/cache.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/compat.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/controller.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/serialize.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/certifi/core.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/big5freq.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/big5prober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/chardistribution.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/charsetprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/cp949prober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/enums.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/escprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/escsm.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/eucjpprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euckrfreq.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euckrprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euctwfreq.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euctwprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/gb2312freq.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/gb2312prober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/hebrewprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/jisfreq.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/johabfreq.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/johabprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/jpcntx.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langthaimodel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/latin1prober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/macromanprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/mbcssm.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/metadata/languages.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/sjisprober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/universaldetector.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/utf1632prober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/chardet/utf8prober.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/ansi.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/ansitowin32.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/initialise.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/utils.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/win32.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/colorama/winterm.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/compat.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/database.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/index.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/locators.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/manifest.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/markers.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/metadata.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/resources.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/scripts.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/util.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/version.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distlib/wheel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distro/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/distro/distro.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/codec.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/core.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/idnadata.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/intranges.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/idna/uts46data.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/exceptions.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/ext.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/fallback.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/__about__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/_manylinux.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/_musllinux.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/_structures.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/markers.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/requirements.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/specifiers.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/tags.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/utils.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/packaging/version.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pkg_resources/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/__main__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/android.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/api.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/macos.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/unix.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/windows.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/cmdline.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/console.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/filter.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/filters/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatter.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/groff.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/html.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/img.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/irc.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/latex.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/other.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/svg.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexer.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/python.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/modeline.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/plugin.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/regexopt.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/scanner.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/sphinxext.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/style.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/styles/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/token.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/unistring.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pygments/util.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/actions.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/common.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/core.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/exceptions.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/helpers.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/results.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/testing.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/unicode.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/util.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/_internal_utils.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/adapters.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/api.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/auth.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/certs.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/compat.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/cookies.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/exceptions.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/help.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/hooks.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/models.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/packages.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/sessions.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/status_codes.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/structures.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/requests/utils.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/providers.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/reporters.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/resolvers.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/structs.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/__main__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_cell_widths.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_emoji_codes.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_emoji_replace.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_export_format.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_fileno.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_inspect.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_log_render.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_loop.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_null_file.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_palettes.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_ratio.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_spinners.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_win32_console.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_windows.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_windows_renderer.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/_wrap.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/abc.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/align.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/ansi.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/bar.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/box.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/cells.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/color.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/color_triplet.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/columns.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/console.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/constrain.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/containers.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/control.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/default_styles.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/diagnose.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/emoji.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/errors.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/file_proxy.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/filesize.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/highlighter.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/json.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/jupyter.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/layout.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/live.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/live_render.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/logging.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/markup.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/measure.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/padding.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/pager.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/palette.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/panel.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/pretty.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/progress.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/progress_bar.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/prompt.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/protocol.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/repr.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/rule.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/scope.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/screen.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/segment.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/spinner.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/status.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/style.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/styled.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/syntax.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/table.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/terminal_theme.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/text.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/theme.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/traceback.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/rich/tree.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/six.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/_asyncio.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/_utils.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/after.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/before.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/before_sleep.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/nap.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/retry.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/stop.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/wait.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tomli/_parser.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/tomli/_re.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/typing_extensions.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/_collections.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/connection.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/connectionpool.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/exceptions.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/fields.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/filepost.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/six.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/poolmanager.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/request.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/response.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/connection.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/proxy.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/request.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/response.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/retry.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/timeout.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/url.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/wait.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/__init__.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/labels.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/mklabels.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/tests.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/AUTHORS.txt` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/LICENSE.txt` & `pythonce-0.0.5/env/lib64/python3.13/site-packages/pip-23.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/pythonce/c-torrent.c` & `pythonce-0.0.5/pythonce/c-torrent.c`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/pythonce/calculadora.c` & `pythonce-0.0.5/pythonce/calculadora.c`

 * *Files identical despite different names*

### Comparing `pythonce-0.0.4/pythonce.egg-info/PKG-INFO` & `pythonce-0.0.5/pythonce.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonce
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Library writen in C 
 Home-page: UNKNOWN
 Author: carlinhoshk
 Author-email: carlosmdohk@gmail.com
 License: MIT
 Keywords: c
 Platform: UNKNOWN
@@ -25,18 +25,22 @@
 - Create sample code in C
 
 ## [0.0.2] - 07-06-2023
 
 - Release version 0.0.2
 - Fix C path issue
 
-## [0.0.3] - 11-06-2023
+## [0.0.3] Dev-Version - 11-06-2023
 
 - Release version 0.0.3
 - Release OlaMi 
 
-## [0.0.4] - 11-06-2023
+## [0.0.4] Dev-Version- 11-06-2023
 
 - Release version 0.0.4
 - Release Subtraction 
 
+## [0.0.5] - Dev-Version-
+
+- Fix 0.0.4 troubles 
+
```

### Comparing `pythonce-0.0.4/pythonce.egg-info/SOURCES.txt` & `pythonce-0.0.5/pythonce.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CHANGELOG.txt
 LINCENCE.txt
 MANIFEST.in
 README.txt
 setup.py
+soma
 teste.py
 env/lib/python3.13/site-packages/pip/__init__.py
 env/lib/python3.13/site-packages/pip/__main__.py
 env/lib/python3.13/site-packages/pip/__pip-runner__.py
 env/lib/python3.13/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
 env/lib/python3.13/site-packages/pip-23.1.2.dist-info/LICENSE.txt
 env/lib/python3.13/site-packages/pip-23.1.2.dist-info/entry_points.txt
@@ -995,18 +996,20 @@
 env/lib64/python3.13/site-packages/pip/_vendor/webencodings/tests.py
 env/lib64/python3.13/site-packages/pip/_vendor/webencodings/x_user_defined.py
 pythonce/OlaMi.c
 pythonce/OlaMi.py
 pythonce/__init__.py
 pythonce/c-teste.c
 pythonce/c-torrent.c
+pythonce/c_torrent.c
 pythonce/calculadora.c
 pythonce/count.c
 pythonce/count.py
 pythonce/ola.c
 pythonce/ola.py
 pythonce/soma.c
-pythonce/sub.c
+pythonce/subtracao.c
+pythonce/wozidown.py
 pythonce.egg-info/PKG-INFO
 pythonce.egg-info/SOURCES.txt
 pythonce.egg-info/dependency_links.txt
 pythonce.egg-info/top_level.txt
```

