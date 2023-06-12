# Comparing `tmp/pyaoscx-2.4.0.tar.gz` & `tmp/pyaoscx-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/ws/chiapuzi/tme/pyaoscx/dist/.tmp-eyqizy5b/pyaoscx-2.4.0.tar", last modified: Tue Apr 18 21:01:16 2023, max compression
+gzip compressed data, was "/ws/pyaoscx/dist/.tmp-xk4mdnyh/pyaoscx-2.4.1.tar", last modified: Mon Jun 12 19:52:59 2023, max compression
```

## Comparing `pyaoscx-2.4.0.tar` & `pyaoscx-2.4.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     4495 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/PKG-INFO
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     3892 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/README.md
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    18333 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/acl.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    21841 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/acl_entry.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    14710 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/aggregate_address.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     6590 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/api.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    14625 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/bgp_neighbor.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    15388 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/bgp_router.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    16209 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/configuration.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    18864 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/device.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    13836 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/dhcp_relay.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    10951 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/dns.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/exceptions/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1087 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/generic_op_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      801 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/login_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      320 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/parameter_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      450 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/pyaoscx_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      879 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/response_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      321 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/unsupported_capability_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      871 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/exceptions/verification_error.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1005 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/firmware.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    83726 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/interface.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    12912 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/ipv6.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    13019 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/mac.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    11167 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/ospf_area.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    10174 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/ospf_interface.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    13376 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/ospf_router.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     8406 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/ospf_virtual_link.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      321 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/ospfv3_router.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     8680 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/poe_interface.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    56938 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/pyaoscx_factory.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    12301 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/pyaoscx_module.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     9780 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/qos.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     9149 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/qos_cos.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    11962 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/qos_dscp.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     9377 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/queue.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     7452 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/queue_profile.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     7662 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/queue_profile_entry.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/rest/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/__init__.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/rest/v1/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v1/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     2703 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v1/api.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    32985 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v1/interface.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_04/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_04/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1321 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_04/api.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      286 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_04/interface.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_08/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_08/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1322 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_08/api.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      286 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_08/interface.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_09/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-10-24 22:31:14.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_09/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1369 2022-10-24 22:31:14.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_09/api.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)      281 2022-10-24 22:31:14.000000 pyaoscx-2.4.0/pyaoscx/rest/v10_09/interface.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    12436 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/session.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    11182 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/static_mac.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    15678 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/static_nexthop.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    16433 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/static_route.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     8288 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/tunnel_endpoint.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx/utils/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/utils/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     3693 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/pyaoscx/utils/list_attributes.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    11109 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/utils/util.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    18698 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/vlan.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     9887 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/vni.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    25272 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/vrf.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)    13186 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/vrf_address_family.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     8257 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/pyaoscx/vsx.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx.egg-info/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     4495 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx.egg-info/PKG-INFO
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1851 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx.egg-info/SOURCES.txt
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        1 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx.egg-info/dependency_links.txt
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        1 2022-08-01 21:22:25.000000 pyaoscx-2.4.0/pyaoscx.egg-info/not-zip-safe
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)       48 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx.egg-info/requires.txt
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)       18 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/pyaoscx.egg-info/top_level.txt
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)       38 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/setup.cfg
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     1159 2023-04-18 21:00:13.000000 pyaoscx-2.4.0/setup.py
-drwxr-xr-x   0 chiapuzi (60029124) warp      (2000)        0 2023-04-18 21:01:16.000000 pyaoscx-2.4.0/workflows/
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)        0 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/workflows/__init__.py
--rw-r--r--   0 chiapuzi (60029124) warp      (2000)     3929 2022-03-04 22:37:13.000000 pyaoscx-2.4.0/workflows/workflow.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-06-12 19:52:59.594485 pyaoscx-2.4.1/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     4495 2023-06-12 19:52:59.594485 pyaoscx-2.4.1/PKG-INFO
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     3892 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/README.md
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-06-12 19:52:59.582485 pyaoscx-2.4.1/pyaoscx/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    18333 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/acl.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    21841 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/acl_entry.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    14710 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/aggregate_address.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     6590 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/api.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    14625 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/bgp_neighbor.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    15388 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/bgp_router.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    16209 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/configuration.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    18864 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/device.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    13836 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/dhcp_relay.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    10951 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/dns.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-06-12 19:52:59.586485 pyaoscx-2.4.1/pyaoscx/exceptions/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/exceptions/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1087 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/exceptions/generic_op_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      801 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/exceptions/login_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      320 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/exceptions/parameter_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      450 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/exceptions/pyaoscx_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      879 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/exceptions/response_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      321 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/exceptions/unsupported_capability_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      871 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/exceptions/verification_error.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1005 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/firmware.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    83726 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/interface.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    12912 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/ipv6.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    13019 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/mac.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    11167 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/ospf_area.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    10174 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/ospf_interface.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    13376 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/ospf_router.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     8406 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/ospf_virtual_link.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      321 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/ospfv3_router.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     8680 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/poe_interface.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    56938 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/pyaoscx_factory.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    12301 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/pyaoscx_module.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     9780 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/qos.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     9149 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/qos_cos.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    11962 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/qos_dscp.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     9377 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/queue.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     7452 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/queue_profile.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     7662 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/queue_profile_entry.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-06-12 19:52:59.586485 pyaoscx-2.4.1/pyaoscx/rest/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/rest/__init__.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-06-12 19:52:59.586485 pyaoscx-2.4.1/pyaoscx/rest/v1/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/rest/v1/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     2703 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/rest/v1/api.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    32985 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/rest/v1/interface.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-06-12 19:52:59.590485 pyaoscx-2.4.1/pyaoscx/rest/v10_04/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/rest/v10_04/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1321 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/rest/v10_04/api.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      286 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/rest/v10_04/interface.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-06-12 19:52:59.590485 pyaoscx-2.4.1/pyaoscx/rest/v10_08/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/rest/v10_08/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1322 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/rest/v10_08/api.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      286 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/rest/v10_08/interface.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-06-12 19:52:59.590485 pyaoscx-2.4.1/pyaoscx/rest/v10_09/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/rest/v10_09/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1369 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/rest/v10_09/api.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)      281 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/rest/v10_09/interface.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    12398 2023-06-12 19:46:52.000000 pyaoscx-2.4.1/pyaoscx/session.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    11182 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/static_mac.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    15678 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/static_nexthop.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    16433 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/static_route.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     8288 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/tunnel_endpoint.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-06-12 19:52:59.590485 pyaoscx-2.4.1/pyaoscx/utils/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/utils/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     3693 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/utils/list_attributes.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    11109 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/utils/util.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    18698 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/vlan.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     9887 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/vni.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    25272 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/vrf.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)    13186 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/vrf_address_family.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     8257 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/pyaoscx/vsx.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-06-12 19:52:59.582485 pyaoscx-2.4.1/pyaoscx.egg-info/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     4495 2023-06-12 19:52:59.000000 pyaoscx-2.4.1/pyaoscx.egg-info/PKG-INFO
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1851 2023-06-12 19:52:59.000000 pyaoscx-2.4.1/pyaoscx.egg-info/SOURCES.txt
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        1 2023-06-12 19:52:59.000000 pyaoscx-2.4.1/pyaoscx.egg-info/dependency_links.txt
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        1 2023-04-18 20:03:22.000000 pyaoscx-2.4.1/pyaoscx.egg-info/not-zip-safe
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)       48 2023-06-12 19:52:59.000000 pyaoscx-2.4.1/pyaoscx.egg-info/requires.txt
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)       18 2023-06-12 19:52:59.000000 pyaoscx-2.4.1/pyaoscx.egg-info/top_level.txt
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)       38 2023-06-12 19:52:59.594485 pyaoscx-2.4.1/setup.cfg
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     1159 2023-06-12 19:46:52.000000 pyaoscx-2.4.1/setup.py
+drwxrwxr-x   0 administrator  (1000) administrator  (1000)        0 2023-06-12 19:52:59.594485 pyaoscx-2.4.1/workflows/
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)        0 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/workflows/__init__.py
+-rw-rw-r--   0 administrator  (1000) administrator  (1000)     3929 2023-04-18 20:01:33.000000 pyaoscx-2.4.1/workflows/workflow.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyaoscx-2.4.0/PKG-INFO` & `pyaoscx-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaoscx
-Version: 2.4.0
+Version: 2.4.1
 Summary: AOS-CX Python Modules
 Home-page: https://github.com/aruba/pyaoscx
 Author: Aruba Automation
 Author-email: aruba-automation@hpe.com
 License: Apache 2.0
 Keywords: networking aruba aos-cx switch rest api python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyaoscx-2.4.0/README.md` & `pyaoscx-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/acl.py` & `pyaoscx-2.4.1/pyaoscx/acl.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/acl_entry.py` & `pyaoscx-2.4.1/pyaoscx/acl_entry.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/aggregate_address.py` & `pyaoscx-2.4.1/pyaoscx/aggregate_address.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/api.py` & `pyaoscx-2.4.1/pyaoscx/api.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/bgp_neighbor.py` & `pyaoscx-2.4.1/pyaoscx/bgp_neighbor.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/bgp_router.py` & `pyaoscx-2.4.1/pyaoscx/bgp_router.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/configuration.py` & `pyaoscx-2.4.1/pyaoscx/configuration.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/device.py` & `pyaoscx-2.4.1/pyaoscx/device.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/dhcp_relay.py` & `pyaoscx-2.4.1/pyaoscx/dhcp_relay.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/dns.py` & `pyaoscx-2.4.1/pyaoscx/dns.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/exceptions/generic_op_error.py` & `pyaoscx-2.4.1/pyaoscx/exceptions/generic_op_error.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/exceptions/login_error.py` & `pyaoscx-2.4.1/pyaoscx/exceptions/login_error.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/exceptions/response_error.py` & `pyaoscx-2.4.1/pyaoscx/exceptions/response_error.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/exceptions/verification_error.py` & `pyaoscx-2.4.1/pyaoscx/exceptions/verification_error.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/firmware.py` & `pyaoscx-2.4.1/pyaoscx/firmware.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/interface.py` & `pyaoscx-2.4.1/pyaoscx/interface.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/ipv6.py` & `pyaoscx-2.4.1/pyaoscx/ipv6.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/mac.py` & `pyaoscx-2.4.1/pyaoscx/mac.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/ospf_area.py` & `pyaoscx-2.4.1/pyaoscx/ospf_area.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/ospf_interface.py` & `pyaoscx-2.4.1/pyaoscx/ospf_interface.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/ospf_router.py` & `pyaoscx-2.4.1/pyaoscx/ospf_router.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/ospf_virtual_link.py` & `pyaoscx-2.4.1/pyaoscx/ospf_virtual_link.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/poe_interface.py` & `pyaoscx-2.4.1/pyaoscx/poe_interface.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/pyaoscx_factory.py` & `pyaoscx-2.4.1/pyaoscx/pyaoscx_factory.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/pyaoscx_module.py` & `pyaoscx-2.4.1/pyaoscx/pyaoscx_module.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/qos.py` & `pyaoscx-2.4.1/pyaoscx/qos.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/qos_cos.py` & `pyaoscx-2.4.1/pyaoscx/qos_cos.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/qos_dscp.py` & `pyaoscx-2.4.1/pyaoscx/qos_dscp.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/queue.py` & `pyaoscx-2.4.1/pyaoscx/queue.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/queue_profile.py` & `pyaoscx-2.4.1/pyaoscx/queue_profile.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/queue_profile_entry.py` & `pyaoscx-2.4.1/pyaoscx/queue_profile_entry.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/rest/v1/api.py` & `pyaoscx-2.4.1/pyaoscx/rest/v1/api.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/rest/v1/interface.py` & `pyaoscx-2.4.1/pyaoscx/rest/v1/interface.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/rest/v10_04/api.py` & `pyaoscx-2.4.1/pyaoscx/rest/v10_04/api.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/rest/v10_08/api.py` & `pyaoscx-2.4.1/pyaoscx/rest/v10_08/api.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/rest/v10_09/api.py` & `pyaoscx-2.4.1/pyaoscx/rest/v10_09/api.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/session.py` & `pyaoscx-2.4.1/pyaoscx/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,14 @@
         s = requests.Session()
         o = requests.utils.urlparse(base_url)
 
         if use_proxy is False:
             s.proxies["no_proxy"] = o.hostname
 
         try:
