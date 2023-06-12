# Comparing `tmp/octavia-tempest-plugin-2.3.0.tar.gz` & `tmp/octavia-tempest-plugin-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octavia-tempest-plugin-2.3.0.tar", last modified: Fri Mar 10 09:13:39 2023, max compression
+gzip compressed data, was "octavia-tempest-plugin-2.4.0.tar", last modified: Mon Jun 12 13:51:21 2023, max compression
```

## Comparing `octavia-tempest-plugin-2.3.0.tar` & `octavia-tempest-plugin-2.4.0.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.335815 octavia-tempest-plugin-2.3.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1554 2023-03-10 09:13:39.000000 octavia-tempest-plugin-2.3.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10805 2023-03-10 09:13:39.000000 octavia-tempest-plugin-2.3.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2023-03-10 09:13:39.335815 octavia-tempest-plugin-2.3.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1466 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.315815 octavia-tempest-plugin-2.3.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/devstack/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1978 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.315815 octavia-tempest-plugin-2.3.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.315815 octavia-tempest-plugin-2.3.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4629 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/doc/source/configref.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/doc/source/readme.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.315815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.319815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3604 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/common/barbican_client_mgr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9387 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/common/cert_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9202 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2061 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/common/decorators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1438 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/common/requests_adapters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15386 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.319815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/contrib/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.319815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/contrib/test_server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/contrib/test_server/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/contrib/test_server/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6993 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/contrib/test_server/test_server.go
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.319815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10179 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2619 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.319815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.319815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.323815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1910 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12797 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/amphora_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4224 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/availability_zone_capabilities_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15784 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/availability_zone_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16312 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/availability_zone_profile_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23098 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/base_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4056 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/flavor_capabilities_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14890 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/flavor_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15087 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/flavor_profile_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15761 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/healthmonitor_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14377 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/l7policy_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15566 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/l7rule_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22916 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/listener_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22776 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/loadbalancer_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18740 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/member_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16302 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/pool_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3245 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/provider_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.323815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25269 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/RBAC_tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.323815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/act_stdby_scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/act_stdby_scenario/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.327815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/act_stdby_scenario/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/act_stdby_scenario/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12279 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/act_stdby_scenario/v2/test_active_standby.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12620 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/act_stdby_scenario/v2/test_active_standby_iptables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.327815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.327815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13132 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_amphora.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26168 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4496 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_availability_zone_capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28675 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_availability_zone_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21783 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_flavor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4168 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_flavor_capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22233 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_flavor_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    81923 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_healthmonitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42698 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_l7policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34743 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_l7rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    61561 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49079 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_load_balancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   139911 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_member.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    81894 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4102 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_provider.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.327815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/barbican_scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/barbican_scenario/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.327815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/barbican_scenario/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/barbican_scenario/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    75915 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/barbican_scenario/v2/test_tls_barbican.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.327815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.331815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16736 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_healthmonitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22914 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_ipv6_traffic_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8301 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_l7policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7490 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_l7rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18296 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7486 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_load_balancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36374 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_member.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27427 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    74586 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_traffic_ops.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.331815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/spare_pool_scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/spare_pool_scenario/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.331815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/spare_pool_scenario/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/spare_pool_scenario/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9660 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/spare_pool_scenario/v2/test_spare_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    58624 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21555 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/validators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9761 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/waiters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.319815 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2023-03-10 09:13:39.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6658 2023-03-10 09:13:39.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-10 09:13:39.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-03-10 09:13:39.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-10 09:13:39.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-10 09:13:39.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-03-10 09:13:39.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2023-03-10 09:13:39.000000 octavia-tempest-plugin-2.3.0/octavia_tempest_plugin.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.331815 octavia-tempest-plugin-2.3.0/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.331815 octavia-tempest-plugin-2.3.0/playbooks/act_stby_iptables/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      661 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/playbooks/act_stby_iptables/pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/playbooks/prepare-ovn-multinode.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.311815 octavia-tempest-plugin-2.3.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.335815 octavia-tempest-plugin-2.3.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/Add-PROMETHEUS-listener-API-and-scenario-tests-ccab4b09f6a64428.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/Add-RBAC-scoped-tokens-tests-920aa35faf4a8c9d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/Add-amphora-admin-log-offloading-012aca8151ebbc54.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/Fix-service-client-params-41a0f7c9c6b53aac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/Make-sure-member-credentials-have-the-member-role-for-new-defaults-5fbc2e05768c04b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/add-listener-stats-api-test-88947cf5e6ae9cae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/add-pool-client-auth-scenario-02abca554e60d3da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/add-tags-api-tests-1130aab82bb0f7f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/add-tenant-flow-log-offload-scenario-test-39bf9bf51f70d7bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/add-udp-test-scenario-cdd131d1ef7bf8e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/client-auth-scenario-bffa420a2fd38159.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/pool-tls-scenario-test-0eb88e731c595b67.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/pools-service-client-alpn-support-7de3bcd3c901ff1a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/skip-az-api-tests-if-azs-not-configured-c5d06cdcf29beeb5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/notes/test-server-path-3845f619090ba016.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.335815 octavia-tempest-plugin-2.3.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.335815 octavia-tempest-plugin-2.3.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.335815 octavia-tempest-plugin-2.3.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9398 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1551 2023-03-10 09:13:39.335815 octavia-tempest-plugin-2.3.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3378 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-10 09:13:39.335815 octavia-tempest-plugin-2.3.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30327 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/zuul.d/jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2496 2023-03-10 09:11:47.000000 octavia-tempest-plugin-2.3.0/zuul.d/projects.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.356975 octavia-tempest-plugin-2.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1581 2023-06-12 13:51:21.000000 octavia-tempest-plugin-2.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11178 2023-06-12 13:51:21.000000 octavia-tempest-plugin-2.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2023-06-12 13:51:21.356975 octavia-tempest-plugin-2.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1466 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.340975 octavia-tempest-plugin-2.4.0/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/devstack/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1978 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.340975 octavia-tempest-plugin-2.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.340975 octavia-tempest-plugin-2.4.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4629 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/doc/source/configref.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/doc/source/readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.340975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.344975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3604 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/common/barbican_client_mgr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9387 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/common/cert_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9202 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2061 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/common/decorators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1438 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/common/requests_adapters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15594 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.344975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/contrib/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.344975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/contrib/test_server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/contrib/test_server/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/contrib/test_server/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6993 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/contrib/test_server/test_server.go
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.344975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10179 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2619 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.344975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.344975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.344975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1910 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12797 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/amphora_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4224 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/availability_zone_capabilities_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15784 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/availability_zone_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16312 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/availability_zone_profile_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23098 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/base_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4056 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/flavor_capabilities_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14890 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/flavor_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15087 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/flavor_profile_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15761 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/healthmonitor_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14377 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/l7policy_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15566 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/l7rule_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22916 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/listener_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22776 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/loadbalancer_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18740 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/member_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16302 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/pool_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3245 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/provider_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.348975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25269 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/RBAC_tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.348975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/act_stdby_scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/act_stdby_scenario/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.348975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/act_stdby_scenario/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/act_stdby_scenario/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12279 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/act_stdby_scenario/v2/test_active_standby.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12620 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/act_stdby_scenario/v2/test_active_standby_iptables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.348975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.348975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13111 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_amphora.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26151 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4489 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_availability_zone_capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28640 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_availability_zone_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21766 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4161 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_flavor_capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22198 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_flavor_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    82079 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_healthmonitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42854 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_l7policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34911 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_l7rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    61717 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49270 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_load_balancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   140125 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_member.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    82050 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4104 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_provider.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.348975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/barbican_scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/barbican_scenario/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.348975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/barbican_scenario/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/barbican_scenario/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    83172 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/barbican_scenario/v2/test_tls_barbican.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.352975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.352975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16736 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_healthmonitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22914 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_ipv6_traffic_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8301 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_l7policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7490 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_l7rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18296 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7486 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_load_balancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36374 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_member.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27427 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    74586 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_traffic_ops.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.352975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/spare_pool_scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/spare_pool_scenario/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.352975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/spare_pool_scenario/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/spare_pool_scenario/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9660 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/spare_pool_scenario/v2/test_spare_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    58671 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21566 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/validators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9761 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/waiters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.344975 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2023-06-12 13:51:21.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6658 2023-06-12 13:51:21.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-12 13:51:21.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-06-12 13:51:21.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-12 13:51:21.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-06-12 13:51:21.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-06-12 13:51:21.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2023-06-12 13:51:21.000000 octavia-tempest-plugin-2.4.0/octavia_tempest_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.352975 octavia-tempest-plugin-2.4.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.352975 octavia-tempest-plugin-2.4.0/playbooks/act_stby_iptables/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      661 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/playbooks/act_stby_iptables/pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/playbooks/prepare-ovn-multinode.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.340975 octavia-tempest-plugin-2.4.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.352975 octavia-tempest-plugin-2.4.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/Add-PROMETHEUS-listener-API-and-scenario-tests-ccab4b09f6a64428.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/Add-RBAC-scoped-tokens-tests-920aa35faf4a8c9d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/Add-amphora-admin-log-offloading-012aca8151ebbc54.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/Fix-service-client-params-41a0f7c9c6b53aac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/Make-sure-member-credentials-have-the-member-role-for-new-defaults-5fbc2e05768c04b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/add-listener-stats-api-test-88947cf5e6ae9cae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/add-pool-client-auth-scenario-02abca554e60d3da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/add-tags-api-tests-1130aab82bb0f7f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/add-tenant-flow-log-offload-scenario-test-39bf9bf51f70d7bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/add-udp-test-scenario-cdd131d1ef7bf8e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/client-auth-scenario-bffa420a2fd38159.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/pool-tls-scenario-test-0eb88e731c595b67.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/pools-service-client-alpn-support-7de3bcd3c901ff1a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/skip-az-api-tests-if-azs-not-configured-c5d06cdcf29beeb5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/notes/test-server-path-3845f619090ba016.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.352975 octavia-tempest-plugin-2.4.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.352975 octavia-tempest-plugin-2.4.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.352975 octavia-tempest-plugin-2.4.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9398 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1551 2023-06-12 13:51:21.356975 octavia-tempest-plugin-2.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3378 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:51:21.352975 octavia-tempest-plugin-2.4.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34901 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/zuul.d/jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3202 2023-06-12 13:50:54.000000 octavia-tempest-plugin-2.4.0/zuul.d/projects.yaml
```

### Comparing `octavia-tempest-plugin-2.3.0/AUTHORS` & `octavia-tempest-plugin-2.4.0/AUTHORS`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 Jude Cross <jcross@godaddy.com>
 LiZekun <2954674728@qq.com>
 Lingxian Kong <anlin.kong@gmail.com>
 Lukáš Piwowarski <lpiwowar@redhat.com>
 Maciej Józefczyk <mjozefcz@redhat.com>
 Michael Johnson <johnsomor@gmail.com>
 Nguyen Hai <nguyentrihai93@gmail.com>
+Omer <oschwart@redhat.com>
 Reedip <rbanerje@redhat.com>
 Reedip Banerjee <rbanerje@redhat.com>
 ShangXiao <shangxiaobj@inspur.com>
 Takashi Kajinami <tkajinam@redhat.com>
 Tom Stappaerts <tom.stappaerts@nuagenetworks.net>
 Tom Weininger <tweining@redhat.com>
 Vadim Ponomarev <velizarx@gmail.com>
```

