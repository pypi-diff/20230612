# Comparing `tmp/fabric-message-bus-1.5.0b5.tar.gz` & `tmp/fabric-message-bus-1.5.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-message-bus-1.5.0b5.tar", last modified: Sun Jun 11 02:29:17 2023, max compression
+gzip compressed data, was "fabric-message-bus-1.5.0b6.tar", last modified: Sun Jun 11 23:52:04 2023, max compression
```

## Comparing `fabric-message-bus-1.5.0b5.tar` & `fabric-message-bus-1.5.0b6.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0     1856 2023-05-25 14:23:12.456470 fabric-message-bus-1.5.0b5/.gitignore
--rw-r--r--   0        0        0     1071 2023-05-25 14:23:12.456641 fabric-message-bus-1.5.0b5/LICENSE
--rw-r--r--   0        0        0     3990 2023-05-25 14:24:41.685533 fabric-message-bus-1.5.0b5/README.md
--rwxr-xr-x   0        0        0      203 2023-05-25 14:23:12.456973 fabric-message-bus-1.5.0b5/clean.sh
--rw-r--r--   0        0        0     1560 2023-06-01 19:59:30.435322 fabric-message-bus-1.5.0b5/docker-compose-no-ssl-kafka.yaml
--rw-r--r--   0        0        0     2857 2023-05-25 14:23:12.457153 fabric-message-bus-1.5.0b5/docker-compose.yml
--rw-r--r--   0        0        0       24 2023-06-11 02:28:38.536683 fabric-message-bus-1.5.0b5/fabric_mb/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 14:23:12.457626 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/__init__.py
--rw-r--r--   0        0        0     2089 2023-05-25 14:23:12.457824 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/abc_mb_api.py
--rw-r--r--   0        0        0     5899 2023-05-25 14:23:12.458029 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/admin.py
--rw-r--r--   0        0        0     5881 2023-06-02 19:00:21.506228 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/consumer.py
--rw-r--r--   0        0        0     1301 2023-05-25 14:23:12.458360 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/message_bus_exception.py
--rw-r--r--   0        0        0        0 2023-05-25 14:23:12.458458 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/__init__.py
--rw-r--r--   0        0        0     8062 2023-06-02 18:49:03.390770 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/abc_message_avro.py
--rw-r--r--   0        0        0     3915 2023-06-07 20:36:42.802978 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/abc_object_avro.py
--rw-r--r--   0        0        0     6737 2023-05-25 14:23:12.458921 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/actor_avro.py
--rw-r--r--   0        0        0     2306 2023-05-25 14:23:12.459252 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/add_peer_avro.py
--rw-r--r--   0        0        0     1620 2023-05-25 14:23:12.459510 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/add_reservation_avro.py
--rw-r--r--   0        0        0     3647 2023-05-25 14:23:12.459637 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/add_reservations_avro.py
--rw-r--r--   0        0        0     1578 2023-05-25 14:23:12.459736 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/add_slice_avro.py
--rw-r--r--   0        0        0     3815 2023-05-25 14:23:12.459867 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/add_update_reservation_record.py
--rw-r--r--   0        0        0     3068 2023-05-25 14:23:12.459981 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/add_update_slice_record.py
--rw-r--r--   0        0        0     2077 2023-05-25 14:23:12.460090 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/auth_avro.py
--rw-r--r--   0        0        0     2275 2023-05-25 14:23:12.460193 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/broker_query_model_avro.py
--rw-r--r--   0        0        0     1965 2023-05-25 14:23:12.460399 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/claim_delegation_avro.py
--rw-r--r--   0        0        0     2036 2023-05-25 14:23:12.460571 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/claim_resources_avro.py
--rw-r--r--   0        0        0     1924 2023-05-25 14:23:12.460710 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/close_avro.py
--rw-r--r--   0        0        0     2025 2023-05-25 14:23:12.460895 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/close_delegations_avro.py
--rw-r--r--   0        0        0     2029 2023-05-25 14:23:12.461073 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/close_reservations_avro.py
--rw-r--r--   0        0        0     3044 2023-06-07 20:36:50.400191 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/constants.py
--rw-r--r--   0        0        0     3946 2023-06-04 21:13:21.833540 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/delegation_avro.py
--rw-r--r--   0        0        0     2063 2023-05-25 14:23:12.461627 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/demand_reservation_avro.py
--rw-r--r--   0        0        0     1950 2023-05-25 14:23:12.461780 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/extend_lease_avro.py
--rw-r--r--   0        0        0     3384 2023-05-25 14:23:12.461942 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/extend_reservation_avro.py
--rw-r--r--   0        0        0     1977 2023-05-25 14:23:12.462053 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/extend_ticket_avro.py
--rw-r--r--   0        0        0     2199 2023-05-25 14:23:12.462166 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/failed_rpc_avro.py
--rw-r--r--   0        0        0     1593 2023-05-25 14:23:12.462307 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_actors_request_avro.py
--rw-r--r--   0        0        0     1628 2023-05-25 14:23:12.462527 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py
--rw-r--r--   0        0        0     1591 2023-05-25 14:23:12.462698 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_delegations_avro.py
--rw-r--r--   0        0        0     2016 2023-05-25 14:23:12.462860 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py
--rw-r--r--   0        0        0     1967 2023-05-25 14:23:12.463021 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_reservations_request_avro.py
--rw-r--r--   0        0        0     2544 2023-05-25 14:23:12.463335 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py
--rw-r--r--   0        0        0     1939 2023-05-25 14:23:12.463597 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_sites_request_avro.py
--rw-r--r--   0        0        0     1943 2023-05-25 14:23:12.463894 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_slices_request_avro.py
--rw-r--r--   0        0        0     1959 2023-05-25 14:23:12.464127 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_unit_request_avro.py
--rw-r--r--   0        0        0     5914 2023-05-25 14:23:12.464377 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/lease_reservation_avro.py
--rw-r--r--   0        0        0     1891 2023-05-25 14:23:12.464631 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/lease_reservation_state_avro.py
--rw-r--r--   0        0        0     3444 2023-05-25 14:23:12.464856 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/maintenance_request_avro.py
--rw-r--r--   0        0        0     1970 2023-05-25 14:23:12.465020 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/modify_lease_avro.py
--rw-r--r--   0        0        0     3263 2023-06-08 03:34:35.573911 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/poa_avro.py
--rw-r--r--   0        0        0     2961 2023-06-11 02:25:54.068296 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/poa_info_avro.py
--rw-r--r--   0        0        0     3103 2023-05-25 14:23:12.465213 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/proxy_avro.py
--rw-r--r--   0        0        0     2020 2023-05-25 14:23:12.465372 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/query_avro.py
--rw-r--r--   0        0        0     1904 2023-05-25 14:23:12.465547 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/query_result_avro.py
--rw-r--r--   0        0        0     1972 2023-05-25 14:23:12.465826 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reclaim_delegation_avro.py
--rw-r--r--   0        0        0     2043 2023-05-25 14:23:12.466002 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reclaim_resources_avro.py
--rw-r--r--   0        0        0     1948 2023-05-25 14:23:12.466176 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/redeem_avro.py
--rw-r--r--   0        0        0     1964 2023-05-25 14:23:12.466351 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/relinquish_avro.py
--rw-r--r--   0        0        0     1995 2023-05-25 14:23:12.466510 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/remove_delegation_avro.py
--rw-r--r--   0        0        0     1982 2023-05-25 14:23:12.466651 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/remove_reservation_avro.py
--rw-r--r--   0        0        0     1952 2023-05-25 14:23:12.466787 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/remove_slice_avro.py
--rw-r--r--   0        0        0     4120 2023-05-25 14:23:12.467038 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/request_by_id_record.py
--rw-r--r--   0        0        0     3019 2023-05-25 14:23:12.467342 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reservation_avro.py
--rw-r--r--   0        0        0     7721 2023-05-25 14:23:12.467592 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reservation_mng.py
--rw-r--r--   0        0        0     3126 2023-05-25 14:23:12.467825 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reservation_or_delegation_record.py
--rw-r--r--   0        0        0     2059 2023-05-25 14:23:12.468069 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reservation_predecessor_avro.py
--rw-r--r--   0        0        0     2513 2023-05-25 14:23:12.468350 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reservation_state_avro.py
--rw-r--r--   0        0        0     3193 2023-05-25 14:23:12.468583 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/resource_set_avro.py
--rw-r--r--   0        0        0     3431 2023-05-25 14:23:12.468776 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/resource_ticket_avro.py
--rw-r--r--   0        0        0     1587 2023-05-25 14:23:12.468942 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_actor_avro.py
--rw-r--r--   0        0        0     2550 2023-05-25 14:23:12.469128 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_avro.py
--rw-r--r--   0        0        0     1625 2023-05-25 14:23:12.469377 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_broker_query_model_avro.py
--rw-r--r--   0        0        0     1607 2023-05-25 14:23:12.469563 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_delegation_avro.py
--rw-r--r--   0        0        0     1581 2023-06-02 18:48:46.680999 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_poa_avro.py
--rw-r--r--   0        0        0     1588 2023-05-25 14:23:12.469767 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_proxy_avro.py
--rw-r--r--   0        0        0    11980 2023-06-07 16:42:49.661850 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_record_list.py
--rw-r--r--   0        0        0     1611 2023-05-25 14:23:12.470157 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_reservation_avro.py
--rw-r--r--   0        0        0     1633 2023-05-25 14:23:12.470304 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_reservation_state_avro.py
--rw-r--r--   0        0        0     1662 2023-05-25 14:23:12.470471 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_sites_avro.py
--rw-r--r--   0        0        0     1587 2023-05-25 14:23:12.470680 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_slice_avro.py
--rw-r--r--   0        0        0     3167 2023-05-25 14:23:12.470890 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_string_avro.py
--rw-r--r--   0        0        0     3191 2023-05-25 14:23:12.471165 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_strings_avro.py
--rw-r--r--   0        0        0     1662 2023-05-25 14:23:12.471387 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_units_avro.py
--rw-r--r--   0        0        0     1900 2023-05-25 14:23:12.471588 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/site_avro.py
--rw-r--r--   0        0        0     8670 2023-05-25 14:23:12.471759 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/slice_avro.py
--rw-r--r--   0        0        0     1844 2023-05-25 14:23:12.471938 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/term_avro.py
--rw-r--r--   0        0        0     3474 2023-05-25 14:23:12.472208 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/ticket.py
--rw-r--r--   0        0        0     2810 2023-05-25 14:23:12.472453 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/ticket_avro.py
--rw-r--r--   0        0        0     4436 2023-05-25 14:23:12.472668 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/ticket_reservation_avro.py
--rw-r--r--   0        0        0     3512 2023-05-25 14:23:12.472946 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/unit_avro.py
--rw-r--r--   0        0        0     1759 2023-05-25 14:23:12.473229 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/update_data_avro.py
--rw-r--r--   0        0        0     1969 2023-05-25 14:23:12.473537 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/update_delegation_avro.py
--rw-r--r--   0        0        0     1971 2023-05-25 14:23:12.473754 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/update_lease_avro.py
--rw-r--r--   0        0        0     1631 2023-05-25 14:23:12.473942 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/update_reservation_avro.py
--rw-r--r--   0        0        0     1588 2023-05-25 14:23:12.474164 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/update_slice_avro.py
--rw-r--r--   0        0        0     1975 2023-05-25 14:23:12.474363 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/update_ticket_avro.py
--rw-r--r--   0        0        0     7894 2023-05-25 14:23:12.474547 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/producer.py
--rw-r--r--   0        0        0       92 2023-05-25 14:23:12.474798 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/schema/key.avsc
--rw-r--r--   0        0        0    30841 2023-06-11 02:25:21.991849 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/schema/message.avsc
--rw-r--r--   0        0        0        0 2023-05-25 14:23:12.475455 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/test/__init__.py
--rw-r--r--   0        0        0    15232 2023-05-25 14:23:12.475842 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/test/abqm.graphml
--rw-r--r--   0        0        0    44737 2023-06-04 23:16:17.979513 fabric-message-bus-1.5.0b5/fabric_mb/message_bus/test/message_bus_test.py
--rw-r--r--   0        0        0      747 2023-05-25 14:24:41.685910 fabric-message-bus-1.5.0b5/pyproject.toml
--rwxr-xr-x   0        0        0     2190 2023-05-25 14:23:12.476803 fabric-message-bus-1.5.0b5/secrets/create-certs.sh
--rw-r--r--   0        0        0     4553 1970-01-01 00:00:00.000000 fabric-message-bus-1.5.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1856 2023-05-25 14:23:12.456470 fabric-message-bus-1.5.0b6/.gitignore
+-rw-r--r--   0        0        0     1071 2023-05-25 14:23:12.456641 fabric-message-bus-1.5.0b6/LICENSE
+-rw-r--r--   0        0        0     3990 2023-05-25 14:24:41.685533 fabric-message-bus-1.5.0b6/README.md
+-rwxr-xr-x   0        0        0      203 2023-05-25 14:23:12.456973 fabric-message-bus-1.5.0b6/clean.sh
+-rw-r--r--   0        0        0     1560 2023-06-01 19:59:30.435322 fabric-message-bus-1.5.0b6/docker-compose-no-ssl-kafka.yaml
+-rw-r--r--   0        0        0     2857 2023-05-25 14:23:12.457153 fabric-message-bus-1.5.0b6/docker-compose.yml
+-rw-r--r--   0        0        0       24 2023-06-11 23:51:10.773967 fabric-message-bus-1.5.0b6/fabric_mb/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 14:23:12.457626 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/__init__.py
+-rw-r--r--   0        0        0     2089 2023-05-25 14:23:12.457824 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/abc_mb_api.py
+-rw-r--r--   0        0        0     5899 2023-05-25 14:23:12.458029 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/admin.py
+-rw-r--r--   0        0        0     5881 2023-06-02 19:00:21.506228 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/consumer.py
+-rw-r--r--   0        0        0     1301 2023-05-25 14:23:12.458360 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/message_bus_exception.py
+-rw-r--r--   0        0        0        0 2023-05-25 14:23:12.458458 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/__init__.py
+-rw-r--r--   0        0        0     8256 2023-06-11 21:17:17.932314 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/abc_message_avro.py
+-rw-r--r--   0        0        0     3915 2023-06-07 20:36:42.802978 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/abc_object_avro.py
+-rw-r--r--   0        0        0     6737 2023-05-25 14:23:12.458921 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/actor_avro.py
+-rw-r--r--   0        0        0     2306 2023-05-25 14:23:12.459252 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/add_peer_avro.py
+-rw-r--r--   0        0        0     1620 2023-05-25 14:23:12.459510 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/add_reservation_avro.py
+-rw-r--r--   0        0        0     3647 2023-05-25 14:23:12.459637 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/add_reservations_avro.py
+-rw-r--r--   0        0        0     1578 2023-05-25 14:23:12.459736 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/add_slice_avro.py
+-rw-r--r--   0        0        0     3815 2023-05-25 14:23:12.459867 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/add_update_reservation_record.py
+-rw-r--r--   0        0        0     3068 2023-05-25 14:23:12.459981 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/add_update_slice_record.py
+-rw-r--r--   0        0        0     2077 2023-05-25 14:23:12.460090 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/auth_avro.py
+-rw-r--r--   0        0        0     2275 2023-05-25 14:23:12.460193 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/broker_query_model_avro.py
+-rw-r--r--   0        0        0     1965 2023-05-25 14:23:12.460399 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/claim_delegation_avro.py
+-rw-r--r--   0        0        0     2036 2023-05-25 14:23:12.460571 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/claim_resources_avro.py
+-rw-r--r--   0        0        0     1924 2023-05-25 14:23:12.460710 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/close_avro.py
+-rw-r--r--   0        0        0     2025 2023-05-25 14:23:12.460895 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/close_delegations_avro.py
+-rw-r--r--   0        0        0     2029 2023-05-25 14:23:12.461073 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/close_reservations_avro.py
+-rw-r--r--   0        0        0     3104 2023-06-11 21:18:18.037006 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/constants.py
+-rw-r--r--   0        0        0     3946 2023-06-04 21:13:21.833540 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/delegation_avro.py
+-rw-r--r--   0        0        0     2063 2023-05-25 14:23:12.461627 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/demand_reservation_avro.py
+-rw-r--r--   0        0        0     1950 2023-05-25 14:23:12.461780 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/extend_lease_avro.py
+-rw-r--r--   0        0        0     3384 2023-05-25 14:23:12.461942 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/extend_reservation_avro.py
+-rw-r--r--   0        0        0     1977 2023-05-25 14:23:12.462053 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/extend_ticket_avro.py
+-rw-r--r--   0        0        0     2199 2023-05-25 14:23:12.462166 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/failed_rpc_avro.py
+-rw-r--r--   0        0        0     1593 2023-05-25 14:23:12.462307 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_actors_request_avro.py
+-rw-r--r--   0        0        0     1628 2023-05-25 14:23:12.462527 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py
+-rw-r--r--   0        0        0     1591 2023-05-25 14:23:12.462698 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_delegations_avro.py
+-rw-r--r--   0        0        0     2016 2023-05-25 14:23:12.462860 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py
+-rw-r--r--   0        0        0     1967 2023-05-25 14:23:12.463021 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_reservations_request_avro.py
+-rw-r--r--   0        0        0     2544 2023-05-25 14:23:12.463335 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py
+-rw-r--r--   0        0        0     1939 2023-05-25 14:23:12.463597 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_sites_request_avro.py
+-rw-r--r--   0        0        0     1943 2023-05-25 14:23:12.463894 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_slices_request_avro.py
+-rw-r--r--   0        0        0     1959 2023-05-25 14:23:12.464127 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_unit_request_avro.py
+-rw-r--r--   0        0        0     5914 2023-05-25 14:23:12.464377 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/lease_reservation_avro.py
+-rw-r--r--   0        0        0     1891 2023-05-25 14:23:12.464631 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/lease_reservation_state_avro.py
+-rw-r--r--   0        0        0     3444 2023-05-25 14:23:12.464856 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/maintenance_request_avro.py
+-rw-r--r--   0        0        0     1970 2023-05-25 14:23:12.465020 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/modify_lease_avro.py
+-rw-r--r--   0        0        0     3543 2023-06-11 23:46:05.219266 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/poa_avro.py
+-rw-r--r--   0        0        0     2961 2023-06-11 02:25:54.068296 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/poa_info_avro.py
+-rw-r--r--   0        0        0     3103 2023-05-25 14:23:12.465213 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/proxy_avro.py
+-rw-r--r--   0        0        0     2020 2023-05-25 14:23:12.465372 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/query_avro.py
+-rw-r--r--   0        0        0     1904 2023-05-25 14:23:12.465547 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/query_result_avro.py
+-rw-r--r--   0        0        0     1972 2023-05-25 14:23:12.465826 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reclaim_delegation_avro.py
+-rw-r--r--   0        0        0     2043 2023-05-25 14:23:12.466002 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reclaim_resources_avro.py
+-rw-r--r--   0        0        0     1948 2023-05-25 14:23:12.466176 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/redeem_avro.py
+-rw-r--r--   0        0        0     1964 2023-05-25 14:23:12.466351 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/relinquish_avro.py
+-rw-r--r--   0        0        0     1995 2023-05-25 14:23:12.466510 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/remove_delegation_avro.py
+-rw-r--r--   0        0        0     1982 2023-05-25 14:23:12.466651 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/remove_reservation_avro.py
+-rw-r--r--   0        0        0     1952 2023-05-25 14:23:12.466787 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/remove_slice_avro.py
+-rw-r--r--   0        0        0     4120 2023-05-25 14:23:12.467038 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/request_by_id_record.py
+-rw-r--r--   0        0        0     3019 2023-05-25 14:23:12.467342 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reservation_avro.py
+-rw-r--r--   0        0        0     7721 2023-05-25 14:23:12.467592 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reservation_mng.py
+-rw-r--r--   0        0        0     3126 2023-05-25 14:23:12.467825 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reservation_or_delegation_record.py
+-rw-r--r--   0        0        0     2059 2023-05-25 14:23:12.468069 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reservation_predecessor_avro.py
+-rw-r--r--   0        0        0     2513 2023-05-25 14:23:12.468350 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reservation_state_avro.py
+-rw-r--r--   0        0        0     3193 2023-05-25 14:23:12.468583 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/resource_set_avro.py
+-rw-r--r--   0        0        0     3431 2023-05-25 14:23:12.468776 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/resource_ticket_avro.py
+-rw-r--r--   0        0        0     1587 2023-05-25 14:23:12.468942 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_actor_avro.py
+-rw-r--r--   0        0        0     2550 2023-05-25 14:23:12.469128 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_avro.py
+-rw-r--r--   0        0        0     1625 2023-05-25 14:23:12.469377 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_broker_query_model_avro.py
+-rw-r--r--   0        0        0     1607 2023-05-25 14:23:12.469563 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_delegation_avro.py
+-rw-r--r--   0        0        0     1581 2023-06-02 18:48:46.680999 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_poa_avro.py
+-rw-r--r--   0        0        0     1588 2023-05-25 14:23:12.469767 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_proxy_avro.py
+-rw-r--r--   0        0        0    11980 2023-06-07 16:42:49.661850 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_record_list.py
+-rw-r--r--   0        0        0     1611 2023-05-25 14:23:12.470157 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_reservation_avro.py
+-rw-r--r--   0        0        0     1633 2023-05-25 14:23:12.470304 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_reservation_state_avro.py
+-rw-r--r--   0        0        0     1662 2023-05-25 14:23:12.470471 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_sites_avro.py
+-rw-r--r--   0        0        0     1587 2023-05-25 14:23:12.470680 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_slice_avro.py
+-rw-r--r--   0        0        0     3167 2023-05-25 14:23:12.470890 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_string_avro.py
+-rw-r--r--   0        0        0     3191 2023-05-25 14:23:12.471165 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_strings_avro.py
+-rw-r--r--   0        0        0     1662 2023-05-25 14:23:12.471387 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_units_avro.py
+-rw-r--r--   0        0        0     1900 2023-05-25 14:23:12.471588 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/site_avro.py
+-rw-r--r--   0        0        0     8670 2023-05-25 14:23:12.471759 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/slice_avro.py
+-rw-r--r--   0        0        0     1844 2023-05-25 14:23:12.471938 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/term_avro.py
+-rw-r--r--   0        0        0     3474 2023-05-25 14:23:12.472208 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/ticket.py
+-rw-r--r--   0        0        0     2810 2023-05-25 14:23:12.472453 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/ticket_avro.py
+-rw-r--r--   0        0        0     4436 2023-05-25 14:23:12.472668 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/ticket_reservation_avro.py
+-rw-r--r--   0        0        0     3512 2023-05-25 14:23:12.472946 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/unit_avro.py
+-rw-r--r--   0        0        0     1759 2023-05-25 14:23:12.473229 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/update_data_avro.py
+-rw-r--r--   0        0        0     1969 2023-05-25 14:23:12.473537 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/update_delegation_avro.py
+-rw-r--r--   0        0        0     1971 2023-05-25 14:23:12.473754 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/update_lease_avro.py
+-rw-r--r--   0        0        0     1631 2023-05-25 14:23:12.473942 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/update_reservation_avro.py
+-rw-r--r--   0        0        0     1588 2023-05-25 14:23:12.474164 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/update_slice_avro.py
+-rw-r--r--   0        0        0     1975 2023-05-25 14:23:12.474363 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/update_ticket_avro.py
+-rw-r--r--   0        0        0     7894 2023-05-25 14:23:12.474547 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/producer.py
+-rw-r--r--   0        0        0       92 2023-05-25 14:23:12.474798 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/schema/key.avsc
+-rw-r--r--   0        0        0    30757 2023-06-11 20:56:24.991838 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/schema/message.avsc
+-rw-r--r--   0        0        0        0 2023-05-25 14:23:12.475455 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/test/__init__.py
+-rw-r--r--   0        0        0    15232 2023-05-25 14:23:12.475842 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/test/abqm.graphml
+-rw-r--r--   0        0        0    44737 2023-06-04 23:16:17.979513 fabric-message-bus-1.5.0b6/fabric_mb/message_bus/test/message_bus_test.py
+-rw-r--r--   0        0        0      747 2023-05-25 14:24:41.685910 fabric-message-bus-1.5.0b6/pyproject.toml
+-rwxr-xr-x   0        0        0     2190 2023-05-25 14:23:12.476803 fabric-message-bus-1.5.0b6/secrets/create-certs.sh
+-rw-r--r--   0        0        0     4553 1970-01-01 00:00:00.000000 fabric-message-bus-1.5.0b6/PKG-INFO
```

### Comparing `fabric-message-bus-1.5.0b5/.gitignore` & `fabric-message-bus-1.5.0b6/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/LICENSE` & `fabric-message-bus-1.5.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/README.md` & `fabric-message-bus-1.5.0b6/README.md`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/docker-compose-no-ssl-kafka.yaml` & `fabric-message-bus-1.5.0b6/docker-compose-no-ssl-kafka.yaml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/docker-compose.yml` & `fabric-message-bus-1.5.0b6/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/abc_mb_api.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/abc_mb_api.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/admin.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/admin.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/consumer.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/consumer.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/message_bus_exception.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/message_bus_exception.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/abc_message_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/abc_message_avro.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
+import pickle
 from abc import ABC
 from uuid import uuid4
 
 from fabric_mb.message_bus.message_bus_exception import MessageBusException
 from fabric_mb.message_bus.messages.abc_object_avro import AbcObjectAvro
 from fabric_mb.message_bus.messages.auth_avro import AuthAvro
 from fabric_mb.message_bus.messages.constants import Constants
@@ -131,14 +132,18 @@
         result = self.__dict__.copy()
 
         for k in self.__dict__:
             if result[k] is None or k == Constants.ID or k == Constants.ATTEMPT:
                 result.pop(k)
             elif isinstance(result[k], AbcObjectAvro):
                 result[k] = result[k].to_dict()
+            elif k in [Constants.VCPU_CPU_MAP, Constants.NODE_SET]:
+                v = result[k]
+                if v is not None:
+                    result[k] = pickle.dumps(v)
             elif isinstance(result[k], list):
                 temp = []
                 for elem in result[k]:
                     if isinstance(elem, AbcObjectAvro):
                         temp.append(elem.to_dict())
                     else:
                         temp.append(elem)
```

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/abc_object_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/abc_object_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/actor_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/actor_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/add_peer_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/add_peer_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/add_reservation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/add_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/add_reservations_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/add_reservations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/add_slice_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/add_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/add_update_reservation_record.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/add_update_reservation_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/add_update_slice_record.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/add_update_slice_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/auth_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/auth_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/broker_query_model_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/broker_query_model_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/claim_delegation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/claim_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/claim_resources_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/claim_resources_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/close_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/close_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/close_delegations_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/close_delegations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/close_reservations_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/close_reservations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/constants.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     SLICE_ID = "slice_id"
     ACTOR_ID = "actor_id"
     PROPERTIES = "properties"
     SLIVER = "sliver"
     MAINT_INFO = "maint_info"
     POAS = "poas"
     INFO = "info"
