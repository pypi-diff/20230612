# Comparing `tmp/pdm-2.7.1.tar.gz` & `tmp/pdm-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-2.7.1.tar", last modified: Tue Jun  6 03:56:08 2023, max compression
+gzip compressed data, was "pdm-2.7.2.tar", last modified: Mon Jun 12 03:10:47 2023, max compression
```

## Comparing `pdm-2.7.1.tar` & `pdm-2.7.2.tar`

### file list

```diff
@@ -1,272 +1,272 @@
--rw-r--r--   0        0        0   122599 2023-06-06 03:56:01.064340 pdm-2.7.1/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2023-06-06 03:56:01.064340 pdm-2.7.1/LICENSE
--rw-r--r--   0        0        0     1075 2023-06-06 03:56:01.064340 pdm-2.7.1/LICENSE
--rw-r--r--   0        0        0     7986 2023-06-06 03:56:01.064340 pdm-2.7.1/README.md
--rw-r--r--   0        0        0     7986 2023-06-06 03:56:01.064340 pdm-2.7.1/README.md
--rw-r--r--   0        0        0     4396 2023-06-06 03:56:08.520348 pdm-2.7.1/pyproject.toml
--rw-r--r--   0        0        0       65 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/__main__.py
--rw-r--r--   0        0        0      316 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/__version__.py
--rw-r--r--   0        0        0     3282 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/_types.py
--rw-r--r--   0        0        0      237 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/builders/__init__.py
--rw-r--r--   0        0        0    11850 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/builders/base.py
--rw-r--r--   0        0        0     1755 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/builders/editable.py
--rw-r--r--   0        0        0      656 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/builders/sdist.py
--rw-r--r--   0        0        0     1073 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/builders/wheel.py
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/__init__.py
--rw-r--r--   0        0        0    30752 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/actions.py
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/__init__.py
--rw-r--r--   0        0        0     2404 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/add.py
--rw-r--r--   0        0        0     2174 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/base.py
--rw-r--r--   0        0        0     4236 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/build.py
--rw-r--r--   0        0        0     6529 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/cache.py
--rw-r--r--   0        0        0     1324 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/completion.py
--rw-r--r--   0        0        0     5812 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/config.py
--rw-r--r--   0        0        0     2948 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/export.py
--rw-r--r--   0        0        0     3136 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/fix/__init__.py
--rw-r--r--   0        0        0     2309 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/fix/fixers.py
--rw-r--r--   0        0        0     1071 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/import_cmd.py
--rw-r--r--   0        0        0     3032 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/info.py
--rw-r--r--   0        0        0     8510 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/init.py
--rw-r--r--   0        0        0     3589 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/install.py
--rw-r--r--   0        0        0    15743 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/list.py
--rw-r--r--   0        0        0     2196 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/lock.py
--rw-r--r--   0        0        0     6596 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0     8027 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/publish/package.py
--rw-r--r--   0        0        0     6782 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/publish/repository.py
--rw-r--r--   0        0        0     1672 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/remove.py
--rw-r--r--   0        0        0    15445 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/run.py
--rw-r--r--   0        0        0     2436 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/search.py
--rw-r--r--   0        0        0     9364 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/self_cmd.py
--rw-r--r--   0        0        0     2896 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/show.py
--rw-r--r--   0        0        0     1447 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/sync.py
--rw-r--r--   0        0        0     2392 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/update.py
--rw-r--r--   0        0        0     1318 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/use.py
--rw-r--r--   0        0        0     1683 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/__init__.py
--rw-r--r--   0        0        0     2426 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/activate.py
--rw-r--r--   0        0        0     6171 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/backends.py
--rw-r--r--   0        0        0     2155 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/create.py
--rw-r--r--   0        0        0      819 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/list.py
--rw-r--r--   0        0        0     2195 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/purge.py
--rw-r--r--   0        0        0     1279 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/remove.py
--rw-r--r--   0        0        0     2759 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/commands/venv/utils.py
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/completions/__init__.py
--rw-r--r--   0        0        0     5083 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/completions/pdm.bash
--rw-r--r--   0        0        0    38005 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/completions/pdm.fish
--rw-r--r--   0        0        0    18567 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/completions/pdm.ps1
--rw-r--r--   0        0        0    25089 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/completions/pdm.zsh
--rw-r--r--   0        0        0     3840 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/filters.py
--rw-r--r--   0        0        0     1481 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/hooks.py
--rw-r--r--   0        0        0    10461 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/options.py
--rw-r--r--   0        0        0    24722 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/cli/utils.py
--rw-r--r--   0        0        0     2226 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/compat.py
--rw-r--r--   0        0        0    10647 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/core.py
--rw-r--r--   0        0        0      825 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/environments/__init__.py
--rw-r--r--   0        0        0     8850 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/environments/base.py
--rw-r--r--   0        0        0     3560 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/environments/local.py
--rw-r--r--   0        0        0     1600 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/environments/python.py
--rw-r--r--   0        0        0     1365 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/exceptions.py
--rw-r--r--   0        0        0     1202 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/formats/__init__.py
--rw-r--r--   0        0        0     3215 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/formats/base.py
--rw-r--r--   0        0        0     5788 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/formats/flit.py
--rw-r--r--   0        0        0     2400 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/formats/pipfile.py
--rw-r--r--   0        0        0     7490 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/formats/poetry.py
--rw-r--r--   0        0        0     7358 2023-06-06 03:56:01.068340 pdm-2.7.1/src/pdm/formats/requirements.py
--rw-r--r--   0        0        0     2309 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/formats/setup_py.py
--rw-r--r--   0        0        0      119 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/__init__.py
--rw-r--r--   0        0        0     1390 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/core.py
--rw-r--r--   0        0        0    10901 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/installers.py
--rw-r--r--   0        0        0     2091 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/manager.py
--rw-r--r--   0        0        0     2226 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/packages.py
--rw-r--r--   0        0        0    18161 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/synchronizers.py
--rw-r--r--   0        0        0    10990 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/installers/uninstallers.py
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/__init__.py
--rw-r--r--   0        0        0     3162 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/auth.py
--rw-r--r--   0        0        0     4394 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/backends.py
--rw-r--r--   0        0        0    11466 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/caches.py
--rw-r--r--   0        0        0    26568 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/candidates.py
--rw-r--r--   0        0        0      287 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/environment.py
--rw-r--r--   0        0        0     1714 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/in_process/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/in_process/get_abi_tag.py
--rw-r--r--   0        0        0     6182 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/in_process/parse_setup.py
--rw-r--r--   0        0        0     1165 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/in_process/pep508.py
--rw-r--r--   0        0        0     1653 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/in_process/sysconfig_get_paths.py
--rw-r--r--   0        0        0     5701 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/markers.py
--rw-r--r--   0        0        0     3507 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/project_info.py
--rw-r--r--   0        0        0     2195 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/python.py
--rw-r--r--   0        0        0      318 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/python_max_versions.json
--rw-r--r--   0        0        0    21340 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/repositories.py
--rw-r--r--   0        0        0    18677 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/requirements.py
--rw-r--r--   0        0        0     2313 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/search.py
--rw-r--r--   0        0        0     1344 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/session.py
--rw-r--r--   0        0        0    14482 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/setup.py
--rw-r--r--   0        0        0    16337 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/specifiers.py
--rw-r--r--   0        0        0     1300 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/venv.py
--rw-r--r--   0        0        0     5924 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/versions.py
--rw-r--r--   0        0        0     2721 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/models/working_set.py
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/pep582/__init__.py
--rw-r--r--   0        0        0     4481 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/pep582/sitecustomize.py
--rw-r--r--   0        0        0      134 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/project/__init__.py
--rw-r--r--   0        0        0    16748 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/project/config.py
--rw-r--r--   0        0        0    26273 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/project/core.py
--rw-r--r--   0        0        0     2093 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/project/lockfile.py
--rw-r--r--   0        0        0     3385 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/project/project_file.py
--rw-r--r--   0        0        0     1070 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/project/toml_file.py
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/py.typed
--rw-r--r--   0        0        0    19876 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/pytest.py
--rw-r--r--   0        0        0       61 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/resolver/__init__.py
--rw-r--r--   0        0        0     1954 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/resolver/core.py
--rw-r--r--   0        0        0    13119 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/resolver/providers.py
--rw-r--r--   0        0        0     1580 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/resolver/python.py
--rw-r--r--   0        0        0     3742 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/resolver/reporters.py
--rw-r--r--   0        0        0     4027 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/signals.py
--rw-r--r--   0        0        0     8054 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/termui.py
--rw-r--r--   0        0        0    13866 2023-06-06 03:56:01.072340 pdm-2.7.1/src/pdm/utils.py
--rw-r--r--   0        0        0       72 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/__init__.py
--rw-r--r--   0        0        0     3723 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/conftest.py
--rw-r--r--   0        0        0    12377 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_add.py
--rw-r--r--   0        0        0     5799 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_build.py
--rw-r--r--   0        0        0     5229 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_cache.py
--rw-r--r--   0        0        0     9286 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_config.py
--rw-r--r--   0        0        0     2029 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_fix.py
--rw-r--r--   0        0        0    10375 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_hooks.py
--rw-r--r--   0        0        0     4496 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_init.py
--rw-r--r--   0        0        0    11265 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_install.py
--rw-r--r--   0        0        0    28998 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_list.py
--rw-r--r--   0        0        0     6324 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_lock.py
--rw-r--r--   0        0        0     7796 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_others.py
--rw-r--r--   0        0        0     6052 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_publish.py
--rw-r--r--   0        0        0     3872 2023-06-06 03:56:01.072340 pdm-2.7.1/tests/cli/test_remove.py
--rw-r--r--   0        0        0    29259 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/cli/test_run.py
--rw-r--r--   0        0        0     3599 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/cli/test_self_command.py
--rw-r--r--   0        0        0     8888 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/cli/test_update.py
--rw-r--r--   0        0        0     2942 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/cli/test_use.py
--rw-r--r--   0        0        0    10430 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/cli/test_venv.py
--rw-r--r--   0        0        0     3079 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/conftest.py
--rw-r--r--   0        0        0      235 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/Pipfile
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0    49497 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
--rw-r--r--   0        0        0      546 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
--rw-r--r--   0        0        0   422824 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1254 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
--rw-r--r--   0        0        0     1254 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1038 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1.tar.gz
--rw-r--r--   0        0        0     2615 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1.zip
--rw-r--r--   0        0        0     4595 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
--rw-r--r--   0        0        0     5359 2023-06-06 03:56:01.076340 pdm-2.7.1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0    56715 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
--rw-r--r--   0        0        0     6138 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5786 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
--rw-r--r--   0        0        0    17978 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
--rw-r--r--   0        0        0    24489 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0   156727 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
--rw-r--r--   0        0        0     1401 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     1405 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
--rw-r--r--   0        0        0   305481 2023-06-06 03:56:01.080340 pdm-2.7.1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   531270 2023-06-06 03:56:01.084340 pdm-2.7.1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
--rw-r--r--   0        0        0  1232518 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
--rw-r--r--   0        0        0    26662 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
--rw-r--r--   0        0        0    35301 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5312 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
--rw-r--r--   0        0        0      326 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/index/demo.html
--rw-r--r--   0        0        0      511 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/index/future-fstrings.html
--rw-r--r--   0        0        0      262 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/index/pep345-legacy.html
--rw-r--r--   0        0        0      262 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/index/wheel.html
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/__init__.py
--rw-r--r--   0        0        0       42 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-#-with-hash/demo.py
--rw-r--r--   0        0        0      332 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-#-with-hash/setup.py
--rw-r--r--   0        0        0       26 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      462 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-failure-no-dep/demo.py
--rw-r--r--   0        0        0      246 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-failure-no-dep/setup.py
--rw-r--r--   0        0        0       42 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-failure/demo.py
--rw-r--r--   0        0        0      345 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-failure/setup.py
--rw-r--r--   0        0        0       12 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       36 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      442 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0     3983 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
--rw-r--r--   0        0        0      318 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
--rw-r--r--   0        0        0      157 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
--rw-r--r--   0        0        0       12 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/my_package/data.json
--rw-r--r--   0        0        0    29800 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      574 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0      122 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/requirements.ini
--rw-r--r--   0        0        0     7521 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      211 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0      728 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/setup.txt
--rw-r--r--   0        0        0       21 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       18 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-parent-package/README.md
--rw-r--r--   0        0        0       22 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-parent-package/package-a/foo.py
--rw-r--r--   0        0        0      120 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-parent-package/package-a/setup.py
--rw-r--r--   0        0        0       22 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-parent-package/package-b/bar.py
--rw-r--r--   0        0        0      197 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-prerelease/demo.py
--rw-r--r--   0        0        0      334 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-prerelease/setup.py
--rw-r--r--   0        0        0       12 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      456 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       42 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo/demo.py
--rw-r--r--   0        0        0      332 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo/setup.py
--rw-r--r--   0        0        0       26 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo_extras/demo.py
--rw-r--r--   0        0        0      250 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/demo_extras/setup.py
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/flit-demo/README.rst
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/flit-demo/doc/index.html
--rw-r--r--   0        0        0       49 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/flit-demo/flit.py
--rw-r--r--   0        0        0      969 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/flit-demo/pyproject.toml
--rw-r--r--   0        0        0       12 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/poetry-demo/mylib.py
--rw-r--r--   0        0        0      863 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/poetry-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-hatch-static/README.md
--rw-r--r--   0        0        0      386 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-hatch-static/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/README.md
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/core/core.py
--rw-r--r--   0        0        0      179 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/core/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/package_a/alice.py
--rw-r--r--   0        0        0      231 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/package_b/bob.py
--rw-r--r--   0        0        0      231 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
--rw-r--r--   0        0        0      237 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-monorepo/pyproject.toml
--rw-r--r--   0        0        0      380 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-plugin-pdm/hello.py
--rw-r--r--   0        0        0      312 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
--rw-r--r--   0        0        0      380 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-plugin/hello.py
--rw-r--r--   0        0        0      168 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-plugin/setup.py
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-removal/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-removal/bar.py
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-removal/foo.py
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-removal/subdir/__init__.py
--rw-r--r--   0        0        0       10 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-setuptools/AUTHORS
--rw-r--r--   0        0        0       12 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-setuptools/README.md
--rw-r--r--   0        0        0       22 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-setuptools/mymodule.py
--rw-r--r--   0        0        0      398 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-setuptools/setup.cfg
--rw-r--r--   0        0        0      308 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/projects/test-setuptools/setup.py
--rw-r--r--   0        0        0     1525 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/pypi.json
--rw-r--r--   0        0        0     1330 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/pyproject.toml
--rw-r--r--   0        0        0       20 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/requirements-include.txt
--rw-r--r--   0        0        0      502 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/fixtures/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_backends.py
--rw-r--r--   0        0        0    13344 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_candidates.py
--rw-r--r--   0        0        0     1971 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_marker.py
--rw-r--r--   0        0        0     2679 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_requirements.py
--rw-r--r--   0        0        0     2526 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_setup_parsing.py
--rw-r--r--   0        0        0     3418 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_specifiers.py
--rw-r--r--   0        0        0     2703 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/models/test_versions.py
--rw-r--r--   0        0        0        0 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/resolver/__init__.py
--rw-r--r--   0        0        0    11567 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/resolver/test_resolve.py
--rw-r--r--   0        0        0     7197 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/test_formats.py
--rw-r--r--   0        0        0     7231 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/test_installer.py
--rw-r--r--   0        0        0     1829 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/test_integration.py
--rw-r--r--   0        0        0     3435 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/test_plugin.py
--rw-r--r--   0        0        0    12085 2023-06-06 03:56:01.092340 pdm-2.7.1/tests/test_project.py
--rw-r--r--   0        0        0     1103 2023-06-06 03:56:01.096340 pdm-2.7.1/tests/test_signals.py
--rw-r--r--   0        0        0     4419 2023-06-06 03:56:01.096340 pdm-2.7.1/tests/test_utils.py
--rw-r--r--   0        0        0     9611 1970-01-01 00:00:00.000000 pdm-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0   123520 2023-06-12 03:10:34.469287 pdm-2.7.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-06-12 03:10:34.469287 pdm-2.7.2/LICENSE
+-rw-r--r--   0        0        0     1075 2023-06-12 03:10:34.469287 pdm-2.7.2/LICENSE
+-rw-r--r--   0        0        0     7986 2023-06-12 03:10:34.469287 pdm-2.7.2/README.md
+-rw-r--r--   0        0        0     7986 2023-06-12 03:10:34.469287 pdm-2.7.2/README.md
+-rw-r--r--   0        0        0     4396 2023-06-12 03:10:47.977488 pdm-2.7.2/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/__main__.py
+-rw-r--r--   0        0        0      316 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/__version__.py
+-rw-r--r--   0        0        0     3282 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/_types.py
+-rw-r--r--   0        0        0      237 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/builders/__init__.py
+-rw-r--r--   0        0        0    11850 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/builders/base.py
+-rw-r--r--   0        0        0     1755 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/builders/editable.py
+-rw-r--r--   0        0        0      656 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/builders/sdist.py
+-rw-r--r--   0        0        0     1073 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/builders/wheel.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/__init__.py
+-rw-r--r--   0        0        0    14229 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/actions.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/__init__.py
+-rw-r--r--   0        0        0     7095 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/add.py
+-rw-r--r--   0        0        0     2451 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/base.py
+-rw-r--r--   0        0        0     4236 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/build.py
+-rw-r--r--   0        0        0     6542 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/cache.py
+-rw-r--r--   0        0        0     1324 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/completion.py
+-rw-r--r--   0        0        0     5812 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/config.py
+-rw-r--r--   0        0        0     3066 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/export.py
+-rw-r--r--   0        0        0     3136 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/fix/__init__.py
+-rw-r--r--   0        0        0     2309 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/fix/fixers.py
+-rw-r--r--   0        0        0     3689 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/import_cmd.py
+-rw-r--r--   0        0        0     3032 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/info.py
+-rw-r--r--   0        0        0     8612 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/init.py
+-rw-r--r--   0        0        0     3589 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/install.py
+-rw-r--r--   0        0        0    15754 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/list.py
+-rw-r--r--   0        0        0     2196 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/lock.py
+-rw-r--r--   0        0        0     6596 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0     8027 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/publish/package.py
+-rw-r--r--   0        0        0     6782 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/publish/repository.py
+-rw-r--r--   0        0        0     4271 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/remove.py
+-rw-r--r--   0        0        0    15427 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/run.py
+-rw-r--r--   0        0        0     2436 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/search.py
+-rw-r--r--   0        0        0     9373 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/self_cmd.py
+-rw-r--r--   0        0        0     2896 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/show.py
+-rw-r--r--   0        0        0     1447 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/sync.py
+-rw-r--r--   0        0        0     6898 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/update.py
+-rw-r--r--   0        0        0     6489 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/use.py
+-rw-r--r--   0        0        0     1715 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/venv/__init__.py
+-rw-r--r--   0        0        0     2426 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/venv/activate.py
+-rw-r--r--   0        0        0     6149 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/venv/backends.py
+-rw-r--r--   0        0        0     2155 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/venv/create.py
+-rw-r--r--   0        0        0      819 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/venv/list.py
+-rw-r--r--   0        0        0     2195 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/venv/purge.py
+-rw-r--r--   0        0        0     1279 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/venv/remove.py
+-rw-r--r--   0        0        0     2759 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/commands/venv/utils.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/completions/__init__.py
+-rw-r--r--   0        0        0     5096 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/completions/pdm.bash
+-rw-r--r--   0        0        0    38130 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/completions/pdm.fish
+-rw-r--r--   0        0        0    18583 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/completions/pdm.ps1
+-rw-r--r--   0        0        0    25158 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/completions/pdm.zsh
+-rw-r--r--   0        0        0     3840 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/filters.py
+-rw-r--r--   0        0        0     1481 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/hooks.py
+-rw-r--r--   0        0        0    10461 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/options.py
+-rw-r--r--   0        0        0    25027 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/cli/utils.py
+-rw-r--r--   0        0        0     2226 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/compat.py
+-rw-r--r--   0        0        0    10667 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/core.py
+-rw-r--r--   0        0        0      825 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/environments/__init__.py
+-rw-r--r--   0        0        0     8850 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/environments/base.py
+-rw-r--r--   0        0        0     3560 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/environments/local.py
+-rw-r--r--   0        0        0     1600 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/environments/python.py
+-rw-r--r--   0        0        0     1362 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/exceptions.py
+-rw-r--r--   0        0        0     1202 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/formats/__init__.py
+-rw-r--r--   0        0        0     3215 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/formats/base.py
+-rw-r--r--   0        0        0     5788 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/formats/flit.py
+-rw-r--r--   0        0        0     2400 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/formats/pipfile.py
+-rw-r--r--   0        0        0     7490 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/formats/poetry.py
+-rw-r--r--   0        0        0     7502 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/formats/requirements.py
+-rw-r--r--   0        0        0     2309 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/formats/setup_py.py
+-rw-r--r--   0        0        0      119 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/installers/__init__.py
+-rw-r--r--   0        0        0     1390 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/installers/core.py
+-rw-r--r--   0        0        0    10901 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/installers/installers.py
+-rw-r--r--   0        0        0     2091 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/installers/manager.py
+-rw-r--r--   0        0        0     2226 2023-06-12 03:10:34.473287 pdm-2.7.2/src/pdm/installers/packages.py
+-rw-r--r--   0        0        0    18161 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/installers/synchronizers.py
+-rw-r--r--   0        0        0    10990 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/installers/uninstallers.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/__init__.py
+-rw-r--r--   0        0        0     3162 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/auth.py
+-rw-r--r--   0        0        0     4698 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/backends.py
+-rw-r--r--   0        0        0    11466 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/caches.py
+-rw-r--r--   0        0        0    26568 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/candidates.py
+-rw-r--r--   0        0        0      287 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/environment.py
+-rw-r--r--   0        0        0     1845 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/in_process/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/in_process/get_abi_tag.py
+-rw-r--r--   0        0        0     6323 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/in_process/parse_setup.py
+-rw-r--r--   0        0        0     1165 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/in_process/pep508.py
+-rw-r--r--   0        0        0     1653 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/in_process/sysconfig_get_paths.py
+-rw-r--r--   0        0        0     5701 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/markers.py
+-rw-r--r--   0        0        0     3507 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/project_info.py
+-rw-r--r--   0        0        0     2195 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/python.py
+-rw-r--r--   0        0        0      318 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/python_max_versions.json
+-rw-r--r--   0        0        0    21340 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/repositories.py
+-rw-r--r--   0        0        0    18677 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/requirements.py
+-rw-r--r--   0        0        0     2313 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/search.py
+-rw-r--r--   0        0        0     2426 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/session.py
+-rw-r--r--   0        0        0    14482 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/setup.py
+-rw-r--r--   0        0        0    16337 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/specifiers.py
+-rw-r--r--   0        0        0     1300 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/venv.py
+-rw-r--r--   0        0        0     5924 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/versions.py
+-rw-r--r--   0        0        0     2721 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/models/working_set.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/pep582/__init__.py
+-rw-r--r--   0        0        0     4481 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/pep582/sitecustomize.py
+-rw-r--r--   0        0        0      134 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/project/__init__.py
+-rw-r--r--   0        0        0    16748 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/project/config.py
+-rw-r--r--   0        0        0    26273 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/project/core.py
+-rw-r--r--   0        0        0     2093 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/project/lockfile.py
+-rw-r--r--   0        0        0     3385 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/project/project_file.py
+-rw-r--r--   0        0        0     1070 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/project/toml_file.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/py.typed
+-rw-r--r--   0        0        0    19876 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/pytest.py
+-rw-r--r--   0        0        0       61 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/resolver/__init__.py
+-rw-r--r--   0        0        0     1954 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/resolver/core.py
+-rw-r--r--   0        0        0    13119 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/resolver/providers.py
+-rw-r--r--   0        0        0     1580 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/resolver/python.py
+-rw-r--r--   0        0        0     3742 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/resolver/reporters.py
+-rw-r--r--   0        0        0     4027 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/signals.py
+-rw-r--r--   0        0        0     8054 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/termui.py
+-rw-r--r--   0        0        0    13866 2023-06-12 03:10:34.477287 pdm-2.7.2/src/pdm/utils.py
+-rw-r--r--   0        0        0       72 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/__init__.py
+-rw-r--r--   0        0        0     3723 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12362 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_add.py
+-rw-r--r--   0        0        0     5799 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_build.py
+-rw-r--r--   0        0        0     5229 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_cache.py
+-rw-r--r--   0        0        0     9286 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_config.py
+-rw-r--r--   0        0        0     2029 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_fix.py
+-rw-r--r--   0        0        0    10375 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_hooks.py
+-rw-r--r--   0        0        0     4481 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_init.py
+-rw-r--r--   0        0        0    11265 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_install.py
+-rw-r--r--   0        0        0    28998 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_list.py
+-rw-r--r--   0        0        0     6324 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_lock.py
+-rw-r--r--   0        0        0     7796 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_others.py
+-rw-r--r--   0        0        0     6052 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_publish.py
+-rw-r--r--   0        0        0     3888 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_remove.py
+-rw-r--r--   0        0        0    29259 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_run.py
+-rw-r--r--   0        0        0     3599 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_self_command.py
+-rw-r--r--   0        0        0     8876 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_update.py
+-rw-r--r--   0        0        0     2997 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_use.py
+-rw-r--r--   0        0        0    10430 2023-06-12 03:10:34.477287 pdm-2.7.2/tests/cli/test_venv.py
+-rw-r--r--   0        0        0     3079 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/conftest.py
+-rw-r--r--   0        0        0      235 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/Pipfile
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0    49497 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
+-rw-r--r--   0        0        0      546 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
+-rw-r--r--   0        0        0   422824 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1254 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
+-rw-r--r--   0        0        0     1254 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1038 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/demo-0.0.1.tar.gz
+-rw-r--r--   0        0        0     2615 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/demo-0.0.1.zip
+-rw-r--r--   0        0        0     4595 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5359 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    56715 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6138 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5786 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
+-rw-r--r--   0        0        0    17978 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
+-rw-r--r--   0        0        0    24489 2023-06-12 03:10:34.481287 pdm-2.7.2/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   156727 2023-06-12 03:10:34.485287 pdm-2.7.2/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     1401 2023-06-12 03:10:34.485287 pdm-2.7.2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1405 2023-06-12 03:10:34.485287 pdm-2.7.2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
+-rw-r--r--   0        0        0   305481 2023-06-12 03:10:34.485287 pdm-2.7.2/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   531270 2023-06-12 03:10:34.489287 pdm-2.7.2/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
+-rw-r--r--   0        0        0  1232518 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
+-rw-r--r--   0        0        0    26662 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
+-rw-r--r--   0        0        0    35301 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5312 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0      326 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/index/demo.html
+-rw-r--r--   0        0        0      511 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/index/future-fstrings.html
+-rw-r--r--   0        0        0      262 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/index/pep345-legacy.html
+-rw-r--r--   0        0        0      262 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/index/wheel.html
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-#-with-hash/demo.py
+-rw-r--r--   0        0        0      332 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-#-with-hash/setup.py
+-rw-r--r--   0        0        0       26 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      462 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-failure-no-dep/demo.py
+-rw-r--r--   0        0        0      246 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-failure-no-dep/setup.py
+-rw-r--r--   0        0        0       42 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-failure/demo.py
+-rw-r--r--   0        0        0      345 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-failure/setup.py
+-rw-r--r--   0        0        0       12 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       36 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      442 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0     3983 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
+-rw-r--r--   0        0        0      318 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
+-rw-r--r--   0        0        0       12 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package/my_package/data.json
+-rw-r--r--   0        0        0    29800 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      574 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package/requirements.ini
+-rw-r--r--   0        0        0     7521 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      211 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0      728 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package/setup.txt
+-rw-r--r--   0        0        0       21 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       18 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-parent-package/README.md
+-rw-r--r--   0        0        0       22 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-parent-package/package-a/foo.py
+-rw-r--r--   0        0        0      120 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-parent-package/package-a/setup.py
+-rw-r--r--   0        0        0       22 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-parent-package/package-b/bar.py
+-rw-r--r--   0        0        0      197 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-prerelease/demo.py
+-rw-r--r--   0        0        0      334 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-prerelease/setup.py
+-rw-r--r--   0        0        0       12 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      456 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       42 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo/demo.py
+-rw-r--r--   0        0        0      332 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo/setup.py
+-rw-r--r--   0        0        0       26 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo_extras/demo.py
+-rw-r--r--   0        0        0      250 2023-06-12 03:10:34.493287 pdm-2.7.2/tests/fixtures/projects/demo_extras/setup.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/flit-demo/README.rst
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/flit-demo/doc/index.html
+-rw-r--r--   0        0        0       49 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/flit-demo/flit.py
+-rw-r--r--   0        0        0      969 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/flit-demo/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/poetry-demo/mylib.py
+-rw-r--r--   0        0        0      863 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/poetry-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-hatch-static/README.md
+-rw-r--r--   0        0        0      386 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-hatch-static/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-monorepo/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-monorepo/core/core.py
+-rw-r--r--   0        0        0      179 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-monorepo/core/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-monorepo/package_a/alice.py
+-rw-r--r--   0        0        0      231 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-monorepo/package_b/bob.py
+-rw-r--r--   0        0        0      231 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-monorepo/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-plugin-pdm/hello.py
+-rw-r--r--   0        0        0      312 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-plugin/hello.py
+-rw-r--r--   0        0        0      168 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-plugin/setup.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-removal/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-removal/bar.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-removal/foo.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-removal/subdir/__init__.py
+-rw-r--r--   0        0        0       10 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-setuptools/AUTHORS
+-rw-r--r--   0        0        0       12 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-setuptools/README.md
+-rw-r--r--   0        0        0       22 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-setuptools/mymodule.py
+-rw-r--r--   0        0        0      398 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-setuptools/setup.cfg
+-rw-r--r--   0        0        0      308 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/projects/test-setuptools/setup.py
+-rw-r--r--   0        0        0     1525 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/pypi.json
+-rw-r--r--   0        0        0     1330 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/requirements-include.txt
+-rw-r--r--   0        0        0      502 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/fixtures/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/models/__init__.py
+-rw-r--r--   0        0        0     3814 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/models/test_backends.py
+-rw-r--r--   0        0        0    13344 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/models/test_candidates.py
+-rw-r--r--   0        0        0     1971 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/models/test_marker.py
+-rw-r--r--   0        0        0     2679 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/models/test_requirements.py
+-rw-r--r--   0        0        0     2526 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/models/test_setup_parsing.py
+-rw-r--r--   0        0        0     3418 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/models/test_specifiers.py
+-rw-r--r--   0        0        0     2703 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/models/test_versions.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/resolver/__init__.py
+-rw-r--r--   0        0        0    11567 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/resolver/test_resolve.py
+-rw-r--r--   0        0        0     7704 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/test_formats.py
+-rw-r--r--   0        0        0     7231 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/test_installer.py
+-rw-r--r--   0        0        0     1829 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/test_integration.py
+-rw-r--r--   0        0        0     3435 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/test_plugin.py
+-rw-r--r--   0        0        0    12085 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/test_project.py
+-rw-r--r--   0        0        0     1103 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/test_signals.py
+-rw-r--r--   0        0        0     4419 2023-06-12 03:10:34.497287 pdm-2.7.2/tests/test_utils.py
+-rw-r--r--   0        0        0     9611 1970-01-01 00:00:00.000000 pdm-2.7.2/PKG-INFO
```

### Comparing `pdm-2.7.1/CHANGELOG.md` & `pdm-2.7.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Release v2.7.2 (2023-06-12)
+---------------------------
+
+### Features & Improvements
+
+- Add option to expand environment variables when exporting requirements. [#1997](https://github.com/pdm-project/pdm/issues/1997)
+
+### Bug Fixes
+
+- Case-insensitive sorting in `pdm list`. [#1973](https://github.com/pdm-project/pdm/issues/1973)
+- Make a compatible cache reader to read the old cache files. [#1981](https://github.com/pdm-project/pdm/issues/1981)
+- Fix a bug that `pdm init -n` doesn't respect the `--python` option. [#1984](https://github.com/pdm-project/pdm/issues/1984)
+- Do not use the deprecated nested argument groups. [#1988](https://github.com/pdm-project/pdm/issues/1988)
+- Fix an error parsing `setup.py` if it prints something to stdout. [#1995](https://github.com/pdm-project/pdm/issues/1995)
+- Exclude yanked versions when running `install-pdm.py`. [#1996](https://github.com/pdm-project/pdm/issues/1996)
+
+
 Release v2.7.1 (2023-06-06)
 ---------------------------
 
 ### Features & Improvements
 
 - Switch HTTP data cache to use a split body setup, where the actual body contents are not written to disk unless changed. Previously, any changed headers would write the whole body to disk again. [#1971](https://github.com/pdm-project/pdm/issues/1971)
 - Show the specific install commands for different installations when checking update. This was removed before. [#1972](https://github.com/pdm-project/pdm/issues/1972)
```

### Comparing `pdm-2.7.1/LICENSE` & `pdm-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/README.md` & `pdm-2.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 **For Windows**
 
 ```powershell
 (Invoke-WebRequest -Uri https://raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py -UseBasicParsing).Content | python -
 ```
 
 For security reasons, you should verify the checksum of `install-pdm.py`.
-The sha256 checksum is: `06abd94a6678636eba640529bf91b242759363c45d3620cdfabaa0053d826b30`
+The sha256 checksum is: `965900c551b4d1ba5127ecf95c127c99b5a1cccef4c183a5ecf447e876fa3160`
 
 The installer will install PDM into the user site and the location depends on the system:
 
 - `$HOME/.local/bin` for Unix
 - `%APPDATA%\Python\Scripts` on Windows
 
 You can pass additional options to the script to control how PDM is installed:
```

#### html2text {}

```diff
@@ -57,15 +57,15 @@
 Like Pip, PDM provides an installation script that will install PDM into an
 isolated environment. **For Linux/Mac** ```bash curl -sSL https://
 raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py | python3 - ```
 **For Windows** ```powershell (Invoke-WebRequest -Uri https://
 raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py -
 UseBasicParsing).Content | python - ``` For security reasons, you should verify
 the checksum of `install-pdm.py`. The sha256 checksum is:
-`06abd94a6678636eba640529bf91b242759363c45d3620cdfabaa0053d826b30` The
+`965900c551b4d1ba5127ecf95c127c99b5a1cccef4c183a5ecf447e876fa3160` The
 installer will install PDM into the user site and the location depends on the
 system: - `$HOME/.local/bin` for Unix - `%APPDATA%\Python\Scripts` on Windows
 You can pass additional options to the script to control how PDM is installed:
 ``` usage: install-pdm.py [-h] [-v VERSION] [--prerelease] [--remove] [-p PATH]
 [-d DEP] optional arguments: -h, --help show this help message and exit -
 v VERSION, --version VERSION | envvar: PDM_VERSION Specify the version to be
 installed, or HEAD to install from the main branch --prerelease | envvar:
```

### Comparing `pdm-2.7.1/pyproject.toml` & `pdm-2.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "2.7.1"
+version = "2.7.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pdm.fming.dev"
 Repository = "https://github.com/pdm-project/pdm"
```

### Comparing `pdm-2.7.1/src/pdm/_types.py` & `pdm-2.7.2/src/pdm/_types.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/builders/base.py` & `pdm-2.7.2/src/pdm/builders/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/builders/editable.py` & `pdm-2.7.2/src/pdm/builders/editable.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/builders/sdist.py` & `pdm-2.7.2/src/pdm/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/builders/wheel.py` & `pdm-2.7.2/src/pdm/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/actions.py` & `pdm-2.7.2/src/pdm/cli/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,769 +1,688 @@
 from __future__ import annotations
 
-import contextlib
-import datetime
-import hashlib
+import argparse
+import dataclasses as dc
 import json
 import os
 import sys
-import textwrap
-import warnings
-from argparse import Namespace
-from collections import defaultdict
-from itertools import chain
-from typing import Collection, Iterable, cast
+from collections import ChainMap, OrderedDict
+from concurrent.futures import ThreadPoolExecutor
+from json import dumps
+from pathlib import Path
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Iterable,
+    Mapping,
+    MutableMapping,
+    cast,
+    no_type_check,
+)
 
 import tomlkit
-from resolvelib.reporters import BaseReporter
-from resolvelib.resolvers import ResolutionImpossible, ResolutionTooDeep, Resolver
-from tomlkit.items import Array
+from packaging.specifiers import SpecifierSet
+from resolvelib.structs import DirectedGraph
+from rich.tree import Tree
 
 from pdm import termui
-from pdm.cli.filters import GroupSelection
-from pdm.cli.hooks import HookManager
-from pdm.cli.utils import (
-    check_project_file,
-    fetch_hashes,
-    find_importable_files,
-    format_lockfile,
-    format_resolution_impossible,
-    get_pep582_path,
-    merge_dictionary,
-    save_version_specifiers,
-    set_env_in_reg,
+from pdm.exceptions import PdmArgumentError, ProjectError
+from pdm.models.requirements import (
+    Requirement,
+    filter_requirements_with_extras,
+    parse_requirement,
+    strip_extras,
+)
+from pdm.models.specifiers import PySpecSet, get_specifier
+from pdm.utils import (
+    comparable_version,
+    is_path_relative_to,
+    normalize_name,
+    url_to_path,
 )
-from pdm.environments import BareEnvironment, PythonLocalEnvironment
-from pdm.exceptions import NoPythonVersion, PdmUsageError, ProjectError
-from pdm.models.backends import DEFAULT_BACKEND
-from pdm.models.candidates import Candidate
-from pdm.models.python import PythonInfo
-from pdm.models.requirements import Requirement, parse_requirement, strip_extras
-from pdm.models.specifiers import get_specifier
-from pdm.project import Project
-from pdm.resolver import resolve
-from pdm.utils import cd, normalize_name
 
+if TYPE_CHECKING:
+    from argparse import Action, _ArgumentGroup
 
-def do_lock(
-    project: Project,
-    strategy: str = "all",
-    tracked_names: Iterable[str] | None = None,
-    requirements: list[Requirement] | None = None,
-    dry_run: bool = False,
-    refresh: bool = False,
-    groups: list[str] | None = None,
-    cross_platform: bool | None = None,
-    hooks: HookManager | None = None,
-) -> dict[str, Candidate]:
-    """Performs the locking process and update lockfile."""
-    hooks = hooks or HookManager(project)
-    check_project_file(project)
-    if refresh:
-        locked_repo = project.locked_repository
-        repo = project.get_repository()
-        mapping: dict[str, Candidate] = {}
-        dependencies: dict[tuple[str, str | None], list[Requirement]] = {}
-        with project.core.ui.open_spinner("Re-calculating hashes..."):
-            for key, candidate in locked_repo.packages.items():
-                reqs, python_requires, summary = locked_repo.candidate_info[key]
-                candidate.summary = summary
-                candidate.requires_python = python_requires
-                mapping[candidate.identify()] = candidate
-                dependencies[candidate.dep_key] = list(map(parse_requirement, reqs))
-            with project.core.ui.logging("lock"):
-                fetch_hashes(repo, mapping)
-            lockfile = format_lockfile(project, mapping, dependencies)
-        project.write_lockfile(lockfile, groups=groups)
-        return mapping
-    # TODO: multiple dependency definitions for the same package.
-    if cross_platform is None:
-        cross_platform = project.lockfile.cross_platform
-    provider = project.get_provider(strategy, tracked_names, ignore_compatibility=cross_platform)
-    if not requirements:
-        requirements = [
-            r for g, deps in project.all_dependencies.items() if groups is None or g in groups for r in deps.values()
-        ]
-    if not cross_platform:
-        this_env = project.environment.marker_environment
-        requirements = [req for req in requirements if not req.marker or req.marker.evaluate(this_env)]
-    resolve_max_rounds = int(project.config["strategy.resolve_max_rounds"])
-    ui = project.core.ui
-    with ui.logging("lock"):
-        # The context managers are nested to ensure the spinner is stopped before
-        # any message is thrown to the output.
-        try:
-            with ui.open_spinner(title="Resolving dependencies") as spin:
-                reporter = project.get_reporter(requirements, tracked_names, spin)
-                resolver: Resolver = project.core.resolver_class(provider, reporter)
-                hooks.try_emit("pre_lock", requirements=requirements, dry_run=dry_run)
-                mapping, dependencies = resolve(
-                    resolver,
-                    requirements,
-                    project.environment.python_requires,
-                    resolve_max_rounds,
-                )
-                spin.update("Fetching hashes for resolved packages...")
-                fetch_hashes(provider.repository, mapping)
-        except ResolutionTooDeep:
-            ui.echo(f"{termui.Emoji.LOCK} Lock failed", err=True)
-            ui.echo(
-                "The dependency resolution exceeds the maximum loop depth of "
-                f"{resolve_max_rounds}, there may be some circular dependencies "
-                "in your project. Try to solve them or increase the "
-                f"[success]`strategy.resolve_max_rounds`[/] config.",
-                err=True,
-            )
-            raise
-        except ResolutionImpossible as err:
-            ui.echo(f"{termui.Emoji.LOCK} Lock failed", err=True)
-            ui.echo(format_resolution_impossible(err), err=True)
-            raise ResolutionImpossible("Unable to find a resolution") from None
+    from packaging.version import Version
+    from resolvelib.resolvers import RequirementInformation, ResolutionImpossible
+
+    from pdm.compat import Distribution
+    from pdm.compat import importlib_metadata as im
+    from pdm.models.candidates import Candidate
+    from pdm.models.repositories import BaseRepository
+    from pdm.project import Project
+
+
+class PdmFormatter(argparse.RawDescriptionHelpFormatter):
+    def start_section(self, heading: str | None) -> None:
+        return super().start_section(termui.style(heading.title() if heading else "", style="warning"))
+
+    def _format_usage(
+        self,
+        usage: str | None,
+        actions: Iterable[Action],
+        groups: Iterable[_ArgumentGroup],
+        prefix: str | None,
+    ) -> str:
+        if prefix is None:
+            prefix = "Usage: "
+        result = super()._format_usage(usage, actions, groups, prefix)
+        if prefix:
+            return result.replace(prefix, termui.style(prefix, style="warning"))
+        return result
+
+    def _format_action(self, action: Action) -> str:
+        # determine the required width and the entry label
+        help_position = min(self._action_max_length + 2, self._max_help_position)
+        help_width = max(self._width - help_position, 11)
+        action_width = help_position - self._current_indent - 2
+        action_header = self._format_action_invocation(action)
+
+        # no help; start on same line and add a final newline
+        if not action.help:
+            tup = self._current_indent, "", action_header
+            action_header = "%*s%s\n" % tup
+
+        # short action name; start on the same line and pad two spaces
+        elif len(action_header) <= action_width:
+            tup = self._current_indent, "", action_width, action_header  # type: ignore[assignment]
+            action_header = "%*s%-*s  " % tup  # type: ignore[str-format]
+            indent_first = 0
+
+        # long action name; start on the next line
         else:
-            data = format_lockfile(project, mapping, dependencies)
-            ui.echo(f"{termui.Emoji.LOCK} Lock successful")
-            project.write_lockfile(data, write=not dry_run, groups=groups, cross_platform=cross_platform)
-            hooks.try_emit("post_lock", resolution=mapping, dry_run=dry_run)
-
-    return mapping
+            tup = self._current_indent, "", action_header
+            action_header = "%*s%s\n" % tup
+            indent_first = help_position
 
+        # collect the pieces of the action help
+        parts = [termui.style(action_header, style="primary")]
 
-def resolve_candidates_from_lockfile(project: Project, requirements: Iterable[Requirement]) -> dict[str, Candidate]:
-    ui = project.core.ui
-    resolve_max_rounds = int(project.config["strategy.resolve_max_rounds"])
-    reqs = [
-        req for req in requirements if not req.marker or req.marker.evaluate(project.environment.marker_environment)
-    ]
-    with ui.logging("install-resolve"):
-        with ui.open_spinner("Resolving packages from lockfile...") as spinner:
-            reporter = BaseReporter()
-            provider = project.get_provider(for_install=True)
-            resolver: Resolver = project.core.resolver_class(provider, reporter)
-            mapping, *_ = resolve(
-                resolver,
-                reqs,
-                project.environment.python_requires,
-                resolve_max_rounds,
-            )
-            spinner.update("Fetching hashes for resolved packages...")
-            fetch_hashes(provider.repository, mapping)
-    return mapping
-
-
-def check_lockfile(project: Project, raise_not_exist: bool = True) -> str | None:
-    """Check if the lock file exists and is up to date. Return the update strategy."""
-    if not project.lockfile.exists():
-        if raise_not_exist:
-            raise ProjectError("Lock file does not exist, nothing to install")
-        project.core.ui.echo("Lock file does not exist", style="warning", err=True)
-        return "all"
-    elif not project.lockfile.is_compatible():
-        project.core.ui.echo(
-            "Lock file version is not compatible with PDM, installation may fail",
-            style="warning",
-            err=True,
-        )
-        return "reuse"  # try to reuse the lockfile if possible
-    elif not project.is_lockfile_hash_match():
-        project.core.ui.echo(
-            "Lock file hash doesn't match pyproject.toml, packages may be outdated",
-            style="warning",
-            err=True,
-        )
-        return "reuse"
-    return None
+        # if there was help for the action, add lines of help text
+        if action.help:
+            help_text = self._expand_help(action)
+            help_lines = self._split_lines(help_text, help_width)
+            parts.append("%*s%s\n" % (indent_first, "", help_lines[0]))
+            for line in help_lines[1:]:
+                parts.append("%*s%s\n" % (help_position, "", line))
 
+        # or add a newline if the description doesn't end with one
+        elif not action_header.endswith("\n"):
+            parts.append("\n")
 
-def do_sync(
-    project: Project,
-    *,
-    selection: GroupSelection,
-    dry_run: bool = False,
-    clean: bool = False,
-    requirements: list[Requirement] | None = None,
-    tracked_names: Collection[str] | None = None,
-    no_editable: bool | Collection[str] = False,
-    no_self: bool = False,
-    reinstall: bool = False,
-    only_keep: bool = False,
-    fail_fast: bool = False,
-    hooks: HookManager | None = None,
-) -> None:
-    """Synchronize project"""
-    hooks = hooks or HookManager(project)
-    if requirements is None:
-        requirements = []
-        selection.validate()
-        for group in selection:
-            requirements.extend(project.get_dependencies(group).values())
-    candidates = resolve_candidates_from_lockfile(project, requirements)
-    if tracked_names and dry_run:
-        candidates = {name: c for name, c in candidates.items() if name in tracked_names}
-    synchronizer = project.core.synchronizer_class(
-        candidates,
-        project.environment,
-        clean=clean,
-        dry_run=dry_run,
-        no_editable=no_editable,
-        install_self=not no_self and "default" in selection and bool(project.name),
-        reinstall=reinstall,
-        only_keep=only_keep,
-        fail_fast=fail_fast,
-    )
-    with project.core.ui.logging("install"):
-        hooks.try_emit("pre_install", candidates=candidates, dry_run=dry_run)
-        synchronizer.synchronize()
-        hooks.try_emit("post_install", candidates=candidates, dry_run=dry_run)
+        # if there are any sub-actions, add their help as well
+        for subaction in self._iter_indented_subactions(action):
+            parts.append(self._format_action(subaction))
 
+        # return a single string
+        return self._join_parts(parts)
 
-def do_add(
-    project: Project,
-    *,
-    selection: GroupSelection,
-    sync: bool = True,
-    save: str = "compatible",
-    strategy: str = "reuse",
-    editables: Collection[str] = (),
-    packages: Collection[str] = (),
-    unconstrained: bool = False,
-    no_editable: bool = False,
-    no_self: bool = False,
-    dry_run: bool = False,
-    prerelease: bool = False,
-    fail_fast: bool = False,
-    hooks: HookManager | None = None,
-) -> None:
-    """Add packages and install"""
-    hooks = hooks or HookManager(project)
-    check_project_file(project)
-    if editables and no_editable:
-        raise PdmUsageError("Cannot use --no-editable with editable packages given.")
-    group = selection.one()
-    tracked_names: set[str] = set()
-    requirements: dict[str, Requirement] = {}
-    lock_groups = [] if project.lockfile.empty() else project.lockfile.groups
-    if lock_groups is not None and group not in lock_groups:
-        project.core.ui.echo(f"Adding group [success]{group}[/] to lockfile", err=True, style="info")
-        lock_groups.append(group)
-    if group == "default" or not selection.dev and group not in project.pyproject.settings.get("dev-dependencies", {}):
-        if editables:
-            raise PdmUsageError("Cannot add editables to the default or optional dependency group")
-    for r in [parse_requirement(line, True) for line in editables] + [parse_requirement(line) for line in packages]:
-        if project.name and normalize_name(project.name) == r.key and not r.extras:
-            project.core.ui.echo(
-                f"Package [req]{project.name}[/] is the project itself.",
-                err=True,
-                style="warning",
-            )
-            continue
-        if r.is_file_or_url:
-            r.relocate(project.backend)  # type: ignore[attr-defined]
-        key = r.identify()
-        r.prerelease = prerelease
-        tracked_names.add(key)
-        requirements[key] = r
-    if requirements:
-        project.core.ui.echo(
-            f"Adding packages to [primary]{group}[/] "
-            f"{'dev-' if selection.dev else ''}dependencies: "
-            + ", ".join(f"[req]{r.as_line()}[/]" for r in requirements.values())
-        )
-    all_dependencies = project.all_dependencies
-    group_deps = all_dependencies.setdefault(group, {})
-    if unconstrained:
-        if not requirements:
-            raise PdmUsageError("--unconstrained requires at least one package")
-        for req in group_deps.values():
-            req.specifier = get_specifier("")
-    group_deps.update(requirements)
-    reqs = [r for g, deps in all_dependencies.items() if lock_groups is None or g in lock_groups for r in deps.values()]
-    with hooks.skipping("post_lock"):
-        resolved = do_lock(
-            project,
-            strategy,
-            tracked_names,
-            reqs,
-            dry_run=True,
-            hooks=hooks,
-            groups=lock_groups,
-        )
 
-    # Update dependency specifiers and lockfile hash.
-    deps_to_update = group_deps if unconstrained else requirements
-    save_version_specifiers({group: deps_to_update}, resolved, save)
-    if not dry_run:
-        project.add_dependencies(deps_to_update, group, selection.dev or False)
-        project.write_lockfile(project.lockfile._data, False, groups=lock_groups)
-        hooks.try_emit("post_lock", resolution=resolved, dry_run=dry_run)
-    _populate_requirement_names(group_deps)
-    if sync:
-        do_sync(
-            project,
-            selection=GroupSelection(project, groups=[group], default=False),
-            no_editable=no_editable and tracked_names,
-            no_self=no_self,
-            requirements=list(group_deps.values()),
-            dry_run=dry_run,
-            fail_fast=fail_fast,
-            hooks=hooks,
+class ArgumentParser(argparse.ArgumentParser):
+    """A standard argument parser but with title-cased help."""
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        kwargs["formatter_class"] = PdmFormatter
+        kwargs["add_help"] = False
+        super().__init__(*args, **kwargs)
+        self.add_argument(
+            "-h", "--help", action="help", default=argparse.SUPPRESS, help="Show this help message and exit."
         )
 
 
-def _populate_requirement_names(req_mapping: dict[str, Requirement]) -> None:
-    # Update the requirement key if the name changed.
-    for key, req in list(req_mapping.items()):
-        if key and key.startswith(":empty:"):
-            req_mapping[req.identify()] = req
-            del req_mapping[key]
+class ErrorArgumentParser(ArgumentParser):
+    """A subclass of argparse.ArgumentParser that raises
+    parsing error rather than exiting.
 
+    This does the same as passing exit_on_error=False on Python 3.9+
+    """
 
-def do_update(
-    project: Project,
-    *,
-    selection: GroupSelection,
-    strategy: str = "reuse",
-    save: str = "compatible",
-    unconstrained: bool = False,
-    top: bool = False,
-    dry_run: bool = False,
-    packages: Collection[str] = (),
-    sync: bool = True,
-    no_editable: bool = False,
-    no_self: bool = False,
-    prerelease: bool = False,
-    fail_fast: bool = False,
-    hooks: HookManager | None = None,
-) -> None:
-    """Update specified packages or all packages"""
-    hooks = hooks or HookManager(project)
-    check_project_file(project)
-    if len(packages) > 0 and (top or len(selection.groups) > 1 or not selection.default):
-        raise PdmUsageError("packages argument can't be used together with multiple -G or " "--no-default or --top.")
-    all_dependencies = project.all_dependencies
-    updated_deps: dict[str, dict[str, Requirement]] = defaultdict(dict)
-    locked_groups = project.lockfile.groups
-    if not packages:
-        if prerelease:
-            raise PdmUsageError("--prerelease must be used with packages given")
-        selection.validate()
-        for group in selection:
-            updated_deps[group] = all_dependencies[group]
-    else:
-        group = selection.one()
-        if locked_groups and group not in locked_groups:
-            raise ProjectError(f"Requested group not in lockfile: {group}")
-        dependencies = all_dependencies[group]
-        for name in packages:
-            matched_name = next(
-                (k for k in dependencies if normalize_name(strip_extras(k)[0]) == normalize_name(name)),
-                None,
-            )
-            if not matched_name:
-                raise ProjectError(
-                    f"[req]{name}[/] does not exist in [primary]{group}[/] "
-                    f"{'dev-' if selection.dev else ''}dependencies."
+    def _parse_known_args(
+        self, arg_strings: list[str], namespace: argparse.Namespace
+    ) -> tuple[argparse.Namespace, list[str]]:
+        try:
+            return super()._parse_known_args(arg_strings, namespace)
+        except argparse.ArgumentError as e:
+            # We raise a dedicated error to avoid being caught by the caller
+            raise PdmArgumentError(e) from e
+
+
+@dc.dataclass(frozen=True)
+class Package:
+    """An internal class for the convenience of dependency graph building."""
+
+    name: str = dc.field(hash=True, compare=True)
+    version: str | None = dc.field(compare=False)
+    requirements: dict[str, Requirement] = dc.field(compare=False)
+
+    def __repr__(self) -> str:
+        return f"<Package {self.name}=={self.version}>"
+
+
+def build_dependency_graph(
+    working_set: Mapping[str, im.Distribution],
+    marker_env: dict[str, str] | None = None,
+    selected: set[str] | None = None,
+    include_sub: bool = True,
+) -> DirectedGraph:
+    """Build a dependency graph from locked result."""
+    graph: DirectedGraph[Package | None] = DirectedGraph()
+    graph.add(None)  # sentinel parent of top nodes.
+    node_with_extras: set[str] = set()
+
+    def add_package(key: str, dist: Distribution | None) -> Package:
+        name, extras = strip_extras(key)
+        extras = extras or ()
+        reqs: dict[str, Requirement] = {}
+        if dist:
+            requirements = (
+                parse_requirement(r)
+                for r in filter_requirements_with_extras(
+                    cast(str, dist.metadata["Name"]),
+                    dist.requires or [],
+                    extras,
+                    include_default=True,
                 )
-            dependencies[matched_name].prerelease = prerelease
-            updated_deps[group][matched_name] = dependencies[matched_name]
-        project.core.ui.echo(
-            "Updating packages: {}.".format(
-                ", ".join(f"[req]{v}[/]" for v in chain.from_iterable(updated_deps.values()))
             )
-        )
-    if unconstrained:
-        for deps in updated_deps.values():
-            for dep in deps.values():
-                dep.specifier = get_specifier("")
-    reqs = [r for deps in all_dependencies.values() for r in deps.values()]
-    resolved = do_lock(
-        project,
-        strategy,
-        chain.from_iterable(updated_deps.values()),
-        reqs,
-        dry_run=True,
-        hooks=hooks,
-        groups=locked_groups,
+            for req in requirements:
+                if not req.marker or req.marker.evaluate(marker_env):
+                    reqs[req.identify()] = req
+            version: str | None = dist.version
+        else:
+            version = None
+
+        node = Package(key, version, reqs)
+        if node not in graph:
+            if extras:
+                node_with_extras.add(name)
+            graph.add(node)
+            if include_sub:
+                for k in reqs:
+                    child = add_package(k, working_set.get(strip_extras(k)[0]))
+                    graph.connect(node, child)
+
+        return node
+
+    selected_map: dict[str, str] = {}
+    for key in selected or ():
+        name = key.split("[")[0]
+        if len(key) >= len(selected_map.get(name, "")):
+            # Ensure key with extras remains
+            selected_map[name] = key
+    for k, dist in working_set.items():
+        if selected is not None:
+            name = k.split("[")[0]
+            if name not in selected_map:
+                continue
+            k = selected_map[name]
+        add_package(k, dist)
+    for node in list(graph):
+        if node is not None and not list(graph.iter_parents(node)):
+            # Top requirements
+            if node.name in node_with_extras:
+                # Already included in package[extra], no need to keep the top level
+                # non-extra package.
+                graph.remove(node)
+            else:
+                graph.connect(None, node)
+    return graph
+
+
+def specifier_from_requirement(requirement: Requirement) -> str:
+    return str(requirement.specifier or "Any")
+
+
+def add_package_to_tree(
+    root: Tree,
+    graph: DirectedGraph,
+    package: Package,
+    required: str = "",
+    visited: frozenset[str] = frozenset(),
+) -> None:
+    """Format one package.
+
+    :param graph: the dependency graph
+    :param package: the package instance
+    :param required: the version required by its parent
+    :param visited: the visited package collection
+    """
+    version = (
+        "[error][ not installed ][/]"
+        if not package.version
+        else f"[error]{package.version}[/]"
+        if required and required not in ("Any", "This project") and not SpecifierSet(required).contains(package.version)
+        else f"[warning]{package.version}[/]"
     )
-    for deps in updated_deps.values():
-        _populate_requirement_names(deps)
-    if unconstrained:
-        # Need to update version constraints
-        save_version_specifiers(updated_deps, resolved, save)
-        for group, deps in updated_deps.items():
-            project.add_dependencies(deps, group, selection.dev or False)
-    if not dry_run:
-        project.write_lockfile(project.lockfile._data, False, groups=locked_groups)
-    if sync or dry_run:
-        do_sync(
-            project,
-            selection=selection,
-            clean=False,
-            dry_run=dry_run,
-            requirements=[r for deps in updated_deps.values() for r in deps.values()],
-            tracked_names=list(chain.from_iterable(updated_deps.values())) if top else None,
-            no_editable=no_editable,
-            no_self=no_self,
-            fail_fast=fail_fast,
-            hooks=hooks,
-        )
+    # escape deps with extras
+    name = package.name.replace("[", r"\[") if "[" in package.name else package.name
+    if package.name in visited:
+        version = r"[error]\[circular][/]"
+    required = f"[ required: {required} ]" if required else "[ Not required ]"
+    node = root.add(f"[req]{name}[/] {version} {required}")
+    if package.name in visited:
+        return
+    children = sorted(graph.iter_children(package), key=lambda p: p.name)
+    for child in children:
+        required = specifier_from_requirement(package.requirements[child.name])
+        add_package_to_tree(node, graph, child, required, visited | {package.name})
 
 
-def do_remove(
-    project: Project,
-    selection: GroupSelection,
-    sync: bool = True,
-    packages: Collection[str] = (),
-    no_editable: bool = False,
-    no_self: bool = False,
-    dry_run: bool = False,
-    fail_fast: bool = False,
-    hooks: HookManager | None = None,
+def add_package_to_reverse_tree(
+    root: Tree,
+    graph: DirectedGraph,
+    package: Package,
+    child: Package | None = None,
+    requires: str = "",
+    visited: frozenset[str] = frozenset(),
 ) -> None:
-    """Remove packages from working set and pyproject.toml"""
-    hooks = hooks or HookManager(project)
-    check_project_file(project)
-    if not packages:
-        raise PdmUsageError("Must specify at least one package to remove.")
-    group = selection.one()
-    lock_groups = project.lockfile.groups
-
-    deps, _ = project.get_pyproject_dependencies(group, selection.dev or False)
-    project.core.ui.echo(
-        f"Removing packages from [primary]{group}[/] "
-        f"{'dev-' if selection.dev else ''}dependencies: " + ", ".join(f"[req]{name}[/]" for name in packages)
+    """Format one package for output reverse dependency graph."""
+    version = "[error][ not installed ][/]" if not package.version else f"[warning]{package.version}[/]"
+    if package.name in visited:
+        version = r"[error]\[circular][/]"
+    requires = (
+        f"[ requires: [error]{requires}[/] ]"
+        if requires not in ("Any", "")
+        and child
+        and child.version
+        and not SpecifierSet(requires).contains(child.version)
+        else ""
+        if not requires
+        else f"[ requires: {requires} ]"
     )
-    with cd(project.root):
-        for name in packages:
-            req = parse_requirement(name)
-            matched_indexes = sorted((i for i, r in enumerate(deps) if req.matches(r)), reverse=True)
-            if not matched_indexes:
-                raise ProjectError(f"[req]{name}[/] does not exist in [primary]{group}[/] dependencies.")
-            for i in matched_indexes:
-                del deps[i]
-    cast(Array, deps).multiline(True)
-
-    if not dry_run:
-        project.pyproject.write()
-    if lock_groups and group not in lock_groups:
-        project.core.ui.echo(f"Group [success]{group}[/] isn't in lockfile, skipping lock.", style="warning", err=True)
+    name = package.name.replace("[", r"\[") if "[" in package.name else package.name
+    node = root.add(f"[req]{name}[/] {version} {requires}")
+
+    if package.name in visited:
         return
-    do_lock(project, "reuse", dry_run=dry_run, hooks=hooks, groups=lock_groups)
-    if sync:
-        do_sync(
-            project,
-            selection=GroupSelection(project, default=False, groups=[group]),
-            clean=True,
-            no_editable=no_editable,
-            no_self=no_self,
-            dry_run=dry_run,
-            fail_fast=fail_fast,
-            hooks=hooks,
-        )
+    parents: list[Package] = sorted(filter(None, graph.iter_parents(package)), key=lambda p: p.name)
+    for parent in parents:
+        requires = specifier_from_requirement(parent.requirements[package.name])
+        add_package_to_reverse_tree(node, graph, parent, package, requires, visited=visited | {package.name})
+    return
+
+
+def package_is_project(package: Package, project: Project) -> bool:
+    return project.name is not None and package.name == normalize_name(project.name)
+
+
+def _format_forward_dependency_graph(project: Project, graph: DirectedGraph) -> Tree:
+    """Format dependency graph for output."""
+    root = Tree("Dependencies", hide_root=True)
+    all_dependencies = ChainMap(*project.all_dependencies.values())
+    top_level_dependencies = sorted(graph.iter_children(None), key=lambda p: p.name)
+    for package in top_level_dependencies:
+        if package.name in all_dependencies:
+            required = specifier_from_requirement(all_dependencies[package.name])
+        elif package_is_project(package, project):
+            required = "This project"
+        else:
+            required = ""
+        add_package_to_tree(root, graph, package, required)
+    return root
 
 
-def do_use(
+def _format_reverse_dependency_graph(project: Project, graph: DirectedGraph[Package | None]) -> Tree:
+    """Format reverse dependency graph for output."""
+    root = Tree("Dependencies", hide_root=True)
+    leaf_nodes = sorted(
+        (node for node in graph if not list(graph.iter_children(node)) and node),
+        key=lambda p: p.name,
+    )
+    for package in leaf_nodes:
+        if not package:
+            continue
+        add_package_to_reverse_tree(root, graph, package)
+    return root
+
+
+def build_forward_dependency_json_subtree(
+    root: Package,
     project: Project,
-    python: str = "",
-    first: bool = False,
-    ignore_remembered: bool = False,
-    ignore_requires_python: bool = False,
-    save: bool = True,
-    venv: str | None = None,
-    hooks: HookManager | None = None,
-) -> PythonInfo:
-    """Use the specified python version and save in project config.
-    The python can be a version string or interpreter path.
-    """
-    from pdm.cli.commands.venv.utils import get_venv_with_name
-    from pdm.models.caches import JSONFileCache
+    graph: DirectedGraph[Package | None],
+    required_by: Package | None = None,
+    visited: frozenset[str] = frozenset(),
+) -> dict:
+    if not package_is_project(root, project):
+        requirements = required_by.requirements if required_by else ChainMap(*project.all_dependencies.values())
+        if root.name in requirements:
+            required = specifier_from_requirement(requirements[root.name])
+        else:
+            required = "Not required"
+    else:
+        required = "This project"
 
-    def version_matcher(py_version: PythonInfo) -> bool:
-        return py_version.valid and (
-            ignore_requires_python or project.python_requires.contains(str(py_version.version), True)
-        )
+    children = graph.iter_children(root) if root.name not in visited else []
 
-    hooks = hooks or HookManager(project)
+    return OrderedDict(
+        package=root.name,
+        version=root.version,
+        required=required,
+        dependencies=sorted(
+            (
+                build_forward_dependency_json_subtree(p, project, graph, root, visited | {root.name})
+                for p in children
+                if p
+            ),
+            key=lambda d: d["package"],
+        ),
+    )
 
-    selected_python: PythonInfo | None = None
-    if venv:
-        virtualenv = get_venv_with_name(project, venv)
-        selected_python = PythonInfo.from_path(virtualenv.interpreter)
-
-    if not project.cache_dir.exists():
-        project.cache_dir.mkdir(parents=True)
-    use_cache: JSONFileCache[str, str] = JSONFileCache(project.cache_dir / "use_cache.json")
-    if python:
-        python = python.strip()
-    if selected_python is None and python and not ignore_remembered:
-        if python in use_cache:
-            path = use_cache.get(python)
-            cached_python = PythonInfo.from_path(path)
-            if not cached_python.valid:
-                project.core.ui.echo(
-                    f"The last selection is corrupted. {path!r}",
-                    style="error",
-                    err=True,
-                )
-            elif version_matcher(cached_python):
-                project.core.ui.echo(
-                    "Using the last selection, add '-i' to ignore it.",
-                    style="warning",
-                    err=True,
-                )
-                selected_python = cached_python
 
-    if selected_python is None:
-        found_interpreters = list(dict.fromkeys(project.find_interpreters(python)))
-        matching_interpreters = list(filter(version_matcher, found_interpreters))
-        if not found_interpreters:
-            raise NoPythonVersion(f"No Python interpreter matching [success]{python}[/] is found.")
-        if not matching_interpreters:
-            project.core.ui.echo("Interpreters found but not matching:", err=True)
-            for py in found_interpreters:
-                info = py.identifier if py.valid else "Invalid"
-                project.core.ui.echo(f"  - {py.path} ({info})", err=True)
-            raise NoPythonVersion(
-                f"No python is found meeting the requirement [success]python {project.python_requires!s}[/]"
-            )
-        if first or len(matching_interpreters) == 1:
-            selected_python = matching_interpreters[0]
-        else:
-            project.core.ui.echo("Please enter the Python interpreter to use")
-            for i, py_version in enumerate(matching_interpreters):
-                project.core.ui.echo(f"{i}. [success]{py_version.path!s}[/] ({py_version.identifier})")
-            selection = termui.ask(
-                "Please select",
-                default="0",
-                prompt_type=int,
-                choices=[str(i) for i in range(len(matching_interpreters))],
-                show_choices=False,
-            )
-            selected_python = matching_interpreters[int(selection)]
-        if python:
-            use_cache.set(python, selected_python.path.as_posix())
-
-    if not save:
-        return selected_python
-    saved_python = project._saved_python
-    old_python = PythonInfo.from_path(saved_python) if saved_python else None
-    project.core.ui.echo(
-        f"Using Python interpreter: [success]{selected_python.path!s}[/] ({selected_python.identifier})"
+def build_reverse_dependency_json_subtree(
+    root: Package,
+    project: Project,
+    graph: DirectedGraph[Package | None],
+    requires: Package | None = None,
+    visited: frozenset[str] = frozenset(),
+) -> dict:
+    parents = graph.iter_parents(root) if root.name not in visited else []
+    return OrderedDict(
+        package=root.name,
+        version=root.version,
+        requires=specifier_from_requirement(root.requirements[requires.name]) if requires else None,
+        dependents=sorted(
+            (
+                build_reverse_dependency_json_subtree(p, project, graph, root, visited | {root.name})
+                for p in parents
+                if p
+            ),
+            key=lambda d: d["package"],
+        ),
     )
-    project.python = selected_python
-    if project.environment.is_local:
-        project.core.ui.echo(
-            "Using __pypackages__ because non-venv Python is used.",
-            style="primary",
-            err=True,
+
+
+def build_dependency_json_tree(project: Project, graph: DirectedGraph[Package | None], reverse: bool) -> list[dict]:
+    if reverse:
+        top_level_packages = filter(lambda n: not list(graph.iter_children(n)), graph)  # leaf nodes
+        build_dependency_json_subtree: Callable = build_reverse_dependency_json_subtree
+    else:
+        top_level_packages = graph.iter_children(None)  # root nodes
+        build_dependency_json_subtree = build_forward_dependency_json_subtree
+    return [
+        build_dependency_json_subtree(p, project, graph)
+        for p in sorted(top_level_packages, key=lambda p: p.name if p else "")
+        if p
+    ]
+
+
+def show_dependency_graph(
+    project: Project,
+    graph: DirectedGraph[Package | None],
+    reverse: bool = False,
+    json: bool = False,
+) -> None:
+    echo = project.core.ui.echo
+    if json:
+        echo(
+            dumps(
+                build_dependency_json_tree(project, graph, reverse),
+                indent=2,
+            )
         )
-    if (
-        old_python
-        and old_python.executable != selected_python.executable
-        and isinstance(project.environment, PythonLocalEnvironment)
-    ):
-        project.core.ui.echo("Updating executable scripts...", style="primary")
-        project.environment.update_shebangs(selected_python.executable.as_posix())
-    hooks.try_emit("post_use", python=selected_python)
-    return selected_python
+        return
+
+    if reverse:
+        tree = _format_reverse_dependency_graph(project, graph)
+    else:
+        tree = _format_forward_dependency_graph(project, graph)
+    echo(tree)
 
 
-def do_import(
+def format_lockfile(
     project: Project,
-    filename: str,
-    format: str | None = None,
-    options: Namespace | None = None,
+    mapping: dict[str, Candidate],
+    fetched_dependencies: dict[tuple[str, str | None], list[Requirement]],
+) -> dict:
+    """Format lock file from a dict of resolved candidates, a mapping of dependencies
+    and a collection of package summaries.
+    """
+    from pdm.formats.base import make_array, make_inline_table
+
+    packages = tomlkit.aot()
+    file_hashes = tomlkit.table()
+    for k, v in sorted(mapping.items()):
+        base = tomlkit.table()
+        base.update(v.as_lockfile_entry(project.root))
+        base.add("summary", v.summary or "")
+        deps = make_array(sorted(r.as_line() for r in fetched_dependencies[v.dep_key]), True)
+        if len(deps) > 0:
+            base.add("dependencies", deps)
+        packages.append(base)
+        if v.hashes:
+            key = f"{strip_extras(k)[0]} {v.version}"
+            if key in file_hashes:
+                continue
+            array = tomlkit.array().multiline(True)
+            for link, hash_value in sorted(v.hashes.items(), key=lambda l_h: (l_h[0].url_without_fragment, l_h[1])):
+                inline = make_inline_table({"url": link.url_without_fragment, "hash": hash_value})
+                array.append(inline)
+            if array:
+                file_hashes.add(key, array)
+    doc = tomlkit.document()
+    doc.add("package", packages)
+    metadata = tomlkit.table()
+    metadata.add("files", file_hashes)
+    doc.add("metadata", metadata)
+    return cast(dict, doc)
+
+
+def save_version_specifiers(
+    requirements: dict[str, dict[str, Requirement]],
+    resolved: dict[str, Candidate],
+    save_strategy: str,
 ) -> None:
-    """Import project metadata from given file.
+    """Rewrite the version specifiers according to the resolved result and save strategy
 
-    :param project: the project instance
-    :param filename: the file name
-    :param format: the file format, or guess if not given.
-    :param options: other options parsed to the CLI.
+    :param requirements: the requirements to be updated
+    :param resolved: the resolved mapping
+    :param save_strategy: compatible/wildcard/exact
     """
+
+    def candidate_version(c: Candidate) -> Version:
+        assert c.version is not None
+        return comparable_version(c.version)
+
+    for reqs in requirements.values():
+        for name, r in reqs.items():
+            if r.is_named and not r.specifier:
+                if save_strategy == "exact":
+                    r.specifier = get_specifier(f"=={candidate_version(resolved[name])}")
+                elif save_strategy == "compatible":
+                    version = candidate_version(resolved[name])
+                    if version.is_prerelease or version.is_devrelease:
+                        r.specifier = get_specifier(f">={version},<{version.major + 1}")
+                    else:
+                        r.specifier = get_specifier(f"~={version.major}.{version.minor}")
+                elif save_strategy == "minimum":
+                    r.specifier = get_specifier(f">={candidate_version(resolved[name])}")
+
+
+def check_project_file(project: Project) -> None:
+    """Check the existence of the project file and throws an error on failure."""
+    if not project.pyproject.is_valid:
+        raise ProjectError(
+            "The pyproject.toml has not been initialized yet. You can do this by running [success]`pdm init`[/]."
+        ) from None
+
+
+def find_importable_files(project: Project) -> Iterable[tuple[str, Path]]:
+    """Find all possible files that can be imported"""
     from pdm.formats import FORMATS
 
-    if not format:
-        for key in FORMATS:
-            if FORMATS[key].check_fingerprint(project, filename):
-                break
+    for filename in (
+        "Pipfile",
+        "pyproject.toml",
+        "requirements.in",
+        "requirements.txt",
+        "setup.py",
+    ):
+        project_file = project.root / filename
+        if not project_file.exists():
+            continue
+        for key, module in FORMATS.items():
+            if module.check_fingerprint(project, project_file.as_posix()):
+                yield key, project_file
+
+
+@no_type_check
+def set_env_in_reg(env_name: str, value: str) -> None:
+    """Manipulate the WinReg, and add value to the
+    environment variable if exists or create new.
+    """
+    import winreg
+
+    value = os.path.normcase(value)
+
+    with winreg.ConnectRegistry(None, winreg.HKEY_CURRENT_USER) as root:
+        with winreg.OpenKey(root, "Environment", 0, winreg.KEY_ALL_ACCESS) as env_key:
+            try:
+                old_value, type_ = winreg.QueryValueEx(env_key, env_name)
+                paths = [os.path.normcase(item) for item in old_value.split(os.pathsep)]
+                if value in paths:
+                    return
+            except FileNotFoundError:
+                paths, type_ = [], winreg.REG_EXPAND_SZ
+            new_value = os.pathsep.join([value, *paths])
+            winreg.SetValueEx(env_key, env_name, 0, type_, new_value)
+
+
+def format_resolution_impossible(err: ResolutionImpossible) -> str:
+    from pdm.resolver.python import PythonRequirement
+
+    causes: list[RequirementInformation] = err.causes
+    info_lines: set[str] = set()
+    if all(isinstance(cause.requirement, PythonRequirement) for cause in causes):
+        project_requires: PythonRequirement = next(cause.requirement for cause in causes if cause.parent is None)
+        pyspec = cast(PySpecSet, project_requires.specifier)
+        conflicting = [
+            cause
+            for cause in causes
+            if cause.parent is not None and not cause.requirement.specifier.is_superset(pyspec)
+        ]
+        result = [
+            "Unable to find a resolution because the following dependencies don't work "
+            "on all Python versions in the range of the project's `requires-python`: "
+            f"[success]{pyspec}[/]."
+        ]
+        for req, parent in conflicting:
+            pyspec &= req.specifier
+            info_lines.add(f"  {req.as_line()} (from {parent!r})")
+        result.extend(sorted(info_lines))
+        if pyspec.is_impossible:
+            result.append("Consider changing the version specifiers of the dependencies to be compatible")
         else:
-            raise PdmUsageError(
-                "Can't derive the file format automatically, please specify it via '-f/--format' option."
+            result.append(
+                "A possible solution is to change the value of `requires-python` "
+                f"in pyproject.toml to [success]{pyspec}[/]."
             )
-    else:
-        key = format
-    if options is None:
-        options = Namespace(dev=False, group=None)
-    project_data, settings = FORMATS[key].convert(project, filename, options)
-    pyproject = project.pyproject._data
-
-    if "tool" not in pyproject or "pdm" not in pyproject["tool"]:
-        pyproject.setdefault("tool", {})["pdm"] = tomlkit.table()
-    if "build" in pyproject["tool"]["pdm"] and isinstance(pyproject["tool"]["pdm"]["build"], str):
-        pyproject["tool"]["pdm"]["build"] = {
-            "setup-script": pyproject["tool"]["pdm"]["build"],
-            "run-setuptools": True,
-        }
-    if "project" not in pyproject:
-        pyproject.add("project", tomlkit.table())
-        pyproject["project"].add(tomlkit.comment("PEP 621 project metadata"))
-        pyproject["project"].add(tomlkit.comment("See https://www.python.org/dev/peps/pep-0621/"))
-
-    merge_dictionary(pyproject["project"], project_data)
-    merge_dictionary(pyproject["tool"]["pdm"], settings)
-    pyproject.setdefault("build-system", DEFAULT_BACKEND.build_system())
-
-    if "requires-python" not in pyproject["project"]:
-        python_version = f"{project.python.major}.{project.python.minor}"
-        pyproject["project"]["requires-python"] = f">={python_version}"
-        project.core.ui.echo(
-            "The project's [primary]requires-python[/] has been set to [primary]>="
-            f"{python_version}[/]. You can change it later if necessary."
-        )
-    project.pyproject.write()
+        return "\n".join(result)
 
+    if len(causes) == 1:
+        return (
+            "Unable to find a resolution for "
+            f"[success]{causes[0].requirement.identify()}[/]\n"
+            "Please make sure the package name is correct."
+        )
 
-def ask_for_import(project: Project) -> None:
-    """Show possible importable files and ask user to decide"""
-    importable_files = list(find_importable_files(project))
-    if not importable_files:
-        return
-    project.core.ui.echo("Found following files from other formats that you may import:", style="primary")
-    for i, (key, filepath) in enumerate(importable_files):
-        project.core.ui.echo(f"{i}. [success]{filepath.as_posix()}[/] ({key})")
-    project.core.ui.echo(f"{len(importable_files)}. [warning]don't do anything, I will import later.[/]")
-    choice = termui.ask(
-        "Please select",
-        prompt_type=int,
-        choices=[str(i) for i in range(len(importable_files) + 1)],
-        show_choices=False,
+    result = [
+        "Unable to find a resolution for "
+        f"[success]{causes[0].requirement.identify()}[/]\n"
+        "because of the following conflicts:"
+    ]
+    for req, parent in causes:
+        info_lines.add(f"  {req.as_line()} (from {parent if parent else 'project'})")
+    result.extend(sorted(info_lines))
+    result.append(
+        "To fix this, you could loosen the dependency version constraints in "
+        "pyproject.toml. See https://pdm.fming.dev/latest/usage/dependency/"
+        "#solve-the-locking-failure for more details."
     )
-    if int(choice) == len(importable_files):
-        return
-    key, filepath = importable_files[int(choice)]
-    do_import(project, str(filepath), key)
+    return "\n".join(result)
 
 
-def print_pep582_command(project: Project, shell: str = "AUTO") -> None:
-    """Print the export PYTHONPATH line to be evaluated by the shell."""
-    import shellingham
+def merge_dictionary(target: MutableMapping[Any, Any], input: Mapping[Any, Any]) -> None:
+    """Merge the input dict with the target while preserving the existing values
+    properly. This will update the target dictionary in place.
+    List values will be extended, but only if the value is not already in the list.
+    """
+    for key, value in input.items():
+        if key not in target:
+            target[key] = value
+        elif isinstance(value, dict):
+            merge_dictionary(target[key], value)
+        elif isinstance(value, list):
+            target[key].extend(x for x in value if x not in target[key])
+            target[key].multiline(True)  # type: ignore[attr-defined]
+        else:
+            target[key] = value
 
-    pep582_path = get_pep582_path(project)
-    ui = project.core.ui
 
-    if os.name == "nt":
-        try:
-            set_env_in_reg("PYTHONPATH", pep582_path)
-        except PermissionError:
-            ui.echo(
-                "Permission denied, please run the terminal as administrator.",
-                style="error",
-                err=True,
-            )
-        ui.echo(
-            "The environment variable has been saved, please restart the session to take effect.",
-            style="success",
-        )
-        return
-    lib_path = pep582_path.replace("'", "\\'")
-    if shell == "AUTO":
-        shell = shellingham.detect_shell()[0]
-    shell = shell.lower()
-    if shell in ("zsh", "bash", "sh", "dash"):
-        result = textwrap.dedent(
-            f"""
-            if [ -n "$PYTHONPATH" ]; then
-                export PYTHONPATH='{lib_path}':$PYTHONPATH
-            else
-                export PYTHONPATH='{lib_path}'
-            fi
-            """
-        ).strip()
-    elif shell == "fish":
-        result = f"set -x PYTHONPATH '{lib_path}' $PYTHONPATH"
-    elif shell in ("tcsh", "csh"):
-        result = textwrap.dedent(
-            f"""
-            if ( $?PYTHONPATH ) then
-                if ( "$PYTHONPATH" != "" ) then
-                    setenv PYTHONPATH '{lib_path}':$PYTHONPATH
-                else
-                    setenv PYTHONPATH '{lib_path}'
-                endif
-            else
-                setenv PYTHONPATH '{lib_path}'
-            endif
-            """
-        ).strip()
-    else:
-        raise PdmUsageError(f"Unsupported shell: {shell}, please specify another shell via `--pep582 <SHELL>`")
-    ui.echo(result)
+def fetch_hashes(repository: BaseRepository, mapping: Mapping[str, Candidate]) -> None:
+    """Fetch hashes for candidates in parallel"""
 
+    def do_fetch(candidate: Candidate) -> None:
+        candidate.hashes = repository.get_hashes(candidate)
 
-def get_latest_pdm_version_from_pypi(project: Project, prereleases: bool = False) -> str | None:
-    """Get the latest version of PDM from PyPI."""
-    environment = BareEnvironment(project)
-    with environment.get_finder([project.default_source]) as finder:
-        candidate = finder.find_best_match("pdm", allow_prereleases=prereleases).best
-    return cast(str, candidate.version) if candidate else None
-
-
-def get_latest_version(project: Project) -> str | None:
-    """Get the latest version of PDM from PyPI, cache for 7 days"""
-    cache_key = hashlib.sha224(sys.executable.encode()).hexdigest()
-    cache_file = project.cache("self-check") / cache_key
-    state = {}
-    with contextlib.suppress(OSError):
-        state = json.loads(cache_file.read_text())
-    current_time = datetime.datetime.utcnow().timestamp()
-    if state.get("last-check") and current_time - state["last-check"] < 60 * 60 * 24 * 7:
-        return cast(str, state["latest-version"])
-    try:
-        latest_version = get_latest_pdm_version_from_pypi(project)
-    except Exception as e:
-        warnings.warn(f"Failed to get latest version: {e}", RuntimeWarning, stacklevel=1)
-        latest_version = None
-    if latest_version is None:
-        return None
-    state.update({"latest-version": latest_version, "last-check": current_time})
-    with contextlib.suppress(OSError):
-        cache_file.write_text(json.dumps(state))
-    return latest_version
+    with ThreadPoolExecutor() as executor:
+        executor.map(do_fetch, mapping.values())
 
 
-def check_update(project: Project) -> None:
-    """Check if there is a new version of PDM available"""
-    from packaging.version import Version
+def is_pipx_installation() -> bool:
+    return sys.prefix.split(os.sep)[-3:-1] == ["pipx", "venvs"]
 
-    from pdm.cli.utils import is_homebrew_installation, is_pipx_installation, is_scoop_installation
 
-    this_version = project.core.version
-    latest_version = get_latest_version(project)
-    if latest_version is None or Version(this_version) >= Version(latest_version):
-        return
-    disable_command = "pdm config check_update false"
+def is_homebrew_installation() -> bool:
+    return "/libexec" in sys.prefix.replace("\\", "/")
 
-    is_prerelease = Version(latest_version).is_prerelease
 
-    if is_pipx_installation():
-        install_command = f"pipx upgrade {'--pip-args=--pre ' if is_prerelease else ''}pdm"
-    elif is_homebrew_installation():
-        install_command = "brew upgrade pdm"
-    elif is_scoop_installation():
-        install_command = "scoop update pdm"
-    else:
-        install_command = "pdm self update" + (" --pre" if is_prerelease else "")
-        if os.name == "nt":
-            # On Windows, the executable can't replace itself, we add the python prefix to the command
-            # A bit ugly but it works
-            install_command = f"{sys.executable} -m {install_command}"
-
-    message = [
-        f"\nPDM [primary]{this_version}[/]",
-        f" is installed, while [primary]{latest_version}[/]",
-        " is available.\n",
-        f"Please run [req]`{install_command}`[/]",
-        " to upgrade.\n",
-        f"Run [req]`{disable_command}`[/]",
-        " to disable the check.",
-    ]
-    project.core.ui.echo("".join(message), err=True, style="info")
+def is_scoop_installation() -> bool:
+    return os.name == "nt" and is_path_relative_to(sys.prefix, Path.home() / "scoop/apps/pdm")
+
+
+def get_dist_location(dist: Distribution) -> str:
+    direct_url = dist.read_text("direct_url.json")
+    if not direct_url:
+        return ""
+    direct_url_data = json.loads(direct_url)
+    url = cast(str, direct_url_data["url"])
+    if url.startswith("file:"):
+        path = url_to_path(url)
+        editable = direct_url_data.get("dir_info", {}).get("editable", False)
+        return f"{'-e ' if editable else ''}{path}"
+    return ""
+
+
+def get_pep582_path(project: Project) -> str:
+    from pdm.compat import resources_open_binary
+
+    script_dir = Path(__file__).parent.parent / "pep582"
+    if script_dir.exists():
+        return str(script_dir)
+
+    script_dir = project.global_config.config_file.parent / "pep582"
+    if script_dir.joinpath("sitecustomize.py").exists():
+        return str(script_dir)
+    script_dir.mkdir(parents=True, exist_ok=True)
+    with resources_open_binary("pdm.pep582", "sitecustomize.py") as f:
+        script_dir.joinpath("sitecustomize.py").write_bytes(f.read())
+    return str(script_dir)
+
+
+def use_venv(project: Project, name: str) -> None:
+    from pdm.cli.commands.venv.utils import get_venv_with_name
+    from pdm.environments import PythonEnvironment
+
+    venv = get_venv_with_name(project, cast(str, name))
+    project.core.ui.echo(
+        f"In virtual environment: [success]{venv.root}[/]", err=True, style="info", verbosity=termui.Verbosity.DETAIL
+    )
+    project.environment = PythonEnvironment(project, python=str(venv.interpreter))
+
+
+def populate_requirement_names(req_mapping: dict[str, Requirement]) -> None:
+    # Update the requirement key if the name changed.
+    for key, req in list(req_mapping.items()):
+        if key and key.startswith(":empty:"):
+            req_mapping[req.identify()] = req
+            del req_mapping[key]
```

### Comparing `pdm-2.7.1/src/pdm/cli/commands/base.py` & `pdm-2.7.2/src/pdm/cli/commands/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 from __future__ import annotations
 
 import argparse
 from argparse import _SubParsersAction
-from typing import Any
+from typing import Any, TypeVar
 
 from pdm.cli.options import Option, global_option, project_option, verbose_option
 from pdm.project import Project
 
+C = TypeVar("C", bound="BaseCommand")
+
 
 class BaseCommand:
     """A CLI subcommand"""
 
     # The subcommand's name
     name: str | None = None
     # The subcommand's help string, if not given, __doc__ will be used.
     description: str | None = None
     # A list of pre-defined options which will be loaded on initializing
     # Rewrite this if you don't want the default ones
     arguments: list[Option] = [verbose_option, global_option, project_option]
 
-    def __init__(self, parser: argparse.ArgumentParser) -> None:
-        for arg in self.arguments:
+    def __init__(self, parser: argparse.ArgumentParser | None = None) -> None:
+        """For compatibility, the parser is optional and won't be used."""
+
+    @classmethod
+    def init_parser(cls: type[C], parser: argparse.ArgumentParser) -> C:
+        cmd = cls()
+        for arg in cmd.arguments:
             arg.add_to_parser(parser)
-        self.add_arguments(parser)
+        cmd.add_arguments(parser)
+        return cmd
 
     @classmethod
     def register_to(cls, subparsers: _SubParsersAction, name: str | None = None, **kwargs: Any) -> None:
         """Register a subcommand to the subparsers,
         with an optional name of the subcommand.
         """
         help_text = cls.description or cls.__doc__
@@ -37,15 +45,15 @@
         subactions[:] = [action for action in subactions if action.dest != name]
         parser = subparsers.add_parser(
             name,
             description=help_text,
             help=help_text,
             **kwargs,
         )
-        command = cls(parser)
+        command = cls.init_parser(parser)
         command.name = name
         # Store the command instance in the parsed args. See pdm/core.py for more details
         parser.set_defaults(command=command)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         """Manipulate the argument parser to add more arguments"""
         pass
```

### Comparing `pdm-2.7.1/src/pdm/cli/commands/build.py` & `pdm-2.7.2/src/pdm/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/cache.py` & `pdm-2.7.2/src/pdm/cli/commands/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class Command(BaseCommand):
     """Control the caches of PDM"""
 
     arguments = [verbose_option]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        subparsers = parser.add_subparsers(title="Sub commands")
+        subparsers = parser.add_subparsers(title="commands", metavar="cache")
         ClearCommand.register_to(subparsers, "clear")
         RemoveCommand.register_to(subparsers, "remove")
         ListCommand.register_to(subparsers, "list")
         InfoCommand.register_to(subparsers, "info")
         parser.set_defaults(search_parent=False)
         self.parser = parser
```

### Comparing `pdm-2.7.1/src/pdm/cli/commands/completion.py` & `pdm-2.7.2/src/pdm/cli/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/config.py` & `pdm-2.7.2/src/pdm/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/export.py` & `pdm-2.7.2/src/pdm/cli/commands/export.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
             help="Write output to the given file, or print to stdout if not given",
         )
         parser.add_argument(
             "--pyproject",
             action="store_true",
             help="Read the list of packages from pyproject.toml",
         )
+        parser.add_argument("--expandvars", action="store_true", help="Expand environment variables in requirements")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         if options.pyproject:
             options.hashes = False
         selection = GroupSelection.from_options(project, options)
         requirements: dict[str, Requirement] = {}
         packages: Iterable[Requirement] | Iterable[Candidate]
```

### Comparing `pdm-2.7.1/src/pdm/cli/commands/fix/__init__.py` & `pdm-2.7.2/src/pdm/cli/commands/fix/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/fix/fixers.py` & `pdm-2.7.2/src/pdm/cli/commands/fix/fixers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/info.py` & `pdm-2.7.2/src/pdm/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/init.py` & `pdm-2.7.2/src/pdm/cli/commands/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 if TYPE_CHECKING:
     from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Initialize a pyproject.toml for PDM"""
 
-    def __init__(self, parser: argparse.ArgumentParser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
         self.interactive = True
 
     @staticmethod
     def do_init(
         project: Project,
         name: str = "",
         version: str = "",
@@ -108,48 +107,52 @@
         )
         parser.add_argument("--python", help="Specify the Python version/path to use")
         parser.add_argument("--backend", choices=list(_BACKENDS), help="Specify the build backend")
         parser.add_argument("--lib", action="store_true", help="Create a library project")
         parser.set_defaults(search_parent=False)
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
+        from pdm.cli.commands.use import Command as UseCommand
+
         hooks = HookManager(project, options.skip)
         if project.pyproject.exists():
             project.core.ui.echo("pyproject.toml already exists, update it now.", style="primary")
         else:
             project.core.ui.echo("Creating a pyproject.toml for PDM...", style="primary")
         self.set_interactive(not options.non_interactive)
-
+        do_use = UseCommand().do_use
         if self.interactive:
-            python = actions.do_use(
+            python = do_use(
                 project,
                 options.python or "",
                 first=bool(options.python),
                 ignore_remembered=True,
                 ignore_requires_python=True,
+                save=False,
                 hooks=hooks,
             )
         else:
-            python = actions.do_use(
+            python = do_use(
                 project,
                 options.python or "3",
                 first=True,
                 ignore_remembered=True,
                 ignore_requires_python=True,
                 save=False,
                 hooks=hooks,
             )
         if project.config["python.use_venv"] and python.get_venv() is None:
             if not self.interactive or termui.confirm(
                 f"Would you like to create a virtualenv with [success]{python.executable}[/]?",
                 default=True,
             ):
+                project._python = python
                 try:
                     path = project._create_virtualenv()
-                    python = project.python = PythonInfo.from_path(get_venv_python(path))
+                    python = PythonInfo.from_path(get_venv_python(path))
                 except Exception as e:  # pragma: no cover
                     project.core.ui.echo(
                         f"Error occurred when creating virtualenv: {e}\nPlease fix it and create later.",
                         style="error",
                         err=True,
                     )
         if python.get_venv() is None:
@@ -192,14 +195,15 @@
         license = self.ask("License(SPDX name)", "MIT")
 
         git_user, git_email = get_user_email_from_git()
         author = self.ask("Author name", git_user)
         email = self.ask("Author email", git_email)
         python_version = f"{python.major}.{python.minor}"
         python_requires = self.ask("Python requires('*' to allow any)", f">={python_version}")
+        project.python = python
 
         self.do_init(
             project,
             name=name,
             version=version,
             description=description,
             license=license,
```

### Comparing `pdm-2.7.1/src/pdm/cli/commands/install.py` & `pdm-2.7.2/src/pdm/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/list.py` & `pdm-2.7.2/src/pdm/cli/commands/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         ui = project.core.ui
 
         # Order based on a field key.
         if options.sort:
             keys = parse_comma_separated_string(options.sort)
             if not all(key in Listable.KEYS for key in keys):
                 raise PdmUsageError(f"--sort key must be one of: {','.join(Listable.KEYS)}")
-            records.sort(key=lambda d: tuple(d[key] for key in keys))
+            records.sort(key=lambda d: tuple(d[key].casefold() for key in keys))
 
         # Write CSV
         if options.csv:
             buffer = io.StringIO()
             writer = csv.DictWriter(buffer, fieldnames=fields)
             writer.writeheader()
             for row in records:
```

### Comparing `pdm-2.7.1/src/pdm/cli/commands/lock.py` & `pdm-2.7.2/src/pdm/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/publish/__init__.py` & `pdm-2.7.2/src/pdm/cli/commands/publish/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/publish/package.py` & `pdm-2.7.2/src/pdm/cli/commands/publish/package.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/publish/repository.py` & `pdm-2.7.2/src/pdm/cli/commands/publish/repository.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/run.py` & `pdm-2.7.2/src/pdm/cli/commands/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
             if re.search(r"\(.*?\)", func) is None:
                 func += "()"
             args = ["python", "-c", f"import sys, {module} as {short_name};sys.exit({short_name}.{func})", *list(args)]
         elif kind == "composite":
             assert isinstance(value, list)
 
         self.project.core.ui.echo(
-            f"Running {task}: [success]{str(args)}[/]",
+            f"Running {task}: [success]{args}[/]",
             err=True,
             verbosity=termui.Verbosity.DETAIL,
         )
         if kind == "composite":
             args = list(args)
             should_interpolate = any(RE_ARGS_PLACEHOLDER.search(script) for script in value)
             code = 0
@@ -347,15 +347,15 @@
         )
         action.add_argument(
             "-j",
             "--json",
             action="store_true",
             help="Output all scripts infos in JSON",
         )
-        exec = action.add_argument_group("execution", "Execution parameters")
+        exec = parser.add_argument_group("Execution parameters")
         exec.add_argument(
             "-s",
             "--site-packages",
             action="store_true",
             help="Load site-packages from the selected interpreter",
         )
         exec.add_argument("script", nargs="?", help="The command to run")
```

### Comparing `pdm-2.7.1/src/pdm/cli/commands/search.py` & `pdm-2.7.2/src/pdm/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/self_cmd.py` & `pdm-2.7.2/src/pdm/cli/commands/self_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         subparsers: argparse._SubParsersAction,
         name: str | None = None,
         **kwargs: Any,
     ) -> None:
         return super().register_to(subparsers, name, aliases=["plugin"], **kwargs)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        subparsers = parser.add_subparsers(title="Sub commands")
+        subparsers = parser.add_subparsers(title="commands", metavar="self")
         ListCommand.register_to(subparsers)
         if not is_in_zipapp():
             AddCommand.register_to(subparsers)
             RemoveCommand.register_to(subparsers)
             UpdateCommand.register_to(subparsers)
         parser.set_defaults(search_parent=False)
         self.parser = parser
@@ -233,15 +233,15 @@
         else:
             version = get_latest_pdm_version_from_pypi(project, options.pre)
             assert version is not None, "No version found"
             if parse(__version__) >= parse(version):
                 project.core.ui.echo(f"Already up-to-date: [primary]{__version__}[/]")
                 return
             package = f"pdm=={version}"
-        pip_args = ["install", "--upgrade", *shlex.split(options.pip_args)] + [package]
+        pip_args = ["install", "--upgrade", *shlex.split(options.pip_args), package]
         project.core.ui.echo(f"Running pip command: {pip_args}", verbosity=termui.Verbosity.DETAIL)
         try:
             with project.core.ui.open_spinner(f"Updating pdm to version [primary]{version}[/]"):
                 run_pip(project, pip_args)
         except subprocess.CalledProcessError as e:
             project.core.ui.echo(
                 f"[error]Installing version [primary]{version}[/] failed:[/]\n" + e.output,
```

### Comparing `pdm-2.7.1/src/pdm/cli/commands/show.py` & `pdm-2.7.2/src/pdm/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/sync.py` & `pdm-2.7.2/src/pdm/cli/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/update.py` & `pdm-2.7.2/src/pdm/cli/commands/venv/purge.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,63 @@
 import argparse
+import shutil
 
-from pdm.cli import actions
-from pdm.cli.commands.base import BaseCommand
-from pdm.cli.filters import GroupSelection
-from pdm.cli.hooks import HookManager
-from pdm.cli.options import (
-    groups_group,
-    install_group,
-    lockfile_option,
-    prerelease_option,
-    save_strategy_group,
-    skip_option,
-    unconstrained_option,
-    update_strategy_group,
-    venv_option,
-)
 from pdm.project import Project
+from pdm import termui
+from pdm.cli.commands.base import BaseCommand
+from pdm.cli.commands.venv.utils import iter_central_venvs
+from pdm.cli.options import verbose_option
 
 
-class Command(BaseCommand):
-    """Update package(s) in pyproject.toml"""
+class PurgeCommand(BaseCommand):
+    """Purge selected/all created Virtualenvs"""
 
-    arguments = [
-        *BaseCommand.arguments,
-        groups_group,
-        install_group,
-        lockfile_option,
-        save_strategy_group,
-        update_strategy_group,
-        prerelease_option,
-        unconstrained_option,
-        skip_option,
-        venv_option,
-    ]
+    arguments = [verbose_option]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
-            "-t",
-            "--top",
+            "-f",
+            "--force",
             action="store_true",
-            help="Only update those listed in pyproject.toml",
+            help="Force purging without prompting for confirmation",
         )
         parser.add_argument(
-            "--dry-run",
-            "--outdated",
+            "-i",
+            "--interactive",
             action="store_true",
-            dest="dry_run",
-            help="Show the difference only without modifying the lockfile content",
+            help="Interactively purge selected Virtualenvs",
         )
-        parser.add_argument(
-            "--no-sync",
-            dest="sync",
-            default=True,
-            action="store_false",
-            help="Only update lock file but do not sync packages",
-        )
-        parser.add_argument("packages", nargs="*", help="If packages are given, only update them")
-        parser.set_defaults(dev=None)
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
-        actions.do_update(
-            project,
-            selection=GroupSelection.from_options(project, options),
-            save=options.save_strategy or project.config["strategy.save"],
-            strategy=options.update_strategy or project.config["strategy.update"],
-            unconstrained=options.unconstrained,
-            top=options.top,
-            dry_run=options.dry_run,
-            packages=options.packages,
-            sync=options.sync,
-            no_editable=options.no_editable,
-            no_self=options.no_self,
-            prerelease=options.prerelease,
-            fail_fast=options.fail_fast,
-            hooks=HookManager(project, options.skip),
+        all_central_venvs = list(iter_central_venvs(project))
+        if not all_central_venvs:
+            project.core.ui.echo("No virtualenvs to purge, quitting.", style="success")
+            return
+
+        if not options.force:
+            project.core.ui.echo("The following Virtualenvs will be purged:", style="error")
+            for i, venv in enumerate(all_central_venvs):
+                project.core.ui.echo(f"{i}. [success]{venv[0]}[/]")
+
+        if not options.interactive:
+            if options.force or termui.confirm("continue?", default=True):
+                return self.del_all_venvs(project)
+
+        selection = termui.ask(
+            "Please select",
+            choices=([str(i) for i in range(len(all_central_venvs))] + ["all", "none"]),
+            default="none",
+            show_choices=False,
         )
+
+        if selection == "all":
+            self.del_all_venvs(project)
+        elif selection != "none":
+            for i, venv in enumerate(all_central_venvs):
+                if i == int(selection):
+                    shutil.rmtree(venv[1])
+            project.core.ui.echo("Purged successfully!")
+
+    def del_all_venvs(self, project: Project) -> None:
+        for _, venv in iter_central_venvs(project):
+            shutil.rmtree(venv)
+        project.core.ui.echo("Purged successfully!")
```

### Comparing `pdm-2.7.1/src/pdm/cli/commands/use.py` & `pdm-2.7.2/src/pdm/cli/commands/venv/remove.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 import argparse
+import shutil
+from pathlib import Path
 
-from pdm.cli import actions
+from pdm import termui
 from pdm.cli.commands.base import BaseCommand
-from pdm.cli.hooks import HookManager
-from pdm.cli.options import skip_option
+from pdm.cli.commands.venv.utils import get_venv_with_name
+from pdm.cli.options import verbose_option
 from pdm.project import Project
 
 
-class Command(BaseCommand):
-    """Use the given python version or path as base interpreter"""
+class RemoveCommand(BaseCommand):
+    """Remove the virtualenv with the given name"""
+
+    arguments = [verbose_option]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        skip_option.add_to_parser(parser)
         parser.add_argument(
-            "-f",
-            "--first",
+            "-y",
+            "--yes",
             action="store_true",
-            help="Select the first matched interpreter",
+            help="Answer yes on the following question",
         )
-        parser.add_argument(
-            "-i",
-            "--ignore-remembered",
-            action="store_true",
-            help="Ignore the remembered selection",
-        )
-        parser.add_argument("--venv", help="Use the interpreter in the virtual environment with the given name")
-        parser.add_argument("python", nargs="?", help="Specify the Python version or path", default="")
+        parser.add_argument("env", help="The key of the virtualenv")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
-        actions.do_use(
-            project,
-            python=options.python,
-            first=options.first,
-            ignore_remembered=options.ignore_remembered,
-            venv=options.venv,
-            hooks=HookManager(project, options.skip),
-        )
+        project.core.ui.echo("Virtualenvs created with this project:")
+        venv = get_venv_with_name(project, options.env)
+        if options.yes or termui.confirm(f"[warning]Will remove: [success]{venv.root}[/], continue?", default=True):
+            shutil.rmtree(venv.root)
+            saved_python = project._saved_python
+            if saved_python and Path(saved_python).parent.parent == venv.root:
+                project._saved_python = None
+            project.core.ui.echo("Removed successfully!")
```

### Comparing `pdm-2.7.1/src/pdm/cli/commands/venv/__init__.py` & `pdm-2.7.2/src/pdm/cli/commands/venv/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from __future__ import annotations
 
 import argparse
 
-from pdm.project import Project
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.commands.venv.activate import ActivateCommand
 from pdm.cli.commands.venv.create import CreateCommand
 from pdm.cli.commands.venv.list import ListCommand
 from pdm.cli.commands.venv.purge import PurgeCommand
 from pdm.cli.commands.venv.remove import RemoveCommand
 from pdm.cli.commands.venv.utils import get_venv_with_name
 from pdm.cli.options import Option
+from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Virtualenv management"""
 
     name = "venv"
     arguments: list[Option] = []
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         group = parser.add_mutually_exclusive_group()
         group.add_argument("--path", help="Show the path to the given virtualenv")
         group.add_argument("--python", help="Show the python interpreter path for the given virtualenv")
-        subparser = parser.add_subparsers()
+        subparser = parser.add_subparsers(metavar="venv", title="commands")
         CreateCommand.register_to(subparser, "create")
         ListCommand.register_to(subparser, "list")
         RemoveCommand.register_to(subparser, "remove")
         ActivateCommand.register_to(subparser, "activate")
         PurgeCommand.register_to(subparser, "purge")
         self.parser = parser
```

### Comparing `pdm-2.7.1/src/pdm/cli/commands/venv/activate.py` & `pdm-2.7.2/src/pdm/cli/commands/venv/activate.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/venv/backends.py` & `pdm-2.7.2/src/pdm/cli/commands/venv/backends.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     @abc.abstractmethod
     def pip_args(self, with_pip: bool) -> Iterable[str]:
         pass
 
     @cached_property
     def _resolved_interpreter(self) -> PythonInfo:
         if not self.python:
-            saved_python = self.project._saved_python
-            if saved_python:
-                return PythonInfo.from_path(saved_python)
+            project_python = self.project._python
+            if project_python:
+                return project_python
         for py_version in self.project.find_interpreters(self.python):
             if self.python or py_version.valid and self.project.python_requires.contains(py_version.version, True):
                 return py_version
 
         python = f" {self.python}" if self.python else ""
         raise VirtualenvCreateError(f"Can't resolve python interpreter{python}")
```

### Comparing `pdm-2.7.1/src/pdm/cli/commands/venv/create.py` & `pdm-2.7.2/src/pdm/cli/commands/venv/create.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/venv/list.py` & `pdm-2.7.2/src/pdm/cli/commands/venv/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/commands/venv/utils.py` & `pdm-2.7.2/src/pdm/cli/commands/venv/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/completions/pdm.bash` & `pdm-2.7.2/src/pdm/cli/completions/pdm.bash`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             ;;
 
             (config)
             opts="--delete --global --help --local --project --verbose"
             ;;
 
             (export)
-            opts="--dev --format --global --group --help --lockfile --no-default --output --production --project --pyproject --verbose --without-hashes"
+            opts="--dev --expandvars --format --global --group --help --lockfile --no-default --output --production --project --pyproject --verbose --without-hashes"
             ;;
 
             (fix)
             opts="--dry-run --global --help --project --verbose"
             ;;
 
             (import)
```

### Comparing `pdm-2.7.1/src/pdm/cli/completions/pdm.fish` & `pdm-2.7.2/src/pdm/cli/completions/pdm.fish`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l local -d 'Set config in the project\'s local configuration file'
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # export
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l dev -d 'Select dev dependencies'
+complete -c pdm -A -n '__fish_seen_subcommand_from export' -l expandvars -d 'Expand environment variables in pyproject.toml'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l format -d 'Specify the export file format'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l no-default -d 'Don\'t include dependencies from the default group'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l output -d 'Write output to the given file, or print to stdout if not given'
```

### Comparing `pdm-2.7.1/src/pdm/cli/completions/pdm.ps1` & `pdm-2.7.2/src/pdm/cli/completions/pdm.ps1`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
             "config" {
                 $completer.AddOpts(@([Option]::new(@("--delete", "--global", "--local", "-d", "-l", "-g")), $projectOption))
                 $completer.AddParams(@(getConfigKeys), $false)
                 break
             }
             "export" {
                 $completer.AddOpts(@(
-                        [Option]::new(@("--dev", "--output", "--global", "--no-default", "--prod", "--production", "-g", "-d", "-o", "--without-hashes", "-L", "--lockfile")),
+                        [Option]::new(@("--dev", "--output", "--global", "--no-default", "--expandvars", "--prod", "--production", "-g", "-d", "-o", "--without-hashes", "-L", "--lockfile")),
                         $formatOption,
                         $sectionOption,
                         $projectOption
                     ))
                 break
             }
             "fix" {
```

### Comparing `pdm-2.7.1/src/pdm/cli/completions/pdm.zsh` & `pdm-2.7.2/src/pdm/cli/completions/pdm.zsh`

 * *Files 0% similar despite different names*

```diff
@@ -141,14 +141,15 @@
       fi
       ;;
     export)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-f+,--format+}"[Specify the export file format]:format:(pipfile poetry flit requirements setuppy)"
         "--without-hashes[Don't include artifact hashes]"
+        "--expandvars[Expand environment variables in requirements]"
         {-L,--lockfile}'[Specify another lockfile path, or use `PDM_LOCKFILE` env variable. Default: pdm.lock]:lockfile:_files'
         {-o+,--output+}"[Write output to the given file, or print to stdout if not given]:output file:_files"
         {-G+,--group+}'[Select group of optional-dependencies or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species]:group:_pdm_groups'
         {-d,--dev}"[Select dev dependencies]"
         {--prod,--production}"[Unselect dev dependencies]"
         "--no-default[Don't include dependencies from the default group]"
       )
```

### Comparing `pdm-2.7.1/src/pdm/cli/filters.py` & `pdm-2.7.2/src/pdm/cli/filters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/hooks.py` & `pdm-2.7.2/src/pdm/cli/hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/cli/options.py` & `pdm-2.7.2/src/pdm/cli/options.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/compat.py` & `pdm-2.7.2/src/pdm/compat.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/core.py` & `pdm-2.7.2/src/pdm/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             help="Specify another config file path [env var: PDM_CONFIG_FILE] ",
         )
         self.parser._positionals.title = "Commands"
         verbose_option.add_to_parser(self.parser)
         ignore_python_option.add_to_parser(self.parser)
         pep582_option.add_to_parser(self.parser)
 
-        self.subparsers = self.parser.add_subparsers(parser_class=ArgumentParser)
+        self.subparsers = self.parser.add_subparsers(parser_class=ArgumentParser, metavar="__root__")
         for _, name, _ in pkgutil.iter_modules(COMMANDS_MODULE_PATH):
             module = importlib.import_module(f"pdm.cli.commands.{name}", __name__)
             try:
                 klass = module.Command
             except AttributeError:
                 continue
             self.register_command(klass, klass.name or name)
```

### Comparing `pdm-2.7.1/src/pdm/environments/__init__.py` & `pdm-2.7.2/src/pdm/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/environments/base.py` & `pdm-2.7.2/src/pdm/environments/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/environments/local.py` & `pdm-2.7.2/src/pdm/environments/local.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/environments/python.py` & `pdm-2.7.2/src/pdm/environments/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/exceptions.py` & `pdm-2.7.2/src/pdm/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 class CandidateNotFound(PdmException):
     pass
 
 
 class CandidateInfoNotFound(PdmException):
     def __init__(self, candidate: Candidate) -> None:
-        message = f"No metadata information is available for [success]{str(candidate)}[/]."
+        message = f"No metadata information is available for [success]{candidate!s}[/]."
         self.candidate = candidate
         super().__init__(message)
 
 
 class ExtrasWarning(UserWarning):
     def __init__(self, project_name: str, extras: list[str]) -> None:
         super().__init__(f"Extras not found for {project_name}: [{','.join(extras)}]")
```

### Comparing `pdm-2.7.1/src/pdm/formats/__init__.py` & `pdm-2.7.2/src/pdm/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/formats/base.py` & `pdm-2.7.2/src/pdm/formats/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/formats/flit.py` & `pdm-2.7.2/src/pdm/formats/flit.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/formats/pipfile.py` & `pdm-2.7.2/src/pdm/formats/pipfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/formats/poetry.py` & `pdm-2.7.2/src/pdm/formats/poetry.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/formats/requirements.py` & `pdm-2.7.2/src/pdm/formats/requirements.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import hashlib
 import shlex
 import urllib.parse
 from typing import TYPE_CHECKING, Any, Mapping
 
 from pdm.formats.base import make_array
 from pdm.models.requirements import FileRequirement, Requirement, parse_requirement
+from pdm.utils import expand_env_vars_in_auth
 
 if TYPE_CHECKING:
     from argparse import Namespace
     from os import PathLike
 
     from pdm.models.candidates import Candidate
     from pdm.project import Project
@@ -183,21 +184,23 @@
     lines = ["# This file is @generated by PDM.\n# Please do not edit it manually.\n\n"]
     for candidate in sorted(candidates, key=lambda x: x.identify()):  # type: ignore[attr-defined]
         if isinstance(candidate, Candidate):
             req = dataclasses.replace(candidate.req, specifier=f"=={candidate.version}", marker=None)
         else:
             assert isinstance(candidate, Requirement)
             req = candidate
-        lines.append(project.backend.expand_line(req.as_line()))
+        lines.append(project.backend.expand_line(req.as_line(), options.expandvars))
         if options.hashes and getattr(candidate, "hashes", None):
             for item in sorted(set(candidate.hashes.values())):  # type: ignore[attr-defined]
                 lines.append(f" \\\n    --hash={item}")
         lines.append("\n")
     sources = project.pyproject.settings.get("source", [])
     for source in sources:
         url = source["url"]
+        if options.expandvars:
+            url = expand_env_vars_in_auth(url)
         prefix = "--index-url" if source["name"] == "pypi" else "--extra-index-url"
         lines.append(f"{prefix} {url}\n")
         if not source.get("verify_ssl", True):
             host = urllib.parse.urlparse(url).hostname
             lines.append(f"--trusted-host {host}\n")
     return "".join(lines)
```

### Comparing `pdm-2.7.1/src/pdm/formats/setup_py.py` & `pdm-2.7.2/src/pdm/formats/setup_py.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/installers/core.py` & `pdm-2.7.2/src/pdm/installers/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/installers/installers.py` & `pdm-2.7.2/src/pdm/installers/installers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/installers/manager.py` & `pdm-2.7.2/src/pdm/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/installers/packages.py` & `pdm-2.7.2/src/pdm/installers/packages.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/installers/synchronizers.py` & `pdm-2.7.2/src/pdm/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/installers/uninstallers.py` & `pdm-2.7.2/src/pdm/installers/uninstallers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/auth.py` & `pdm-2.7.2/src/pdm/models/auth.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/backends.py` & `pdm-2.7.2/src/pdm/models/backends.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class BuildBackend(metaclass=abc.ABCMeta):
     """A build backend that does not support dynamic values in dependencies"""
 
     def __init__(self, root: Path) -> None:
         self.root = root
 
-    def expand_line(self, line: str) -> str:
+    def expand_line(self, line: str, expand_env: bool = True) -> str:
         return line
 
     def relative_path_to_url(self, path: str) -> str:
         return path_to_url(os.path.join(self.root, path))
 
     @classmethod
     @abc.abstractmethod
@@ -41,16 +41,19 @@
         return {
             "requires": ["setuptools>=61", "wheel"],
             "build-backend": "setuptools.build_meta",
         }
 
 
 class PDMBackend(BuildBackend):
-    def expand_line(self, req: str) -> str:
-        return expand_env_vars(req).replace("file:///${PROJECT_ROOT}", path_to_url(self.root.as_posix()))
+    def expand_line(self, req: str, expand_env: bool = True) -> str:
+        line = req.replace("file:///${PROJECT_ROOT}", path_to_url(self.root.as_posix()))
+        if expand_env:
+            line = expand_env_vars(line)
+        return line
 
     def relative_path_to_url(self, path: str) -> str:
         if os.path.isabs(path):
             return path_to_url(path)
         return f"file:///${{PROJECT_ROOT}}/{urllib.parse.quote(path)}"
 
     @classmethod
@@ -82,27 +85,32 @@
             return path_to_url(self.__path.as_posix())
         elif __format_spec == "real":
             return self.__path.resolve().as_posix()
         raise ValueError(f"Unknown format specifier: {__format_spec}")
 
 
 class EnvContext:
+    def __init__(self, expand: bool = True) -> None:
+        self.expand = expand
+
     def __format__(self, __format_spec: str) -> str:
         name, sep, default = __format_spec.partition(":")
+        if not self.expand:
+            return f"${{{name}}}"
         if name in os.environ:
             return os.environ[name]
         if not sep:
             raise ValueError(f"Nonexistent environment variable must set a default: {name}")
         return default
 
 
 class HatchBackend(BuildBackend):
-    def expand_line(self, line: str) -> str:
+    def expand_line(self, line: str, expand_env: bool = True) -> str:
         return line.format(
-            env=EnvContext(),
+            env=EnvContext(expand=expand_env),
             root=PathContext(self.root),
             home=PathContext(Path.home()),
         )
 
     def relative_path_to_url(self, path: str) -> str:
         if os.path.isabs(path):
             return path_to_url(path)
```

### Comparing `pdm-2.7.1/src/pdm/models/caches.py` & `pdm-2.7.2/src/pdm/models/caches.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/candidates.py` & `pdm-2.7.2/src/pdm/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/in_process/__init__.py` & `pdm-2.7.2/src/pdm/models/in_process/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from __future__ import annotations
 
 import contextlib
 import functools
 import json
 import os
 import subprocess
+import tempfile
 from typing import Any, Generator
 
 from pdm.compat import resources_path
 
 
 @contextlib.contextmanager
 def _in_process_script(name: str) -> Generator[str, None, None]:
@@ -43,9 +44,12 @@
         args = [executable, "-Es", script]
         return json.loads(subprocess.check_output(args))
 
 
 def parse_setup_py(executable: str, path: str) -> dict[str, Any]:
     """Parse setup.py and return the kwargs"""
     with _in_process_script("parse_setup.py") as script:
-        cmd = [executable, "-Es", script, path]
-        return json.loads(subprocess.check_output(cmd))
+        _, outfile = tempfile.mkstemp(suffix=".json")
+        cmd = [executable, "-Es", script, path, outfile]
+        subprocess.check_call(cmd)
+        with open(outfile, "rb") as fp:
+            return json.load(fp)
```

### Comparing `pdm-2.7.1/src/pdm/models/in_process/get_abi_tag.py` & `pdm-2.7.2/src/pdm/models/in_process/get_abi_tag.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/in_process/parse_setup.py` & `pdm-2.7.2/src/pdm/models/in_process/parse_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,11 +195,17 @@
             if os.path.exists(readme_path):
                 parsed["readme"] = readme_file
                 break
     clean_metadata(parsed)
     return parsed
 
 
+def json_default(o):
+    return "<unserializable object>"
+
+
 if __name__ == "__main__":
     import json
 
-    print(json.dumps(parse_setup(sys.argv[1])))
+    outfile = sys.argv[2]
+    with open(outfile, "w") as f:
+        json.dump(parse_setup(sys.argv[1]), f, default=json_default)
```

### Comparing `pdm-2.7.1/src/pdm/models/in_process/pep508.py` & `pdm-2.7.2/src/pdm/models/in_process/pep508.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/in_process/sysconfig_get_paths.py` & `pdm-2.7.2/src/pdm/models/in_process/sysconfig_get_paths.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/markers.py` & `pdm-2.7.2/src/pdm/models/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/project_info.py` & `pdm-2.7.2/src/pdm/models/project_info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/python.py` & `pdm-2.7.2/src/pdm/models/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/repositories.py` & `pdm-2.7.2/src/pdm/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/requirements.py` & `pdm-2.7.2/src/pdm/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/search.py` & `pdm-2.7.2/src/pdm/models/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/setup.py` & `pdm-2.7.2/src/pdm/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/specifiers.py` & `pdm-2.7.2/src/pdm/models/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/venv.py` & `pdm-2.7.2/src/pdm/models/venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/versions.py` & `pdm-2.7.2/src/pdm/models/versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/models/working_set.py` & `pdm-2.7.2/src/pdm/models/working_set.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/pep582/sitecustomize.py` & `pdm-2.7.2/src/pdm/pep582/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/project/config.py` & `pdm-2.7.2/src/pdm/project/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/project/core.py` & `pdm-2.7.2/src/pdm/project/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/project/lockfile.py` & `pdm-2.7.2/src/pdm/project/lockfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/project/project_file.py` & `pdm-2.7.2/src/pdm/project/project_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/project/toml_file.py` & `pdm-2.7.2/src/pdm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/pytest.py` & `pdm-2.7.2/src/pdm/pytest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/resolver/core.py` & `pdm-2.7.2/src/pdm/resolver/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/resolver/providers.py` & `pdm-2.7.2/src/pdm/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/resolver/python.py` & `pdm-2.7.2/src/pdm/resolver/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/resolver/reporters.py` & `pdm-2.7.2/src/pdm/resolver/reporters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/signals.py` & `pdm-2.7.2/src/pdm/signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/termui.py` & `pdm-2.7.2/src/pdm/termui.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/src/pdm/utils.py` & `pdm-2.7.2/src/pdm/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/conftest.py` & `pdm-2.7.2/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/test_add.py` & `pdm-2.7.2/tests/cli/test_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import shutil
 
 import pytest
 from unearth import Link
 
-from pdm.cli import actions
 from pdm.models.requirements import parse_requirement
 from pdm.models.specifiers import PySpecSet
 from pdm.utils import path_to_url
 from tests import FIXTURES
 
 
 def test_add_package(project, working_set, dev_option, pdm):
@@ -22,15 +21,15 @@
     locked_candidates = project.locked_repository.all_candidates
     assert locked_candidates["idna"].version == "2.7"
     for package in ("requests", "idna", "chardet", "urllib3", "certifi"):
         assert package in working_set
 
 
 def test_add_command(project, pdm, mocker):
-    do_add = mocker.patch.object(actions, "do_add")
+    do_add = mocker.patch("pdm.cli.commands.add.Command.do_add")
     pdm(["add", "requests"], obj=project)
     do_add.assert_called_once()
 
 
 def test_add_package_to_custom_group(project, working_set, pdm):
     pdm(["add", "requests", "--group", "test"], obj=project, strict=True)
```

### Comparing `pdm-2.7.1/tests/cli/test_build.py` & `pdm-2.7.2/tests/cli/test_build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/test_cache.py` & `pdm-2.7.2/tests/cli/test_cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/test_config.py` & `pdm-2.7.2/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/test_fix.py` & `pdm-2.7.2/tests/cli/test_fix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/test_hooks.py` & `pdm-2.7.2/tests/cli/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/test_init.py` & `pdm-2.7.2/tests/cli/test_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 from unittest.mock import ANY
 
 import pytest
 
-from pdm.cli import actions
 from pdm.cli.commands.init import Command
 from pdm.models.backends import get_backend
 from pdm.models.python import PythonInfo
 
 PYTHON_VERSION = f"{sys.version_info[0]}.{sys.version_info[1]}"
 
 
@@ -67,15 +66,15 @@
 
 def test_init_non_interactive(project_no_init, pdm, mocker):
     mocker.patch(
         "pdm.cli.commands.init.get_user_email_from_git",
         return_value=("Testing", "me@example.org"),
     )
     do_init = mocker.patch.object(Command, "do_init")
-    do_use = mocker.patch.object(actions, "do_use", return_value=PythonInfo.from_path(sys.executable))
+    do_use = mocker.patch("pdm.cli.commands.use.Command.do_use", return_value=PythonInfo.from_path(sys.executable))
     result = pdm(["init", "-n"], obj=project_no_init)
     assert result.exit_code == 0
     python_version = f"{project_no_init.python.major}.{project_no_init.python.minor}"
     do_use.assert_called_once_with(
         project_no_init,
         ANY,
         first=True,
```

### Comparing `pdm-2.7.1/tests/cli/test_install.py` & `pdm-2.7.2/tests/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/test_list.py` & `pdm-2.7.2/tests/cli/test_list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/test_lock.py` & `pdm-2.7.2/tests/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/test_others.py` & `pdm-2.7.2/tests/cli/test_others.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/test_publish.py` & `pdm-2.7.2/tests/cli/test_publish.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/test_remove.py` & `pdm-2.7.2/tests/cli/test_remove.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pdm.cli import actions
 from pdm.models.requirements import parse_requirement
 from pdm.models.specifiers import PySpecSet
 
 
 def test_remove_command(project, pdm, mocker):
-    do_remove = mocker.patch.object(actions, "do_remove")
+    do_remove = mocker.patch("pdm.cli.commands.remove.Command.do_remove")
     pdm(["remove", "demo"], obj=project)
     do_remove.assert_called_once()
 
 
 @pytest.mark.usefixtures("working_set", "vcs")
 def test_remove_editable_packages_while_keeping_normal(project, pdm):
     project.environment.python_requires = PySpecSet(">=3.6")
```

### Comparing `pdm-2.7.1/tests/cli/test_run.py` & `pdm-2.7.2/tests/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/test_self_command.py` & `pdm-2.7.2/tests/cli/test_self_command.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/cli/test_update.py` & `pdm-2.7.2/tests/cli/test_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import pytest
 
-from pdm.cli import actions
 from pdm.models.requirements import parse_requirement
 
 
 @pytest.mark.usefixtures("working_set")
 def test_update_packages_with_top(project, pdm):
     pdm(["add", "requests"], obj=project, strict=True)
     result = pdm(["update", "--top", "requests"], obj=project)
     assert "PdmUsageError" in result.stderr
 
 
 def test_update_command(project, pdm, mocker):
-    do_update = mocker.patch.object(actions, "do_update")
+    do_update = mocker.patch("pdm.cli.commands.update.Command.do_update")
     pdm(["update"], obj=project)
     do_update.assert_called_once()
 
 
 @pytest.mark.usefixtures("working_set")
 def test_update_ignore_constraints(project, repository, pdm):
     project.project_config["strategy.save"] = "compatible"
```

### Comparing `pdm-2.7.1/tests/cli/test_use.py` & `pdm-2.7.2/tests/cli/test_use.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
 import sys
 from pathlib import Path
 
 import pytest
 
-from pdm.cli import actions
+from pdm.cli.commands.use import Command as UseCommand
 from pdm.exceptions import NoPythonVersion
 from pdm.models.caches import JSONFileCache
 
 
 def test_use_command(project, pdm):
     python = "python" if os.name == "nt" else "python3"
     python_path = shutil.which(python)
@@ -38,48 +38,50 @@
 """.format(
         sys.executable
     )
     shim_path = project.root.joinpath("python_shim.sh")
     shim_path.write_text(wrapper_script)
     shim_path.chmod(0o755)
 
-    actions.do_use(project, shim_path.as_posix())
+    UseCommand().do_use(project, shim_path.as_posix())
     assert project.python.executable == Path(sys.executable)
 
 
 @pytest.mark.skipif(os.name != "posix", reason="Run on POSIX platforms only")
 def test_use_invalid_wrapper_python(project):
     wrapper_script = """#!/bin/bash
 echo hello
 """
     shim_path = project.root.joinpath("python_shim.sh")
     shim_path.write_text(wrapper_script)
     shim_path.chmod(0o755)
     with pytest.raises(NoPythonVersion):
-        actions.do_use(project, shim_path.as_posix())
+        UseCommand().do_use(project, shim_path.as_posix())
 
 
 def test_use_remember_last_selection(project, mocker):
     cache = JSONFileCache(project.cache_dir / "use_cache.json")
     cache.clear()
-    actions.do_use(project, first=True)
+    do_use = UseCommand().do_use
+    do_use(project, first=True)
     cache._read_cache()
     assert not cache._cache
-    actions.do_use(project, "3", first=True)
+    do_use(project, "3", first=True)
     cache._read_cache()
     assert "3" in cache
     mocker.patch.object(project, "find_interpreters")
-    actions.do_use(project, "3")
+    do_use(project, "3")
     project.find_interpreters.assert_not_called()
 
 
 def test_use_venv_python(project, pdm):
     pdm(["venv", "create"], obj=project, strict=True)
     pdm(["venv", "create", "--name", "test"], obj=project, strict=True)
     project.global_config["python.use_venv"] = True
     venv_location = project.config["venv.location"]
-    actions.do_use(project, venv="in-project")
+    do_use = UseCommand().do_use
+    do_use(project, venv="in-project")
     assert project.python.executable.parent.parent == project.root.joinpath(".venv")
-    actions.do_use(project, venv="test")
+    do_use(project, venv="test")
     assert project.python.executable.parent.parent.parent == Path(venv_location)
     with pytest.raises(Exception, match="No virtualenv with key 'non-exists' is found"):
-        actions.do_use(project, venv="non-exists")
+        do_use(project, venv="non-exists")
```

### Comparing `pdm-2.7.1/tests/cli/test_venv.py` & `pdm-2.7.2/tests/cli/test_venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/conftest.py` & `pdm-2.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz` & `pdm-2.7.2/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl` & `pdm-2.7.2/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1.tar.gz` & `pdm-2.7.2/tests/fixtures/artifacts/demo-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/demo-0.0.1.zip` & `pdm-2.7.2/tests/fixtures/artifacts/demo-0.0.1.zip`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz` & `pdm-2.7.2/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl` & `pdm-2.7.2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl` & `pdm-2.7.2/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock` & `pdm-2.7.2/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/projects/demo-package/pdm.lock` & `pdm-2.7.2/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-2.7.2/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-2.7.2/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/projects/demo-package/setup.txt` & `pdm-2.7.2/tests/fixtures/projects/demo-package/setup.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/projects/flit-demo/pyproject.toml` & `pdm-2.7.2/tests/fixtures/projects/flit-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/projects/poetry-demo/pyproject.toml` & `pdm-2.7.2/tests/fixtures/projects/poetry-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/pypi.json` & `pdm-2.7.2/tests/fixtures/pypi.json`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/fixtures/pyproject.toml` & `pdm-2.7.2/tests/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/models/test_backends.py` & `pdm-2.7.2/tests/models/test_backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/models/test_candidates.py` & `pdm-2.7.2/tests/models/test_candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/models/test_marker.py` & `pdm-2.7.2/tests/models/test_marker.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/models/test_requirements.py` & `pdm-2.7.2/tests/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/models/test_setup_parsing.py` & `pdm-2.7.2/tests/models/test_setup_parsing.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/models/test_specifiers.py` & `pdm-2.7.2/tests/models/test_specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/models/test_versions.py` & `pdm-2.7.2/tests/models/test_versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/resolver/test_resolve.py` & `pdm-2.7.2/tests/resolver/test_resolve.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/test_formats.py` & `pdm-2.7.2/tests/test_formats.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     assert settings["source"][0]["url"] == "https://pypi.python.org/simple"
 
 
 @pytest.mark.parametrize("is_dev", [True, False])
 def test_convert_requirements_file(project, is_dev):
     golden_file = FIXTURES / "requirements.txt"
     assert requirements.check_fingerprint(project, golden_file)
-    options = Namespace(dev=is_dev, group=None)
+    options = Namespace(dev=is_dev, group=None, expandvars=False)
     result, settings = requirements.convert(project, golden_file, options)
     group = settings["dev-dependencies"]["dev"] if is_dev else result["dependencies"]
     dev_group = settings["dev-dependencies"]["dev"]
 
     assert len(settings["source"]) == 2
     assert "webassets==2.0" in group
     assert 'whoosh==2.7.4; sys_platform == "win32"' in group
@@ -46,15 +46,15 @@
     )
 
 
 def test_convert_requirements_file_without_name(project, vcs):
     req_file = project.root.joinpath("reqs.txt")
     project.root.joinpath("reqs.txt").write_text("git+https://github.com/test-root/demo.git\n")
     assert requirements.check_fingerprint(project, str(req_file))
-    result, _ = requirements.convert(project, str(req_file), Namespace(dev=False, group=None))
+    result, _ = requirements.convert(project, str(req_file), Namespace(dev=False, group=None, expandvars=None))
 
     assert result["dependencies"] == ["demo @ git+https://github.com/test-root/demo.git"]
 
 
 def test_convert_poetry(project):
     golden_file = FIXTURES / "pyproject.toml"
     assert poetry.check_fingerprint(project, golden_file)
@@ -120,39 +120,47 @@
     assert build["includes"] == ["doc/"]
     assert build["excludes"] == ["doc/*.html"]
 
 
 def test_import_requirements_with_group(project):
     golden_file = FIXTURES / "requirements.txt"
     assert requirements.check_fingerprint(project, golden_file)
-    result, settings = requirements.convert(project, golden_file, Namespace(dev=False, group="test"))
+    result, settings = requirements.convert(project, golden_file, Namespace(dev=False, group="test", expandvars=False))
 
     group = result["optional-dependencies"]["test"]
     dev_group = settings["dev-dependencies"]["dev"]
     assert "webassets==2.0" in group
     assert 'whoosh==2.7.4; sys_platform == "win32"' in group
     assert "-e git+https://github.com/pypa/pip.git@main#egg=pip" not in group
     assert "-e git+https://github.com/pypa/pip.git@main#egg=pip" in dev_group
     assert not result.get("dependencies")
 
 
 def test_keep_env_vars_in_source(project, monkeypatch):
     monkeypatch.setenv("USER", "foo")
     monkeypatch.setenv("PASSWORD", "bar")
     project.pyproject.settings["source"] = [{"url": "https://${USER}:${PASSWORD}@test.pypi.org/simple", "name": "pypi"}]
-    result = requirements.export(project, [], Namespace())
+    result = requirements.export(project, [], Namespace(expandvars=False))
     assert result.strip().splitlines()[-1] == "--index-url https://${USER}:${PASSWORD}@test.pypi.org/simple"
 
 
+def test_expand_env_vars_in_source(project, monkeypatch):
+    monkeypatch.setenv("USER", "foo")
+    monkeypatch.setenv("PASSWORD", "bar")
+    project.pyproject.settings["source"] = [{"url": "https://foo:bar@test.pypi.org/simple", "name": "pypi"}]
+    result = requirements.export(project, [], Namespace(expandvars=True))
+    assert result.strip().splitlines()[-1] == "--index-url https://foo:bar@test.pypi.org/simple"
+
+
 def test_export_replace_project_root(project):
     artifact = FIXTURES / "artifacts/first-2.0.2-py2.py3-none-any.whl"
     shutil.copy2(artifact, project.root)
     with cd(project.root):
         req = parse_requirement(f"./{artifact.name}")
-    result = requirements.export(project, [req], Namespace(hashes=False))
+    result = requirements.export(project, [req], Namespace(hashes=False, expandvars=False))
     assert "${PROJECT_ROOT}" not in result
 
 
 def test_convert_setup_py_project(project):
     golden_file = FIXTURES / "projects/test-setuptools/setup.py"
     assert setup_py.check_fingerprint(project, golden_file)
     result, settings = setup_py.convert(project, golden_file, Namespace())
```

### Comparing `pdm-2.7.1/tests/test_installer.py` & `pdm-2.7.2/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/test_integration.py` & `pdm-2.7.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/test_plugin.py` & `pdm-2.7.2/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/test_project.py` & `pdm-2.7.2/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/test_signals.py` & `pdm-2.7.2/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/tests/test_utils.py` & `pdm-2.7.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.1/PKG-INFO` & `pdm-2.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm
-Version: 2.7.1
+Version: 2.7.2
 Summary: A modern Python package and dependency manager supporting the latest PEP standards
 Keywords: packaging dependency workflow
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -133,15 +133,15 @@
 **For Windows**
 
 ```powershell
 (Invoke-WebRequest -Uri https://raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py -UseBasicParsing).Content | python -
 ```
 
 For security reasons, you should verify the checksum of `install-pdm.py`.
-The sha256 checksum is: `06abd94a6678636eba640529bf91b242759363c45d3620cdfabaa0053d826b30`
+The sha256 checksum is: `965900c551b4d1ba5127ecf95c127c99b5a1cccef4c183a5ecf447e876fa3160`
 
 The installer will install PDM into the user site and the location depends on the system:
 
 - `$HOME/.local/bin` for Unix
 - `%APPDATA%\Python\Scripts` on Windows
 
 You can pass additional options to the script to control how PDM is installed:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm Version: 2.7.1 Summary: A modern Python package
+Metadata-Version: 2.1 Name: pdm Version: 2.7.2 Summary: A modern Python package
 and dependency manager supporting the latest PEP standards Keywords: packaging
 dependency workflow Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Topic :: Software Development :: Build
 Tools Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -79,15 +79,15 @@
 Like Pip, PDM provides an installation script that will install PDM into an
 isolated environment. **For Linux/Mac** ```bash curl -sSL https://
 raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py | python3 - ```
 **For Windows** ```powershell (Invoke-WebRequest -Uri https://
 raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py -
 UseBasicParsing).Content | python - ``` For security reasons, you should verify
 the checksum of `install-pdm.py`. The sha256 checksum is:
-`06abd94a6678636eba640529bf91b242759363c45d3620cdfabaa0053d826b30` The
+`965900c551b4d1ba5127ecf95c127c99b5a1cccef4c183a5ecf447e876fa3160` The
 installer will install PDM into the user site and the location depends on the
 system: - `$HOME/.local/bin` for Unix - `%APPDATA%\Python\Scripts` on Windows
 You can pass additional options to the script to control how PDM is installed:
 ``` usage: install-pdm.py [-h] [-v VERSION] [--prerelease] [--remove] [-p PATH]
 [-d DEP] optional arguments: -h, --help show this help message and exit -
 v VERSION, --version VERSION | envvar: PDM_VERSION Specify the version to be
 installed, or HEAD to install from the main branch --prerelease | envvar:
```