### Comparing `octavia-tempest-plugin-2.3.0/CONTRIBUTING.rst` & `octavia-tempest-plugin-2.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/ChangeLog` & `octavia-tempest-plugin-2.4.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 CHANGES
 =======
 
+2.4.0
+-----
+
+* Splitting scenario jobs in 2 jobs
+* Fix jobs running on Jammy vs. Focal vs. Bionic nodes
+* Updating Octavia tempest jobs on Ubuntu jammy (22.04)
+* Fix request interval in \_wait\_for\_lb\_functional
+* Fix the pool client auth test
+* Update Octavia tempest tests for no scoped tokens
+
 2.3.0
 -----
 
 * Fix legacy admin in RBAC tests
+* Spliting centos scenario job into 2 jobs
+* Add h2 traffic/scenario test
 * Add "member" role to non-admin test credentials
 
 2.2.0
 -----
 
 * Make user role logging optional
 * tox skipsdist seems to be problematic
```

### Comparing `octavia-tempest-plugin-2.3.0/LICENSE` & `octavia-tempest-plugin-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/PKG-INFO` & `octavia-tempest-plugin-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: octavia-tempest-plugin
-Version: 2.3.0
+Version: 2.4.0
 Summary: Tempest plugin for Octavia
 Home-page: https://docs.openstack.org/octavia-tempest-plugin/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ======================
         Octavia Tempest Plugin
