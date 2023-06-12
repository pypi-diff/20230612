# Comparing `tmp/openstack-image-manager-0.2.6.tar.gz` & `tmp/openstack-image-manager-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstack-image-manager-0.2.6.tar", last modified: Sun Mar 12 17:38:20 2023, max compression
+gzip compressed data, was "openstack-image-manager-0.3.0.tar", last modified: Mon Jun 12 17:22:08 2023, max compression
```

## Comparing `openstack-image-manager-0.2.6.tar` & `openstack-image-manager-0.3.0.tar`

### file list

```diff
@@ -1,140 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.587434 openstack-image-manager-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/.clouds.yml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.575434 openstack-image-manager-0.2.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/.github/renovate.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.575434 openstack-image-manager-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/.github/workflows/build-container-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/.github/workflows/mirror-images.yml
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/.github/workflows/run-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/.github/workflows/test-python-setup.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/.github/workflows/update-images.yml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/.github/workflows/validate-configuration.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/.yamllint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/.zuul.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-12 17:38:20.000000 openstack-image-manager-0.2.6/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-12 17:38:20.000000 openstack-image-manager-0.2.6/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-12 17:38:20.587434 openstack-image-manager-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/clouds.yml.sample
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.579434 openstack-image-manager-0.2.6/crawler/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.579434 openstack-image-manager-0.2.6/crawler/crawler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/crawler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.579434 openstack-image-manager-0.2.6/crawler/crawler/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/crawler/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/crawler/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/crawler/core/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/crawler/core/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/crawler/core/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.579434 openstack-image-manager-0.2.6/crawler/crawler/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/crawler/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/crawler/git/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.579434 openstack-image-manager-0.2.6/crawler/crawler/updater/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/crawler/updater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/crawler/updater/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.579434 openstack-image-manager-0.2.6/crawler/crawler/web/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/crawler/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/crawler/web/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/crawler/web/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.579434 openstack-image-manager-0.2.6/crawler/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/docs/background.md
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/docs/git-handling.md
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/docs/templates.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.579434 openstack-image-manager-0.2.6/crawler/etc/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/etc/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/etc/image-sources.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      112 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/git_ssh_command.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     8445 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/historian.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5207 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/image-crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.579434 openstack-image-manager-0.2.6/crawler/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/lib/initialize-image-catalog.sql
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/lib/populate-catalog-test-data.sql
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.579434 openstack-image-manager-0.2.6/crawler/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/templates/almalinux.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/templates/debian.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/templates/header.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/templates/ubuntu.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/crawler/templates/ubuntu_minimal.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.583434 openstack-image-manager-0.2.6/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/doc/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/doc/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/doc/getting_started.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.583434 openstack-image-manager-0.2.6/doc/images/
--rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/doc/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/doc/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/doc/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/doc/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.583434 openstack-image-manager-0.2.6/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.583434 openstack-image-manager-0.2.6/etc/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/images/almalinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/images/centos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/images/cirros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/images/clearlinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/images/debian.yml
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/images/fedora.yml
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/images/flatcar.yml
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/images/gardenlinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/images/kubernetes.yml
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/images/opensense.yml
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/images/opensuse.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/images/rockylinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/images/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/etc/schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.583434 openstack-image-manager-0.2.6/openstack_image_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/openstack_image_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43973 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/openstack_image_manager/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/openstack_image_manager/mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/openstack_image_manager/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/openstack_image_manager/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.587434 openstack-image-manager-0.2.6/openstack_image_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-12 17:38:20.000000 openstack-image-manager-0.2.6/openstack_image_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-03-12 17:38:20.000000 openstack-image-manager-0.2.6/openstack_image_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 17:38:20.000000 openstack-image-manager-0.2.6/openstack_image_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-12 17:38:20.000000 openstack-image-manager-0.2.6/openstack_image_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 17:38:20.000000 openstack-image-manager-0.2.6/openstack_image_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-12 17:38:20.000000 openstack-image-manager-0.2.6/openstack_image_manager.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-12 17:38:20.000000 openstack-image-manager-0.2.6/openstack_image_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-12 17:38:20.000000 openstack-image-manager-0.2.6/openstack_image_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.587434 openstack-image-manager-0.2.6/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/playbooks/integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/playbooks/pre-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/playbooks/pre-real-world.yml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/playbooks/real-world.yml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.587434 openstack-image-manager-0.2.6/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      723 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/scripts/build.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      477 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/scripts/push.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/secure.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-12 17:38:20.587434 openstack-image-manager-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.587434 openstack-image-manager-0.2.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43973 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/src/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/src/mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/src/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/src/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.587434 openstack-image-manager-0.2.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.587434 openstack-image-manager-0.2.6/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/test/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.587434 openstack-image-manager-0.2.6/test/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/test/integration/fixtures/test_image.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/test/integration/test_manage_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:20.587434 openstack-image-manager-0.2.6/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/test/unit/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-12 17:38:10.000000 openstack-image-manager-0.2.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.clouds.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.660799 openstack-image-manager-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/renovate.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.660799 openstack-image-manager-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/build-container-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/mirror-images-dry-run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/mirror-images.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/test-python-setup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/update-images.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/validate-configuration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.yamllint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.zuul.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    40761 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/clouds.yml.sample
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.664799 openstack-image-manager-0.3.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/getting_started.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.664799 openstack-image-manager-0.3.0/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.664799 openstack-image-manager-0.3.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.664799 openstack-image-manager-0.3.0/etc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/almalinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/centos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/cirros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/clearlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/debian.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/fedora.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/flatcar.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/gardenlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/kubernetes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/octavia.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/opensuse.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/opnsense.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/rockylinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/talos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.664799 openstack-image-manager-0.3.0/openstack_image_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/openstack_image_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47634 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/openstack_image_manager/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/openstack_image_manager/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/openstack_image_manager/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/openstack_image_manager/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.664799 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/playbooks/integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/playbooks/pre-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/playbooks/pre-real-world.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/playbooks/real-world.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      723 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/scripts/build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      477 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/scripts/push.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/secure.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/test/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/test/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/test/integration/fixtures/test_image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/test/integration/test_manage_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/test/unit/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/tox.ini
```

### Comparing `openstack-image-manager-0.2.6/.github/workflows/build-container-image.yml` & `openstack-image-manager-0.3.0/.github/workflows/build-container-image.yml`

 * *Files 13% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 "on":
   workflow_dispatch:
   push:
     paths:
       - .github/workflows/build-container-image.yml
       - Containerfile
-      - src/**
+      - openstack_image_manager/**
     branches:
       - main
   pull_request:
     paths:
       - .github/workflows/build-container-image.yml
       - Containerfile
-      - src/**
+      - openstack_image_manager/**
 
 jobs:
   build-container-image:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: docker/setup-buildx-action@v2
```

### Comparing `openstack-image-manager-0.2.6/.github/workflows/mirror-images.yml` & `openstack-image-manager-0.3.0/.github/workflows/mirror-images.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ---
 name: Mirror images
 
 "on":