+    VCPU_CPU_MAP = "vcpu_cpu_map"
+    NODE_SET = "node_set"
     BROKER = "broker"
     TICKET = "ticket"
     RENEWABLE = "renewable"
     RENEW_TIME = "renew_time"
     UNIT_SET = "unit_set"
     UNITS = "units"
     PROXIES = "proxies"
```

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/delegation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/demand_reservation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/demand_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/extend_lease_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/extend_lease_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/extend_reservation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/extend_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/extend_ticket_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/extend_ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/failed_rpc_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/failed_rpc_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_actors_request_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_actors_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_delegations_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_delegations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_reservations_request_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_reservations_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_sites_request_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_sites_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_slices_request_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_slices_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/get_unit_request_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/get_unit_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/lease_reservation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/lease_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/lease_reservation_state_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/lease_reservation_state_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/maintenance_request_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/maintenance_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/modify_lease_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/modify_lease_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/poa_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/poa_info_avro.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,69 +19,72 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
-from typing import List, Dict
-from uuid import uuid4
+import pickle
 
-from fabric_mb.message_bus.messages.abc_message_avro import AbcMessageAvro
+from fabric_mb.message_bus.messages.abc_object_avro import AbcObjectAvro
 from fabric_mb.message_bus.messages.auth_avro import AuthAvro
 
 
-class PoaAvro(AbcMessageAvro):
+class PoaInfoAvro(AbcObjectAvro):
     """
     Implements Avro representation of a query Message
     """
-    def __init__(self, *, operation: str = None, vcpu_cpu_map: List[Dict[str, str]] = None,
-                 node_set: List[str] = None, callback_topic: str = None, rid: str = None, project_id: str = None,
-                 id_token: str = None, message_id: str = None, auth: AuthAvro = None, poa_id: str = None,
-                 sequence: int = None, slice_id: str = None):
-        super(PoaAvro, self).__init__(callback_topic=callback_topic, id_token=id_token,
-                                      name=AbcMessageAvro.poa, message_id=message_id)
+    def __init__(self, *, operation: str = None, info=None, rid: str = None, auth: AuthAvro = None,
+                 poa_id: str = None, project_id: str = None, slice_id: str = None, state: str = None,
+                 error: str = None):
         self.operation = operation
-        self.auth = auth
+        self.info = info
         self.rid = rid
-        self.vcpu_cpu_map = vcpu_cpu_map
-        self.node_set = node_set
+        self.auth = auth
         self.poa_id = poa_id
         self.project_id = project_id
-        self.sequence = sequence
         self.slice_id = slice_id
-        if self.poa_id is None:
-            self.poa_id = uuid4().__str__()
+        self.state = state
+        self.error = error
 
-    def get_node_set(self) -> List[str]:
-        return self.node_set
-
-    def get_vcpu_cpu_map(self) -> List[Dict[str, str]]:
-        return self.vcpu_cpu_map
+    def get_info(self) -> dict:
+        """
+        Return Cpu Info
+        """
+        if self.info is not None:
+            if not isinstance(self.info, dict):
+                self.info = pickle.loads(self.info)
+        return self.info
 
     def get_operation(self) -> str:
         return self.operation
 
-    def get_poa_id(self) -> str:
-        return self.poa_id
-
     def get_rid(self) -> str:
         return self.rid
 
     def get_project_id(self) -> str:
         return self.project_id
 
-    def get_sequence(self) -> int:
-        return self.sequence
+    def get_auth(self) -> AuthAvro:
+        return self.auth
+
+    def get_poa_id(self) -> str:
+        return self.poa_id
 
     def get_slice_id(self) -> str:
         return self.slice_id
 
+    def get_state(self) -> str:
+        return self.state
+
+    def get_error(self) -> str:
+        return self.error
+
     def validate(self) -> bool:
         """
         Check if the object is valid and contains all mandatory fields
         :return True on success; False on failure
         """
-        ret_val = super().validate()
-        if self.callback_topic is None or self.operation is None:
+        ret_val = True
+        if self.operation is None:
             ret_val = False
         return ret_val
```

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/poa_info_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/poa_avro.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,71 +20,74 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import pickle
+from typing import List, Dict
+from uuid import uuid4
 