```

### Comparing `octavia-tempest-plugin-2.3.0/README.rst` & `octavia-tempest-plugin-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/devstack/plugin.sh` & `octavia-tempest-plugin-2.4.0/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/doc/source/conf.py` & `octavia-tempest-plugin-2.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/doc/source/configref.rst` & `octavia-tempest-plugin-2.4.0/doc/source/configref.rst`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/doc/source/index.rst` & `octavia-tempest-plugin-2.4.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/__init__.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/common/barbican_client_mgr.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/common/barbican_client_mgr.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/common/cert_utils.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/common/cert_utils.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/common/constants.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/common/constants.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/common/decorators.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/common/decorators.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/common/requests_adapters.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/common/requests_adapters.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/config.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,19 @@
     # Note: Also see the enforce_scope section (from tempest) for Octavia API
     #       scope checking setting.
     cfg.BoolOpt('enforce_new_defaults',
                 default=False,
                 help='Does the load-balancer service API policies enforce '
                      'the new keystone default roles? This configuration '
                      'value should be same as octavia.conf: '
-                     '[oslo_policy].enforce_new_defaults option.'),
+                     '[oslo_policy].enforce_new_defaults option.',
+                deprecated_for_removal=True,
+                deprecated_reason='Consolidated into the RBAC_test_type '
+                                  'setting.',
+                deprecated_since='bobcat'),
 ]
 
 lb_feature_enabled_group = cfg.OptGroup(name='loadbalancer-feature-enabled',
                                         title='Enabled/Disabled LB features')
 LBFeatureEnabledGroup = [
     cfg.BoolOpt('not_implemented_is_error',
                 default=True,
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/contrib/test_server/README.rst` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/contrib/test_server/README.rst`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/contrib/test_server/test_server.go` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/contrib/test_server/test_server.go`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/hacking/checks.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/plugin.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/__init__.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/__init__.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/__init__.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/amphora_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/amphora_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/availability_zone_capabilities_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/availability_zone_capabilities_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/availability_zone_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/availability_zone_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/availability_zone_profile_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/availability_zone_profile_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/base_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/base_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/flavor_capabilities_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/flavor_capabilities_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/flavor_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/flavor_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/flavor_profile_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/flavor_profile_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/healthmonitor_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/healthmonitor_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/l7policy_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/l7policy_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/l7rule_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/l7rule_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/listener_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/listener_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/loadbalancer_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/loadbalancer_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/member_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/member_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/pool_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/pool_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/services/load_balancer/v2/provider_client.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/services/load_balancer/v2/provider_client.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/RBAC_tests.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/RBAC_tests.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/act_stdby_scenario/v2/test_active_standby.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/act_stdby_scenario/v2/test_active_standby.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/act_stdby_scenario/v2/test_active_standby_iptables.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/act_stdby_scenario/v2/test_active_standby_iptables.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_amphora.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_amphora.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                                 CONF.load_balancer.lb_build_timeout)
 
         # Test RBAC for list amphorae
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_list_RBAC_enforcement(
                 'AmphoraClient', 'list_amphorae', expected_allowed)
 
         # Get an actual list of the amphorae
@@ -178,15 +178,15 @@
         amphora_1 = amphorae[0]
 
         # Test RBAC for update an amphora
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'AmphoraClient', 'update_amphora_config', expected_allowed,
                 None, None, amphora_1[const.ID])
 
@@ -213,15 +213,15 @@
         amphora_1 = amphorae[0]
 
         # Test RBAC for failover an amphora
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'AmphoraClient', 'amphora_failover', expected_allowed,
                 None, None, amphora_1[const.ID])
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_availability_zone.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_availability_zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # create an availability zone.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_create_RBAC_enforcement(
                 'AvailabilityZoneClient', 'create_availability_zone',
                 expected_allowed, **availability_zone_kwargs)
 
@@ -228,15 +228,15 @@
         # list availability zones.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = [
                 'os_admin', 'os_primary', 'os_roles_lb_admin',
                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary', 'os_system_admin',
+            expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_system_reader', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = [
                 'os_system_admin', 'os_system_reader', 'os_roles_lb_admin',
                 'os_roles_lb_observer', 'os_roles_lb_global_observer',
@@ -381,15 +381,15 @@
         # show availability zone details.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = [
                 'os_admin', 'os_primary', 'os_roles_lb_admin',
                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary', 'os_system_admin',
+            expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_system_reader', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = [
                 'os_system_admin', 'os_system_reader', 'os_roles_lb_admin',
                 'os_roles_lb_observer', 'os_roles_lb_global_observer',
@@ -454,15 +454,15 @@
 
         # Test that a user without the load balancer role cannot
         # update availability zone details.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'AvailabilityZoneClient', 'update_availability_zone',
                 expected_allowed, None, None, availability_zone[const.NAME],
                 **availability_zone_updated_kwargs)
@@ -531,15 +531,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # delete an availability zone.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_delete_RBAC_enforcement(
                 'AvailabilityZoneClient', 'delete_availability_zone',
                 expected_allowed, None, None, availability_zone[const.NAME])
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_availability_zone_capabilities.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_availability_zone_capabilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # list provider availability zone capabilities.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_list_RBAC_enforcement(
                 'AvailabilityZoneCapabilitiesClient',
                 'list_availability_zone_capabilities', expected_allowed,
                 CONF.load_balancer.provider)
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_availability_zone_profile.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_availability_zone_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # create an availability zone profile.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_create_RBAC_enforcement(
                 'AvailabilityZoneProfileClient',
                 'create_availability_zone_profile',
                 expected_allowed, **availability_zone_profile_kwargs)
@@ -231,15 +231,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # list availability zone profiles.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_list_RBAC_enforcement(
                 'AvailabilityZoneProfileClient',
                 'list_availability_zone_profiles', expected_allowed)
 
@@ -392,15 +392,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # show an availability zone profile
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_show_RBAC_enforcement(
                 'AvailabilityZoneProfileClient',
                 'show_availability_zone_profile', expected_allowed,
                 availability_zone_profile[const.ID])
@@ -494,15 +494,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # update an availability zone profile.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'AvailabilityZoneProfileClient',
                 'update_availability_zone_profile', expected_allowed,
                 None, None, availability_zone_profile[const.ID],
@@ -576,15 +576,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # delete an availability zone profile.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_delete_RBAC_enforcement(
                 'AvailabilityZoneProfileClient',
                 'delete_availability_zone_profile', expected_allowed,
                 None, None, availability_zone_profile[const.ID])
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_flavor.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_flavor.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # create a flavor.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_create_RBAC_enforcement(
                 'FlavorClient', 'create_flavor',
                 expected_allowed, None, None, **flavor_kwargs)
 
@@ -194,15 +194,15 @@
         # list flavors.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = [
                 'os_admin', 'os_primary', 'os_roles_lb_admin',
                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary', 'os_system_admin',
+            expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_system_reader', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = [
                 'os_system_admin', 'os_system_reader', 'os_roles_lb_admin',
                 'os_roles_lb_observer', 'os_roles_lb_global_observer',
@@ -322,15 +322,15 @@
         # show flavor details.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = [
                 'os_admin', 'os_primary', 'os_roles_lb_admin',
                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary', 'os_system_admin',
+            expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_system_reader', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = [
                 'os_system_admin', 'os_system_reader', 'os_roles_lb_admin',
                 'os_roles_lb_observer', 'os_roles_lb_global_observer',
@@ -390,15 +390,15 @@
 
         # Test that a user without the load balancer role cannot
         # update flavor details.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'FlavorClient', 'update_flavor', expected_allowed, None, None,
                 flavor[const.ID], **flavor_updated_kwargs)
 
@@ -454,15 +454,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # delete a flavor.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_delete_RBAC_enforcement(
                 'FlavorClient', 'delete_flavor', expected_allowed,
                 None, None, flavor[const.ID])
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_flavor_capabilities.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_flavor_capabilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # list provider flavor capabilities.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_list_RBAC_enforcement(
                 'FlavorCapabilitiesClient',
                 'list_flavor_capabilities', expected_allowed,
                 CONF.load_balancer.provider)
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_flavor_profile.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_flavor_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # create a flavor profile
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_create_RBAC_enforcement(
                 'FlavorProfileClient', 'create_flavor_profile',
                 expected_allowed, None, None, **flavor_profile_kwargs)
 
@@ -180,15 +180,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # list flavor profiles.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_list_RBAC_enforcement(
                 'FlavorProfileClient', 'list_flavor_profiles',
                 expected_allowed)
 
@@ -309,15 +309,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # show a flavor profile.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_show_RBAC_enforcement(
                 'FlavorProfileClient', 'show_flavor_profile',
                 expected_allowed, flavor_profile[const.ID])
 
@@ -387,15 +387,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # update a flavor profile.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'FlavorProfileClient', 'update_flavor_profile',
                 expected_allowed, None, None, flavor_profile[const.ID],
                 **flavor_profile_updated_kwargs)
@@ -454,15 +454,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # delete a flavor profile
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_delete_RBAC_enforcement(
                 'FlavorProfileClient', 'delete_flavor_profile',
                 expected_allowed, None, None, flavor_profile[const.ID])
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_healthmonitor.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_healthmonitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,16 @@
         # Test that a user without the loadbalancer role cannot
         # create a healthmonitor
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_create_RBAC_enforcement(
                 'HealthMonitorClient', 'create_healthmonitor',
                 expected_allowed,
@@ -720,31 +721,31 @@
         test_ids.append(hm3[const.ID])
 
         # Test that a different users cannot see the lb_member healthmonitors
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_primary', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary',
-                                'os_roles_lb_member2', 'os_roles_lb_observer',
+            expected_allowed = ['os_primary', 'os_roles_lb_member2',
+                                'os_roles_lb_observer',
                                 'os_roles_lb_global_observer']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_roles_lb_observer', 'os_roles_lb_member2']
         if expected_allowed:
             self.check_list_RBAC_enforcement_count(
                 'HealthMonitorClient', 'list_healthmonitors',
                 expected_allowed, 0)
 
         # Test credentials that should see these healthmonitors can see them.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin', 'os_roles_lb_member',
                                 'os_roles_lb_global_observer']
         if expected_allowed:
             self.check_list_IDs_RBAC_enforcement(
                 'HealthMonitorClient', 'list_healthmonitors',
@@ -759,15 +760,15 @@
             expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         # Note: os_admin is here because it evaluaties to "project_admin"
         #       in oslo_policy and since keystone considers "project_admin"
         #       a superscope of "project_reader". This means it can read
         #       objects in the "admin" credential's project.
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary', 'os_system_admin',
+            expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_system_reader', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
@@ -1189,16 +1190,16 @@
         # Test that the appropriate users can see or not see the health
         # monitors based on the API RBAC.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_show_RBAC_enforcement(
@@ -1471,15 +1472,16 @@
         # Test that a user, without the loadbalancer member role, cannot
         # update this healthmonitor.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'HealthMonitorClient', 'update_healthmonitor',
                 expected_allowed, None, None, hm[const.ID],
@@ -1774,15 +1776,16 @@
         # Test that a user without the loadbalancer role cannot delete this
         # healthmonitor.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_delete_RBAC_enforcement(
                 'HealthMonitorClient', 'delete_healthmonitor',
                 expected_allowed, None, None, hm[const.ID])
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_l7policy.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_l7policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,16 @@
         # Test that a user without the load balancer role cannot
         # create a l7policy
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_create_RBAC_enforcement(
                 'L7PolicyClient', 'create_l7policy',
                 expected_allowed,
@@ -361,31 +362,31 @@
         test_ids.append(l7policy3[const.ID])
 
         # Test that a different users cannot see the lb_member l7policies
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_primary', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary',
-                                'os_roles_lb_member2', 'os_roles_lb_observer',
+            expected_allowed = ['os_primary', 'os_roles_lb_member2',
+                                'os_roles_lb_observer',
                                 'os_roles_lb_global_observer']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_roles_lb_observer', 'os_roles_lb_member2']
         if expected_allowed:
             self.check_list_RBAC_enforcement_count(
                 'L7PolicyClient', 'list_l7policies',
                 expected_allowed, 0)
 
         # Test credentials that should see these l7policies can see them.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin', 'os_roles_lb_member',
                                 'os_roles_lb_global_observer']
         if expected_allowed:
             self.check_list_IDs_RBAC_enforcement(
                 'L7PolicyClient', 'list_l7policies',
@@ -402,15 +403,15 @@
             expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         # Note: os_admin is here because it evaluaties to "project_admin"
         #       in oslo_policy and since keystone considers "project_admin"
         #       a superscope of "project_reader". This means it can read
         #       objects in the "admin" credential's project.
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary', 'os_system_admin',
+            expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_system_reader', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
@@ -648,16 +649,16 @@
         # Test that the appropriate users can see or not see the L7 policies
         # based on the API RBAC.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_show_RBAC_enforcement(
@@ -757,15 +758,16 @@
         # Test that a user, without the loadbalancer member role, cannot
         # update this L7 policy.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'L7PolicyClient', 'update_l7policy',
                 expected_allowed, None, None, l7policy[const.ID],
@@ -868,15 +870,16 @@
         # Test that a user without the loadbalancer role cannot delete this
         # L7 policy.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_delete_RBAC_enforcement(
                 'L7PolicyClient', 'delete_l7policy',
                 expected_allowed, None, None, l7policy[const.ID])
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_l7rule.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_l7rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,16 @@
         # Test that a user without the loadbalancer role cannot
         # create an L7 rule.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_create_RBAC_enforcement(
                 'L7RuleClient', 'create_l7rule',
                 expected_allowed,
@@ -353,16 +354,16 @@
         test_ids.append(l7rule3[const.ID])
 
         # Test credentials that should see these L7 rules can see them.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin', 'os_roles_lb_member',
                                 'os_roles_lb_global_observer']
         if expected_allowed:
             self.check_list_IDs_RBAC_enforcement(
                 'L7RuleClient', 'list_l7rules', expected_allowed, test_ids,
@@ -376,15 +377,15 @@
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         # Note: os_admin is here because it evaluaties to "project_admin"
         #       in oslo_policy and since keystone considers "project_admin"
         #       a superscope of "project_reader". This means it can read
         #       objects in the "admin" credential's project.
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_system_admin',
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member']
         if expected_allowed:
@@ -562,16 +563,16 @@
         # Test that the appropriate users can see or not see the L7 rule
         # based on the API RBAC.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_show_RBAC_enforcement(
@@ -650,15 +651,16 @@
         # Test that a user, without the loadbalancer member role, cannot
         # update this L7 rule.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'L7RuleClient', 'update_l7rule',
                 expected_allowed, None, None, l7rule[const.ID],
@@ -752,15 +754,16 @@
         # Test that a user without the loadbalancer role cannot delete this
         # L7 rule.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_delete_RBAC_enforcement(
                 'L7RuleClient', 'delete_l7rule',
                 expected_allowed, None, None, l7rule[const.ID],
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_listener.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_listener.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,16 @@
         # Test that a user without the loadbalancer role cannot
         # create a listener.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_create_RBAC_enforcement(
                 'ListenerClient', 'create_listener',
                 expected_allowed,
@@ -560,31 +561,31 @@
                 CONF.load_balancer.build_timeout)
 
         # Test that a different users cannot see the lb_member listeners.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_primary', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary',
-                                'os_roles_lb_member2', 'os_roles_lb_observer',
+            expected_allowed = ['os_primary', 'os_roles_lb_member2',
+                                'os_roles_lb_observer',
                                 'os_roles_lb_global_observer']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_roles_lb_observer', 'os_roles_lb_member2']
         if expected_allowed:
             self.check_list_RBAC_enforcement_count(
                 'ListenerClient', 'list_listeners', expected_allowed, 0,
                 query_params='loadbalancer_id={lb_id}'.format(lb_id=lb_id))
 
         # Test credentials that should see these listeners can see them.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin', 'os_roles_lb_member',
                                 'os_roles_lb_global_observer']
         if expected_allowed:
             self.check_list_IDs_RBAC_enforcement(
                 'ListenerClient', 'list_listeners', expected_allowed,
@@ -600,15 +601,15 @@
             expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         # Note: os_admin is here because it evaluaties to "project_admin"
         #       in oslo_policy and since keystone considers "project_admin"
         #       a superscope of "project_reader". This means it can read
         #       objects in the "admin" credential's project.
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary', 'os_system_admin',
+            expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_system_reader', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
@@ -883,16 +884,16 @@
         # Test that the appropriate users can see or not see the listener
         # based on the API RBAC.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_show_RBAC_enforcement(
@@ -1032,15 +1033,16 @@
         # Test that a user without the loadbalancer role cannot
         # update a listener.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'ListenerClient', 'update_listener',
                 expected_allowed,
@@ -1211,15 +1213,16 @@
         # Test that a user without the loadbalancer role cannot
         # delete a listener.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'ListenerClient', 'delete_listener',
                 expected_allowed,
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_load_balancer.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_load_balancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         lb_kwargs_with_project_id[const.PROJECT_ID] = (
             self.os_roles_lb_member.credentials.project_id)
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin',
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         if expected_allowed:
             self.check_create_RBAC_enforcement(
                 'LoadbalancerClient', 'create_loadbalancer',
@@ -189,15 +189,16 @@
         # Test that a user without the loadbalancer role cannot delete this
         # load balancer.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_delete_RBAC_enforcement(
                 'LoadbalancerClient', 'delete_loadbalancer',
                 expected_allowed, None, None, lb[const.ID])
@@ -238,15 +239,16 @@
         # Test that a user without the loadbalancer role cannot delete this
         # load balancer.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_delete_RBAC_enforcement(
                 'LoadbalancerClient', 'delete_loadbalancer',
                 expected_allowed, None, None, lb[const.ID], cascade=True)
@@ -414,31 +416,31 @@
         test_ids.append(lb3[const.ID])
 
         # Test that a different users cannot see the lb_member load balancers.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_primary', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary',
-                                'os_roles_lb_member2', 'os_roles_lb_observer',
+            expected_allowed = ['os_primary', 'os_roles_lb_member2',
+                                'os_roles_lb_observer',
                                 'os_roles_lb_global_observer']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_roles_lb_observer', 'os_roles_lb_member2']
         if expected_allowed:
             self.check_list_RBAC_enforcement_count(
                 'LoadbalancerClient', 'list_loadbalancers',
                 expected_allowed, 0)
 
         # Test credentials that should see these load balancers can see them.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin', 'os_roles_lb_member',
                                 'os_roles_lb_global_observer']
         if expected_allowed:
             self.check_list_IDs_RBAC_enforcement(
                 'LoadbalancerClient', 'list_loadbalancers',
@@ -453,15 +455,15 @@
             expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         # Note: os_admin is here because it evaluaties to "project_admin"
         #       in oslo_policy and since keystone considers "project_admin"
         #       a superscope of "project_reader". This means it can read
         #       objects in the "admin" credential's project.
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary', 'os_system_admin',
+            expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_system_reader', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
@@ -631,16 +633,16 @@
         # Test that the appropriate users can see or not see the load
         # balancer based on the API RBAC.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_show_RBAC_enforcement(
@@ -735,15 +737,16 @@
         # Test that a user, without the loadbalancer member role, cannot
         # update this load balancer.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'LoadbalancerClient', 'update_loadbalancer',
                 expected_allowed, None, None, lb[const.ID],
@@ -827,16 +830,16 @@
         # Test that the appropriate users can see or not see the load
         # balancer stats based on the API RBAC.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_show_RBAC_enforcement(
@@ -898,16 +901,16 @@
         # Test that the appropriate users can see or not see the load
         # balancer status based on the API RBAC.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_show_RBAC_enforcement(
@@ -974,15 +977,15 @@
 
         # Test that a user without the load balancer admin role cannot
         # failover a load balancer.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'LoadbalancerClient', 'failover_loadbalancer',
                 expected_allowed, None, None, lb[const.ID])
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_member.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_member.py`

 * *Files 0% similar despite different names*