-            print(base_url + "login")
             response = s.post(
                 base_url + "login",
                 data=login_data,
                 verify=False,
                 timeout=5,
                 proxies=s.proxies,
                 headers=login_headers,
```

### Comparing `pyaoscx-2.4.0/pyaoscx/static_mac.py` & `pyaoscx-2.4.1/pyaoscx/static_mac.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/static_nexthop.py` & `pyaoscx-2.4.1/pyaoscx/static_nexthop.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/static_route.py` & `pyaoscx-2.4.1/pyaoscx/static_route.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/tunnel_endpoint.py` & `pyaoscx-2.4.1/pyaoscx/tunnel_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/utils/list_attributes.py` & `pyaoscx-2.4.1/pyaoscx/utils/list_attributes.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/utils/util.py` & `pyaoscx-2.4.1/pyaoscx/utils/util.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/vlan.py` & `pyaoscx-2.4.1/pyaoscx/vlan.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/vni.py` & `pyaoscx-2.4.1/pyaoscx/vni.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/vrf.py` & `pyaoscx-2.4.1/pyaoscx/vrf.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/vrf_address_family.py` & `pyaoscx-2.4.1/pyaoscx/vrf_address_family.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx/vsx.py` & `pyaoscx-2.4.1/pyaoscx/vsx.py`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/pyaoscx.egg-info/PKG-INFO` & `pyaoscx-2.4.1/pyaoscx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaoscx
-Version: 2.4.0
+Version: 2.4.1
 Summary: AOS-CX Python Modules
 Home-page: https://github.com/aruba/pyaoscx
 Author: Aruba Automation
 Author-email: aruba-automation@hpe.com
 License: Apache 2.0
 Keywords: networking aruba aos-cx switch rest api python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyaoscx-2.4.0/pyaoscx.egg-info/SOURCES.txt` & `pyaoscx-2.4.1/pyaoscx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyaoscx-2.4.0/setup.py` & `pyaoscx-2.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pyaoscx",
-    version="2.4.0",
+    version="2.4.1",
     description="AOS-CX Python Modules",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aruba/pyaoscx",
     author="Aruba Automation",
     author_email="aruba-automation@hpe.com",
     license="Apache 2.0",
```

### Comparing `pyaoscx-2.4.0/workflows/workflow.py` & `pyaoscx-2.4.1/workflows/workflow.py`

 * *Files identical despite different names*