-from fabric_mb.message_bus.messages.abc_object_avro import AbcObjectAvro
+from fabric_mb.message_bus.messages.abc_message_avro import AbcMessageAvro
 from fabric_mb.message_bus.messages.auth_avro import AuthAvro
 
 
-class PoaInfoAvro(AbcObjectAvro):
+class PoaAvro(AbcMessageAvro):
     """
     Implements Avro representation of a query Message
     """
-    def __init__(self, *, operation: str = None, info=None, rid: str = None, auth: AuthAvro = None,
-                 poa_id: str = None, project_id: str = None, slice_id: str = None, state: str = None,
-                 error: str = None):
+    def __init__(self, *, operation: str = None, vcpu_cpu_map = None, node_set = None, callback_topic: str = None,
+                 rid: str = None, project_id: str = None, id_token: str = None, message_id: str = None,
+                 auth: AuthAvro = None, poa_id: str = None, sequence: int = None, slice_id: str = None):
+        super(PoaAvro, self).__init__(callback_topic=callback_topic, id_token=id_token,
+                                      name=AbcMessageAvro.poa, message_id=message_id)
         self.operation = operation
-        self.info = info
-        self.rid = rid
         self.auth = auth
+        self.rid = rid
+        self.vcpu_cpu_map = vcpu_cpu_map
+        self.node_set = node_set
         self.poa_id = poa_id
         self.project_id = project_id