```diff
@@ -898,15 +898,16 @@
         # Test that a user without the loadbalancer role cannot
         # create a member.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_create_RBAC_enforcement(
                 'MemberClient', 'create_member',
                 expected_allowed,
@@ -1229,16 +1230,16 @@
         test_ids.append(member3[const.ID])
 
         # Test credentials that should see these members can see them.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin', 'os_roles_lb_member',
                                 'os_roles_lb_global_observer']
         if expected_allowed:
             self.check_list_IDs_RBAC_enforcement(
                 'MemberClient', 'list_members', expected_allowed,
@@ -1251,15 +1252,15 @@
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         # Note: os_admin is here because it evaluaties to "project_admin"
         #       in oslo_policy and since keystone considers "project_admin"
         #       a superscope of "project_reader". This means it can read
         #       objects in the "admin" credential's project.
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_system_admin',
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member']
         if expected_allowed:
@@ -1794,16 +1795,16 @@
         # Test that the appropriate users can see or not see the member
         # based on the API RBAC.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_show_RBAC_enforcement(
@@ -2251,15 +2252,16 @@
         # Test that a user, without the loadbalancer member role, cannot
         # update this member.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'MemberClient', 'update_member',
                 expected_allowed, None, None, member[const.ID],
@@ -2709,15 +2711,16 @@
         # Test that a user, without the loadbalancer member role, cannot
         # batch update this member.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'MemberClient', 'update_members',
                 expected_allowed, None, None,
@@ -2954,15 +2957,16 @@
         # Test that a user without the loadbalancer role cannot delete this
         # member.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_delete_RBAC_enforcement(
                 'MemberClient', 'delete_member',
                 expected_allowed, None, None, member[const.ID],
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_pool.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,16 @@
         # Test that a user without the loadbalancer role cannot
         # create a pool.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_create_RBAC_enforcement(
                 'PoolClient', 'create_pool',
                 expected_allowed,
@@ -748,31 +749,31 @@
         test_ids.append(pool3[const.ID])
 
         # Test that a different users cannot see the lb_member pools.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_primary', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary',
-                                'os_roles_lb_member2', 'os_roles_lb_observer',
+            expected_allowed = ['os_primary', 'os_roles_lb_member2',
+                                'os_roles_lb_observer',
                                 'os_roles_lb_global_observer']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_roles_lb_observer', 'os_roles_lb_member2']
         if expected_allowed:
             self.check_list_RBAC_enforcement_count(
                 'PoolClient', 'list_pools', expected_allowed, 0,
                 query_params='loadbalancer_id={lb_id}'.format(lb_id=lb_id))
 
         # Test credentials that should see these pools can see them.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin', 'os_roles_lb_member',
                                 'os_roles_lb_global_observer']
         if expected_allowed:
             self.check_list_IDs_RBAC_enforcement(
                 'PoolClient', 'list_pools', expected_allowed, test_ids,
@@ -787,15 +788,15 @@
             expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         # Note: os_admin is here because it evaluaties to "project_admin"
         #       in oslo_policy and since keystone considers "project_admin"
         #       a superscope of "project_reader". This means it can read
         #       objects in the "admin" credential's project.
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary', 'os_system_admin',
+            expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_system_reader', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
@@ -1127,16 +1128,16 @@
         # Test that the appropriate users can see or not see the pool
         # based on the API RBAC.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_system_reader',
-                                'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_system_reader', 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_system_reader',
                                 'os_roles_lb_admin',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_show_RBAC_enforcement(
@@ -1367,15 +1368,16 @@
         # Test that a user, without the loadbalancer member role, cannot
         # update this pool.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_update_RBAC_enforcement(
                 'PoolClient', 'update_pool',
                 expected_allowed, None, None, pool[const.ID],
@@ -1669,15 +1671,16 @@
         # Test that a user without the loadbalancer role cannot delete this
         # pool.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = ['os_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_system_admin', 'os_roles_lb_member']
+            expected_allowed = ['os_admin', 'os_roles_lb_admin',
+                                'os_roles_lb_member']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = ['os_system_admin', 'os_roles_lb_admin',
                                 'os_roles_lb_member']
         if expected_allowed:
             self.check_delete_RBAC_enforcement(
                 'PoolClient', 'delete_pool',
                 expected_allowed, None, None, pool[const.ID])
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/api/v2/test_provider.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/api/v2/test_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         # list providers.
         expected_allowed = []
         if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
             expected_allowed = [
                 'os_admin', 'os_primary', 'os_roles_lb_admin',
                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
-            expected_allowed = ['os_admin', 'os_primary', 'os_system_admin',
+            expected_allowed = ['os_admin', 'os_primary', 'os_roles_lb_admin',
                                 'os_system_reader', 'os_roles_lb_observer',
                                 'os_roles_lb_global_observer',
                                 'os_roles_lb_member', 'os_roles_lb_member2']
         if CONF.load_balancer.RBAC_test_type == const.ADVANCED:
             expected_allowed = [
                 'os_system_admin', 'os_system_reader', 'os_roles_lb_observer',
                 'os_roles_lb_global_observer', 'os_roles_lb_admin',
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/barbican_scenario/v2/test_tls_barbican.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/barbican_scenario/v2/test_tls_barbican.py`

 * *Files 2% similar despite different names*