+  workflow_dispatch:
   push:
     paths:
       - .github/workflows/mirror-images.yml
       - etc/images/*.yml
     branches:
       - main
```

### Comparing `openstack-image-manager-0.2.6/.github/workflows/publish.yml` & `openstack-image-manager-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/.github/workflows/test-python-setup.yml` & `openstack-image-manager-0.3.0/.github/workflows/test-python-setup.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/.github/workflows/update-images.yml` & `openstack-image-manager-0.3.0/.github/workflows/update-images.yml`

 * *Files 25% similar despite different names*

```diff
@@ -4,24 +4,14 @@
 "on":
   workflow_dispatch:
   schedule:
     - cron: '0 0 * * 0'
 
 jobs:
   update-images:
-    name: ${{ matrix.image }}
-    strategy:
-      fail-fast: false
-      matrix:
-        image:
-          - almalinux
-          - centos
-          - debian
-          - rockylinux
-          - ubuntu
     runs-on: ubuntu-latest
     steps:
       - name: Checkout repo
         uses: actions/checkout@v3
 
       - name: Set up python
         uses: actions/setup-python@v4
@@ -31,18 +21,18 @@
       - name: Install pip3
         run: pip3 install tox
 
       - name: Update ${{ matrix.image }} images
         uses: technote-space/create-pr-action@v2
         with:
           EXECUTE_COMMANDS: |
-            tox -e update -- --minio-access-key ${{ secrets.MINIO_ACCESS_KEY }} --minio-secret-key ${{ secrets.MINIO_SECRET_KEY }} --image ${{ matrix.image }}
+            tox -e update -- --minio-access-key ${{ secrets.MINIO_ACCESS_KEY }} --minio-secret-key ${{ secrets.MINIO_SECRET_KEY }}
           COMMIT_EMAIL: 'bot@osism.tech'
           COMMIT_MESSAGE: |
-            chore: update ${{ matrix.image }} images
+            chore: update images
 
             Signed-off-by: OSISM Bot <bot@osism.tech>
           COMMIT_NAME: "OSISM Bot"
           ONLY_DEFAULT_BRANCH: true
-          PR_BRANCH_NAME: "update-${{ matrix.image }}-images"
+          PR_BRANCH_NAME: "update-images"
           PR_BRANCH_PREFIX: "chore/"
-          PR_TITLE: "chore: update ${{ matrix.image }} images"
+          PR_TITLE: "chore: update images"
```

### Comparing `openstack-image-manager-0.2.6/.github/workflows/validate-configuration.yml` & `openstack-image-manager-0.3.0/.github/workflows/validate-configuration.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/Containerfile` & `openstack-image-manager-0.3.0/Containerfile`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/Dockerfile` & `openstack-image-manager-0.3.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/LICENSE` & `openstack-image-manager-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/PKG-INFO` & `openstack-image-manager-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstack-image-manager
-Version: 0.2.6
+Version: 0.3.0
 Summary: OpenStack image manager
 Home-page: https://github.com/osism/openstack-image-manager
 Author: OSISM community
 Author-email: info@osism.tech
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -24,9 +24,9 @@
 # openstack-image-manager
 
 [![PyPi version](https://badgen.net/pypi/v/openstack-image-manager/)](https://pypi.org/project/openstack-image-manager/)
 [![PyPi license](https://badgen.net/pypi/license/openstack-image-manager/)](https://pypi.org/project/openstack-image-manager/)
 
 Easily manage and keep up to date a large number of images on an OpenStack environment
 
-Documentation: <https://docs.osism.tech/openstack-image-manager/>
+Documentation: <https://docs.scs.community/docs/category/openstack-image-manager/>
```

### Comparing `openstack-image-manager-0.2.6/Pipfile.lock` & `openstack-image-manager-0.3.0/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9637522247648106%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'5815d8516002d1097aa337a720f60a3ed7025e766d2111f9c163db86f84da742'}}",*

 * * "'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7', "*

 * *              "'sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716'], "*

 * *              "'version': '==2023.5.7'}, 'cryptography': {'hashes': "*

 * *              "['sha256:0ddaee209d1cf1f180f1efa338a68c4621154de0afaef92b89486f5f96047c55', "*

 * *     […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "0fc2b3d5b506f6417e094aa0471afd1002e4b221cfd7c8d5120d9b3d24351bc0"
+            "sha256": "5815d8516002d1097aa337a720f60a3ed7025e766d2111f9c163db86f84da742"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9"
         },
         "sources": [
             {
@@ -48,19 +48,19 @@
                 "sha256:fbdaec13c5105f0c4e5c52614d04f0bca5f5af007910daa8b6b12095edaa67b3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==4.0.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -219,65 +219,54 @@
         "colorama": {
             "hashes": [
                 "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
                 "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
             "version": "==0.4.6"
         },
-        "commonmark": {
-            "hashes": [
-                "sha256:452f9dc859be7f06631ddcb328b6919c67984aca654e5fefb3914d54691aed60",
-                "sha256:da2f38c92590f83de410ba1a3cbceafbc74fee9def35f9251ba9a971d6d66fd9"
-            ],
-            "version": "==0.9.1"
-        },
         "cryptography": {
             "hashes": [
-                "sha256:103e8f7155f3ce2ffa0049fe60169878d47a4364b277906386f8de21c9234aa1",
-                "sha256:23df8ca3f24699167daf3e23e51f7ba7334d504af63a94af468f468b975b7dd7",
-                "sha256:2725672bb53bb92dc7b4150d233cd4b8c59615cd8288d495eaa86db00d4e5c06",
-                "sha256:30b1d1bfd00f6fc80d11300a29f1d8ab2b8d9febb6ed4a38a76880ec564fae84",
-                "sha256:35d658536b0a4117c885728d1a7032bdc9a5974722ae298d6c533755a6ee3915",
-                "sha256:50cadb9b2f961757e712a9737ef33d89b8190c3ea34d0fb6675e00edbe35d074",
-                "sha256:5f8c682e736513db7d04349b4f6693690170f95aac449c56f97415c6980edef5",
-                "sha256:6236a9610c912b129610eb1a274bdc1350b5df834d124fa84729ebeaf7da42c3",
-                "sha256:788b3921d763ee35dfdb04248d0e3de11e3ca8eb22e2e48fef880c42e1f3c8f9",
-                "sha256:8bc0008ef798231fac03fe7d26e82d601d15bd16f3afaad1c6113771566570f3",
-                "sha256:8f35c17bd4faed2bc7797d2a66cbb4f986242ce2e30340ab832e5d99ae60e011",
-                "sha256:b49a88ff802e1993b7f749b1eeb31134f03c8d5c956e3c125c75558955cda536",
-                "sha256:bc0521cce2c1d541634b19f3ac661d7a64f9555135e9d8af3980965be717fd4a",
-                "sha256:bc5b871e977c8ee5a1bbc42fa8d19bcc08baf0c51cbf1586b0e87a2694dde42f",
-                "sha256:c43ac224aabcbf83a947eeb8b17eaf1547bce3767ee2d70093b461f31729a480",
-                "sha256:d15809e0dbdad486f4ad0979753518f47980020b7a34e9fc56e8be4f60702fac",
-                "sha256:d7d84a512a59f4412ca8549b01f94be4161c94efc598bf09d027d67826beddc0",
-                "sha256:e029b844c21116564b8b61216befabca4b500e6816fa9f0ba49527653cae2108",
-                "sha256:e8a0772016feeb106efd28d4a328e77dc2edae84dfbac06061319fdb669ff828",
-                "sha256:e944fe07b6f229f4c1a06a7ef906a19652bdd9fd54c761b0ff87e83ae7a30354",
-                "sha256:eb40fe69cfc6f5cdab9a5ebd022131ba21453cf7b8a7fd3631f45bbf52bed612",
-                "sha256:fa507318e427169ade4e9eccef39e9011cdc19534f55ca2f36ec3f388c1f70f3",
-                "sha256:ffd394c7896ed7821a6d13b24657c6a34b6e2650bd84ae063cf11ccffa4f1a97"
+                "sha256:0ddaee209d1cf1f180f1efa338a68c4621154de0afaef92b89486f5f96047c55",
+                "sha256:14754bcdae909d66ff24b7b5f166d69340ccc6cb15731670435efd5719294895",
+                "sha256:344c6de9f8bda3c425b3a41b319522ba3208551b70c2ae00099c205f0d9fd3be",
+                "sha256:34d405ea69a8b34566ba3dfb0521379b210ea5d560fafedf9f800a9a94a41928",
+                "sha256:3680248309d340fda9611498a5319b0193a8dbdb73586a1acf8109d06f25b92d",
+                "sha256:3c5ef25d060c80d6d9f7f9892e1d41bb1c79b78ce74805b8cb4aa373cb7d5ec8",
+                "sha256:4ab14d567f7bbe7f1cdff1c53d5324ed4d3fc8bd17c481b395db224fb405c237",
+                "sha256:5c1f7293c31ebc72163a9a0df246f890d65f66b4a40d9ec80081969ba8c78cc9",
+                "sha256:6b71f64beeea341c9b4f963b48ee3b62d62d57ba93eb120e1196b31dc1025e78",
+                "sha256:7d92f0248d38faa411d17f4107fc0bce0c42cae0b0ba5415505df72d751bf62d",
+                "sha256:8362565b3835ceacf4dc8f3b56471a2289cf51ac80946f9087e66dc283a810e0",
+                "sha256:84a165379cb9d411d58ed739e4af3396e544eac190805a54ba2e0322feb55c46",
+                "sha256:88ff107f211ea696455ea8d911389f6d2b276aabf3231bf72c8853d22db755c5",
+                "sha256:9f65e842cb02550fac96536edb1d17f24c0a338fd84eaf582be25926e993dde4",
+                "sha256:a4fc68d1c5b951cfb72dfd54702afdbbf0fb7acdc9b7dc4301bbf2225a27714d",
+                "sha256:b7f2f5c525a642cecad24ee8670443ba27ac1fab81bba4cc24c7b6b41f2d0c75",
+                "sha256:b846d59a8d5a9ba87e2c3d757ca019fa576793e8758174d3868aecb88d6fc8eb",
+                "sha256:bf8fc66012ca857d62f6a347007e166ed59c0bc150cefa49f28376ebe7d992a2",
+                "sha256:f5d0bf9b252f30a31664b6f64432b4730bb7038339bd18b1fafe129cfc2be9be"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==39.0.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==41.0.0"
         },
         "decorator": {
             "hashes": [
                 "sha256:637996211036b6385ef91435e4fae22989472f9d571faba8927ba8253acbc330",
                 "sha256:b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==5.1.1"
         },
         "dogpile.cache": {
             "hashes": [
-                "sha256:3f0ca10b46b165e0b0e65e0e74b1a4b36187787b69db7c0f7073077adff2f05d",
-                "sha256:d844e8bb638cc4f544a4c89a834dfd36fe935400b71a16cbd744ebdfb720fd4e"
+                "sha256:1d0be0cef90505c9f24e9f00aedab8dce9356d28a4153d5660ab13eeb6a0cfd4",
+                "sha256:fa9c9c07640bdb66c5f5574e308123119b96c9a95c6856151d3fd2c91b4fb06a"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==1.1.8"
+            "version": "==1.2.1"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -313,43 +302,59 @@
                 "sha256:97cba51526c829282218feb99dab1b1e6bdf8efd1c43dc9d57be093c0d69c99a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.3"
         },
         "keystoneauth1": {
             "hashes": [
-                "sha256:d9f7484ad5fc9b0bbb7ecc3cbf3795a170694fbd848251331e54ba48bbeecc72",
-                "sha256:dc71d6a5d22bbf69b024d7dc7ca1e1213cbcc91a3a7d437a68cb3013a53d1633"
+                "sha256:84feba003301c2042693eb9366b0008eabd47b221c65f8106f0049f54eba989d",
+                "sha256:af54bcb9cf3b5d8492894ff8b6680447c8ef1fb880734a5d3ce3a78ed8459844"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==5.1.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==5.2.0"
         },
         "loguru": {
             "hashes": [
-                "sha256:066bd06758d0a513e9836fd9c6b5a75bfb3fd36841f4b996bc60b547a309d41c",
-                "sha256:4e2414d534a2ab57573365b3e6d0234dfb1d84b68b7f3b948e6fb743860a77c3"
+                "sha256:1612053ced6ae84d7959dd7d5e431a0532642237ec21f7fd83ac73fe539e03e1",
+                "sha256:b93aa30099fa6860d4727f1b81f8718e965bb96253fa190fab2077aaad6d15d3"
             ],
             "index": "pypi",
-            "version": "==0.6.0"
+            "version": "==0.7.0"
+        },
+        "markdown-it-py": {
+            "hashes": [
+                "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
+                "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.2.0"
+        },
+        "mdurl": {
+            "hashes": [
+                "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
+                "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.1.2"
         },
         "minio": {
             "hashes": [
-                "sha256:462aebd79000d5b923b2a728352014f76292bbd81a9d00e3ed25aa6ec4dc41f2",
-                "sha256:8828615a20cde82df79c5a52005252ad29bb022cde25177a4a43952a04c3222c"
+                "sha256:1afdf01c1bc8b57ddd12d438e3e168d625465b56f4d1c2af7576744c688e84c6",
+                "sha256:fcf8ac2cef310d5ddff2bef2c42f4e5a8bb546b87bca5bf8832135db054ca4e1"
             ],
             "index": "pypi",
-            "version": "==7.1.13"
+            "version": "==7.1.15"
         },
         "munch": {
             "hashes": [
-                "sha256:2d735f6f24d4dba3417fa448cae40c6e896ec1fdab6cdb5e6510999758a4dbd2",
-                "sha256:6f44af89a2ce4ed04ff8de41f70b226b984db10a91dcc7b9ac2efc1c77022fdd"
+                "sha256:0e4108418cfea898dcad01ff9569c30ff58f01d6f699331d04364f51623627c0",
+                "sha256:5284603030c00906d9d64d8108728c004fbeb91fc1c1e4caca342bc48f2a6dfd"
             ],
             "index": "pypi",
-            "version": "==2.5.0"
+            "version": "==3.0.0"
         },
         "natsort": {
             "hashes": [
                 "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
                 "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
             ],
             "index": "pypi",
@@ -388,34 +393,34 @@
                 "sha256:e76c7f351e0444721e85f975ae92718e21c1f361bda946d60a214061de1f00a1",
                 "sha256:eb4813b77d5df99903af4757ce980a98c4d702bbcb81f32a0b305a1537bdf0b1"
             ],
             "version": "==0.11.0"
         },
         "openstacksdk": {
             "hashes": [
-                "sha256:365e5dcca64e16e74a4f9f9d2a1f2207970e946d9a5c482549cfa5ec02ca2c98",
-                "sha256:b433bc3d22d6e645a653b0d48919b36bec033081d5d89daaa5d6800a0935e990"
+                "sha256:bc4b340fde80503b839bda72a32eb7d630ccde5c2c1ff4952840d79fca5bce7f",
+                "sha256:d73b5b9825b14230d8faca0acc9dbbfacf1299eb8eceae1f0f6900ed17aede6e"
             ],
             "index": "pypi",
-            "version": "==1.0.1"
+            "version": "==1.2.0"
         },
         "os-service-types": {
             "hashes": [
                 "sha256:0505c72205690910077fb72b88f2a1f07533c8d39f2fe75b29583481764965d6",
                 "sha256:31800299a82239363995b91f1ebf9106ac7758542a1e4ef6dc737a5932878c6c"
             ],
             "version": "==1.7.0"
         },
         "paramiko": {
             "hashes": [
-                "sha256:6950faca6819acd3219d4ae694a23c7a87ee38d084f70c1724b0c0dbb8b75769",
-                "sha256:f0caa660e797d9cd10db6fc6ae81e2c9b2767af75c3180fcd0e46158cd368d7f"
+                "sha256:93cdce625a8a1dc12204439d45033f3261bdb2c201648cfcdc06f9fd0f94ec29",
+                "sha256:df0f9dd8903bc50f2e10580af687f3015bf592a377cd438d2ec9546467a14eb8"
             ],
             "index": "pypi",
-            "version": "==3.1.0"
+            "version": "==3.2.0"
         },
         "patool": {
             "hashes": [
                 "sha256:3f642549c9a78f5b8bef1af92df385b521d360520d1f34e4dba3fd1dee2a21bc",
                 "sha256:e3180cf8bfe13bedbcf6f5628452fca0c2c84a3b5ae8c2d3f55720ea04cb1097"
             ],
             "index": "pypi",
@@ -434,19 +439,19 @@
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pynacl": {
             "hashes": [
                 "sha256:06b8f6fa7f5de8d5d2f7573fe8c863c051225a27b61e6860fd047b1775807858",
                 "sha256:0c84947a22519e013607c9be43706dd42513f9e6ae5d39d3613ca1e142fba44d",
                 "sha256:20f42270d27e1b6a29f54032090b972d97f0a1b0948cc52392041ef7831fee93",
                 "sha256:401002a4aaa07c9414132aaed7f6836ff98f59277a234704ff66878c2ee4a0d1",
@@ -504,47 +509,48 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
-            "version": "==2.28.2"
+            "version": "==2.31.0"
         },
         "requestsexceptions": {
             "hashes": [
                 "sha256:3083d872b6e07dc5c323563ef37671d992214ad9a32b0ca4a3d7f5500bf38ce3",
                 "sha256:b095cbc77618f066d459a02b137b020c37da9f46d9b057704019c9f77dba3065"
             ],
             "version": "==1.4.0"
         },
         "rich": {
             "hashes": [
-                "sha256:a4eb26484f2c82589bd9a17c73d32a010b1e29d89f1604cd9bf3a2097b81bb5e",
-                "sha256:ba3a3775974105c221d31141f2c116f4fd65c5ceb0698657a11e9f295ec93fd0"
+                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
+                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
             ],
-            "version": "==12.6.0"
+            "version": "==13.3.5"
         },
         "ruamel.yaml": {
             "hashes": [
-                "sha256:742b35d3d665023981bd6d16b3d24248ce5df75fdb4e2924e93a05c1f8b61ca7",
-                "sha256:8b7ce697a2f212752a35c1ac414471dc16c424c9573be4926b56ff3f5d23b7af"
+                "sha256:098ed1eb6d338a684891a72380277c1e6fc4d4ae0e120de9a447275056dda335",
+                "sha256:3cf153f0047ced526e723097ac615d3009371779432e304dbd5596b6f3a4c777"
             ],
             "index": "pypi",
-            "version": "==0.17.21"
+            "version": "==0.17.31"
         },
         "ruamel.yaml.clib": {
             "hashes": [
                 "sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e",
                 "sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3",
                 "sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5",
+                "sha256:1a6391a7cabb7641c32517539ca42cf84b87b667bad38b78d4d42dd23e957c81",
                 "sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497",
                 "sha256:2aa261c29a5545adfef9296b7e33941f46aa5bbd21164228e833412af4c9c75f",
                 "sha256:3110a99e0f94a4a3470ff67fc20d3f96c25b13d24c6980ff841e82bafe827cac",
                 "sha256:3243f48ecd450eddadc2d11b5feb08aca941b5cd98c9b1db14b2fd128be8c697",
                 "sha256:370445fd795706fd291ab00c9df38a0caed0f17a6fb46b0f607668ecb16ce763",
                 "sha256:40d030e2329ce5286d6b231b8726959ebbe0404c92f0a578c0e2482182e38282",
                 "sha256:41d0f1fa4c6830176eef5b276af04c89320ea616655d01327d5ce65e50575c94",
@@ -554,14 +560,15 @@
                 "sha256:721bc4ba4525f53f6a611ec0967bdcee61b31df5a56801281027a3a6d1c2daf5",
                 "sha256:763d65baa3b952479c4e972669f679fe490eee058d5aa85da483ebae2009d231",
                 "sha256:7bdb4c06b063f6fd55e472e201317a3bb6cdeeee5d5a38512ea5c01e1acbdd93",
                 "sha256:8831a2cedcd0f0927f788c5bdf6567d9dc9cc235646a434986a852af1cb54b4b",
                 "sha256:91a789b4aa0097b78c93e3dc4b40040ba55bef518f84a40d4442f713b4094acb",
                 "sha256:92460ce908546ab69770b2e576e4f99fbb4ce6ab4b245345a3869a0a0410488f",
                 "sha256:99e77daab5d13a48a4054803d052ff40780278240a902b880dd37a51ba01a307",
+                "sha256:9c7617df90c1365638916b98cdd9be833d31d337dbcd722485597b43c4a215bf",
                 "sha256:a234a20ae07e8469da311e182e70ef6b199d0fbeb6c6cc2901204dd87fb867e8",
                 "sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b",
                 "sha256:be2a7ad8fd8f7442b24323d24ba0b56c51219513cfa45b9ada3b87b76c374d4b",
                 "sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640",
                 "sha256:c3ca1fbba4ae962521e5eb66d72998b51f0f4d0f608d3c0347a48e1af262efa7",
                 "sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a",
                 "sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71",
@@ -571,15 +578,15 @@
                 "sha256:df5828871e6648db72d1c19b4bd24819b80a755c4541d3409f0f7acd0f335c80",
                 "sha256:ecdf1a604009bd35c674b9225a8fa609e0282d9b896c03dd441a91e5f53b534e",
                 "sha256:efa08d63ef03d079dcae1dfe334f6c8847ba8b645d08df286358b1f5293d24ab",
                 "sha256:f01da5790e95815eb5a8a138508c01c758e5f5bc0ce4286c4f7028b8dd7ac3d0",
                 "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646",
                 "sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38"
             ],
-            "markers": "python_version < '3.11' and platform_python_implementation == 'CPython'",
+            "markers": "python_version < '3.12' and platform_python_implementation == 'CPython'",
             "version": "==0.2.7"
         },
         "shellingham": {
             "hashes": [
                 "sha256:368bf8c00754fd4f55afb7bbb86e272df77e4dc76ac29dbcbb81a59e9fc15744",
                 "sha256:823bc5fb5c34d60f285b624e7264f4dda254bc803a3774a147bf99c0e3004a28"
             ],
@@ -591,46 +598,54 @@
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
         "stevedore": {
             "hashes": [
-                "sha256:2c428d2338976279e8eb2196f7a94910960d9f7ba2f41f3988511e95ca447021",
-                "sha256:bd5a71ff5e5e5f5ea983880e4a1dd1bb47f8feebbb3d95b592398e2f02194771"
+                "sha256:8cc040628f3cea5d7128f2e76cf486b2251a4e543c7b938f58d9a377f6694a2d",
+                "sha256:a54534acf9b89bc7ed264807013b505bf07f74dbe4bcfa37d32bd063870b087c"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==5.0.0"
+            "version": "==5.1.0"
         },
         "tabulate": {
             "hashes": [
                 "sha256:0095b12bf5966de529c0feb1fa08671671b3368eec77d7ef7ab114be2c068b3c",
                 "sha256:024ca478df22e9340661486f85298cff5f6dcdba14f3813e8830015b9ed1948f"
             ],
             "index": "pypi",
             "version": "==0.9.0"
         },
         "typer": {
             "extras": [
                 "all"
             ],
             "hashes": [
-                "sha256:b5e704f4e48ec263de1c0b3a2387cd405a13767d2f907f44c1a08cbad96f606d",
-                "sha256:ff797846578a9f2a201b53442aedeb543319466870fbe1c701eab66dd7681165"
+                "sha256:50922fd79aea2f4751a8e0408ff10d2662bd0c8bbfa84755a699f3bada2978b2",
+                "sha256:5d96d986a21493606a358cae4461bd8cdf83cbf33a5aa950ae629ca3b51467ee"
             ],
             "index": "pypi",
-            "version": "==0.7.0"
+            "version": "==0.9.0"
+        },
+        "typing-extensions": {
+            "hashes": [
+                "sha256:06006244c70ac8ee83fa8282cb188f697b8db25bc8b4df07be1873c43897060c",
+                "sha256:3a8b36f13dd5fdc5d1b16fe317f5668545de77fa0b8e02006381fd49d731ab98"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==4.6.2"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
+                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.2"
         },
         "yamale": {
             "hashes": [
                 "sha256:04f914c0886bda03ac20f8468272cfd9374a634a062549490eff2beedeb30497",
                 "sha256:e524caf71cbbbd15aa295e8bdda01688ac4b5edaf38dd60851ddff6baef383ba"
             ],
             "index": "pypi",
```

### Comparing `openstack-image-manager-0.2.6/doc/conf.py` & `openstack-image-manager-0.3.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/doc/configuration.md` & `openstack-image-manager-0.3.0/doc/configuration.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/doc/contribute.md` & `openstack-image-manager-0.3.0/doc/contribute.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/doc/getting_started.md` & `openstack-image-manager-0.3.0/doc/getting_started.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/doc/images/logo.png` & `openstack-image-manager-0.3.0/doc/images/logo.png`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/doc/overview.md` & `openstack-image-manager-0.3.0/doc/overview.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/doc/quickstart.md` & `openstack-image-manager-0.3.0/doc/quickstart.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/doc/requirements.md` & `openstack-image-manager-0.3.0/doc/requirements.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/etc/images/almalinux.yml` & `openstack-image-manager-0.3.0/etc/images/almalinux.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ---
 images:
   - name: AlmaLinux 8
+    enable: true
     shortname: almalinux-8
     format: qcow2
     login: almalinux
     min_disk: 10
     min_ram: 512
     status: active
     visibility: public
@@ -18,21 +19,24 @@
       os_distro: centos
       os_version: '8'
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://repo.almalinux.org/almalinux/8/cloud/x86_64/images/CHECKSUM
-    latest_url: https://repo.almalinux.org/almalinux/8/cloud/x86_64/images/AlmaLinux-8-GenericCloud-latest.x86_64.qcow2
+    latest_url: 
+      https://repo.almalinux.org/almalinux/8/cloud/x86_64/images/AlmaLinux-8-GenericCloud-latest.x86_64.qcow2
     versions:
-      - version: '20221111'
-        url: https://minio.services.osism.tech/openstack-image-manager/almalinux-8/20221111-almalinux-8.qcow2
-        checksum: sha256:9505239cbaf56fae0abc93a2dba312606540014fcc01e74f196edac0b5fbe783
-        build_date: 2022-11-11
+      - version: '20230524'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/almalinux-8/20230524-almalinux-8.qcow2
+        checksum: sha256:c0ad09255d91288dac590d99c95197d83a2846f1bcbec3f4222fb04265a2a4d7
+        build_date: '2023-05-24'
   - name: AlmaLinux 9
+    enable: true
     shortname: almalinux-9
     format: qcow2
     login: almalinux
     min_disk: 10
     min_ram: 512
     status: active
     visibility: public
@@ -46,13 +50,15 @@
       os_distro: centos
       os_version: '9'
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://repo.almalinux.org/almalinux/9/cloud/x86_64/images/CHECKSUM
-    latest_url: https://repo.almalinux.org/almalinux/9/cloud/x86_64/images/AlmaLinux-9-GenericCloud-latest.x86_64.qcow2
+    latest_url: 
+      https://repo.almalinux.org/almalinux/9/cloud/x86_64/images/AlmaLinux-9-GenericCloud-latest.x86_64.qcow2
     versions:
-      - version: '20221118'
-        url: https://minio.services.osism.tech/openstack-image-manager/almalinux-9/20221118-almalinux-9.qcow2
-        checksum: sha256:1e93210a0c534de76ae01dc02e8224be14264fa8d54ad6cff9af15b673c6db1a
-        build_date: 2022-11-18
+      - version: '20230513'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/almalinux-9/20230513-almalinux-9.qcow2
+        checksum: sha256:207d885ca8140e3106098e946cfc04088b0e21f50d24815051520d452eae0a50
+        build_date: '2023-05-13'
```

### Comparing `openstack-image-manager-0.2.6/etc/images/centos.yml` & `openstack-image-manager-0.3.0/etc/images/centos.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ---
 images:
   - name: CentOS 7
+    enable: false
     shortname: centos-7
     format: qcow2
     login: centos
     min_disk: 8
     min_ram: 512
     status: active
     visibility: public
@@ -18,21 +19,24 @@
       os_distro: centos
       os_version: '7'
       replace_frequency: critical_bug
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud.centos.org/centos/7/images/sha256sum.txt
-    latest_url: https://cloud.centos.org/centos/7/images/CentOS-7-x86_64-GenericCloud-HEREBE\d+\.qcow2$DRAGONS
+    latest_url: 
+      https://cloud.centos.org/centos/7/images/CentOS-7-x86_64-GenericCloud-HEREBE\d+\.qcow2$DRAGONS
     versions:
       - version: '20201112'
-        url: https://minio.services.osism.tech/openstack-image-manager/centos-7/20201112-centos-7.qcow2
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/centos-7/20201112-centos-7.qcow2
         checksum: sha256:e38bab0475cc6d004d2e17015969c659e5a308111851b0e2715e84646035bdd3
         build_date: 2020-11-12
   - name: CentOS Stream 8
+    enable: true
     shortname: centos-stream-8
     format: qcow2
     login: centos
     min_disk: 10
     min_ram: 512
     status: active
     visibility: public
@@ -46,21 +50,24 @@
       os_distro: centos
       os_version: '8'
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud.centos.org/centos/8-stream/x86_64/images/CHECKSUM
-    latest_url: https://cloud.centos.org/centos/8-stream/x86_64/images/CentOS-Stream-GenericCloud-8-HEREBE\d+\.\dDRAGONS.x86_64.qcow2
+    latest_url: 
+      https://cloud.centos.org/centos/8-stream/x86_64/images/CentOS-Stream-GenericCloud-8-HEREBE\d+\.\dDRAGONS.x86_64.qcow2
     versions:
-      - version: '20220913'
-        url: https://minio.services.osism.tech/openstack-image-manager/centos-stream-8/20220913-centos-stream-8.qcow2
-        checksum: sha256:8717251f8e4d2fe3e5032799caae89358c1ba68d65a16b5128a59ec6003aac1c
-        build_date: 2022-09-13
+      - version: '20230608'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/centos-stream-8/20230608-centos-stream-8.qcow2
+        checksum: sha256:b8bf004b0f1d9924d9516ff4ad1ecfcf2300469d811a18bc605c45c9732faaaa
+        build_date: '2023-06-08'
   - name: CentOS Stream 9
+    enable: true
     shortname: centos-stream-9
     format: qcow2
     login: centos
     min_disk: 10
     min_ram: 512
     status: active
     visibility: public
@@ -74,13 +81,15 @@
       os_distro: centos
       os_version: '9'
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud.centos.org/centos/9-stream/x86_64/images/CHECKSUM
-    latest_url: https://cloud.centos.org/centos/9-stream/x86_64/images/CentOS-Stream-GenericCloud-9-HEREBE\d+\.\dDRAGONS.x86_64.qcow2
+    latest_url: 
+      https://cloud.centos.org/centos/9-stream/x86_64/images/CentOS-Stream-GenericCloud-9-HEREBE\d+\.\dDRAGONS.x86_64.qcow2
     versions:
-      - version: '20230308'
-        url: https://minio.services.osism.tech/openstack-image-manager/centos-stream-9/20230308-centos-stream-9.qcow2
-        checksum: sha256:2630ea63ddff00b81e2189b6af13e35c9db943049a7ab7c35fe4b558a661496a
-        build_date: '2023-03-08'
+      - version: '20230606'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/centos-stream-9/20230606-centos-stream-9.qcow2
+        checksum: sha256:6193a49c545425f99d23f59ea792f79a7a6b2e3557fc2d3f6d42c3e5274061de
+        build_date: '2023-06-06'
```

### Comparing `openstack-image-manager-0.2.6/etc/images/cirros.yml` & `openstack-image-manager-0.3.0/etc/images/cirros.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ---
 images:
 
   - name: Cirros
+    enable: true
     format: qcow2
     login: cirros
     password: gocubsgo
     min_disk: 1
     min_ram: 32
     status: active
     visibility: public
```

### Comparing `openstack-image-manager-0.2.6/etc/images/clearlinux.yml` & `openstack-image-manager-0.3.0/etc/images/fedora.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 ---
 images:
 
-  - name: Clear Linux
-    shortname: clearlinux
+  - name: Fedora 37
+    enable: true
+    shortname: fedora-37
     format: qcow2
-    login: root
-    min_disk: 1
+    login: fedora
+    min_disk: 4
     min_ram: 512
     status: active
     visibility: public
-    multi: false
+    multi: true
     meta:
       architecture: x86_64
       hw_disk_bus: scsi
-      hw_rng_model: virtio
       hw_scsi_model: virtio-scsi
+      hw_rng_model: virtio
       hw_watchdog_action: reset
-      os_distro: clearlinux
-      replace_frequency: never
-      uuid_validity: none
+      os_distro: fedora
+      os_version: '37'
+      replace_frequency: quarterly
+      uuid_validity: last-3
       provided_until: none
     tags: []
     versions:
-      - version: '35440'
-        url: https://minio.services.osism.tech/openstack-image-manager/clearlinux/35440/clear-35440-cloudguest.img
-        source: https://cdn.download.clearlinux.org/releases/35440/clear/clear-35440-cloudguest.img.xz
-        checksum: "sha256:5e03015be709a893e8d3b7134f7b453862287fea5aabe0b6cb17273bb963701f"
-        build_date: 2021-12-17
+      - version: '20230402'
+        url: https://minio.services.osism.tech/openstack-image-manager/fedora-37/20230402/Fedora-Cloud-Base-37-1.7.x86_64.qcow2
+        source: https://download.fedoraproject.org/pub/fedora/linux/releases/37/Cloud/x86_64/images/Fedora-Cloud-Base-37-1.7.x86_64.qcow2
+        checksum: "sha256:b5b9bec91eee65489a5745f6ee620573b23337cbb1eb4501ce200b157a01f3a0"
+        build_date: '2022-11-05'
```

### Comparing `openstack-image-manager-0.2.6/etc/images/debian.yml` & `openstack-image-manager-0.3.0/etc/images/debian.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ---
 images:
   - name: Debian 10
+    enable: true
     shortname: debian-10
     format: qcow2
     login: debian
     min_disk: 8
     min_ram: 512
     status: active
     visibility: public
@@ -18,21 +19,25 @@
       os_distro: debian
       os_version: '10'
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cdimage.debian.org/cdimage/cloud/buster/latest/SHA512SUMS
-    latest_url: https://cdimage.debian.org/cdimage/cloud/buster/latest/debian-10-genericcloud-amd64.qcow2
+    latest_url: 
+      https://cdimage.debian.org/cdimage/cloud/buster/latest/debian-10-genericcloud-amd64.qcow2
     versions:
-      - version: '20230223'
-        url: https://minio.services.osism.tech/openstack-image-manager/debian-10/20230223-debian-10.qcow2
-        checksum: sha512:9522ebd80d7577d7a679bb876d7aa4da066947986809ccf75ae140b26550aa8cf7c46a38084941bd316cfab602565581aa5f1efd66538b9577b7559154c30356
-        build_date: '2023-02-23'
+      - version: '20230601'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/debian-10/20230601-debian-10.qcow2
+        checksum: 
+          sha512:d8956fecfff4a176190b77484657e581bb1f7ceaacce6e905e5ab62a899d120e9a7a120c9c4acad89fb29b3e3b6c6666f9579e0e0409bb50ac642bf800b5b918
+        build_date: '2023-06-01'
   - name: Debian 11
+    enable: true
     shortname: debian-11
     format: qcow2
     login: debian
     min_disk: 8
     min_ram: 512
     status: active
     visibility: public
@@ -45,13 +50,47 @@
       os_distro: debian
       os_version: '11'
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cdimage.debian.org/cdimage/cloud/bullseye/latest/SHA512SUMS
-    latest_url: https://cdimage.debian.org/cdimage/cloud/bullseye/latest/debian-11-genericcloud-amd64.qcow2
+    latest_url: 
+      https://cdimage.debian.org/cdimage/cloud/bullseye/latest/debian-11-genericcloud-amd64.qcow2
     versions:
-      - version: '20230124'
-        url: https://minio.services.osism.tech/openstack-image-manager/debian-11/20230124-debian-11.qcow2
-        checksum: sha512:7a7a546b9928f0d375c332a39db2d1af56fce3432b8a5dee0d4f71777efa7463a6b1fc797bcf3b12ca7d8f47d66824abbcbf0a0bdc94be5e90e5a90e8628fae6
-        build_date: 2023-01-24
+      - version: '20230602'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/debian-11/20230602-debian-11.qcow2
+        checksum: 
+          sha512:83227f671b403b73ed6e870273500153240b828a2625b16090dd4e1a2847ce51a081503564a183506093fc24f10f6656dca4c9f6ac1e0a24e1e0f7986b32757c
+        build_date: '2023-06-02'
+  - name: Debian 12
+    enable: true
+    shortname: debian-12
+    format: qcow2
+    login: debian
+    min_disk: 8
+    min_ram: 512
+    status: active
+    visibility: public
+    multi: true
+    meta:
+      architecture: x86_64
+      hw_disk_bus: scsi
+      hw_scsi_model: virtio-scsi
+      hw_watchdog_action: reset
+      os_distro: debian
+      os_version: '12'
+      replace_frequency: quarterly
+      uuid_validity: last-3
+      provided_until: none
+    tags: []
+    latest_checksum_url: https://cdimage.debian.org/cdimage/cloud/bookworm/daily/latest/SHA512SUMS
+    latest_url: 
+      https://cdimage.debian.org/cdimage/cloud/bookworm/daily/latest/debian-12-genericcloud-amd64-daily.qcow2
+    versions:
+      - build_date: '2023-06-09'
+        checksum: 
+          sha512:4d817039e11418c3e3cf7fc46a130dcac21b27322128c13d2f83fe4aa3684cabb8ff28efee54b2a106a851b04115de293c51acfe552bf50d85a1b3dd3d59a916
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/debian-12/20230609-debian-12.qcow2
+        version: '20230609'
```

### Comparing `openstack-image-manager-0.2.6/etc/images/fedora.yml` & `openstack-image-manager-0.3.0/etc/images/clearlinux.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 ---
 images:
 
-  - name: Fedora 36
-    shortname: fedora-36
+  - name: Clear Linux
+    enable: false
+    shortname: clearlinux
     format: qcow2
-    login: fedora
-    min_disk: 4
+    login: root
+    min_disk: 1
     min_ram: 512
     status: active
     visibility: public
-    multi: true
+    multi: false
     meta:
       architecture: x86_64
       hw_disk_bus: scsi
-      hw_scsi_model: virtio-scsi
       hw_rng_model: virtio
+      hw_scsi_model: virtio-scsi
       hw_watchdog_action: reset
-      os_distro: fedora
-      os_version: '36'
-      replace_frequency: quarterly
-      uuid_validity: last-3
+      os_distro: clearlinux
+      replace_frequency: never
+      uuid_validity: none
       provided_until: none
     tags: []
     versions:
-      - version: '20220504'
-        url: https://minio.services.osism.tech/openstack-image-manager/fedora-36/20220504/Fedora-Cloud-Base-36-1.5.x86_64.qcow2
-        source: https://mirror.23m.com/fedora/linux/releases/36/Cloud/x86_64/images/Fedora-Cloud-Base-36-1.5.x86_64.qcow2
-        checksum: "sha256:ca9e514cc2f4a7a0188e7c68af60eb4e573d2e6850cc65b464697223f46b4605"
-        build_date: 2022-05-04
+      - version: '38700'
+        url: https://minio.services.osism.tech/openstack-image-manager/clearlinux/38700/clear-38700-cloudguest.img
+        source: https://cdn.download.clearlinux.org/releases/38700/clear/clear-38700-cloudguest.img.xz
+        checksum: "sha256:554f2e9f1c5cd3caa7ca9043e9379ab7bac36f8004ae6023f2fb642b80ace173"
+        build_date: '2023-03-31'
```

### Comparing `openstack-image-manager-0.2.6/etc/images/flatcar.yml` & `openstack-image-manager-0.3.0/etc/images/flatcar.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ---
 images:
 
   - name: Flatcar Container Linux
+    enable: false
     shortname: flatcar
     format: qcow2
     login: root
     min_disk: 10
     min_ram: 2048
     status: active
     visibility: public
```

### Comparing `openstack-image-manager-0.2.6/etc/images/gardenlinux.yml` & `openstack-image-manager-0.3.0/etc/images/gardenlinux.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ---
 images:
   - name: Garden Linux
+    enable: true
     format: qcow2
     login: admin
     min_disk: 10
     min_ram: 512
     status: active
     visibility: public
     multi: false
@@ -20,11 +21,15 @@
       provided_until: none
     tags: []
     versions:
       - version: '576.12'
         url: https://minio.services.osism.tech/openstack-image-gardenlinux/gardenlinux-amd64.576.12.qcow2
         checksum: "sha256:6f1b68b2c36d22add37a81f89f30e47083ea473bfe92d36faf5bfe722e19e109"
         build_date: 2022-09-09
-      - version: '934.2'
-        url: https://minio.services.osism.tech/openstack-image-gardenlinux/gardenlinux-amd64.934.2.qcow2
-        checksum: "sha256:949082a3394276672228fad993e1d1d06b490b96d0cd6aea001231162473bffc"
-        build_date: 2023-01-13
+      - version: '934.8'
+        url: https://minio.services.osism.tech/openstack-image-gardenlinux/gardenlinux-amd64.934.8.qcow2
+        checksum: "sha256:68a4cb768224aec313a8c974cec412fe8b2754f0189a318ce9dbdba13fd89597"
+        build_date: 2023-05-12
+      - version: '934.9'
+        url: https://minio.services.osism.tech/openstack-image-gardenlinux/gardenlinux-amd64.934.9.qcow2
+        checksum: "sha256:314aa8369a46a7c9fd97343a688c75b9c282f654fb05e9bb4d6b94646bf3670c"
+        build_date: 2023-06-03
```

### Comparing `openstack-image-manager-0.2.6/etc/images/opensuse.yml` & `openstack-image-manager-0.3.0/etc/images/opensuse.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ---
 images:
   - name: openSUSE Leap 15.4
+    enable: true
     shortname: opensuse-leap-15.4
     format: qcow2
     login: opensuse
     min_disk: 10
     min_ram: 512
     status: active
     visibility: public
```

### Comparing `openstack-image-manager-0.2.6/etc/images/rockylinux.yml` & `openstack-image-manager-0.3.0/etc/images/rockylinux.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ---
 images:
   - name: Rocky 8
+    enable: true
     shortname: rocky-8
     format: qcow2
     login: rocky
     min_disk: 10
     min_ram: 512
     status: active
     visibility: public
@@ -17,22 +18,26 @@
       hw_watchdog_action: reset
       os_distro: centos
       os_version: '8'
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
-    latest_checksum_url: https://download.rockylinux.org/pub/rocky/8/images/CHECKSUM
-    latest_url: https://download.rockylinux.org/pub/rocky/8/images/Rocky-8-GenericCloud.latest.x86_64.qcow2
+    latest_checksum_url: 
+      https://download.rockylinux.org/pub/rocky/8/images/x86_64/Rocky-8-GenericCloud.latest.x86_64.qcow2.CHECKSUM
+    latest_url: 
+      https://download.rockylinux.org/pub/rocky/8/images/x86_64/Rocky-8-GenericCloud.latest.x86_64.qcow2
     versions:
-      - version: '20220703'
-        url: https://minio.services.osism.tech/openstack-image-manager/rocky-8/20220703-rocky-8.qcow2
-        checksum: sha256:7b786a39eeb96e22dd85386377ff186737f6c1b9a5faa105b0a0a7a4895c29d0
-        build_date: 2022-07-03
+      - version: '20230518'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/rocky-8/20230518-rocky-8.qcow2
+        checksum: sha256:086bf68f84c974cfcf533741c5be8752270df681a38f20423cf24b851d5edf77
+        build_date: '2023-05-18'
   - name: Rocky 9
+    enable: true
     shortname: rocky-9
     format: qcow2
     login: rocky
     min_disk: 10
     min_ram: 512
     status: active
     visibility: public
@@ -45,14 +50,17 @@
       hw_watchdog_action: reset
       os_distro: centos
       os_version: '9'
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
-    latest_checksum_url: https://download.rockylinux.org/pub/rocky/9/images/x86_64/Rocky-9-GenericCloud.latest.x86_64.qcow2.CHECKSUM
-    latest_url: https://download.rockylinux.org/pub/rocky/9/images/x86_64/Rocky-9-GenericCloud.latest.x86_64.qcow2
+    latest_checksum_url: 
+      https://download.rockylinux.org/pub/rocky/9/images/x86_64/Rocky-9-GenericCloud.latest.x86_64.qcow2.CHECKSUM
+    latest_url: 
+      https://download.rockylinux.org/pub/rocky/9/images/x86_64/Rocky-9-GenericCloud.latest.x86_64.qcow2
     versions:
-      - version: '20220830'
-        url: https://minio.services.osism.tech/openstack-image-manager/rocky-9/20220830-rocky-9.qcow2
-        checksum: sha256:f02570e0ad3653df7f56baa8157739dbe92a003234acd5824dcf94d24694e20b
-        build_date: 2022-08-30
+      - version: '20230515'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/rocky-9/20230515-rocky-9.qcow2
+        checksum: sha256:50510f98abe1b20a548102a05a9be83153b0bf634fc502d5c8d1f508f6de1430
+        build_date: '2023-05-15'
```

### Comparing `openstack-image-manager-0.2.6/etc/images/ubuntu.yml` & `openstack-image-manager-0.3.0/etc/images/ubuntu.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ---
 images:
   - name: Ubuntu 14.04
+    enable: false
     shortname: ubuntu-14.04
     format: qcow2
     login: ubuntu
     min_disk: 8
     min_ram: 512
     status: active
     visibility: public
@@ -18,21 +19,24 @@
       os_distro: ubuntu
       os_version: '14.04'
       replace_frequency: never
       uuid_validity: none
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud-images.ubuntu.com/trusty/current/SHA256SUMS
-    latest_url: https://cloud-images.ubuntu.com/trusty/current/trusty-server-cloudimg-amd64-disk1.img
+    latest_url: 
+      https://cloud-images.ubuntu.com/trusty/current/trusty-server-cloudimg-amd64-disk1.img
     versions:
       - version: '20191107'
-        url: https://minio.services.osism.tech/openstack-image-manager/ubuntu-14.04/20191107-ubuntu-14.04.qcow2
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/ubuntu-14.04/20191107-ubuntu-14.04.qcow2
         checksum: sha256:3c4ad0defbe729dd3c16d2851d775575d1c5351c85734418d3b89bfdfd28ebd1
         build_date: 2019-11-07
   - name: Ubuntu 16.04
+    enable: false
     shortname: ubuntu-16.04
     format: qcow2
     login: ubuntu
     min_disk: 8
     min_ram: 512
     status: active
     visibility: public
@@ -46,21 +50,24 @@
       os_distro: ubuntu
       os_version: '16.04'
       replace_frequency: never
       uuid_validity: none
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud-images.ubuntu.com/xenial/current/SHA256SUMS
-    latest_url: https://cloud-images.ubuntu.com/xenial/current/xenial-server-cloudimg-amd64-disk1.img
+    latest_url: 
+      https://cloud-images.ubuntu.com/xenial/current/xenial-server-cloudimg-amd64-disk1.img
     versions:
       - version: '20211001'
-        url: https://minio.services.osism.tech/openstack-image-manager/ubuntu-16.04/20211001-ubuntu-16.04.qcow2
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/ubuntu-16.04/20211001-ubuntu-16.04.qcow2
         checksum: sha256:fff2494a70bcaffb59f26f71ec49e137dd87d319341c35832dbe0ea65ff15140
         build_date: 2021-10-01
   - name: Ubuntu 16.04 Minimal
+    enable: false
     shortname: ubuntu-16.04-minimal
     format: qcow2
     login: ubuntu
     min_disk: 8
     min_ram: 512
     status: active
     visibility: public
@@ -74,21 +81,24 @@
       os_distro: ubuntu
       os_version: '16.04'
       replace_frequency: never
       uuid_validity: none
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud-images.ubuntu.com/minimal/releases/xenial/release/SHA256SUMS
-    latest_url: https://cloud-images.ubuntu.com/minimal/releases/xenial/release/ubuntu-16.04-minimal-cloudimg-amd64-disk1.img
+    latest_url: 
+      https://cloud-images.ubuntu.com/minimal/releases/xenial/release/ubuntu-16.04-minimal-cloudimg-amd64-disk1.img
     versions:
       - version: '20210929'
-        url: https://minio.services.osism.tech/openstack-image-manager/ubuntu-16.04-minimal/20210929-ubuntu-16.04-minimal.qcow2
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/ubuntu-16.04-minimal/20210929-ubuntu-16.04-minimal.qcow2
         checksum: sha256:7658ec30373e7ad1a1858744f395a89713d333721d7d1986ee8b71680b81a0a9
         build_date: 2021-09-20
   - name: Ubuntu 18.04
+    enable: false
     shortname: ubuntu-18.04
     format: qcow2
     login: ubuntu
     min_disk: 8
     min_ram: 512
     status: active
     visibility: public
@@ -104,19 +114,21 @@
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud-images.ubuntu.com/bionic/current/SHA256SUMS
     latest_url: https://cloud-images.ubuntu.com/bionic/current/bionic-server-cloudimg-amd64.img
     versions:
-      - version: '20230303'
-        url: https://minio.services.osism.tech/openstack-image-manager/ubuntu-18.04/20230303-ubuntu-18.04.qcow2
-        checksum: sha256:75deaa0e8fa5f2751c0864251e43fb62e8da2f059c201e60f194eb9a0b43b03f
-        build_date: '2023-03-03'
+      - version: '20230607'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/ubuntu-18.04/20230607-ubuntu-18.04.qcow2
+        checksum: sha256:8dd2e6b5e5aad20c3f836123b300cba9861249408cbb07c359145a65d6bab6b6
+        build_date: '2023-06-07'
   - name: Ubuntu 18.04 Minimal
+    enable: false
     shortname: ubuntu-18.04-minimal
     format: qcow2
     login: ubuntu
     min_disk: 8
     min_ram: 512
     status: active
     visibility: public
@@ -130,21 +142,24 @@
       os_distro: ubuntu
       os_version: '18.04'
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud-images.ubuntu.com/minimal/releases/bionic/release/SHA256SUMS
-    latest_url: https://cloud-images.ubuntu.com/minimal/releases/bionic/release/ubuntu-18.04-minimal-cloudimg-amd64.img
+    latest_url: 
+      https://cloud-images.ubuntu.com/minimal/releases/bionic/release/ubuntu-18.04-minimal-cloudimg-amd64.img
     versions:
-      - version: '20230307'
-        url: https://minio.services.osism.tech/openstack-image-manager/ubuntu-18.04-minimal/20230307-ubuntu-18.04-minimal.qcow2
-        checksum: sha256:96c3a40acf7360a4ea4750cc035f1e3d6ce3fdb8b36fe7bb193252200ddbfd7f
-        build_date: '2023-03-07'
+      - version: '20230602'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/ubuntu-18.04-minimal/20230602-ubuntu-18.04-minimal.qcow2
+        checksum: sha256:2d9755669c499e88d51da0638cd20e0983a248828e2153906c013bea0ee2f45a
+        build_date: '2023-06-02'
   - name: Ubuntu 20.04
+    enable: true
     shortname: ubuntu-20.04
     format: qcow2
     login: ubuntu
     min_disk: 8
     min_ram: 512
     status: active
     visibility: public
@@ -160,19 +175,21 @@
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud-images.ubuntu.com/focal/current/SHA256SUMS
     latest_url: https://cloud-images.ubuntu.com/focal/current/focal-server-cloudimg-amd64.img
     versions:
-      - version: '20230215'
-        url: https://minio.services.osism.tech/openstack-image-manager/ubuntu-20.04/20230215-ubuntu-20.04.qcow2
-        checksum: sha256:786a425717f411be89c41c88420a14471e1888569f9193cfb3b7dbb56e6a538f
-        build_date: '2023-02-15'
+      - version: '20230607'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/ubuntu-20.04/20230607-ubuntu-20.04.qcow2
+        checksum: sha256:e386db128554f8b866cff311955e099efd00c3d51cda5d592ee430d76f67dcb0
+        build_date: '2023-06-07'
   - name: Ubuntu 20.04 Minimal
+    enable: true
     shortname: ubuntu-20.04-minimal
     format: qcow2
     login: ubuntu
     min_disk: 8
     min_ram: 512
     status: active
     visibility: public
@@ -186,21 +203,24 @@
       os_distro: ubuntu
       os_version: '20.04'
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud-images.ubuntu.com/minimal/releases/focal/release/SHA256SUMS
-    latest_url: https://cloud-images.ubuntu.com/minimal/releases/focal/release/ubuntu-20.04-minimal-cloudimg-amd64.img
+    latest_url: 
+      https://cloud-images.ubuntu.com/minimal/releases/focal/release/ubuntu-20.04-minimal-cloudimg-amd64.img
     versions:
-      - version: '20230303'
-        url: https://minio.services.osism.tech/openstack-image-manager/ubuntu-20.04-minimal/20230303-ubuntu-20.04-minimal.qcow2
-        checksum: sha256:ec0e98854677ace76d33bdc57478f14369bb353c1e660acfe4fd958aaf0e9c04
-        build_date: '2023-03-03'
+      - version: '20230606'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/ubuntu-20.04-minimal/20230606-ubuntu-20.04-minimal.qcow2
+        checksum: sha256:201a642529acca34b731457d586ae21858098849b9bce39fe3936db19d689d65
+        build_date: '2023-06-06'
   - name: Ubuntu 22.04
+    enable: true
     shortname: ubuntu-22.04
     format: qcow2
     login: ubuntu
     min_disk: 8
     min_ram: 512
     status: active
     visibility: public
@@ -216,19 +236,21 @@
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud-images.ubuntu.com/jammy/current/SHA256SUMS
     latest_url: https://cloud-images.ubuntu.com/jammy/current/jammy-server-cloudimg-amd64.img
     versions:
-      - version: '20230311'
-        url: https://minio.services.osism.tech/openstack-image-manager/ubuntu-22.04/20230311-ubuntu-22.04.qcow2
-        checksum: sha256:70c3e63539a61e7ef8a88296fc3e3048b7f74754bea904734414bf40bdb5bedf
-        build_date: '2023-03-11'
+      - version: '20230608'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/ubuntu-22.04/20230608-ubuntu-22.04.qcow2
+        checksum: sha256:929965d004dd89417d3aedc3a05d13e6f208ce7177d1cc38c993c0e02538be93
+        build_date: '2023-06-08'
   - name: Ubuntu 22.04 Minimal
+    enable: true
     shortname: ubuntu-22.04-minimal
     format: qcow2
     login: ubuntu
     min_disk: 8
     min_ram: 512
     status: active
     visibility: public
@@ -242,13 +264,15 @@
       os_distro: ubuntu
       os_version: '22.04'
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud-images.ubuntu.com/minimal/releases/jammy/release/SHA256SUMS
-    latest_url: https://cloud-images.ubuntu.com/minimal/releases/jammy/release/ubuntu-22.04-minimal-cloudimg-amd64.img
+    latest_url: 
+      https://cloud-images.ubuntu.com/minimal/releases/jammy/release/ubuntu-22.04-minimal-cloudimg-amd64.img
     versions:
-      - version: '20230309'
-        url: https://minio.services.osism.tech/openstack-image-manager/ubuntu-22.04-minimal/20230309-ubuntu-22.04-minimal.qcow2
-        checksum: sha256:811eb8e45937dda484ed55ccc4474e9e50f32dc46d7aa171791451dd03253418
-        build_date: '2023-03-09'
+      - version: '20230606'
+        url: 
+          https://minio.services.osism.tech/openstack-image-manager/ubuntu-22.04-minimal/20230606-ubuntu-22.04-minimal.qcow2
+        checksum: sha256:83b441bed3b65042d8993570ea7e9c35d3d88c5ae96dec25fc2efa4721d5a92f
+        build_date: '2023-06-06'
```

### Comparing `openstack-image-manager-0.2.6/etc/schema.yaml` & `openstack-image-manager-0.3.0/etc/schema.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ---
 images: list(include('image'), min=1)
 
 ---
 image:
+  enable: bool()
   format: enum('aki', 'ari', 'ami', 'raw', 'iso', 'vhd', 'vdi', 'qcow2', 'vmdk')
   latest_checksum_url: regex('^(http|ftp)s?:\/\/\w+.*', name='valid URL', required=False)
   latest_url: regex('^(http|ftp)s?:\/\/\w+.*', name='valid URL', required=False)
   login: str()
   meta: include('meta', required=True)
   min_disk: int(min=0)
   min_ram: int(min=0)
@@ -24,15 +25,15 @@
   architecture: enum('x86_64', 'aarch64', 'risc-v')
   hotfix_hours: int(min=0, required=False)
   hw_disk_bus: enum('virtio', 'scsi', None)
   hw_rng_model: enum('virtio', None, required=False)
   hw_scsi_model: enum('virtio-scsi', required=False)
   hw_watchdog_action: enum('disabled', 'reset', 'poweroff', 'pause', 'none', required=False)
   image_description: str(required=False)
-  os_distro: enum('arch', 'centos', 'cirros', 'clearlinux', 'debian', 'fedora', 'freebsd', 'opensuse', 'rhel', 'ubuntu', 'windows')
+  os_distro: enum('arch', 'centos', 'cirros', 'clearlinux', 'debian', 'fedora', 'freebsd', 'opensuse', 'rhel', 'talos', 'ubuntu', 'windows')
   os_version: str(required=False)
   patchlevel: str(required=False)
   provided_until: any(enum('none'), day())
   replace_frequency: enum('yearly', 'quarterly', 'monthly', 'weekly', 'daily', 'critical_bug', 'never')
   uuid_validity: any(enum('none', 'forever', 'notice'), str(starts_with='last-'), day())
 
 ---
```

### Comparing `openstack-image-manager-0.2.6/openstack_image_manager/manage.py` & `openstack-image-manager-0.3.0/openstack_image_manager/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import yamale
 
 from datetime import datetime
 from decimal import Decimal, ROUND_UP
 from loguru import logger
 from munch import Munch
 from natsort import natsorted
-from typing import List, Optional
 from yamale import YamaleError
 from openstack.image.v2.image import Image
 from openstack.exceptions import DuplicateResource
 
 
 class ImageManager:
     def __init__(self) -> None:
@@ -30,14 +29,19 @@
             False, "--dry-run", help="Do not perform any changes"
         ),
         latest: bool = typer.Option(
             False,
             "--latest",
             help="Only import the latest version for images of type multi",
         ),
+        keep: bool = typer.Option(
+            False,
+            "--keep",
+            help="Keep versions of images where the version is not longer defined",
+        ),
         cloud: str = typer.Option("openstack", help="Cloud name in clouds.yaml"),
         images: str = typer.Option(
             "etc/images/",
             help="Path to the directory containing all image files or path to "
             "a single image file",
         ),
         tag: str = typer.Option(
@@ -51,14 +55,17 @@
         ),
         deactivate: bool = typer.Option(
             False, "--deactivate", help="Deactivate images that should be deleted"
         ),
         hide: bool = typer.Option(
             False, "--hide", help="Hide images that should be deleted"
         ),
+        force: bool = typer.Option(
+            False, "--force", help="Force upload of disabled images"
+        ),
         delete: bool = typer.Option(False, "--delete", help="Delete outdated images"),
         yes_i_really_know_what_i_do: bool = typer.Option(
             False, "--yes-i-really-know-what-i-do", help="Really delete images"
         ),
         use_os_hidden: bool = typer.Option(
             False, "--use-os-hidden", help="Use the os_hidden property"
         ),
@@ -89,28 +96,32 @@
         ),
     ):
         self.CONF = Munch.fromDict(locals())
         self.CONF.pop("self")  # remove the self object from CONF
 
         if self.CONF.debug:
             level = "DEBUG"
+            log_fmt = (
+                "<green>{time:YYYY-MM-DD HH:mm:ss}</green> | <level>{level: <8}</level> | "
+                "<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>"
+            )
         else:
             level = "INFO"
+            log_fmt = (
+                "<green>{time:YYYY-MM-DD HH:mm:ss}</green> | <level>{level: <8}</level> | "
+                "<level>{message}</level>"
+            )
 
-        logger.remove()  # remove the default sink
-        log_fmt = (
-            "<green>{time:YYYY-MM-DD HH:mm:ss}</green> | <level>{level: <8}</level> | "
-            "<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>"
-        )
+        logger.remove()
         logger.add(sys.stderr, format=log_fmt, level=level, colorize=True)
 
         if __name__ == "__main__" or __name__ == "openstack_image_manager.manage":
             self.main()
 
-    def read_image_files(self) -> list:
+    def read_image_files(self, return_all_images=False) -> list:
         """Read all YAML files in self.CONF.images"""
         image_files = []
 
         if os.path.isdir(self.CONF.images):
             for file in os.listdir(self.CONF.images):
                 if file.endswith(tuple([".yml", "yaml"])):
                     image_files.append(file)
@@ -122,19 +133,34 @@
             if os.path.isdir(self.CONF.images):
                 file = os.path.join(self.CONF.images, file)
             with open(file) as fp:
                 try:
                     data = yaml.load(fp, Loader=yaml.SafeLoader)
                     images = data.get("images")
                     for image in images:
-                        if self.CONF.filter:
+                        if return_all_images:
+                            all_images.append(image)
+
+                        elif self.CONF.filter:
                             if re.search(self.CONF.filter, image["name"]):
-                                all_images.append(image)
+                                if "enable" in image and (
+                                    (image["enable"])
+                                    or (not image["enable"] and self.CONF.force)
+                                ):
+                                    all_images.append(image)
+                                elif "enable" not in image:
+                                    all_images.append(image)
                         else:
-                            all_images.append(image)
+                            if "enable" in image and (
+                                (image["enable"])
+                                or (not image["enable"] and self.CONF.force)
+                            ):
+                                all_images.append(image)
+                            elif "enable" not in image:
+                                all_images.append(image)
                 except yaml.YAMLError as exc:
                     logger.error(exc)
         return all_images
 
     def get_checksum(self, url: str, checksums_url: str) -> str:
         """
         Get the checksum of an upstream image by parsing its corresponding checksums file
@@ -216,22 +242,21 @@
 
         # manage images
         else:
             self.create_connection()
             images = self.read_image_files()
             managed_images = self.process_images(images)
 
-            if not self.CONF.dry_run:
-                # ignore all non-specified images when using --filter
-                if self.CONF.filter:
-                    cloud_images = self.get_images()
-                    for image in cloud_images:
-                        if not re.search(self.CONF.filter, image):
-                            managed_images.add(image)
-                self.manage_outdated_images(managed_images)
+            # ignore all non-specified images when using --filter
+            if self.CONF.filter:
+                cloud_images = self.get_images()
+                for image in cloud_images:
+                    if not re.search(self.CONF.filter, image):
+                        managed_images.add(image)
+            self.manage_outdated_images(managed_images)
 
         if self.exit_with_error:
             sys.exit(
                 "\nERROR: One or more errors occurred during the execution of the program, "
                 "please check the output."
             )
 
@@ -534,14 +559,18 @@
                 if not self.CONF.dry_run:
                     self.import_image(image, name, url, versions, version)
                     logger.info(
                         "Import of '%s' successfully completed, reloading images" % name
                     )
                     cloud_images = self.get_images()
                     imported_image = cloud_images[name]
+                else:
+                    logger.info(
+                        f"Skipping required import of image '{name}', running in dry-run mode"
+                    )
 
             elif self.CONF.latest and version != sorted_versions[-1]:
                 logger.info(
                     "Skipping image '%s' (only importing the latest version from type multi)"
                     % name
                 )
 
@@ -812,50 +841,108 @@
         Raises:
             Exception: when the image is still in use and cannot be deleted
             Exception: when the image cannot be deactivated or its visibility cannot be changed
         Returns:
             List with all images that are unmanaged and get affected by this method
         """
 
+        images = {}
+        for d in self.read_image_files(return_all_images=True):
+            images[d["name"]] = d
         cloud_images = self.get_images()
-        unmanaged_images = [x for x in cloud_images if x not in managed_images]
+
+        # NOTE: ensure to not handle images that should be not handled
+        if self.CONF.filter:
+            unmanaged_images = natsorted(
+                [
+                    x
+                    for x in cloud_images
+                    if x not in managed_images and re.search(self.CONF.filter, x)
+                ],
+                reverse=True,
+            )
+        else:
+            unmanaged_images = natsorted(
+                [x for x in cloud_images if x not in managed_images], reverse=True
+            )
+
+        counter = {}
 
         for image in unmanaged_images:
+            logger.info(f"Processing image '{image}' (removal candidate)")
+
             cloud_image = cloud_images[image]
-            if self.CONF.delete and self.CONF.yes_i_really_know_what_i_do:
-                try:
-                    logger.info("Deactivating image '%s'" % image)
-                    self.conn.image.deactivate_image(cloud_image.id)
+            image_name = cloud_image.properties["image_description"]
 
-                    logger.info("Setting visibility of '%s' to 'community'" % image)
-                    self.conn.image.update_image(cloud_image.id, visibility="community")
+            if image_name not in images:
+                logger.warning(
+                    f"No image definition found for '{image}', image will be ignored"
+                )
+                continue
 
-                    logger.info("Deleting %s" % image)
-                    self.conn.image.delete_image(cloud_image.id)
-                except Exception as e:
-                    logger.info(
-                        "%s is still in use and cannot be deleted\n %s" % (image, e)
-                    )
+            # Always skip the last imported image
+            if image_name == image:
+                continue
+
+            image_definition = images[image_name]
+            counter[image_name] = counter.get(image_name, 0) + 1
 
+            uuid_validity = cloud_image.properties["uuid_validity"]
+            if "last" in uuid_validity:
+                last = int(uuid_validity[5:]) - 1
             else:
-                logger.warning("Image %s should be deleted" % image)
-                try:
-                    if self.CONF.deactivate:
+                last = 0
+
+            if self.CONF.keep and not image_definition["multi"]:
+                logger.info(
+                    f"Image '{image}' will not be deleted, undefined versions of defined images are kept"
+                )
+
+            elif uuid_validity == "none":
+                logger.info(f"Image '{image}' will not be deleted, UUID validity is 'none'")
+            elif counter[image_name] > last:
+                if self.CONF.delete and self.CONF.yes_i_really_know_what_i_do and not self.CONF.dry_run:
+                    try:
                         logger.info("Deactivating image '%s'" % image)
                         self.conn.image.deactivate_image(cloud_image.id)
 
-                    if self.CONF.hide:
-                        cloud_image = cloud_images[image]
                         logger.info("Setting visibility of '%s' to 'community'" % image)
                         self.conn.image.update_image(
                             cloud_image.id, visibility="community"
                         )
-                except Exception as e:
-                    logger.error("An Exception occurred: \n%s" % e)
-                    self.exit_with_error = True
+
+                        logger.info("Deleting %s" % image)
+                        self.conn.image.delete_image(cloud_image.id)
+                    except Exception as e:
+                        logger.info(
+                            "%s is still in use and cannot be deleted\n %s" % (image, e)
+                        )
+
+                else:
+                    logger.warning(
+                        "Image %s should be deleted, but deletion is disabled" % image
+                    )
+                    try:
+                        if self.CONF.deactivate and not self.CONF.dry_run:
+                            logger.info("Deactivating image '%s'" % image)
+                            self.conn.image.deactivate_image(cloud_image.id)
+
+                        if self.CONF.hide and not self.CONF.dry_run:
+                            logger.info(
+                                "Setting visibility of '%s' to 'community'" % image
+                            )
+                            self.conn.image.update_image(
+                                cloud_image.id, visibility="community"
+                            )
+                    except Exception as e:
+                        logger.error("An Exception occurred: \n%s" % e)
+                        self.exit_with_error = True
+            elif counter[image_name] < last and self.CONF.hide and not self.CONF.dry_run:
+                logger.info("Setting visibility of '%s' to 'community'" % image)
+                self.conn.image.update_image(cloud_image.id, visibility="community")
         return unmanaged_images
 
     def check_image_metadata(self):
         """
         Retrieve metadata from managed images and check for compliance with SCS specifications:
         -> https://github.com/SovereignCloudStack/Docs/blob/main/Design-Docs/Image-Properties-Spec.md
```

### Comparing `openstack-image-manager-0.2.6/openstack_image_manager/mirror.py` & `openstack-image-manager-0.3.0/openstack_image_manager/mirror.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,118 @@
 # NOTE(berendt): quick & dirty (but it works for the moment)
 
 import logging
 import os
-import shutil
 import patoolib
 import requests
-import yaml
+import shutil
 import typer
-from urllib.parse import urlparse
+import yaml
 
 from minio import Minio
 from minio.error import S3Error
 from munch import Munch
 from os import listdir
 from os.path import isfile, join
+from urllib.parse import urlparse
 
 
 app = typer.Typer(add_completion=False)
 
 
 @app.command()
 def main(
-        debug: bool = typer.Option(False, '--debug', help='Enable debug logging'),
-        dry_run: bool = typer.Option(False, '--dry-run', help='Do not perform any changes'),
-        images: str = typer.Option('etc/images/', help='Path to the directory containing all image files'),
-        minio_access_key: str = typer.Option(None, help='Minio access key'),
-        minio_secret_key: str = typer.Option(None, help='Minio secret key'),
-        minio_server: str = typer.Option('minio.services.osism.tech', help='Minio server'),
-        minio_bucket: str = typer.Option('openstack-image-manager', help='Minio bucket')
+    debug: bool = typer.Option(False, "--debug", help="Enable debug logging"),
+    dry_run: bool = typer.Option(False, "--dry-run", help="Do not perform any changes"),
+    images: str = typer.Option(
+        "etc/images/", help="Path to the directory containing all image files"
+    ),
+    minio_access_key: str = typer.Option(None, help="Minio access key"),
+    minio_secret_key: str = typer.Option(None, help="Minio secret key"),
+    minio_server: str = typer.Option("minio.services.osism.tech", help="Minio server"),
+    minio_bucket: str = typer.Option("openstack-image-manager", help="Minio bucket"),
 ):
     CONF = Munch.fromDict(locals())
 
     if CONF.debug:
         level = logging.DEBUG
         logging.getLogger("paramiko").setLevel(logging.DEBUG)
     else:
         level = logging.INFO
         logging.getLogger("paramiko").setLevel(logging.WARNING)
-    logging.basicConfig(format='%(asctime)s - %(message)s', level=level, datefmt='%Y-%m-%d %H:%M:%S')
+    logging.basicConfig(
+        format="%(asctime)s - %(message)s", level=level, datefmt="%Y-%m-%d %H:%M:%S"
+    )
 
     onlyfiles = []
     for f in listdir(CONF.images):
         if isfile(join(CONF.images, f)):
             onlyfiles.append(f)
 
     all_images = []
     for file in onlyfiles:
         with open(join(CONF.images, file)) as fp:
             data = yaml.load(fp, Loader=yaml.SafeLoader)
-            images = data.get('images')
+            images = data.get("images")
             for image in images:
                 all_images.append(image)
 
     client = Minio(
         CONF.minio_server,
         access_key=CONF.minio_access_key,
-        secret_key=CONF.minio_secret_key
+        secret_key=CONF.minio_secret_key,
     )
 
     for image in all_images:
-        for version in image['versions']:
-            if 'source' not in version:
+        for version in image["versions"]:
+            if "source" not in version:
                 continue
 
-            logging.debug("source: %s" % version['source'])
+            logging.debug("source: %s" % version["source"])
 
-            path = urlparse(version['source'])
+            path = urlparse(version["source"])
+            url = urlparse(version["url"])
 
-            dirname = "%s/%s" % (image['shortname'], version['version'])
+            dirname = "%s/%s" % (image["shortname"], version["version"])
             filename, fileextension = os.path.splitext(os.path.basename(path.path))
+            _, fileextension2 = os.path.splitext(filename)
 
-            if fileextension not in ['.bz2', '.zip', '.xz']:
+            if fileextension not in [".bz2", ".zip", ".xz", ".gz"]:
                 filename += fileextension
 
+            if fileextension2 == ".tar":
+                filename2 = filename
+                filename = os.path.basename(url.path)
+
             logging.debug("dirname: %s" % dirname)
             logging.debug("filename: %s" % filename)
 
             try:
                 client.stat_object(CONF.minio_bucket, os.path.join(dirname, filename))
                 logging.info("'%s' available in '%s'" % (filename, dirname))
             except S3Error:
                 logging.info("'%s' not yet available in '%s'" % (filename, dirname))
 
-                if not CONF.dry_run:
-                    logging.info("Downloading '%s'" % version['source'])
-                    response = requests.get(version['source'], stream=True)
-                    with open(os.path.basename(path.path), 'wb') as fp:
-                        shutil.copyfileobj(response.raw, fp)
-                    del response
-
-                    if fileextension in ['.bz2', '.zip', '.xz']:
-                        logging.info("Decompressing '%s'" % os.path.basename(path.path))
-                        patoolib.extract_archive(os.path.basename(path.path), outdir='.')
-                        os.remove(os.path.basename(path.path))
+                logging.info("Downloading '%s'" % version["source"])
+                response = requests.get(version["source"], stream=True, allow_redirects=True)
+                with open(os.path.basename(path.path), "wb") as fp:
+                    shutil.copyfileobj(response.raw, fp)
+                del response
+
+                if fileextension in [".bz2", ".zip", ".xz", ".gz"]:
+                    logging.info("Decompressing '%s'" % os.path.basename(path.path))
+                    patoolib.extract_archive(os.path.basename(path.path), outdir=".")
+                    os.remove(os.path.basename(path.path))
 
+                if not CONF.dry_run:
                     logging.info("Uploading '%s' to '%s'" % (filename, dirname))
+                    client.fput_object(
+                        CONF.minio_bucket, os.path.join(dirname, filename), filename
+                    )
+                else:
+                    logging.info("Not uploading '%s' to '%s' (dry-run enabled)" % (filename, dirname))
 
-                    client.fput_object(CONF.minio_bucket, os.path.join(dirname, filename), filename)
-                    os.remove(filename)
+                os.remove(filename)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     app()
```

### Comparing `openstack-image-manager-0.2.6/openstack_image_manager/table.py` & `openstack-image-manager-0.3.0/openstack_image_manager/table.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,38 +8,38 @@
 
 
 app = typer.Typer(add_completion=False)
 
 
 @app.command()
 def main(
-    images: str = typer.Option('etc/images/', help='Path to the directory containing all image files')
+    images: str = typer.Option(
+        "etc/images/", help="Path to the directory containing all image files"
+    )
 ):
     CONF = Munch.fromDict(locals())
 
     onlyfiles = []
     for f in listdir(CONF.images):
         if isfile(join(CONF.images, f)):
             onlyfiles.append(f)
 
     all_images = []
     for file in onlyfiles:
         with open(join(CONF.images, file)) as fp:
             data = yaml.load(fp, Loader=yaml.SafeLoader)
-            images = data.get('images')
+            images = data.get("images")
             for image in images:
                 all_images.append(image)
 
     data = []
     for image in all_images:
-        data.append([image['name'], image['login'], image.get('password', '')])
+        data.append([image["name"], image["login"], image.get("password", "")])
 
     result = tabulate.tabulate(
-        sorted(data),
-        headers=['Name', 'Login user', 'Password'],
-        tablefmt="rst"
+        sorted(data), headers=["Name", "Login user", "Password"], tablefmt="rst"
     )
     print(result)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     app()
```

### Comparing `openstack-image-manager-0.2.6/openstack_image_manager/update.py` & `openstack-image-manager-0.3.0/openstack_image_manager/update.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 import requests
 import ruamel.yaml
 import typer
 import yaml
 
 app = typer.Typer()
 
+IMAGES = ["almalinux", "centos", "debian", "rockylinux", "ubuntu"]
+
 
 def mirror_image(image, latest_url, CONF):
     client = Minio(
         CONF.minio_server,
         access_key=CONF.minio_access_key,
         secret_key=CONF.minio_secret_key,
     )
@@ -34,15 +36,15 @@
     version = image["versions"][0]
     version["source"] = latest_url
 
     path = urlparse(version["source"])
     dirname = image["shortname"]
     filename, fileextension = os.path.splitext(os.path.basename(path.path))
 
-    if fileextension not in [".bz2", ".zip", ".xz"]:
+    if fileextension not in [".bz2", ".zip", ".xz", ".gz"]:
         filename += fileextension
 
     shortname = image["shortname"]
     format = image["format"]
     new_version = version["version"]
     new_filename = f"{new_version}-{shortname}.{format}"
 
@@ -53,15 +55,15 @@
         logger.info("'%s' not yet available in '%s'" % (new_filename, dirname))
         logger.info("Downloading '%s'" % version["source"])
         response = requests.get(version["source"], stream=True)
         with open(os.path.basename(path.path), "wb") as fp:
             shutil.copyfileobj(response.raw, fp)
         del response
 
-        if fileextension in [".bz2", ".zip", ".xz"]:
+        if fileextension in [".bz2", ".zip", ".xz", ".gz"]:
             logger.info("Decompressing '%s'" % os.path.basename(path.path))
             patoolib.extract_archive(os.path.basename(path.path), outdir=".")
             os.remove(os.path.basename(path.path))
 
         logger.info(
             "Uploading '%s' to '%s' as '%s'" % (filename, dirname, new_filename)
         )
@@ -90,19 +92,19 @@
 
     checksum_type = "sha256"
     filename_pattern = None
 
     if image["shortname"] in ["centos-stream-8", "centos-stream-9", "centos-7"]:
         filename_pattern = latest_filename.replace("HEREBE", "")
         filename_pattern = filename_pattern.replace("DRAGONS", "")
-    elif image["shortname"] in ["debian-10", "debian-11"]:
+    elif image["shortname"] in ["debian-10", "debian-11", "debian-12"]:
         checksum_type = "sha512"
 
     for line in result.text.split("\n"):
-        if image["shortname"] == "rocky-9":
+        if image["shortname"] in ["rocky-8", "rocky-9"]:
             splitted_line = re.split("\s+", line)  # noqa W605
             if splitted_line[0] == "SHA256":
                 checksums[latest_filename] = splitted_line[3]
         elif image["shortname"] in [
             "ubuntu-14.04",
             "ubuntu-16.04",
             "ubuntu-16.04-minimal",
@@ -141,17 +143,29 @@
 
         latest_filename = new_latest_filename
         latest_url = new_latest_url
 
     current_checksum = f"{checksum_type}:{checksums[latest_filename]}"
     logger.info(f"Checksum of current {latest_filename} is {current_checksum}")
 
-    latest_version = image["versions"][0]
-    latest_checksum = latest_version["checksum"]
-    logger.info(f"Our checksum is {latest_checksum}")
+    try:
+        latest_version = image["versions"][0]
+        latest_checksum = latest_version["checksum"]
+        logger.info(f"Our checksum is {latest_checksum}")
+    except IndexError:
+        latest_checksum = None
+        logger.info("No image available so far")
+        image["versions"].append(
+            {
+                "build_date": None,
+                "checksum": None,
+                "url": None,
+                "version": None,
+            }
+        )
 
     if latest_checksum != current_checksum:
         logger.info(f"Checking {latest_url}")
 
         conn = urlopen(latest_url, timeout=30)
         struct = time.strptime(
             conn.headers["last-modified"], "%a, %d %b %Y %H:%M:%S %Z"
@@ -186,15 +200,14 @@
 
     return image
 
 
 @app.command()
 def main(
     debug: bool = typer.Option(False, "--debug", help="Enable debug logging"),
-    image: str = typer.Option("almalinux", help="Image to update"),
     minio_access_key: str = typer.Option(None, help="Minio access key"),
     minio_secret_key: str = typer.Option(None, help="Minio secret key"),
     minio_server: str = typer.Option("minio.services.osism.tech", help="Minio server"),
     minio_bucket: str = typer.Option("openstack-image-manager", help="Minio bucket"),
 ):
 
     CONF = Munch.fromDict(locals())
@@ -207,26 +220,27 @@
     logger.remove()  # remove the default sink
     log_fmt = (
         "<green>{time:YYYY-MM-DD HH:mm:ss}</green> | <level>{level: <8}</level> | "
         "<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>"
     )
     logger.add(sys.stderr, format=log_fmt, level=level, colorize=True)
 
-    p = f"etc/images/{image}.yml"
+    for image in IMAGES:
+        p = f"etc/images/{image}.yml"
 
-    with open(p) as fp:
-        data = yaml.safe_load(fp)
+        with open(p) as fp:
+            data = yaml.safe_load(fp)
 
-    for index, image in enumerate(data["images"]):
-        if "latest_url" in image:
-            updated_image = update_image(image, CONF)
-            data["images"][index] = updated_image
-
-    with open(p, "w+") as fp:
-        ryaml = ruamel.yaml.YAML()
-        ryaml.explicit_start = True
-        ryaml.indent(sequence=4, offset=2)
-        ryaml.dump(data, fp)
+        for index, image in enumerate(data["images"]):
+            if "latest_url" in image:
+                updated_image = update_image(image, CONF)
+                data["images"][index] = updated_image
+
+        with open(p, "w+") as fp:
+            ryaml = ruamel.yaml.YAML()
+            ryaml.explicit_start = True
+            ryaml.indent(sequence=4, offset=2)
+            ryaml.dump(data, fp)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `openstack-image-manager-0.2.6/openstack_image_manager.egg-info/PKG-INFO` & `openstack-image-manager-0.3.0/openstack_image_manager.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstack-image-manager
-Version: 0.2.6
+Version: 0.3.0
 Summary: OpenStack image manager
 Home-page: https://github.com/osism/openstack-image-manager
 Author: OSISM community
 Author-email: info@osism.tech
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -24,9 +24,9 @@
 # openstack-image-manager
 
 [![PyPi version](https://badgen.net/pypi/v/openstack-image-manager/)](https://pypi.org/project/openstack-image-manager/)
 [![PyPi license](https://badgen.net/pypi/license/openstack-image-manager/)](https://pypi.org/project/openstack-image-manager/)
 
 Easily manage and keep up to date a large number of images on an OpenStack environment
 
-Documentation: <https://docs.osism.tech/openstack-image-manager/>
+Documentation: <https://docs.scs.community/docs/category/openstack-image-manager/>
```

### Comparing `openstack-image-manager-0.2.6/openstack_image_manager.egg-info/SOURCES.txt` & `openstack-image-manager-0.3.0/openstack_image_manager.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -9,60 +9,28 @@
 Dockerfile
 LICENSE
 Pipfile
 Pipfile.lock
 README.md
 _config.yml
 clouds.yml.sample
-openstack_image_manager
 requirements.txt
 secure.yml.sample
 setup.cfg
 setup.py
 tox.ini
 .github/renovate.json
 .github/workflows/build-container-image.yml
+.github/workflows/mirror-images-dry-run.yml
 .github/workflows/mirror-images.yml
 .github/workflows/publish.yml
 .github/workflows/run-unit-tests.yml
 .github/workflows/test-python-setup.yml
 .github/workflows/update-images.yml
 .github/workflows/validate-configuration.yml
-crawler/LICENSE
-crawler/README.md
-crawler/git_ssh_command.sh
-crawler/historian.py
-crawler/image-crawler.py
-crawler/requirements.txt
-crawler/setup.sh
-crawler/crawler/__init__.py
-crawler/crawler/core/__init__.py
-crawler/crawler/core/config.py
-crawler/crawler/core/database.py
-crawler/crawler/core/exporter.py
-crawler/crawler/core/main.py
-crawler/crawler/git/__init__.py
-crawler/crawler/git/base.py
-crawler/crawler/updater/__init__.py
-crawler/crawler/updater/service.py
-crawler/crawler/web/__init__.py
-crawler/crawler/web/directory.py
-crawler/crawler/web/generic.py
-crawler/docs/background.md
-crawler/docs/git-handling.md
-crawler/docs/templates.md
-crawler/etc/config.yaml
-crawler/etc/image-sources.yaml
-crawler/lib/initialize-image-catalog.sql
-crawler/lib/populate-catalog-test-data.sql
-crawler/templates/almalinux.yml.j2
-crawler/templates/debian.yml.j2
-crawler/templates/header.yml
-crawler/templates/ubuntu.yml.j2
-crawler/templates/ubuntu_minimal.yml.j2
 doc/conf.py
 doc/configuration.md
 doc/contribute.md
 doc/getting_started.md
 doc/overview.md
 doc/quickstart.md
 doc/requirements.md
@@ -74,17 +42,19 @@
 etc/images/cirros.yml
 etc/images/clearlinux.yml
 etc/images/debian.yml
 etc/images/fedora.yml
 etc/images/flatcar.yml
 etc/images/gardenlinux.yml
 etc/images/kubernetes.yml
-etc/images/opensense.yml
+etc/images/octavia.yml
 etc/images/opensuse.yml
+etc/images/opnsense.yml
 etc/images/rockylinux.yml
+etc/images/talos.yml
 etc/images/ubuntu.yml
 openstack_image_manager/__init__.py
 openstack_image_manager/manage.py
 openstack_image_manager/mirror.py
 openstack_image_manager/table.py
 openstack_image_manager/update.py
 openstack_image_manager.egg-info/PKG-INFO
@@ -97,18 +67,13 @@
 openstack_image_manager.egg-info/top_level.txt
 playbooks/integration-test.yml
 playbooks/pre-integration-test.yml
 playbooks/pre-real-world.yml
 playbooks/real-world.yml
 scripts/build.sh
 scripts/push.sh
-src/__init__.py
-src/manage.py
-src/mirror.py
-src/table.py
-src/update.py
 test/__init__.py
 test/integration/__init__.py
 test/integration/test_manage_api.py
 test/integration/fixtures/test_image.yml
 test/unit/__init__.py
 test/unit/test_manage.py
```

### Comparing `openstack-image-manager-0.2.6/scripts/build.sh` & `openstack-image-manager-0.3.0/scripts/build.sh`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/setup.cfg` & `openstack-image-manager-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.2.6/test/integration/fixtures/test_image.yml` & `openstack-image-manager-0.3.0/test/integration/fixtures/test_image.yml`

 * *Files 13% similar despite different names*

```diff
@@ -16,13 +16,14 @@
       hw_scsi_model: virtio-scsi
       hw_watchdog_action: reset
       replace_frequency: never
       uuid_validity: none
       provided_until: none
       os_distro: cirros
       os_version: '0.6.0'
+      image_description: Cirros_test
     tags: []
     versions:
       - version: '1'
         url: https://github.com/cirros-dev/cirros/releases/download/0.6.0/cirros-0.6.0-x86_64-disk.img
         checksum: "sha256:94e1e2c94dbbae7d4bdc38e68590a1daf73c9de2d03dd693857b4b0a042548e8"
         build_date: 2022-09-28
```

### Comparing `openstack-image-manager-0.2.6/test/integration/test_manage_api.py` & `openstack-image-manager-0.3.0/test/integration/test_manage_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import openstack
 from loguru import logger
 from munch import Munch
 from unittest import TestCase
 
-from src import manage
+from openstack_image_manager import manage
 
 logger.remove()   # disable all logging from manage.py
 
 
 class TestManageAPI(TestCase):
 
     def setUp(self):
@@ -21,24 +21,27 @@
             yes_i_really_know_what_i_do=True,
             hide=False,
             deactivate=False,
             cloud='openstack',
             images='test/integration/fixtures/',
             tag='fake_tag',
             filter='',
+            keep=False,
+            force=False,
+            hypervisor=None,
             validate=False
         )
         self.image = self.sot.read_image_files()[0]
         self.assertEqual(self.image['name'], 'Cirros_test')
         self.image['tags'].append(self.sot.CONF.tag)
         self.name = self.image['name'] + ' (1)'
 
     def test_api_functions(self):
         '''
-        Test all used API functions, as they appear in src.manage.py
+        Test all used API functions, as they appear in openstack_image_manager.manage.py
         Import the image, set its properties, rename it and delete it afterwards
         '''
         self.sot.conn = openstack.connect(cloud=self.sot.CONF.cloud)
 
         # make sure there are no images in the cloud already
         cloud_images = self.sot.get_images()
         self.assertEqual(cloud_images,
@@ -93,14 +96,17 @@
         # test image rename
         self.sot.rename_images(self.image['name'], ['1'], None, None)
 
         # assert the image got renamed
         cloud_images = self.sot.get_images()
         self.assertEqual(list(cloud_images.keys()), [self.image['name']])
 
-        # Finally delete the image, also works as a cleanup
-        res = self.sot.manage_outdated_images(set())
-        self.assertEqual(res, [self.image['name']])
+        # Make sure no images are considered unmanaged
+        res = self.sot.manage_outdated_images({'Cirros_test'})
+        self.assertEqual(res, [])
+
+        # Manually delete the image
+        self.sot.conn.image.delete_image(cloud_images['Cirros_test'].id)
 
         # make sure the image is gone
         cloud_images = self.sot.get_images()
-        self.assertEqual(cloud_images, {}, f"Cloud not delete image {self.image['name']}, please do so manually")
+        self.assertEqual(cloud_images, {}, f"Could not delete image {self.image['name']}, please do so manually")
```