+        self.sequence = sequence
         self.slice_id = slice_id
-        self.state = state
-        self.error = error
+        if self.poa_id is None:
+            self.poa_id = uuid4().__str__()
 
-    def get_info(self) -> dict:
-        """
-        Return Cpu Info
-        """
-        if self.info is not None:
-            if not isinstance(self.info, dict):
-                self.info = pickle.loads(self.info)
-        return self.info
+    def get_node_set(self) -> List[str]:
+        if self.node_set is not None:
+            if not isinstance(self.node_set, List):
+                self.node_set = pickle.loads(self.node_set)
+        return self.node_set
+
+    def get_vcpu_cpu_map(self) -> List[Dict[str, str]]:
+        if self.vcpu_cpu_map is not None:
+            if not isinstance(self.vcpu_cpu_map, List):
+                self.vcpu_cpu_map = pickle.loads(self.vcpu_cpu_map)
+        return self.vcpu_cpu_map
 
     def get_operation(self) -> str:
         return self.operation
 
+    def get_poa_id(self) -> str:
+        return self.poa_id
+
     def get_rid(self) -> str:
         return self.rid
 
     def get_project_id(self) -> str:
         return self.project_id
 
-    def get_auth(self) -> AuthAvro:
-        return self.auth
-
-    def get_poa_id(self) -> str:
-        return self.poa_id
+    def get_sequence(self) -> int:
+        return self.sequence
 
     def get_slice_id(self) -> str:
         return self.slice_id
 