```diff
@@ -1467,15 +1467,15 @@
             const.ADMIN_STATE_UP: True,
             const.ADDRESS: self.webserver1_ip,
             const.PROTOCOL_PORT: 9443,
         }
         if self.lb_member_1_subnet:
             member1_kwargs[const.SUBNET_ID] = self.lb_member_1_subnet[const.ID]
 
-        self.mem_member_client.create_member(**member1_kwargs)
+        member1 = self.mem_member_client.create_member(**member1_kwargs)
         waiters.wait_for_status(
             self.mem_lb_client.show_loadbalancer, self.lb_id,
             const.PROVISIONING_STATUS, const.ACTIVE,
             CONF.load_balancer.check_interval,
             CONF.load_balancer.check_timeout)
 
         # Set up Member 2 for Webserver 2
@@ -1487,15 +1487,15 @@
             const.ADMIN_STATE_UP: True,
             const.ADDRESS: self.webserver2_ip,
             const.PROTOCOL_PORT: 9443,
         }
         if self.lb_member_2_subnet:
             member2_kwargs[const.SUBNET_ID] = self.lb_member_2_subnet[const.ID]
 
-        self.mem_member_client.create_member(**member2_kwargs)
+        member2 = self.mem_member_client.create_member(**member2_kwargs)
         waiters.wait_for_status(
             self.mem_lb_client.show_loadbalancer, self.lb_id,
             const.PROVISIONING_STATUS, const.ACTIVE,
             CONF.load_balancer.check_interval,
             CONF.load_balancer.check_timeout)
 
         listener_name = data_utils.rand_name(
@@ -1534,17 +1534,187 @@
             CONF.load_balancer.check_timeout)
         waiters.wait_for_status(
             self.mem_pool_client.show_pool, pool_id,
             const.PROVISIONING_STATUS, const.ACTIVE,
             CONF.load_balancer.check_interval,
             CONF.load_balancer.check_timeout)
 
+        # Make sure the health monitor has brought the members up after the
+        # the pool update.
+        waiters.wait_for_status(
+            self.mem_member_client.show_member, member1[const.ID],
+            const.OPERATING_STATUS, const.ONLINE,
+            CONF.load_balancer.check_interval,
+            CONF.load_balancer.check_timeout, error_ok=True, pool_id=pool_id)
+        waiters.wait_for_status(
+            self.mem_member_client.show_member, member2[const.ID],
+            const.OPERATING_STATUS, const.ONLINE,
+            CONF.load_balancer.check_interval,
+            CONF.load_balancer.check_timeout, error_ok=True, pool_id=pool_id)
+
         self.check_members_balanced(self.lb_vip_address, protocol=const.HTTP,
                                     protocol_port=85)
 
+    @decorators.idempotent_id('d3e4c5fe-1726-49e4-b0b0-7a5a47749fc9')
+    def test_basic_h2_listener_http_listener_pool_reencryption(self):
+        """Test both h2 and HTTP traffic on the same load balancer.
+
+        In this test we deploy the following Octavia resources:
+            HTTPS_TERMINATED listener with h2 alpn protocols
+            HTTP listener
+            HTTP pool with both h2 alpn protocols and backend re-encryption
+
+        we send both h2 and http traffic from a client to the load balancer vip
+        and we make sure h2 traffic was negotiated when it was sent on 443 port
+        :raises self.skipException: ALPN support for pools not available prior
+        to v2.24.
+        """
+        if not self.mem_listener_client.is_version_supported(
+                self.api_version, '2.24'):
+            raise self.skipException('ALPN protocols are only available on '
+                                     'pools in Octavia API version 2.24 or'
+                                     ' newer.')
+        pool_name = data_utils.rand_name("lb_member_pool1-tls-alpn")
+        pool_kwargs = {
+            const.NAME: pool_name,
+            const.PROTOCOL: const.HTTP,
+            const.LB_ALGORITHM: self.lb_algorithm,
+            const.LOADBALANCER_ID: self.lb_id,
+            const.TLS_ENABLED: True,
+            const.ALPN_PROTOCOLS: ['h2', 'http/1.1'],
+        }
+
+        pool = self.mem_pool_client.create_pool(**pool_kwargs)
+        pool_id = pool[const.ID]
+
+        self.addCleanup(
+            self.mem_pool_client.cleanup_pool,
+            pool_id,
+            lb_client=self.mem_lb_client, lb_id=self.lb_id)
+
+        waiters.wait_for_status(self.mem_lb_client.show_loadbalancer,
+                                self.lb_id, const.PROVISIONING_STATUS,
+                                const.ACTIVE,
+                                CONF.load_balancer.build_interval,
+                                CONF.load_balancer.build_timeout)
+
+        # Set up Member 1 for Webserver 1
+        member1_name = data_utils.rand_name("lb_member_member1-tls-reencrypt")
+        member1_kwargs = {
+            const.POOL_ID: pool_id,
+            const.NAME: member1_name,
+            const.ADMIN_STATE_UP: True,
+            const.ADDRESS: self.webserver1_ip,
+            const.PROTOCOL_PORT: 443,
+        }
+        if self.lb_member_1_subnet:
+            member1_kwargs[const.SUBNET_ID] = self.lb_member_1_subnet[const.ID]
+
+        member1 = self.mem_member_client.create_member(**member1_kwargs)
+
+        self.addCleanup(
+            self.mem_member_client.cleanup_member,
+            member1[const.ID], pool_id=pool_id,
+            lb_client=self.mem_lb_client,
+            lb_id=self.lb_id)
+
+        waiters.wait_for_status(
+            self.mem_lb_client.show_loadbalancer, self.lb_id,
+            const.PROVISIONING_STATUS, const.ACTIVE,
+            CONF.load_balancer.check_interval,
+            CONF.load_balancer.check_timeout)
+
+        # Set up Member 2 for Webserver 2
+        member2_name = data_utils.rand_name("lb_member_member2-tls-reencrypt")
+        member2_kwargs = {
+            const.POOL_ID: pool_id,
+            const.NAME: member2_name,
+            const.ADMIN_STATE_UP: True,
+            const.ADDRESS: self.webserver2_ip,
+            const.PROTOCOL_PORT: 443,
+        }
+        if self.lb_member_2_subnet:
+            member2_kwargs[const.SUBNET_ID] = self.lb_member_2_subnet[const.ID]
+
+        member2 = self.mem_member_client.create_member(**member2_kwargs)
+
+        self.addCleanup(
+            self.mem_member_client.cleanup_member,
+            member2[const.ID], pool_id=pool_id,
+            lb_client=self.mem_lb_client,
+            lb_id=self.lb_id)
+
+        waiters.wait_for_status(
+            self.mem_lb_client.show_loadbalancer, self.lb_id,
+            const.PROVISIONING_STATUS, const.ACTIVE,
+            CONF.load_balancer.check_interval,
+            CONF.load_balancer.check_timeout)
+
+        listener_name = data_utils.rand_name(
+            "lb_member_listener1-tls-terminated-alpn")
+        listener_kwargs = {
+            const.NAME: listener_name,
+            const.PROTOCOL: const.TERMINATED_HTTPS,
+            const.PROTOCOL_PORT: '443',
+            const.LOADBALANCER_ID: self.lb_id,
+            const.DEFAULT_POOL_ID: pool_id,
+            const.DEFAULT_TLS_CONTAINER_REF: self.server_secret_ref,
+            const.ALPN_PROTOCOLS: ['h2', 'http/1.1']
+        }
+        listener = self.mem_listener_client.create_listener(**listener_kwargs)
+
+        self.addCleanup(
+            self.mem_listener_client.cleanup_listener,
+            listener[const.ID],
+            lb_client=self.mem_lb_client,
+            lb_id=self.lb_id)
+
+        waiters.wait_for_status(self.mem_lb_client.show_loadbalancer,
+                                self.lb_id, const.PROVISIONING_STATUS,
+                                const.ACTIVE,
+                                CONF.load_balancer.build_interval,
+                                CONF.load_balancer.build_timeout)
+
+        listener_name = data_utils.rand_name(
+            "lb_member_listener1-http")
+        listener_kwargs = {
+            const.NAME: listener_name,
+            const.PROTOCOL: const.HTTP,
+            const.PROTOCOL_PORT: 80,
+            const.LOADBALANCER_ID: self.lb_id,
+            const.DEFAULT_POOL_ID: pool_id,
+        }
+        listener = self.mem_listener_client.create_listener(**listener_kwargs)
+        self.listener_id = listener[const.ID]
+        self.addCleanup(
+            self.mem_listener_client.cleanup_listener,
+            self.listener_id,
+            lb_client=self.mem_lb_client, lb_id=self.lb_id)
+
+        waiters.wait_for_status(self.mem_lb_client.show_loadbalancer,
+                                self.lb_id, const.PROVISIONING_STATUS,
+                                const.ACTIVE,
+                                CONF.load_balancer.build_interval,
+                                CONF.load_balancer.build_timeout)
+
+        context = ssl.SSLContext(ssl.PROTOCOL_TLS)
+        context.set_alpn_protocols(['h2', 'http/1.1'])
+        s = socket.socket()
+        ssl_sock = context.wrap_socket(s)
+        ssl_sock.connect((self.lb_vip_address, 443))
+        selected_proto = ssl_sock.selected_alpn_protocol()
+        self.assertEqual('h2', selected_proto)
+
+        # Test HTTPS listener load balancing.
+        self.check_members_balanced(self.lb_vip_address, protocol=const.HTTPS,
+                                    HTTPS_verify=False, protocol_port=443)
+
+        # Test HTTP listener load balancing.
+        self.check_members_balanced(self.lb_vip_address)
+
     @decorators.idempotent_id('7d9dcae6-3e2c-4eae-9bfb-1ef0d00aa530')
     @testtools.skipUnless(
         CONF.loadbalancer_feature_enabled.prometheus_listener_enabled,
         'PROMETHEUS listener tests are disabled in the tempest configuration.')
     def test_tls_prometheus_client_auth_mandatory(self):
         if not self.mem_listener_client.is_version_supported(
                 self.api_version, '2.25'):
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_healthmonitor.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_healthmonitor.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_ipv6_traffic_ops.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_ipv6_traffic_ops.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_l7policy.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_l7policy.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_l7rule.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_l7rule.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_listener.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_listener.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_load_balancer.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_load_balancer.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_member.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_member.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_pool.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_pool.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/scenario/v2/test_traffic_ops.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/scenario/v2/test_traffic_ops.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/spare_pool_scenario/v2/test_spare_pool.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/spare_pool_scenario/v2/test_spare_pool.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/test_base.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,17 +52,18 @@
     """Base class for load balancer tests."""
 
     if CONF.load_balancer.RBAC_test_type == const.OWNERADMIN:
         credentials = [
             'admin', 'primary', ['lb_admin', CONF.load_balancer.admin_role],
             ['lb_member', CONF.load_balancer.member_role],
             ['lb_member2', CONF.load_balancer.member_role]]
-    elif CONF.load_balancer.enforce_new_defaults:
+    elif CONF.load_balancer.RBAC_test_type == const.KEYSTONE_DEFAULT_ROLES:
         credentials = [
-            'admin', 'primary', ['lb_admin', CONF.load_balancer.admin_role],
+            'admin', 'primary',
+            ['lb_admin', CONF.load_balancer.admin_role, 'admin'],
             ['lb_observer', CONF.load_balancer.observer_role, 'reader'],
             ['lb_global_observer', CONF.load_balancer.global_observer_role,
              'reader'],
             ['lb_member', CONF.load_balancer.member_role, 'member'],
             ['lb_member2', CONF.load_balancer.member_role, 'member'],
             ['lb_member_not_default_member', CONF.load_balancer.member_role]]
     else:
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/validators.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,15 +408,15 @@
                 if traffic_member_count == len(response_counts):
                     LOG.debug('Loadbalancer response totals: %s',
                               response_counts)
                     time.sleep(1)
                     return
             except Exception:
                 LOG.warning('Server is not passing initial traffic. Waiting.')
-                time.sleep(1)
+            time.sleep(request_interval)
 
         LOG.debug('Loadbalancer wait for load balancer response totals: %s',
                   response_counts)
         message = ('Server %s on port %s did not begin passing traffic within '
                    'the timeout period. Failing test.' % (vip_address,
                                                           protocol_port))
         LOG.error(message)
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/tests/waiters.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/tests/waiters.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin/version.py` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin/version.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin.egg-info/PKG-INFO` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: octavia-tempest-plugin
-Version: 2.3.0
+Version: 2.4.0
 Summary: Tempest plugin for Octavia
 Home-page: https://docs.openstack.org/octavia-tempest-plugin/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ======================
         Octavia Tempest Plugin
```

### Comparing `octavia-tempest-plugin-2.3.0/octavia_tempest_plugin.egg-info/SOURCES.txt` & `octavia-tempest-plugin-2.4.0/octavia_tempest_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/playbooks/act_stby_iptables/pre.yaml` & `octavia-tempest-plugin-2.4.0/playbooks/act_stby_iptables/pre.yaml`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/releasenotes/notes/Add-RBAC-scoped-tokens-tests-920aa35faf4a8c9d.yaml` & `octavia-tempest-plugin-2.4.0/releasenotes/notes/Add-RBAC-scoped-tokens-tests-920aa35faf4a8c9d.yaml`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/releasenotes/source/conf.py` & `octavia-tempest-plugin-2.4.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/requirements.txt` & `octavia-tempest-plugin-2.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/setup.cfg` & `octavia-tempest-plugin-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/setup.py` & `octavia-tempest-plugin-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/tox.ini` & `octavia-tempest-plugin-2.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `octavia-tempest-plugin-2.3.0/zuul.d/jobs.yaml` & `octavia-tempest-plugin-2.4.0/zuul.d/jobs.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,24 @@
         label: nested-virt-ubuntu-focal
     groups:
       - name: tempest
         nodes:
           - controller
 
 - nodeset:
+    name: octavia-single-node-ubuntu-jammy
+    nodes:
+      - name: controller
+        label: nested-virt-ubuntu-jammy
+    groups:
+      - name: tempest
+        nodes:
+          - controller
+
+- nodeset:
     name: octavia-single-node-centos-7
     nodes:
       - name: controller
         label: nested-virt-centos-7
     groups:
       - name: tempest
         nodes:
@@ -58,17 +68,17 @@
         nodes:
           - controller
 
 - nodeset:
     name: octavia-two-node
     nodes:
       - name: controller
-        label: nested-virt-ubuntu-focal
+        label: nested-virt-ubuntu-jammy
       - name: controller2
-        label: nested-virt-ubuntu-focal
+        label: nested-virt-ubuntu-jammy
     groups:
       - name: controller
         nodes:
           - controller
       # Node where tests are executed and test results collected
       - name: tempest
         nodes:
@@ -205,15 +215,15 @@
         neutron: https://opendev.org/openstack/neutron.git
       tempest_plugins:
         - octavia-tempest-plugin
 
 - job:
     name: octavia-dsvm-live-base
     parent: octavia-dsvm-base
-    nodeset: octavia-single-node-ubuntu-focal
+    nodeset: octavia-single-node-ubuntu-jammy
     timeout: 9000
     required-projects:
       - openstack/diskimage-builder
     vars:
       configure_swap_size: 8192
       devstack_localrc:
         DIB_LOCAL_ELEMENTS: openstack-ci-mirrors
@@ -241,15 +251,15 @@
         '/var/log/dib-build' : logs
         '/var/log/octavia-amphora.log': logs
         '/var/log/octavia-tenant-traffic.log': logs
 
 - job:
     name: octavia-dsvm-live-base-ipv6-only
     parent: octavia-dsvm-base-ipv6-only