-    def get_state(self) -> str:
-        return self.state
-
-    def get_error(self) -> str:
-        return self.error
-
     def validate(self) -> bool:
         """
         Check if the object is valid and contains all mandatory fields
         :return True on success; False on failure
         """
-        ret_val = True
-        if self.operation is None:
+        ret_val = super().validate()
+        if self.callback_topic is None or self.operation is None:
             ret_val = False
         return ret_val
```

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/proxy_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/proxy_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/query_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/query_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/query_result_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/query_result_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reclaim_delegation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reclaim_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reclaim_resources_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reclaim_resources_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/redeem_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/redeem_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/relinquish_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/relinquish_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/remove_delegation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/remove_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/remove_reservation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/remove_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/remove_slice_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/remove_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/request_by_id_record.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/request_by_id_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reservation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reservation_mng.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reservation_mng.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reservation_or_delegation_record.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reservation_or_delegation_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reservation_predecessor_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reservation_predecessor_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/reservation_state_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/reservation_state_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/resource_set_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/resource_set_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/resource_ticket_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/resource_ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_actor_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_actor_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_broker_query_model_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_broker_query_model_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_delegation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_poa_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_poa_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_proxy_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_proxy_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_record_list.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_record_list.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_reservation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_reservation_state_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_reservation_state_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_sites_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_sites_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_slice_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_string_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_string_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_strings_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_strings_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/result_units_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/result_units_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/site_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/site_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/slice_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/term_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/term_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/ticket.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/ticket.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/ticket_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/ticket_reservation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/ticket_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/unit_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/unit_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/update_data_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/update_data_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/update_delegation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/update_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/update_lease_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/update_lease_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/update_reservation_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/update_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/update_slice_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/update_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/messages/update_ticket_avro.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/messages/update_ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/producer.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/producer.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/schema/message.avsc` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/schema/message.avsc`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999352499352501%*

 * *Differences: {'20': "{'fields': {11: {'type': {insert: [(1, 'bytes')], delete: [1]}}, 12: {'type': {insert: "*

 * *       "[(1, 'bytes')], delete: [1]}}}}"}*

```diff
@@ -1140,32 +1140,23 @@
                 ]
             },
             {
                 "default": null,
                 "name": "vcpu_cpu_map",
                 "type": [
                     "null",
-                    {
-                        "items": {
-                            "type": "map",
-                            "values": "string"
-                        },
-                        "type": "array"
-                    }
+                    "bytes"
                 ]
             },
             {
                 "default": null,
                 "name": "node_set",
                 "type": [
                     "null",
-                    {
-                        "items": "string",
-                        "type": "array"
-                    }
+                    "bytes"
                 ]
             }
         ],
         "name": "PoaRequest",
         "namespace": "fabric.cf.model",
         "type": "record"
     },
```

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/test/abqm.graphml` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/test/abqm.graphml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/fabric_mb/message_bus/test/message_bus_test.py` & `fabric-message-bus-1.5.0b6/fabric_mb/message_bus/test/message_bus_test.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/pyproject.toml` & `fabric-message-bus-1.5.0b6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/secrets/create-certs.sh` & `fabric-message-bus-1.5.0b6/secrets/create-certs.sh`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b5/PKG-INFO` & `fabric-message-bus-1.5.0b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-message-bus
-Version: 1.5.0b5
+Version: 1.5.0b6
 Summary: Fabric Message Bus Schema
 Keywords: Kafka,Fabric Message Bus Schema,Avro
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