-    nodeset: octavia-single-node-ubuntu-focal
+    nodeset: octavia-single-node-ubuntu-jammy
     timeout: 9000
     required-projects:
       - openstack/diskimage-builder
     vars:
       configure_swap_size: 8192
       devstack_localrc:
         DIB_LOCAL_ELEMENTS: openstack-ci-mirrors
@@ -502,54 +512,59 @@
       - ^api-ref/.*$
       - ^doc/.*$
       - ^etc/.*$
       - ^releasenotes/.*$
       - ^octavia_tempest_plugin/tests/(?!api/|\w+\.py).*
 
 - job:
-    name: octavia-v2-dsvm-noop-api-scoped-tokens
+    name: octavia-v2-dsvm-noop-api-keystone-default-roles
     parent: octavia-v2-dsvm-noop-api
     vars:
+      devstack_localrc:
+        OCTAVIA_USE_KEYSTONE_DEFAULT_ROLES: True
       devstack_local_conf:
         post-config:
           $OCTAVIA_CONF:
             oslo_policy:
-              enforce_scope: True
+              enforce_scope: False
               enforce_new_defaults: True
         test-config:
           "$TEMPEST_CONFIG":
             enforce_scope:
-              octavia: True
+              octavia: False
             load_balancer:
-              enforce_new_defaults: True
+              RBAC_test_type: keystone_default_roles
 
 - job:
     name: octavia-v2-dsvm-noop-py2-api
     parent: octavia-v2-dsvm-noop-api
     vars:
       devstack_localrc:
         USE_PYTHON3: False
 
 - job:
     name: octavia-v2-dsvm-noop-api-stable-yoga
     parent: octavia-v2-dsvm-noop-api
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/yoga
 
 - job:
     name: octavia-v2-dsvm-noop-api-stable-xena
     parent: octavia-v2-dsvm-noop-api
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/xena
 
 - job:
     name: octavia-v2-dsvm-noop-api-stable-wallaby
     parent: octavia-v2-dsvm-noop-api
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/wallaby
 
 - job:
-    name: octavia-v2-dsvm-scenario
+    name: octavia-v2-dsvm-scenario-base
     parent: octavia-dsvm-live-base
     vars:
       devstack_local_conf:
         post-config:
           $OCTAVIA_CONF:
             api_settings:
               api_v1_enabled: False
@@ -565,14 +580,44 @@
       - ^api-ref/.*$
       - ^doc/.*$
       - ^etc/.*$
       - ^releasenotes/.*$
       - ^octavia_tempest_plugin/tests/(?!scenario/|\w+\.py).*
 
 - job:
+    name: octavia-v2-dsvm-scenario
+    parent: octavia-v2-dsvm-scenario-base
+    branches: ^(?!stable/(train|ussuri|victoria|wallaby|xena|yoga|zed))
+    nodeset: octavia-single-node-ubuntu-jammy
+
+- job:
+    name: octavia-v2-dsvm-scenario
+    parent: octavia-v2-dsvm-scenario-base
+    branches: ^(stable/(victoria|wallaby|xena|yoga|zed))
+    nodeset: octavia-single-node-ubuntu-focal
+
+- job:
+    name: octavia-v2-dsvm-scenario
+    parent: octavia-v2-dsvm-scenario-base
+    branches: ^(stable/(train|ussuri))
+    nodeset: octavia-single-node-ubuntu-bionic
+
+- job:
+    name: octavia-v2-dsvm-scenario-traffic-ops
+    parent: octavia-v2-dsvm-scenario
+    vars:
+      tempest_test_regex: ^octavia_tempest_plugin.tests.scenario.v2.*traffic_ops
+
+- job:
+    name: octavia-v2-dsvm-scenario-non-traffic-ops
+    parent: octavia-v2-dsvm-scenario
+    vars:
+      tempest_test_regex: ^octavia_tempest_plugin.tests.scenario.v2.(?!.*traffic_ops)
+
+- job:
     name: octavia-v2-dsvm-scenario-ipv6-only
     parent: octavia-dsvm-live-base-ipv6-only
     vars:
       devstack_local_conf:
         post-config:
           $OCTAVIA_CONF:
             api_settings:
@@ -597,26 +642,66 @@
     required-projects:
       - name: openstack/diskimage-builder
         override-checkout: 2.30.0
 
 - job:
     name: octavia-v2-dsvm-scenario-stable-yoga
     parent: octavia-v2-dsvm-scenario
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/yoga
 
 - job:
+    name: octavia-v2-dsvm-scenario-traffic-ops-stable-yoga
+    parent: octavia-v2-dsvm-scenario-stable-yoga
+    vars:
+      tempest_test_regex: ^octavia_tempest_plugin.tests.scenario.v2.*traffic_ops
+
+- job:
+    name: octavia-v2-dsvm-scenario-non-traffic-ops-stable-yoga
+    parent: octavia-v2-dsvm-scenario-stable-yoga
+    vars:
+      tempest_test_regex: ^octavia_tempest_plugin.tests.scenario.v2.(?!.*traffic_ops)
+
+
+- job:
     name: octavia-v2-dsvm-scenario-stable-xena
     parent: octavia-v2-dsvm-scenario
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/xena
 
 - job:
+    name: octavia-v2-dsvm-scenario-traffic-ops-stable-xena
+    parent: octavia-v2-dsvm-scenario-stable-xena
+    vars:
+      tempest_test_regex: ^octavia_tempest_plugin.tests.scenario.v2.*traffic_ops
+
+- job:
+    name: octavia-v2-dsvm-scenario-non-traffic-ops-stable-xena
+    parent: octavia-v2-dsvm-scenario-stable-xena
+    vars:
+      tempest_test_regex: ^octavia_tempest_plugin.tests.scenario.v2.(?!.*traffic_ops)
+
+- job:
     name: octavia-v2-dsvm-scenario-stable-wallaby
     parent: octavia-v2-dsvm-scenario
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/wallaby
 
+- job:
+    name: octavia-v2-dsvm-scenario-traffic-ops-stable-wallaby
+    parent: octavia-v2-dsvm-scenario-stable-wallaby
+    vars:
+      tempest_test_regex: ^octavia_tempest_plugin.tests.scenario.v2.*traffic_ops
+
+- job:
+    name: octavia-v2-dsvm-scenario-non-traffic-ops-stable-wallaby
+    parent: octavia-v2-dsvm-scenario-stable-wallaby
+    vars:
+      tempest_test_regex: ^octavia_tempest_plugin.tests.scenario.v2.(?!.*traffic_ops)
+
 # Legacy jobs for the transition to the act-stdby two node jobs
 - job:
     name: octavia-v2-dsvm-scenario-two-node
     parent: octavia-dsvm-live-two-node-base
     vars:
       tempest_concurrency: 2
       tempest_test_regex: ^octavia_tempest_plugin.tests.scenario.v2
@@ -719,31 +804,42 @@
       devstack_local_conf:
         test-config:
           "$TEMPEST_CONFIG":
             validation:
               ssh_key_type: ecdsa
 
 - job:
-    name: octavia-v2-dsvm-scenario-ubuntu-focal
+    name: octavia-v2-dsvm-scenario-centos-9-stream-traffic-ops
+    parent: octavia-v2-dsvm-scenario-centos-9-stream
+    vars:
+      tempest_test_regex: ^octavia_tempest_plugin.tests.scenario.v2.*traffic_ops
+
+- job:
+    name: octavia-v2-dsvm-scenario-centos-9-stream-non-traffic-ops
+    parent: octavia-v2-dsvm-scenario-centos-9-stream
+    vars:
+      tempest_test_regex: ^octavia_tempest_plugin.tests.scenario.v2.(?!.*traffic_ops)
+
+- job:
+    name: octavia-v2-dsvm-scenario-ubuntu-jammy
     parent: octavia-v2-dsvm-scenario
     vars:
       devstack_localrc:
         OCTAVIA_AMP_BASE_OS: ubuntu
-        OCTAVIA_AMP_DISTRIBUTION_RELEASE_ID: focal
+        OCTAVIA_AMP_DISTRIBUTION_RELEASE_ID: jammy
 
 - job:
-    name: octavia-v2-dsvm-tls-barbican
+    name: octavia-v2-dsvm-tls-barbican-base
     parent: octavia-v2-dsvm-scenario
-    branches: ^(?!stable/(train|ussuri)).*$
     required-projects:
       - openstack/barbican
       - openstack/diskimage-builder
       - openstack/python-barbicanclient
       - openstack/barbican-tempest-plugin
-    vars: &octavia-v2-dsvm-tls-barbican-vars
+    vars:
       tempest_test_regex: ^octavia_tempest_plugin.tests.barbican_scenario.v2
       devstack_services:
         barbican: true
       devstack_plugins:
         barbican: https://opendev.org/openstack/barbican.git
       tempest_plugins:
         - octavia-tempest-plugin
@@ -754,42 +850,58 @@
       - ^doc/.*$
       - ^etc/.*$
       - ^releasenotes/.*$
       - ^octavia_tempest_plugin/tests/(?!barbican_scenario/|\w+\.py).*
 
 - job:
     name: octavia-v2-dsvm-tls-barbican
-    parent: octavia-v2-dsvm-scenario
-    branches: ^(stable/(train|ussuri)).*$
+    parent: octavia-v2-dsvm-tls-barbican-base
+    branches: ^(?!stable/(train|ussuri|victoria|wallaby|xena|yoga|zed))
+    nodeset: octavia-single-node-ubuntu-jammy
+
+- job:
+    name: octavia-v2-dsvm-tls-barbican
+    parent: octavia-v2-dsvm-tls-barbican-base
+    branches: ^(stable/(victoria|wallaby|xena|yoga|zed))
+    nodeset: octavia-single-node-ubuntu-focal
+
+- job:
+    name: octavia-v2-dsvm-tls-barbican
+    parent: octavia-v2-dsvm-tls-barbican-base
+    branches: ^(stable/(train|ussuri))
+    nodeset: octavia-single-node-ubuntu-bionic
     required-projects:
       - openstack/barbican
       - openstack/diskimage-builder
       - openstack/python-barbicanclient
       - name: openstack/barbican-tempest-plugin
         override-checkout: 1.6.0
-    vars: *octavia-v2-dsvm-tls-barbican-vars
 
 - job:
     name: octavia-v2-dsvm-tls-barbican-stable-yoga
     parent: octavia-v2-dsvm-tls-barbican
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/yoga
 
 - job:
     name: octavia-v2-dsvm-tls-barbican-stable-xena
     parent: octavia-v2-dsvm-tls-barbican
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/xena
 
 - job:
     name: octavia-v2-dsvm-tls-barbican-stable-wallaby
     parent: octavia-v2-dsvm-tls-barbican
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/wallaby
 
 - job:
     name: octavia-v2-dsvm-tls-barbican-stable-victoria
     parent: octavia-v2-dsvm-tls-barbican
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/victoria
 
 - job:
     name: octavia-v2-dsvm-tls-barbican-stable-ussuri
     parent: octavia-v2-dsvm-tls-barbican
     nodeset: octavia-single-node-ubuntu-bionic
     override-checkout: stable/ussuri
@@ -824,14 +936,15 @@
     required-projects:
       - name: openstack/diskimage-builder
         override-checkout: 2.30.0
 
 - job:
     name: octavia-v2-dsvm-spare-pool-stable-wallaby
     parent: octavia-v2-dsvm-spare-pool
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/wallaby
 
 - job:
     name: octavia-v2-dsvm-cinder-amphora
     parent: octavia-v2-dsvm-scenario
     required-projects:
       - openstack/cinder
@@ -939,15 +1052,15 @@
       devstack_local_conf:
         test-config:
           "$TEMPEST_CONFIG":
             load_balancer:
               amphora_ssh_user: centos
 
 - job:
-    name: octavia-v2-act-stdby-dsvm-scenario
+    name: octavia-v2-act-stdby-dsvm-scenario-base
     parent: octavia-dsvm-live-base
     vars:
       devstack_local_conf:
         post-config:
           $OCTAVIA_CONF:
             api_settings:
               api_v1_enabled: False
@@ -956,26 +1069,47 @@
             task_flow:
               engine: parallel
       tempest_concurrency: 2
       tempest_test_regex: ^octavia_tempest_plugin.tests.act_stdby_scenario.v2.test_active_standby\.
       tox_envlist: all
 
 - job:
+    name: octavia-v2-act-stdby-dsvm-scenario
+    parent: octavia-v2-act-stdby-dsvm-scenario-base
+    branches: ^(?!stable/(train|ussuri|victoria|wallaby|xena|yoga|zed))
+    nodeset: octavia-single-node-ubuntu-jammy
+
+- job:
+    name: octavia-v2-act-stdby-dsvm-scenario
+    parent: octavia-v2-act-stdby-dsvm-scenario-base
+    branches: ^(stable/(victoria|wallaby|xena|yoga|zed))
+    nodeset: octavia-single-node-ubuntu-focal
+
+- job:
+    name: octavia-v2-act-stdby-dsvm-scenario
+    parent: octavia-v2-act-stdby-dsvm-scenario-base
+    branches: ^(stable/(train|ussuri))
+    nodeset: octavia-single-node-ubuntu-bionic
+
+- job:
     name: octavia-v2-act-stdby-dsvm-scenario-stable-yoga
     parent: octavia-v2-act-stdby-dsvm-scenario
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/yoga
 
 - job:
     name: octavia-v2-act-stdby-dsvm-scenario-stable-xena
     parent: octavia-v2-act-stdby-dsvm-scenario
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/xena
 
 - job:
     name: octavia-v2-act-stdby-dsvm-scenario-stable-wallaby
     parent: octavia-v2-act-stdby-dsvm-scenario
+    nodeset: octavia-single-node-ubuntu-focal
     override-checkout: stable/wallaby
 
 ######### Third party jobs ##########
 
 - job:
     name: neutron-ovn-provider-v2-api
     parent: ovn-octavia-provider-tempest-release
```

### Comparing `octavia-tempest-plugin-2.3.0/zuul.d/projects.yaml` & `octavia-tempest-plugin-2.4.0/zuul.d/projects.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -8,28 +8,34 @@
       - release-notes-jobs-python3
     check:
       jobs:
         - octavia-v2-dsvm-noop-api
         - octavia-v2-dsvm-noop-api-stable-yoga
         - octavia-v2-dsvm-noop-api-stable-xena
         - octavia-v2-dsvm-noop-api-stable-wallaby
-        - octavia-v2-dsvm-noop-api-scoped-tokens
-        - octavia-v2-dsvm-scenario
-        - octavia-v2-dsvm-scenario-stable-yoga
-        - octavia-v2-dsvm-scenario-stable-xena
-        - octavia-v2-dsvm-scenario-stable-wallaby
+        - octavia-v2-dsvm-noop-api-keystone-default-roles
+        - octavia-v2-dsvm-scenario-traffic-ops
+        - octavia-v2-dsvm-scenario-non-traffic-ops
+        - octavia-v2-dsvm-scenario-traffic-ops-stable-yoga
+        - octavia-v2-dsvm-scenario-non-traffic-ops-stable-yoga
+        - octavia-v2-dsvm-scenario-traffic-ops-stable-xena
+        - octavia-v2-dsvm-scenario-non-traffic-ops-stable-xena
+        - octavia-v2-dsvm-scenario-traffic-ops-stable-wallaby
+        - octavia-v2-dsvm-scenario-non-traffic-ops-stable-wallaby
         - octavia-v2-dsvm-tls-barbican
         - octavia-v2-dsvm-tls-barbican-stable-yoga
         - octavia-v2-dsvm-tls-barbican-stable-xena
         - octavia-v2-dsvm-tls-barbican-stable-wallaby
         - octavia-v2-dsvm-scenario-ipv6-only:
             voting: false
         - octavia-v2-dsvm-scenario-centos-8-stream:
             voting: false
-        - octavia-v2-dsvm-scenario-centos-9-stream:
+        - octavia-v2-dsvm-scenario-centos-9-stream-traffic-ops:
+            voting: false
+        - octavia-v2-dsvm-scenario-centos-9-stream-non-traffic-ops:
             voting: false
         - octavia-v2-act-stdby-dsvm-scenario-two-node:
             voting: false
         - octavia-v2-act-stdby-dsvm-scenario:
             voting: false
         - octavia-v2-act-stdby-dsvm-scenario-stable-yoga:
             voting: false
@@ -50,16 +56,20 @@
     gate:
       fail-fast: true
       jobs:
         - octavia-v2-dsvm-noop-api
         - octavia-v2-dsvm-noop-api-stable-yoga
         - octavia-v2-dsvm-noop-api-stable-xena
         - octavia-v2-dsvm-noop-api-stable-wallaby
-        - octavia-v2-dsvm-noop-api-scoped-tokens
-        - octavia-v2-dsvm-scenario
-        - octavia-v2-dsvm-scenario-stable-yoga
-        - octavia-v2-dsvm-scenario-stable-xena
-        - octavia-v2-dsvm-scenario-stable-wallaby
+        - octavia-v2-dsvm-noop-api-keystone-default-roles
+        - octavia-v2-dsvm-scenario-traffic-ops
+        - octavia-v2-dsvm-scenario-non-traffic-ops
+        - octavia-v2-dsvm-scenario-traffic-ops-stable-yoga
+        - octavia-v2-dsvm-scenario-non-traffic-ops-stable-yoga
+        - octavia-v2-dsvm-scenario-traffic-ops-stable-xena
+        - octavia-v2-dsvm-scenario-non-traffic-ops-stable-xena
+        - octavia-v2-dsvm-scenario-traffic-ops-stable-wallaby
+        - octavia-v2-dsvm-scenario-non-traffic-ops-stable-wallaby
         - octavia-v2-dsvm-tls-barbican
         - octavia-v2-dsvm-tls-barbican-stable-yoga
         - octavia-v2-dsvm-tls-barbican-stable-xena
         - octavia-v2-dsvm-tls-barbican-stable-wallaby
```

