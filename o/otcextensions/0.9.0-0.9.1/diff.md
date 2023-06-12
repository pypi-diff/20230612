# Comparing `tmp/otcextensions-0.9.0.tar.gz` & `tmp/otcextensions-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/otcextensions-0.9.0.tar", last modified: Wed Sep  2 15:41:36 2020, max compression
+gzip compressed data, was "dist/otcextensions-0.9.1.tar", last modified: Thu Oct 15 10:30:05 2020, max compression
```

## Comparing `otcextensions-0.9.0.tar` & `otcextensions-0.9.1.tar`

### file list

```diff
@@ -1,1431 +1,1531 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2020-09-02 15:40:47.000000 otcextensions-0.9.0/.stestr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/clustering/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/clustering/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4231 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/clustering/cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/clustering/policy_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2221 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/clustering/node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1109 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/clustering/action.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/clustering/profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/clustering/profile_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2111 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/clustering/receiver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1875 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/clustering/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1094 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/clustering/event.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/dns/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/list_nameservers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/find_recordset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/create_recordset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/get_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/get_recordset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/unset_floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/get_floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/find_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/update_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/update_floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/delete_recordset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/delete_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/list_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/remove_router_from_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/update_recordset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/list_recordsets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/list_floating_ips.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      864 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/set_floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/add_router_to_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1298 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dns/create_zone.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/cts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cts/list_traces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cts/create_tracker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cts/get_tracker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cts/delete_tracker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1246 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cts/update_tracker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/rds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/get_instance_backup_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/create_backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1055 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/create_configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/find_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/apply_configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/list_datastores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      985 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/wait_for_backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1547 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/create_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/delete_configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/get_configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/get_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/get_instance_restore_time.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/list_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/find_backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/list_backup_download_links.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1150 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/update_configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/restore_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/list_configurations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/list_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/list_datastore_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/find_configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/set_instance_backup_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/rds/list_backups.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2098 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/compute/create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/compute/delete.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/compute/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/compute/find.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/compute/list.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/cloud/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/debug-logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/munch-dict-object.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/upload-object.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/service-conditional-overrides.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/service-conditionals.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/create-server-name-or-id.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/strict-mode.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/upload-large-object.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/http-debug-logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/normalization.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/user-agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/cleanup-servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/server-information.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/find-an-image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1469 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cloud/create-server-dict.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/connect_otc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/cce/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cce/list_clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cce/list_cluster_nodes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cce/get_job.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cce/delete_cluster_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cce/get_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cce/find_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cce/find_cluster_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cce/delete_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1566 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cce/create_cluster_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1556 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cce/create_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cce/get_cluster_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/cce/wait_for_job.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/dcs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/create_backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      827 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/find_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/delete_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/list_statistics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/create_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/stop_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/delete_backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/get_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      839 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/list_instance_params.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      822 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/update_instance_params.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/list_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/start_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/update_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/extend_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/restore_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/list_restore_records.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/change_instance_password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/list_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/dcs/restart_instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/auto_scaling/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/execute_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/create_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/get_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/batch_instance_action.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/find_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/get_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/get_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/pause_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/list_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/list_policies.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/remove_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/list_activities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/delete_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/list_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      874 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/resume_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/resume_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/list_configs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/delete_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/find_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/create_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/batch_delete_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/list_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/init.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1233 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/update_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/pause_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/find_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/create_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/auto_scaling/delete_group.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/identity/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2522 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/identity/list.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/key_manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/key_manager/create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/key_manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/key_manager/get.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/key_manager/list.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/kms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      726 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/list_keys.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/create_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/create_datakey.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/encrypt_datakey.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/enable_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/get_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/create_datakey_without_plaintext.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/generate_random_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/schedule_key_deletion.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/cancel_key_deletion.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/disable_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/list_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/find_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/get_instance_number.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/kms/decrypt_datakey.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/vpc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/vpc/create_peering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/vpc/find_peering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/vpc/get_peering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/vpc/get_route.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      738 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/vpc/list_peerings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/vpc/add_route.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/vpc/set_peering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/vpc/list_routes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/vpc/update_peering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/vpc/delete_route.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/vpc/delete_peering.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/network/create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/network/delete.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/network/find.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/network/list.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/network/security_group_rules.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/baremetal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/baremetal/provisioning.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/baremetal/list.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/anti_ddos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/anti_ddos/update_floating_ip_policies.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/anti_ddos/list_floating_ip_stat_day.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/anti_ddos/list_floating_ip_events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/anti_ddos/list_configs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/anti_ddos/get_floating_ip_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/anti_ddos/protect_floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/anti_ddos/get_floating_ip_policies.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/anti_ddos/unprotect_floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/anti_ddos/list_floating_ips.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/anti_ddos/list_floating_ip_stat_week.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/image/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1162 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/image/create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      927 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/image/delete.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/image/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2261 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/image/download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/image/list.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/deh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/deh/create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/deh/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/deh/list.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/deh/list_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/deh/list_servers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/examples/nat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      827 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/get_dnat_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/create_snat_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/create_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/update_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/delete_snat_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/get_snat_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/find_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/delete_dnat_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1213 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/create_dnat_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/list_gateways.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/delete_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/list_dnat_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/list_snat_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/nat/get_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2830 2020-09-02 15:40:47.000000 otcextensions-0.9.0/examples/connect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2020-09-02 15:40:47.000000 otcextensions-0.9.0/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10909 2020-09-02 15:41:36.000000 otcextensions-0.9.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2020-09-02 15:40:47.000000 otcextensions-0.9.0/bindep.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2020-09-02 15:40:47.000000 otcextensions-0.9.0/.testr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4525 2020-09-02 15:40:47.000000 otcextensions-0.9.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/spec/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3616 2020-09-02 15:40:47.000000 otcextensions-0.9.0/spec/python-otcextensions.spec
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3945 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/architecture.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/dns/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/dns/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dns/v2/floating_ip.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dns/v2/recordset.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dns/v2/nameserver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dns/v2/zone.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dns/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/cts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/cts/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/cts/v1/tracker.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/cts/v1/trace.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/cts/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/rds/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/rds/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/rds/v1/flavor.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/rds/v1/configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/rds/v1/instance.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/rds/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/rds/v3/flavor.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/rds/v3/configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/rds/v3/instance.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/rds/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/cce/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/cce/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/cce/v1/cluster.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/cce/v1/cluster_node.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/cce/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/cce/v3/cluster.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/cce/v3/cluster_node.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/cce/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/dcs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/dcs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dcs/v1/config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dcs/v1/restore.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dcs/v1/instance.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dcs/v1/backup.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dcs/v1/statistic.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dcs/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/obs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/obs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/obs/v1/obj.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/obs/v1/container.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/obs/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/auto_scaling/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/auto_scaling/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/auto_scaling/v1/config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/auto_scaling/v1/quota.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/auto_scaling/v1/instance.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/auto_scaling/v1/policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/auto_scaling/v1/activity.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/auto_scaling/v1/group.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/auto_scaling/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/kms/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/kms/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/kms/v1/data_key.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/kms/v1/key.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/kms/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/vpc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/vpc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/vpc/v2/peering.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/vpc/v2/route.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/vpc/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/dms/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/dms/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dms/v1/misc.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dms/v1/message.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dms/v1/topic.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dms/v1/queue.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dms/v1/misc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dms/v1/instance.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dms/v1/group.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/dms/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/anti_ddos/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/anti_ddos/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/anti_ddos/v1/status.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/anti_ddos/v1/floating_ip.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/anti_ddos/v1/config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/anti_ddos/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/deh/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/deh/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/deh/v1/host.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/deh/v1/server.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/deh/v1/host_type.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/deh/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/nat/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/nat/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/nat/v2/snat.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/nat/v2/gateway.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/nat/v2/dnat.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/nat/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1568 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/waf/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/resources/waf/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/waf/v1/domain.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/waf/v1/certificate.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/resources/waf/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/proxies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/cce_v1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1184 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/rds_v1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/kms.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/dms.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1557 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/rds_v3.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/volume_backup.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/dns.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/dcs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/vpc.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/deh.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/anti_ddos.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1519 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/auto_scaling.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/nat.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/waf.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1962 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/cce_v3.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/proxies/cts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2991 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/getting_started.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/sdk/guides/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4855 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/guides/kms.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6155 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/guides/dns.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5230 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/guides/dcs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3486 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/guides/vpc.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1987 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/guides/deh.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6864 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/guides/rds.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3022 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/guides/anti_ddos.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8050 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/guides/auto_scaling.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4302 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/guides/nat.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3605 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/guides/cce.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4100 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/guides/logging.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/guides/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2336 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/guides/cts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/sdk/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/kms.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/dms.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      915 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/rds_v3.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      601 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/volume_backup.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/dns.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/dcs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/vpc.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/deh.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      581 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/anti_ddos.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/auto_scaling.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/load_balancer.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/nat.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/cce_v2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/cli/cts.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/appendices/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3595 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/appendices/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6762 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/appendices/issues.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4901 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/appendices/glossary.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/appendices/releasenotes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/appendices/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4942 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/enforcer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1850 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/coverage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3167 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/install/source_install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5595 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/install/configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3645 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4509 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/install/pip_install.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/contributor/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/contributor/create/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7623 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/contributor/create/resource.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/contributor/create/examples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/doc/source/contributor/create/examples/resource/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/contributor/create/examples/resource/fake_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/contributor/create/examples/resource/fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4773 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/contributor/setup.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4763 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/contributor/testing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/contributor/local.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/contributor/layout.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5236 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/contributor/coding.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4268 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/contributor/layout.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2445 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/source/contributor/clouds.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/rtfd_requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2020-09-02 15:40:47.000000 otcextensions-0.9.0/doc/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2020-09-02 15:40:47.000000 otcextensions-0.9.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1117 2020-09-02 15:40:47.000000 otcextensions-0.9.0/.travis.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2020-09-02 15:40:47.000000 otcextensions-0.9.0/.coveragerc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1383 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/_hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/plas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/plas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/plas/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/plas/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/plas/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/plas/plas_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/css/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/css/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/css/css_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/css/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4557 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/css/v1/flavor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/css/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2793 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/css/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4488 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/css/v1/cluster.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dns/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dns/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dns/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12609 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dns/v2/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4070 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dns/v2/zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dns/v2/nameserver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1390 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dns/v2/floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2346 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dns/v2/recordset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4439 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dns/v2/_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dns/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dns/dns_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/lts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/lts/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/lts/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/lts/v2/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/lts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/lts/lts_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/cts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/cts/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4475 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cts/v1/tracker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cts/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3442 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cts/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cts/v1/trace.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cts/cts_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/mrs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/mrs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/mrs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/mrs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/mrs/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/mrs/mrs_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10253 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/rds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1369 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v1/flavor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20634 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6952 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v1/configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1782 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v1/datastore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3953 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v1/backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7549 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v1/instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v3/flavor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16084 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v3/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3683 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v3/configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5890 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v3/_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v3/datastore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5618 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v3/backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11919 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/v3/instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/rds/rds_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/compute/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/compute/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/compute/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/compute/v2/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2663 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/compute/v2/server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/compute/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/cloud/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cloud/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10617 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cloud/rds.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dws/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dws/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dws/dws_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dws/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dws/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dws/v1/_proxy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/cce/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8030 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/cce_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6244 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6687 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v1/cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9547 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v1/cluster_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1372 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v1/_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9413 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v3/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3216 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v3/cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3259 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v3/cluster_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2835 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v3/cluster_cert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8845 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v3/_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/cce/v3/job.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dcs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dcs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dcs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dcs/v1/restore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dcs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10461 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dcs/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1816 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dcs/v1/statistic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1987 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dcs/v1/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2950 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dcs/v1/backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8774 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dcs/v1/instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dcs/dcs_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/obs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/obs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/obs/obs_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/obs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/obs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17367 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/obs/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5346 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/obs/v1/container.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1694 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/obs/v1/_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6116 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/obs/v1/obj.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/sdrs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/sdrs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/sdrs/sdrs_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/sdrs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/sdrs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/sdrs/v1/_proxy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/auto_scaling/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/auto_scaling/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/auto_scaling/auto_scaling_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18682 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2324 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/activity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4056 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2834 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5061 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4239 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6948 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5351 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11569 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/sdk_proxy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dcaas/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dcaas/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dcaas/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dcaas/v2/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dcaas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dcaas/dcaas_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dis/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dis/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dis/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dis/v2/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dis/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dis/dis_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/volume_backup/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/volume_backup/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/volume_backup/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9204 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/volume_backup/v2/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5180 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/volume_backup/v2/backup_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1648 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/volume_backup/v2/backup_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/volume_backup/v2/job.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/volume_backup/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/volume_backup/volume_backup_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/ces/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/ces/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/ces/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/ces/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/ces/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/ces/ces_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/smn/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/smn/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/smn/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/smn/v2/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/smn/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/smn/smn_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/kms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/kms/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/kms/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4258 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/kms/v1/data_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1959 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/kms/v1/misc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/kms/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8687 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/kms/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6637 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/kms/v1/key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3953 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/kms/v1/_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/kms/kms_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/vpc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/vpc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/vpc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6891 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/vpc/v2/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1725 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/vpc/v2/route.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2371 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/vpc/v2/peering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/vpc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/vpc/vpc_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2568 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/queue.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15863 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1544 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/topic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2968 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/group_message.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1501 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/product.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1444 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/maintenance_window.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4335 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3713 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/message.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3065 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/az.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5511 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/v1/instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dms/dms_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dds/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dds/dds_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/dds/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dds/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/dds/v3/_proxy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/anti_ddos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/anti_ddos/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/anti_ddos/anti_ddos_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/anti_ddos/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/anti_ddos/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6314 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/anti_ddos/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/anti_ddos/v1/alert_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4649 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/anti_ddos/v1/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3141 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/anti_ddos/v1/floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/anti_ddos/v1/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/ecs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/ecs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/ecs/ecs_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/ecs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/ecs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/ecs/v1/_proxy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/deh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/deh/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/deh/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/deh/v1/host_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/deh/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5553 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/deh/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/deh/v1/server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5812 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/deh/v1/host.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/deh/deh_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/nat/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/nat/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2435 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/nat/v2/snat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/nat/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7740 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/nat/v2/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2355 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/nat/v2/gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2868 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/nat/v2/dnat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/nat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/nat/nat_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3865 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/job.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/waf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/waf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/waf/waf_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/sdk/waf/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/waf/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7899 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/waf/v1/_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/waf/v1/certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3476 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/waf/v1/domain.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7823 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/waf/v1/_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14713 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/ak_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25496 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/sdk/sdk_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1345 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7402 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/common/exc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3633 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/common/sdk_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4823 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/common/format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/common/errors.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/plas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/plas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/plas/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/plas/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/plas/v1/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/css/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/css/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/css/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/css/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/css/v1/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/test_openstacksdk_init.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dns/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dns/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dns/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dns/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dns/v1/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/lts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/lts/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/lts/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/lts/v2/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/lts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/cts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/cts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/cts/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/cts/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/cts/v1/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/mrs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/mrs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/mrs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/mrs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/mrs/v1/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/rds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/rds/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/rds/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/rds/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/rds/v1/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dws/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dws/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dws/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dws/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dws/v1/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/cce/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/cce/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/cce/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/cce/v1/test_cluster_nodes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/cce/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/cce/v1/test_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/cce/v1/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dcs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dcs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dcs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dcs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dcs/v1/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/obs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/obs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/obs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/obs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/obs/v1/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/sdrs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/sdrs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/sdrs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/sdrs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/sdrs/v1/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/auto_scaling/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/auto_scaling/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/auto_scaling/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/auto_scaling/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/auto_scaling/v1/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dcaas/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dcaas/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dcaas/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dcaas/v2/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dcaas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dis/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dis/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dis/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dis/v2/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dis/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/volume_backup/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/volume_backup/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/volume_backup/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/volume_backup/v2/test_job.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2702 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/volume_backup/v2/test_backup_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3905 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/volume_backup/v2/test_backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/volume_backup/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/ces/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/ces/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/ces/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/ces/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/ces/v1/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/smn/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/smn/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/smn/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/smn/v2/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/smn/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/kms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/kms/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/kms/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/kms/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1709 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/kms/v1/test_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2369 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/kms/v1/test_data_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/kms/v1/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1184 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/kms/v1/test_misc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/vpc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/vpc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/vpc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/vpc/v2/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/vpc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dms/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dms/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4378 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dms/v1/test_message.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6487 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dms/v1/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dms/v1/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1790 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dms/v1/test_queue.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dms/v1/test_misc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dds/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dds/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dds/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/dds/v3/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/anti_ddos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/anti_ddos/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/anti_ddos/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/anti_ddos/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/anti_ddos/v1/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/deh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/deh/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/deh/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/deh/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2000 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/deh/v1/test_host.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/deh/v1/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/nat/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/nat/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/nat/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1693 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/nat/v2/test_dnat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1530 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/nat/v2/test_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/nat/v2/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/nat/v2/test_snat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/nat/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/waf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/waf/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/waf/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/waf/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6434 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/waf/v1/test_domain.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/waf/v1/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5232 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/sdk/waf/v1/test_certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2650 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/dns/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/dns/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/dns/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4708 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/dns/v2/test_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/dns/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/rds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/rds/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/rds/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3659 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/rds/v3/test_configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/rds/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12928 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/rds/v3/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/rds/v3/test_datastore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2472 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/rds/v3/test_flavor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/obs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/obs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/obs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/obs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3244 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/obs/v1/test_obj.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1785 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/obs/v1/test_container.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/volume_backup/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/volume_backup/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/volume_backup/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2732 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/volume_backup/v2/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/volume_backup/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/vpc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/vpc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2539 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/vpc/v2/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/vpc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3966 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/vpc/v2/test_peering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/vpc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/nat/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/nat/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5608 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/nat/v2/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/nat/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2813 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/nat/v2/test_dnat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3608 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/nat/v2/test_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/nat/v2/test_snat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/osclient/nat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      439 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/functional/run_stestr.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/plas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/plas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/plas/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/plas/v1/test_proxy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/css/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/css/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/css/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1659 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/css/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/css/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4313 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/css/v1/test_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2514 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/css/v1/test_flavor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5574 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/v2/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3724 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/v2/test_recordset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4228 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/v2/test_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/v2/test_nameserver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1922 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/v2/test_floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/lts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/lts/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/lts/v2/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/lts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cts/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2812 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cts/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cts/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2292 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cts/v1/test_trace.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cts/v1/test_tracker.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/mrs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/mrs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/mrs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/mrs/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11339 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13402 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/test_configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11207 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2625 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/test_datastore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7097 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/test_backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3312 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/test_flavor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7341 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9141 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1566 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1557 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_datastore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4659 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3902 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_flavor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/compute/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/compute/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2535 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/compute/v2/test_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/compute/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/compute/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cloud/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29896 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cloud/test_rds.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cloud/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dws/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dws/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dws/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dws/v1/test_proxy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4647 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11129 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v1/test_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6874 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v1/test_cluster_node.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5463 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v3/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v3/test_job.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4561 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v3/test_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3182 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v3/test_cluster_cert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5144 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v3/test_cluster_node.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9237 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2289 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/test_restore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6254 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1991 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/test_statistic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3127 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/test_backup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/obs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/obs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/obs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5969 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/obs/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/obs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3496 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/obs/v1/test_obj.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2973 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/obs/v1/test_container.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/sdrs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/sdrs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/sdrs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/sdrs/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/sdrs/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9745 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7422 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8071 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3820 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_activity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4835 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2841 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4297 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1544 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcaas/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcaas/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcaas/v2/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcaas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dis/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dis/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dis/v2/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dis/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5276 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2590 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/test_job.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6029 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/test_backup_policy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/get_backup.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/unlink_resources.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/create_native_backup_response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_backup_policies.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_backups.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/link_resources.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/update_policy.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2944 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_backup_details.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_tasks.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3115 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/test_backup_policy_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/ces/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/ces/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/ces/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/ces/v1/test_proxy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/smn/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/smn/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/smn/v2/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/smn/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/smn/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/kms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/kms/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/kms/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5320 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/kms/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/kms/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10239 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/kms/v1/test_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/kms/v1/test_data_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4341 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/kms/v1/test_misc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/vpc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/vpc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3070 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/vpc/v2/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/vpc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3270 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/vpc/v2/test_peering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2077 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/vpc/v2/test_route.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/vpc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9267 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2493 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_message.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7596 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_product_spec.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_mw.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_topic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_az.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3379 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2030 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_queue.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2608 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_quota.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dds/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dds/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/dds/v3/test_proxy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/anti_ddos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/anti_ddos/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/anti_ddos/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3235 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/anti_ddos/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5529 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/anti_ddos/v1/test_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/anti_ddos/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2297 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/anti_ddos/v1/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2002 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/anti_ddos/v1/test_floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3428 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/test_sdk_resource.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/deh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/deh/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/deh/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2174 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/deh/v1/test_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2523 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/deh/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1440 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/deh/v1/test_host_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/deh/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7191 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/deh/v1/test_host.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/nat/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/nat/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3435 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/nat/v2/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/nat/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/nat/v2/test_dnat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2395 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/nat/v2/test_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2473 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/nat/v2/test_snat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/nat/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/waf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/waf/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/waf/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2811 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/waf/v1/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2913 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/waf/v1/test_domain.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2004 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/sdk/waf/v1/test_certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/common/test_format.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dns/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dns/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13642 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dns/v2/test_recordset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dns/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14949 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dns/v2/test_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3690 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dns/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5059 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dns/v2/test_ptr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dns/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cts/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cts/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5089 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cts/v1/test_trace.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2657 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cts/v1/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8957 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cts/v1/test_tracker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3729 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v1/test_configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12654 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v1/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4948 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v1/test_datastore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7551 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v1/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5038 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v1/test_backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3618 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v1/test_flavor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11953 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/test_configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18098 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2964 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/test_datastore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6541 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10533 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/test_backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/test_flavor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11285 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/test_health_monitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10771 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/test_load_balancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12576 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/test_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10793 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/test_listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10085 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/test_pool_member.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5096 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8769 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v2/test_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9154 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v2/test_cluster_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3436 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7898 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v1/test_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10383 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v1/test_cluster_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4254 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v1/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4465 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/test_restore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15463 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/test_statistic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6265 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5071 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5919 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/test_backup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/obs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/obs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/obs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/obs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4411 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/obs/v1/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7814 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12496 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2926 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/test_activity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6152 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7235 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12718 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/test_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2731 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/test_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2446 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/test_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/volume_backup/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/volume_backup/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/volume_backup/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15770 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/volume_backup/v2/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1744 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/volume_backup/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/volume_backup/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/kms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/kms/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/kms/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9160 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/kms/v1/test_cmk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/kms/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1900 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/kms/v1/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/vpc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/vpc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/vpc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13798 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/vpc/v2/test_peering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9034 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/vpc/v2/test_route.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2881 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/vpc/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/vpc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13643 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5847 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/test_topic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5271 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6289 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/test_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6448 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/test_queue.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1912 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/test_quota.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/anti_ddos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/anti_ddos/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/anti_ddos/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4881 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/anti_ddos/v1/test_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/anti_ddos/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4661 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/anti_ddos/v1/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/anti_ddos/v1/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7352 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/anti_ddos/v1/test_floating_ip.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/deh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/deh/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/deh/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/deh/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17684 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/deh/v1/test_host.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4223 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/deh/v1/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/nat/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/nat/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/nat/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10603 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/nat/v2/test_dnat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11068 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/nat/v2/test_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10017 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/nat/v2/test_snat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4055 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/nat/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/tests/unit/osclient/nat/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/dns/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/dns/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4258 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dns/v2/ptr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dns/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11509 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dns/v2/zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9530 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dns/v2/recordset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dns/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dns/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/cts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/cts/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/cts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/cts/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11572 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/cts/v1/tracker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/cts/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5577 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/cts/v1/trace.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/rds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1657 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2834 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v1/flavor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14673 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v1/configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4025 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v1/datastore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3914 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v1/backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28291 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v1/instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v3/flavor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10033 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v3/configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2091 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v3/datastore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7733 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v3/backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19513 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/rds/v3/instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/load_balancer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/load_balancer/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/load_balancer/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/load_balancer/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/load_balancer/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9458 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/load_balancer/v1/load_balancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13287 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/load_balancer/v1/health_monitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12079 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/load_balancer/v1/pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10245 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/load_balancer/v1/pool_member.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11747 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/load_balancer/v1/listener.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/compute/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/compute/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/compute/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6747 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/compute/v2/server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/compute/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/cce/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/cce/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/cce/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7120 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/cce/v2/cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9243 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/cce/v2/cluster_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/cce/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/cce/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/cce/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/cce/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5768 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/cce/v1/cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10305 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/cce/v1/cluster_node.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/dcs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dcs/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dcs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/dcs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4254 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dcs/v1/restore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dcs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1425 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dcs/v1/statistic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4710 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dcs/v1/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4958 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dcs/v1/backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20850 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dcs/v1/instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/obs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1969 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/obs/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/obs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/obs/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/obs/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/obs/v1/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8584 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/obs/v1/container.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10056 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/obs/v1/object.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/auto_scaling/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1329 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/auto_scaling/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/auto_scaling/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2634 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/activity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1680 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10991 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20528 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18479 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5489 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/volume_backup/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/volume_backup/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/volume_backup/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13593 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/volume_backup/v2/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1657 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/volume_backup/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/volume_backup/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/kms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/kms/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/kms/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/kms/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/kms/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8015 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/kms/v1/cmk.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/vpc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/vpc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/vpc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6775 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/vpc/v2/route.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10828 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/vpc/v2/peering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1567 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/vpc/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/vpc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/dms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dms/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dms/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/dms/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8557 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dms/v1/queue.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dms/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5818 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dms/v1/topic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dms/v1/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dms/v1/product.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dms/v1/maintenance_window.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3548 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dms/v1/group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dms/v1/az.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15274 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/dms/v1/instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/anti_ddos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1338 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/anti_ddos/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/anti_ddos/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/anti_ddos/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/anti_ddos/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3574 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/anti_ddos/v1/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5809 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/anti_ddos/v1/floating_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1628 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/anti_ddos/v1/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/deh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/deh/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/deh/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/deh/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/deh/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14381 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/deh/v1/host.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/nat/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions/osclient/nat/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8809 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/nat/v2/snat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/nat/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10331 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/nat/v2/gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9629 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/nat/v2/dnat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1567 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/nat/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:40:47.000000 otcextensions-0.9.0/otcextensions/osclient/nat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2020-09-02 15:40:47.000000 otcextensions-0.9.0/CONTRIBUTING.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/openstack/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/openstack/tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/openstack/tests/unit/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4701 2020-09-02 15:40:47.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/catalog-v3.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4702 2020-09-02 15:40:47.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/catalog-v3-suburl.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2020-09-02 15:40:47.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/image-version-v2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2020-09-02 15:40:47.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/image-version-v1.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2020-09-02 15:40:47.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/image-version-suburl.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/clouds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2020-09-02 15:40:47.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/clouds/clouds_cache.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      671 2020-09-02 15:40:47.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/clouds/clouds.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2020-09-02 15:40:47.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/image-version.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2020-09-02 15:40:47.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/dns.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2020-09-02 15:40:47.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/discovery.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2020-09-02 15:40:47.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/baremetal.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1059 2020-09-02 15:40:47.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/image-version-broken.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4582 2020-09-02 15:40:47.000000 otcextensions-0.9.0/openstack/tests/unit/fixtures/catalog-v2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6632 2020-09-02 15:41:36.000000 otcextensions-0.9.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20457 2020-09-02 15:41:36.000000 otcextensions-0.9.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-09-02 15:40:47.000000 otcextensions-0.9.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2020-09-02 15:40:47.000000 otcextensions-0.9.0/.stestr.blacklist.functional
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2020-09-02 15:40:47.000000 otcextensions-0.9.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2020-09-02 15:40:47.000000 otcextensions-0.9.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2020-09-02 15:41:36.000000 otcextensions-0.9.0/AUTHORS
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47027 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18774 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6632 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2020-09-02 15:41:36.000000 otcextensions-0.9.0/otcextensions.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3327 2020-09-02 15:40:47.000000 otcextensions-0.9.0/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2020-09-02 15:40:47.000000 otcextensions-0.9.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/rds/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/rds/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/rds/v3/test_datastore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2472 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/rds/v3/test_flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/rds/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12928 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/rds/v3/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3659 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/rds/v3/test_configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/rds/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/vpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/vpc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/vpc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/vpc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2539 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/vpc/v2/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3966 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/vpc/v2/test_peering.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/volume_backup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/volume_backup/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/volume_backup/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/volume_backup/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2732 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/volume_backup/v2/test_policy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/nat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/nat/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/nat/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3608 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/nat/v2/test_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/nat/v2/test_snat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/nat/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5608 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/nat/v2/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2813 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/nat/v2/test_dnat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/dns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/dns/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/dns/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4708 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/dns/v2/test_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/dns/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/obs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/obs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/obs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3244 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/obs/v1/test_obj.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1785 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/obs/v1/test_container.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/osclient/obs/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2650 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/rds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/rds/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/rds/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/rds/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/rds/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/cts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/cts/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/cts/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/cts/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/cts/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/vpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/vpc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/vpc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/vpc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/vpc/v2/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/cce/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/cce/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/cce/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/cce/v1/test_cluster_nodes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/cce/v1/test_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/cce/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/cce/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/anti_ddos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/anti_ddos/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/anti_ddos/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/anti_ddos/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/anti_ddos/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dms/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dms/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1790 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dms/v1/test_queue.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6487 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dms/v1/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4378 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dms/v1/test_message.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dms/v1/test_misc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dms/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/volume_backup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/volume_backup/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/volume_backup/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/volume_backup/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2702 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/volume_backup/v2/test_backup_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3905 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/volume_backup/v2/test_backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/volume_backup/v2/test_job.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/ces/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/ces/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/ces/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/ces/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/ces/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/deh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/deh/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/deh/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2000 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/deh/v1/test_host.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/deh/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/deh/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/sdrs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/sdrs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/sdrs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/sdrs/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/sdrs/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/nat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/nat/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/nat/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1530 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/nat/v2/test_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/nat/v2/test_snat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/nat/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1693 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/nat/v2/test_dnat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/nat/v2/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/css/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/css/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/css/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/css/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/css/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/plas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/plas/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/plas/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/plas/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/plas/v1/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/smn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/smn/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/smn/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/smn/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/smn/v2/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dcaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dcaas/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dcaas/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dcaas/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dcaas/v2/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dns/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dns/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dns/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dns/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dis/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dis/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dis/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dis/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dis/v2/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/test_openstacksdk_init.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/mrs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/mrs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/mrs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/mrs/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/mrs/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dws/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dws/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dws/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dws/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dws/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/auto_scaling/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/auto_scaling/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/auto_scaling/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/auto_scaling/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/auto_scaling/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/kms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/kms/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/kms/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2369 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/kms/v1/test_data_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/kms/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1709 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/kms/v1/test_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1184 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/kms/v1/test_misc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/kms/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dcs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dcs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dcs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dcs/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dcs/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/waf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/waf/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/waf/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5232 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/waf/v1/test_certificate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6434 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/waf/v1/test_domain.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/waf/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/waf/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dds/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dds/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dds/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dds/v3/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/dds/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/obs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/obs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/obs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/obs/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/obs/v1/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/lts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/lts/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/lts/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/lts/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/sdk/lts/v2/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      439 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/functional/run_stestr.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2964 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/test_datastore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/test_flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18098 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11953 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/test_configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10533 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/test_backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6541 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4948 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v1/test_datastore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3618 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v1/test_flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12654 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v1/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3729 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v1/test_configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5038 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v1/test_backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7551 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v1/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cts/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cts/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5089 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cts/v1/test_trace.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cts/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8957 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cts/v1/test_tracker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2657 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cts/v1/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/vpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/vpc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/vpc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9034 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/vpc/v2/test_route.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/vpc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13798 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/vpc/v2/test_peering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2881 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/vpc/v2/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7898 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v1/test_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10383 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v1/test_cluster_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4254 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v1/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8769 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v2/test_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9154 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v2/test_cluster_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3436 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v2/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/anti_ddos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/anti_ddos/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/anti_ddos/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4881 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/anti_ddos/v1/test_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7352 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/anti_ddos/v1/test_floating_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/anti_ddos/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/anti_ddos/v1/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4661 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/anti_ddos/v1/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5847 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/test_topic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6289 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/test_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6448 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/test_queue.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13643 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1912 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/test_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5271 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/volume_backup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/volume_backup/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/volume_backup/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/volume_backup/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15770 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/volume_backup/v2/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1744 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/volume_backup/v2/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2446 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/test_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/deh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/deh/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/deh/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17690 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/deh/v1/test_host.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/deh/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4223 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/deh/v1/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/nat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/nat/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/nat/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11068 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/nat/v2/test_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10017 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/nat/v2/test_snat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/nat/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10603 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/nat/v2/test_dnat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4055 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/nat/v2/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10771 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/test_load_balancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10085 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/test_pool_member.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11285 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/test_health_monitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10793 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/test_listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5096 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12576 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/test_pool.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dns/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dns/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14949 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dns/v2/test_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5059 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dns/v2/test_ptr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dns/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13642 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dns/v2/test_recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3690 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dns/v2/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12718 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/test_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7814 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2926 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/test_activity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2731 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/test_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12496 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7235 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6152 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/kms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/kms/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/kms/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9160 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/kms/v1/test_cmk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/kms/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1900 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/kms/v1/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/identity/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/identity/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/identity/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2644 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/identity/v3/test_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1957 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/identity/v3/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/identity/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4465 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/test_restore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15463 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/test_statistic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5071 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5919 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/test_backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6265 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/obs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/obs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/obs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/obs/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4411 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/osclient/obs/v1/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3946 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/common/test_agency_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/common/test_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1557 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_datastore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1566 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7341 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9141 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4659 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3902 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2625 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/test_datastore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11339 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3312 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/test_flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11207 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13402 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/test_configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7097 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/test_backup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/compute/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/compute/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/compute/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2535 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/compute/v2/test_server.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cts/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cts/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2812 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cts/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2292 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cts/v1/test_trace.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cts/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cts/v1/test_tracker.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/vpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/vpc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/vpc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2077 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/vpc/v2/test_route.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3070 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/vpc/v2/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/vpc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3270 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/vpc/v2/test_peering.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4561 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v3/test_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5463 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v3/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3182 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v3/test_cluster_cert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5144 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v3/test_cluster_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v3/test_job.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11129 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v1/test_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4647 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6874 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v1/test_cluster_node.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/anti_ddos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/anti_ddos/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/anti_ddos/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5529 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/anti_ddos/v1/test_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2002 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/anti_ddos/v1/test_floating_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3235 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/anti_ddos/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/anti_ddos/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2297 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/anti_ddos/v1/test_config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_topic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_mw.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9267 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_az.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3379 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2030 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_queue.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7596 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2608 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_product_spec.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2493 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_message.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5276 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/test_proxy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/unlink_resources.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/update_policy.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_backups.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/create_native_backup_response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_backup_policies.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/link_resources.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2944 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_backup_details.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/get_backup.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_tasks.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6029 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/test_backup_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3115 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/test_backup_policy_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2590 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/test_job.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/ces/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/ces/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/ces/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3098 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/ces/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/ces/v1/test_metric_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/ces/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1001 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/ces/v1/test_event_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3051 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/ces/v1/test_alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/ces/v1/test_metric.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/ces/v1/test_quota.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/deh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/deh/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/deh/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1440 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/deh/v1/test_host_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2523 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/deh/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7194 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/deh/v1/test_host.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/deh/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2174 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/deh/v1/test_server.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/sdrs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/sdrs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/sdrs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/sdrs/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/sdrs/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/nat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/nat/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/nat/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2335 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/nat/v2/test_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2412 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/nat/v2/test_snat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3435 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/nat/v2/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/nat/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2713 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/nat/v2/test_dnat.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/css/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/css/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/css/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4313 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/css/v1/test_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1659 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/css/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2514 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/css/v1/test_flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/css/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/plas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/plas/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/plas/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/plas/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/smn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/smn/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/smn/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/smn/v2/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/smn/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cloud/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cloud/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29896 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/cloud/test_rds.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcaas/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcaas/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcaas/v2/test_proxy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1922 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/v2/test_floating_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5574 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/v2/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4228 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/v2/test_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3724 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/v2/test_recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/v2/test_nameserver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1544 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dis/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dis/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dis/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dis/v2/test_proxy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/mrs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/mrs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/mrs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/mrs/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3428 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/test_sdk_resource.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dws/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dws/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dws/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dws/v1/test_proxy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9745 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2841 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7422 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3820 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_activity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4297 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8071 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4835 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/kms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/kms/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/kms/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5320 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/kms/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/kms/v1/test_data_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/kms/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10239 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/kms/v1/test_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4341 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/kms/v1/test_misc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/identity/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/identity/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2494 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/identity/v3/test_agency.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2071 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/identity/v3/test_agency_role.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12390 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/identity/v3/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/identity/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2180 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/identity/v3/test_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/identity/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2289 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/test_restore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9237 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6254 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1991 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/test_statistic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3127 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/test_backup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/waf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/waf/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/waf/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2004 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/waf/v1/test_certificate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2913 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/waf/v1/test_domain.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/waf/v1/test_proxy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dds/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dds/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dds/v3/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/dds/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/obs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/obs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/obs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3496 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/obs/v1/test_obj.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5969 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/obs/v1/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2973 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/obs/v1/test_container.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/obs/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/lts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/lts/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/lts/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/tests/unit/sdk/lts/v2/test_proxy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/rds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1657 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10033 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v3/configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7733 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v3/backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v3/flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2091 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v3/datastore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19513 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v3/instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14673 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v1/configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3914 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v1/backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2834 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v1/flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4025 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v1/datastore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28291 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/rds/v1/instance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/compute/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/compute/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/compute/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6747 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/compute/v2/server.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/cts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/cts/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/cts/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/cts/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11572 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/cts/v1/tracker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/cts/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5577 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/cts/v1/trace.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/vpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1567 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/vpc/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/vpc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/vpc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10828 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/vpc/v2/peering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/vpc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6775 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/vpc/v2/route.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/cce/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/cce/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/cce/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/cce/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10305 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/cce/v1/cluster_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5768 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/cce/v1/cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/cce/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/cce/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9243 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/cce/v2/cluster_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7120 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/cce/v2/cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/cce/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/anti_ddos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1338 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/anti_ddos/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/anti_ddos/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/anti_ddos/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1628 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/anti_ddos/v1/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/anti_ddos/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3574 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/anti_ddos/v1/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5809 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/anti_ddos/v1/floating_ip.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/dms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dms/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dms/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/dms/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5818 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dms/v1/topic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dms/v1/az.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8557 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dms/v1/queue.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dms/v1/maintenance_window.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dms/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dms/v1/product.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dms/v1/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3548 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dms/v1/group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15274 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dms/v1/instance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/volume_backup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1657 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/volume_backup/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/volume_backup/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/volume_backup/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13593 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/volume_backup/v2/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/volume_backup/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/ces/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/ces/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/ces/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/ces/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2764 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/ces/v1/metric.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2703 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/ces/v1/metric_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12534 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/ces/v1/alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/ces/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2701 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/ces/v1/event_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/ces/v1/quota.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/deh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/deh/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/deh/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/deh/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/deh/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14386 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/deh/v1/host.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/nat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1567 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/nat/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/nat/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/nat/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/nat/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9629 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/nat/v2/dnat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10331 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/nat/v2/gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8809 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/nat/v2/snat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/load_balancer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/load_balancer/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/load_balancer/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/load_balancer/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11747 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/load_balancer/v1/listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12079 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/load_balancer/v1/pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9458 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/load_balancer/v1/load_balancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/load_balancer/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10245 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/load_balancer/v1/pool_member.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13287 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/load_balancer/v1/health_monitor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/dns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dns/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dns/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/dns/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9530 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dns/v2/recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dns/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4258 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dns/v2/ptr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11509 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dns/v2/zone.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/auto_scaling/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1329 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/auto_scaling/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/auto_scaling/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10991 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18479 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1680 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20528 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2634 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/activity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5489 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/instance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/kms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/kms/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/kms/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/kms/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/kms/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8015 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/kms/v1/cmk.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1233 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/identity/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/identity/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/identity/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5970 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/identity/v3/credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/identity/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/dcs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dcs/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dcs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/dcs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1425 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dcs/v1/statistic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4958 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dcs/v1/backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4710 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dcs/v1/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dcs/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4254 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dcs/v1/restore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20850 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/dcs/v1/instance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/obs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1969 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/obs/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/obs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/osclient/obs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8584 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/obs/v1/container.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10056 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/obs/v1/object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/obs/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/osclient/obs/v1/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1383 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/_hacking.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7402 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/common/exc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/common/errors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7680 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/common/agency_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3633 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/common/sdk_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4823 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/common/format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1345 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11569 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/sdk_proxy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/rds/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16084 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v3/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5890 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v3/_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3683 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v3/configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5618 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v3/backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v3/flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v3/datastore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11919 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v3/instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/rds_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20634 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6952 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v1/configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3953 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v1/backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1369 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v1/flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1782 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v1/datastore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7549 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/rds/v1/instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25496 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/sdk_resource.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/compute/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/compute/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/compute/v2/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/compute/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2663 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/compute/v2/server.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/cts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cts/cts_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/cts/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3442 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cts/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4475 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cts/v1/tracker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cts/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cts/v1/trace.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3865 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/job.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/ecs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ecs/ecs_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ecs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/ecs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ecs/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ecs/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/vpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/vpc/vpc_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/vpc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/vpc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7652 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/vpc/v2/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2371 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/vpc/v2/peering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/vpc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1725 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/vpc/v2/route.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/cce/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3259 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v3/cluster_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2835 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v3/cluster_cert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v3/job.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9413 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v3/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8845 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v3/_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3216 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v3/cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8030 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/cce_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9547 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v1/cluster_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6244 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1372 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v1/_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6687 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v1/cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cce/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/anti_ddos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/anti_ddos/anti_ddos_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/anti_ddos/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/anti_ddos/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6708 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/anti_ddos/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/anti_ddos/v1/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/anti_ddos/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/anti_ddos/v1/alert_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4649 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/anti_ddos/v1/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3141 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/anti_ddos/v1/floating_ip.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/dms_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15863 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4335 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2968 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/group_message.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1544 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/topic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/az.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2568 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/queue.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1444 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/maintenance_window.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3713 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/message.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/product.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1501 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3065 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5511 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dms/v1/instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14713 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ak_auth.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/volume_backup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/volume_backup/volume_backup_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/volume_backup/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/volume_backup/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/volume_backup/v2/job.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9204 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/volume_backup/v2/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1648 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/volume_backup/v2/backup_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/volume_backup/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5180 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/volume_backup/v2/backup_policy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/ces/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ces/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ces/ces_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/ces/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1633 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ces/v1/metric.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5780 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ces/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1644 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ces/v1/metric_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8750 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ces/v1/alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ces/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ces/v1/event_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/ces/v1/quota.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/deh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/deh/deh_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/deh/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/deh/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5553 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/deh/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/deh/v1/host_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/deh/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/deh/v1/server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5814 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/deh/v1/host.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/sdrs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/sdrs/sdrs_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/sdrs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/sdrs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/sdrs/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/sdrs/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/nat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/nat/nat_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/nat/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/nat/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8686 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/nat/v2/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/nat/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2868 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/nat/v2/dnat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2355 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/nat/v2/gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2435 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/nat/v2/snat.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/css/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/css/css_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/css/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/css/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2793 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/css/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4488 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/css/v1/cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4557 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/css/v1/flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/css/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/plas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/plas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/plas/plas_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/plas/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/plas/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/plas/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10520 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/smn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/smn/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/smn/smn_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/smn/__init_.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/smn/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/smn/v2/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/smn/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/cloud/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10617 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cloud/rds.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/cloud/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dcaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dcaas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dcaas/dcaas_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dcaas/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dcaas/v2/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dcaas/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dns/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dns/dns_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dns/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2346 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dns/v2/recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12609 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dns/v2/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4439 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dns/v2/_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dns/v2/nameserver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dns/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4070 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dns/v2/zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1390 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dns/v2/floating_ip.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dis/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dis/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dis/dis_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dis/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dis/v2/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dis/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/mrs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/mrs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/mrs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/mrs/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/mrs/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/mrs/mrs_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dws/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dws/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dws/dws_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dws/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dws/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dws/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/auto_scaling/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/auto_scaling/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/auto_scaling/auto_scaling_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19096 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2834 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5061 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6948 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4056 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4239 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2324 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/activity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5351 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/instance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/kms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/kms/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/kms/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8687 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/kms/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3953 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/kms/v1/_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1959 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/kms/v1/misc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/kms/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4258 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/kms/v1/data_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6637 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/kms/v1/key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/kms/kms_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/identity/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/identity/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16771 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/identity/v3/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1732 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/identity/v3/agency.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/identity/v3/_bad_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1549 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/identity/v3/agency_role.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/identity/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1476 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/identity/v3/credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/identity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/identity/identity_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dcs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dcs/dcs_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dcs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dcs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1816 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dcs/v1/statistic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10461 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dcs/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2950 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dcs/v1/backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1987 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dcs/v1/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dcs/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dcs/v1/restore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8774 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dcs/v1/instance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/waf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/waf/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/waf/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9036 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/waf/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7823 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/waf/v1/_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/waf/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/waf/v1/certificate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3476 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/waf/v1/domain.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/waf/waf_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dds/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/dds/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dds/v3/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dds/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dds/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/dds/dds_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/obs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/obs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/obs/obs_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/obs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17367 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/obs/v1/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1694 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/obs/v1/_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5346 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/obs/v1/container.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/obs/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6116 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/obs/v1/obj.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/lts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/lts/lts_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/lts/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions/sdk/lts/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/lts/v2/_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/otcextensions/sdk/lts/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3328 2020-10-15 10:29:16.000000 otcextensions-0.9.1/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2020-10-15 10:29:16.000000 otcextensions-0.9.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2020-10-15 10:29:16.000000 otcextensions-0.9.1/.testr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2020-10-15 10:29:16.000000 otcextensions-0.9.1/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2020-10-15 10:29:16.000000 otcextensions-0.9.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2020-10-15 10:29:16.000000 otcextensions-0.9.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1117 2020-10-15 10:29:16.000000 otcextensions-0.9.1/.travis.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/rtfd_requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/appendices/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4901 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/appendices/glossary.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6762 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/appendices/issues.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/appendices/releasenotes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3595 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/appendices/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/appendices/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4509 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/install/pip_install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/install/source_install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6650 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/install/configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3645 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3945 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4990 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/enforcer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/contributor/layout.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/contributor/clouds.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4773 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/contributor/setup.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5236 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/contributor/coding.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/contributor/local.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/contributor/create/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7623 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/contributor/create/resource.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/contributor/create/examples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/contributor/create/examples/resource/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/contributor/create/examples/resource/fake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/contributor/create/examples/resource/fake_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4763 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/contributor/testing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2445 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4268 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/contributor/layout.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      601 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/volume_backup.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/ces.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      915 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/rds_v3.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/dms.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/dns.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/cce_v2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/cts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/kms.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/deh.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/vpc.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      581 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/anti_ddos.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/dcs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/auto_scaling.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/identity.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/nat.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/cli/load_balancer.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2991 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/getting_started.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/proxies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/volume_backup.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/cce_v1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/ces.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1557 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/rds_v3.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/dms.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/dns.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/cts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1184 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/rds_v1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/kms.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/deh.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/vpc.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3321 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/identity_v3.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/anti_ddos.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/cce_v3.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/dcs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1519 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/auto_scaling.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/waf.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/proxies/nat.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/rds/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/rds/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/rds/v3/instance.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/rds/v3/configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/rds/v3/flavor.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/rds/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/rds/v1/instance.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/rds/v1/configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/rds/v1/flavor.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/rds/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/cts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/cts/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/cts/v1/trace.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/cts/v1/tracker.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/cts/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/vpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/vpc/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/vpc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/vpc/v2/peering.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/vpc/v2/route.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/cce/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/cce/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/cce/v3/cluster.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/cce/v3/cluster_node.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/cce/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/cce/v1/cluster.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/cce/v1/cluster_node.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/cce/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/anti_ddos/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/anti_ddos/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/anti_ddos/v1/floating_ip.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/anti_ddos/v1/status.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/anti_ddos/v1/config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/anti_ddos/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/dms/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/dms/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dms/v1/misc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dms/v1/topic.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dms/v1/queue.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dms/v1/message.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dms/v1/group.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dms/v1/instance.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dms/v1/misc.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dms/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/ces/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/ces/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/ces/v1/metric_data.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/ces/v1/event_data.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/ces/v1/alarm.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/ces/v1/metric.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/ces/v1/quota.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/ces/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/deh/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/deh/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/deh/v1/server.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/deh/v1/host.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/deh/v1/host_type.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/deh/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/nat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/nat/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/nat/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/nat/v2/gateway.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/nat/v2/snat.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/nat/v2/dnat.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/dns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dns/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/dns/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dns/v2/floating_ip.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dns/v2/nameserver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dns/v2/zone.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dns/v2/recordset.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/auto_scaling/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/auto_scaling/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/auto_scaling/v1/group.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/auto_scaling/v1/policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/auto_scaling/v1/activity.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/auto_scaling/v1/config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/auto_scaling/v1/instance.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/auto_scaling/v1/quota.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/auto_scaling/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/kms/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/kms/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/kms/v1/data_key.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/kms/v1/key.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/kms/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/identity/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/identity/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/identity/v3/service.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/identity/v3/agency.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/identity/v3/user.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/identity/v3/endpoint.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/identity/v3/domain.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/identity/v3/group.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/identity/v3/agency_role.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/identity/v3/policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/identity/v3/credential.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/identity/v3/project.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/identity/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/dcs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/dcs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dcs/v1/statistic.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dcs/v1/restore.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dcs/v1/config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dcs/v1/instance.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dcs/v1/backup.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/dcs/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/waf/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/waf/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/waf/v1/certificate.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/waf/v1/domain.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/waf/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1650 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/obs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/resources/obs/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/obs/v1/obj.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/obs/v1/container.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/resources/obs/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/architecture.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/doc/source/sdk/guides/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3353 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/ces.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3605 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/cce.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4100 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/logging.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6155 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/dns.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2336 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/cts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4855 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/kms.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1987 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/deh.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3486 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/vpc.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3022 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/anti_ddos.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5230 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/dcs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8050 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/auto_scaling.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6864 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/rds.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1501 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4302 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/guides/nat.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/sdk/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3167 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1854 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/source/coverage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2020-10-15 10:29:16.000000 otcextensions-0.9.1/doc/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5125 2020-10-15 10:29:16.000000 otcextensions-0.9.1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21145 2020-10-15 10:30:05.000000 otcextensions-0.9.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2020-10-15 10:29:16.000000 otcextensions-0.9.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11277 2020-10-15 10:30:04.000000 otcextensions-0.9.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2020-10-15 10:29:16.000000 otcextensions-0.9.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-10-15 10:29:16.000000 otcextensions-0.9.1/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/spec/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3616 2020-10-15 10:29:16.000000 otcextensions-0.9.1/spec/python-otcextensions.spec
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2020-10-15 10:30:04.000000 otcextensions-0.9.1/AUTHORS
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50624 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19452 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7305 2020-10-15 10:30:05.000000 otcextensions-0.9.1/otcextensions.egg-info/PKG-INFO
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/openstack/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/openstack/tests/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/openstack/tests/unit/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2020-10-15 10:29:16.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/image-version-suburl.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1059 2020-10-15 10:29:16.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/image-version-broken.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2020-10-15 10:29:16.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/image-version-v1.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2020-10-15 10:29:16.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/discovery.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2020-10-15 10:29:16.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/dns.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4582 2020-10-15 10:29:16.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/catalog-v2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4701 2020-10-15 10:29:16.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/catalog-v3.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2020-10-15 10:29:16.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/image-version.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2020-10-15 10:29:16.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/image-version-v2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2020-10-15 10:29:16.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/baremetal.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/clouds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      671 2020-10-15 10:29:16.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/clouds/clouds.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2020-10-15 10:29:16.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/clouds/clouds_cache.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4702 2020-10-15 10:29:16.000000 otcextensions-0.9.1/openstack/tests/unit/fixtures/catalog-v3-suburl.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/rds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/list_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/delete_configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/get_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/apply_configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/list_datastores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/find_configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/list_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/list_configurations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/list_datastore_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/create_backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1150 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/update_configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/list_backup_download_links.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/find_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/get_configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1055 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/create_configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1547 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/create_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/set_instance_backup_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/find_backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/get_instance_restore_time.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/get_instance_backup_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/restore_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      985 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/wait_for_backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/rds/list_flavors.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/compute/find.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/compute/list.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2098 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/compute/create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/compute/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/compute/delete.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/cts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cts/get_tracker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cts/list_traces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cts/delete_tracker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1246 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cts/update_tracker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cts/create_tracker.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/vpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/vpc/delete_peering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/vpc/create_peering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/vpc/set_peering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/vpc/get_route.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/vpc/get_peering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/vpc/find_peering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/vpc/add_route.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/vpc/delete_route.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/vpc/update_peering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      738 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/vpc/list_peerings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/vpc/list_routes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/cce/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cce/find_cluster_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1556 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cce/create_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cce/get_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cce/delete_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cce/list_cluster_nodes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1566 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cce/create_cluster_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cce/wait_for_job.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cce/get_job.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cce/delete_cluster_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cce/get_cluster_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cce/find_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cce/list_clusters.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/anti_ddos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/anti_ddos/list_floating_ip_events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/anti_ddos/protect_floating_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/anti_ddos/list_floating_ip_stat_day.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/anti_ddos/get_floating_ip_policies.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/anti_ddos/unprotect_floating_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/anti_ddos/update_floating_ip_policies.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/anti_ddos/get_floating_ip_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/anti_ddos/list_floating_ips.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/anti_ddos/list_floating_ip_stat_week.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/anti_ddos/list_configs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/network/find.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/network/list.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/network/create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/network/security_group_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/network/delete.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/key_manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/key_manager/list.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/key_manager/create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/key_manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/key_manager/get.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/ces/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/ces/list_event_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1700 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/ces/create_metric_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/ces/list_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/ces/list_metric_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/ces/delete_alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/ces/list_metrics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2892 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/ces/create_alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/ces/get_alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/ces/find_alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/ces/list_alarms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/ces/switch_alarm_state.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/deh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/deh/list_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/deh/list.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/deh/list_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/deh/create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/deh/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/deh/list_deh_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/deh/list_deh_hosts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/nat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/get_snat_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      827 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/get_dnat_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/update_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/list_gateways.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/list_snat_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1213 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/create_dnat_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/list_dnat_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/get_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/create_snat_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/create_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/delete_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/find_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/delete_dnat_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/nat/delete_snat_rule.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/baremetal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/baremetal/list.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/baremetal/provisioning.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/connect_otc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/cloud/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/normalization.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/server-information.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/debug-logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1469 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/create-server-dict.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/cleanup-servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/strict-mode.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/munch-dict-object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/create-server-name-or-id.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/service-conditionals.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/upload-large-object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/service-conditional-overrides.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/upload-object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/http-debug-logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/user-agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/cloud/find-an-image.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/dns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/remove_router_from_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/get_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/find_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/update_recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/get_recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1298 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/create_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/update_floating_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/list_recordsets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/find_recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/delete_recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/unset_floating_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/list_nameservers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/add_router_to_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/delete_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/get_floating_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/list_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/list_floating_ips.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/update_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/create_recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      864 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dns/set_floating_ip.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/clustering/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/clustering/profile_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4231 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/clustering/cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/clustering/policy_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/clustering/profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2111 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/clustering/receiver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1875 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/clustering/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/clustering/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1094 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/clustering/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1109 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/clustering/action.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2221 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/clustering/node.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/auto_scaling/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/list_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      874 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/resume_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/execute_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/pause_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/list_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/remove_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/list_activities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/list_policies.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/batch_delete_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/init.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/find_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/list_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/pause_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/batch_instance_action.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/delete_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/find_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/delete_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/create_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/create_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1233 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/update_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/delete_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/get_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/create_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/find_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/get_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/list_configs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/get_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/auto_scaling/resume_group.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/kms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/generate_random_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/list_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/disable_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/schedule_key_deletion.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/find_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/encrypt_datakey.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/create_datakey_without_plaintext.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/enable_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/decrypt_datakey.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/create_datakey.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/get_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/create_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/cancel_key_deletion.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      726 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/list_keys.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/kms/get_instance_number.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/identity/update_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2522 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/identity/list.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/identity/get_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/identity/create_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/identity/list_credentials.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/identity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/identity/delete_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/identity/find_credential.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/dcs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/list_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/list_restore_records.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/get_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/extend_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/list_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/create_backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/restart_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/list_statistics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/start_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      827 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/find_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/stop_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/delete_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/create_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/update_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      839 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/list_instance_params.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/change_instance_password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/delete_backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/restore_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      822 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/dcs/update_instance_params.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2830 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/connect.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:30:05.000000 otcextensions-0.9.1/examples/image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/image/list.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2261 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/image/download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1162 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/image/create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/image/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      927 2020-10-15 10:29:16.000000 otcextensions-0.9.1/examples/image/delete.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2020-10-15 10:29:16.000000 otcextensions-0.9.1/.stestr.blacklist.functional
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2020-10-15 10:29:16.000000 otcextensions-0.9.1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2020-10-15 10:29:16.000000 otcextensions-0.9.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7305 2020-10-15 10:30:05.000000 otcextensions-0.9.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2020-10-15 10:29:16.000000 otcextensions-0.9.1/bindep.txt
```

### Comparing `otcextensions-0.9.0/examples/clustering/cluster.py` & `otcextensions-0.9.1/examples/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/clustering/policy_type.py` & `otcextensions-0.9.1/examples/clustering/policy_type.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/clustering/node.py` & `otcextensions-0.9.1/examples/clustering/node.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/clustering/action.py` & `otcextensions-0.9.1/examples/clustering/action.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/clustering/profile.py` & `otcextensions-0.9.1/examples/clustering/profile.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/clustering/profile_type.py` & `otcextensions-0.9.1/examples/clustering/profile_type.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/clustering/receiver.py` & `otcextensions-0.9.1/examples/clustering/receiver.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/clustering/policy.py` & `otcextensions-0.9.1/examples/clustering/policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/clustering/event.py` & `otcextensions-0.9.1/examples/clustering/event.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/list_nameservers.py` & `otcextensions-0.9.1/examples/dns/list_nameservers.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/find_recordset.py` & `otcextensions-0.9.1/examples/dns/find_recordset.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/create_recordset.py` & `otcextensions-0.9.1/examples/dns/create_recordset.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/get_zone.py` & `otcextensions-0.9.1/examples/dns/get_zone.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/get_recordset.py` & `otcextensions-0.9.1/examples/dns/get_recordset.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/unset_floating_ip.py` & `otcextensions-0.9.1/examples/dns/unset_floating_ip.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/get_floating_ip.py` & `otcextensions-0.9.1/examples/dns/get_floating_ip.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/find_zone.py` & `otcextensions-0.9.1/examples/dns/find_zone.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/update_zone.py` & `otcextensions-0.9.1/examples/dns/update_zone.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/update_floating_ip.py` & `otcextensions-0.9.1/examples/dns/update_floating_ip.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/delete_recordset.py` & `otcextensions-0.9.1/examples/dns/delete_recordset.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/delete_zone.py` & `otcextensions-0.9.1/examples/dns/delete_zone.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/list_zones.py` & `otcextensions-0.9.1/examples/dns/list_zones.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/remove_router_from_zone.py` & `otcextensions-0.9.1/examples/dns/remove_router_from_zone.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/update_recordset.py` & `otcextensions-0.9.1/examples/dns/update_recordset.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/list_recordsets.py` & `otcextensions-0.9.1/examples/dns/list_recordsets.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/list_floating_ips.py` & `otcextensions-0.9.1/examples/dns/list_floating_ips.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/set_floating_ip.py` & `otcextensions-0.9.1/examples/dns/set_floating_ip.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/add_router_to_zone.py` & `otcextensions-0.9.1/examples/dns/add_router_to_zone.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dns/create_zone.py` & `otcextensions-0.9.1/examples/dns/create_zone.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cts/list_traces.py` & `otcextensions-0.9.1/examples/cts/list_traces.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cts/create_tracker.py` & `otcextensions-0.9.1/examples/cts/create_tracker.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cts/get_tracker.py` & `otcextensions-0.9.1/examples/cts/get_tracker.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cts/delete_tracker.py` & `otcextensions-0.9.1/examples/cts/delete_tracker.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cts/update_tracker.py` & `otcextensions-0.9.1/examples/cts/update_tracker.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/get_instance_backup_policy.py` & `otcextensions-0.9.1/examples/rds/get_instance_backup_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/create_backup.py` & `otcextensions-0.9.1/examples/rds/create_backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/create_configuration.py` & `otcextensions-0.9.1/examples/rds/create_configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/find_instance.py` & `otcextensions-0.9.1/examples/rds/find_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/apply_configuration.py` & `otcextensions-0.9.1/examples/rds/apply_configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/list_datastores.py` & `otcextensions-0.9.1/examples/rds/list_datastores.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/wait_for_backup.py` & `otcextensions-0.9.1/examples/rds/wait_for_backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/create_instance.py` & `otcextensions-0.9.1/examples/rds/create_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/delete_configuration.py` & `otcextensions-0.9.1/examples/rds/delete_configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/get_configuration.py` & `otcextensions-0.9.1/examples/rds/get_configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/get_instance.py` & `otcextensions-0.9.1/examples/rds/get_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/get_instance_restore_time.py` & `otcextensions-0.9.1/examples/rds/get_instance_restore_time.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/list_instances.py` & `otcextensions-0.9.1/examples/rds/list_instances.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/find_backup.py` & `otcextensions-0.9.1/examples/rds/find_backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/list_backup_download_links.py` & `otcextensions-0.9.1/examples/rds/list_backup_download_links.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/update_configuration.py` & `otcextensions-0.9.1/examples/rds/update_configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/restore_instance.py` & `otcextensions-0.9.1/examples/rds/restore_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/list_configurations.py` & `otcextensions-0.9.1/examples/rds/list_configurations.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/list_flavors.py` & `otcextensions-0.9.1/examples/rds/list_flavors.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/list_datastore_types.py` & `otcextensions-0.9.1/examples/rds/list_datastore_types.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/find_configuration.py` & `otcextensions-0.9.1/examples/rds/find_configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/set_instance_backup_policy.py` & `otcextensions-0.9.1/examples/rds/set_instance_backup_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/rds/list_backups.py` & `otcextensions-0.9.1/examples/rds/list_backups.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/compute/create.py` & `otcextensions-0.9.1/examples/compute/create.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/compute/delete.py` & `otcextensions-0.9.1/examples/compute/delete.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/compute/find.py` & `otcextensions-0.9.1/examples/compute/find.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/compute/list.py` & `otcextensions-0.9.1/examples/compute/list.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/debug-logging.py` & `otcextensions-0.9.1/examples/cloud/debug-logging.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/munch-dict-object.py` & `otcextensions-0.9.1/examples/cloud/munch-dict-object.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/upload-object.py` & `otcextensions-0.9.1/examples/cloud/upload-large-object.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/service-conditional-overrides.py` & `otcextensions-0.9.1/examples/cloud/service-conditional-overrides.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/service-conditionals.py` & `otcextensions-0.9.1/examples/cloud/service-conditionals.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/create-server-name-or-id.py` & `otcextensions-0.9.1/examples/cloud/create-server-name-or-id.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/strict-mode.py` & `otcextensions-0.9.1/examples/cloud/strict-mode.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/upload-large-object.py` & `otcextensions-0.9.1/examples/cloud/upload-object.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/http-debug-logging.py` & `otcextensions-0.9.1/examples/cloud/http-debug-logging.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/normalization.py` & `otcextensions-0.9.1/examples/cloud/normalization.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/user-agent.py` & `otcextensions-0.9.1/examples/cloud/user-agent.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/cleanup-servers.py` & `otcextensions-0.9.1/examples/cloud/cleanup-servers.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/server-information.py` & `otcextensions-0.9.1/examples/cloud/server-information.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/find-an-image.py` & `otcextensions-0.9.1/examples/cloud/find-an-image.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cloud/create-server-dict.py` & `otcextensions-0.9.1/examples/cloud/create-server-dict.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/connect_otc.py` & `otcextensions-0.9.1/examples/connect_otc.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cce/list_clusters.py` & `otcextensions-0.9.1/examples/cce/list_clusters.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cce/list_cluster_nodes.py` & `otcextensions-0.9.1/examples/cce/list_cluster_nodes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cce/get_job.py` & `otcextensions-0.9.1/examples/cce/get_job.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cce/delete_cluster_node.py` & `otcextensions-0.9.1/examples/cce/delete_cluster_node.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cce/get_cluster.py` & `otcextensions-0.9.1/examples/cce/get_cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cce/find_cluster.py` & `otcextensions-0.9.1/examples/cce/find_cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cce/find_cluster_node.py` & `otcextensions-0.9.1/examples/cce/find_cluster_node.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cce/delete_cluster.py` & `otcextensions-0.9.1/examples/cce/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cce/create_cluster_node.py` & `otcextensions-0.9.1/examples/cce/create_cluster_node.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cce/create_cluster.py` & `otcextensions-0.9.1/examples/cce/create_cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cce/get_cluster_node.py` & `otcextensions-0.9.1/examples/cce/get_cluster_node.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/cce/wait_for_job.py` & `otcextensions-0.9.1/examples/cce/wait_for_job.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/create_backup.py` & `otcextensions-0.9.1/examples/dcs/create_backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/find_instance.py` & `otcextensions-0.9.1/examples/dcs/find_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/delete_instance.py` & `otcextensions-0.9.1/examples/dcs/delete_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/list_statistics.py` & `otcextensions-0.9.1/examples/dcs/list_statistics.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/create_instance.py` & `otcextensions-0.9.1/examples/dcs/create_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/stop_instance.py` & `otcextensions-0.9.1/examples/dcs/stop_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/delete_backup.py` & `otcextensions-0.9.1/examples/dcs/delete_backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/get_instance.py` & `otcextensions-0.9.1/examples/dcs/get_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/list_instance_params.py` & `otcextensions-0.9.1/examples/dcs/list_instance_params.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/update_instance_params.py` & `otcextensions-0.9.1/examples/dcs/update_instance_params.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/list_instances.py` & `otcextensions-0.9.1/examples/dcs/list_instances.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/start_instance.py` & `otcextensions-0.9.1/examples/dcs/start_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/update_instance.py` & `otcextensions-0.9.1/examples/dcs/update_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/extend_instance.py` & `otcextensions-0.9.1/examples/dcs/extend_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/restore_instance.py` & `otcextensions-0.9.1/examples/dcs/restore_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/list_restore_records.py` & `otcextensions-0.9.1/examples/dcs/list_restore_records.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/change_instance_password.py` & `otcextensions-0.9.1/examples/dcs/change_instance_password.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/list_backups.py` & `otcextensions-0.9.1/examples/dcs/list_backups.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/dcs/restart_instance.py` & `otcextensions-0.9.1/examples/dcs/restart_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/execute_policy.py` & `otcextensions-0.9.1/examples/auto_scaling/execute_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/create_config.py` & `otcextensions-0.9.1/examples/auto_scaling/create_config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/get_policy.py` & `otcextensions-0.9.1/examples/auto_scaling/get_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/batch_instance_action.py` & `otcextensions-0.9.1/examples/auto_scaling/batch_instance_action.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/find_config.py` & `otcextensions-0.9.1/examples/auto_scaling/find_config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/get_group.py` & `otcextensions-0.9.1/examples/auto_scaling/get_group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/get_config.py` & `otcextensions-0.9.1/examples/auto_scaling/get_config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/pause_group.py` & `otcextensions-0.9.1/examples/auto_scaling/pause_group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/list_groups.py` & `otcextensions-0.9.1/examples/auto_scaling/list_groups.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/list_policies.py` & `otcextensions-0.9.1/examples/auto_scaling/list_policies.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/remove_instance.py` & `otcextensions-0.9.1/examples/auto_scaling/remove_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/list_activities.py` & `otcextensions-0.9.1/examples/auto_scaling/list_activities.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/delete_config.py` & `otcextensions-0.9.1/examples/auto_scaling/delete_config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/list_instances.py` & `otcextensions-0.9.1/examples/auto_scaling/list_instances.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/resume_policy.py` & `otcextensions-0.9.1/examples/auto_scaling/resume_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/resume_group.py` & `otcextensions-0.9.1/examples/auto_scaling/resume_group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/list_configs.py` & `otcextensions-0.9.1/examples/auto_scaling/list_configs.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/delete_policy.py` & `otcextensions-0.9.1/examples/auto_scaling/delete_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/find_group.py` & `otcextensions-0.9.1/examples/auto_scaling/find_group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/create_policy.py` & `otcextensions-0.9.1/examples/auto_scaling/create_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/batch_delete_config.py` & `otcextensions-0.9.1/examples/auto_scaling/batch_delete_config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/list_quotas.py` & `otcextensions-0.9.1/examples/auto_scaling/list_quotas.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/update_policy.py` & `otcextensions-0.9.1/examples/auto_scaling/update_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/pause_policy.py` & `otcextensions-0.9.1/examples/auto_scaling/pause_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/find_policy.py` & `otcextensions-0.9.1/examples/auto_scaling/find_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/create_group.py` & `otcextensions-0.9.1/examples/auto_scaling/create_group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/auto_scaling/delete_group.py` & `otcextensions-0.9.1/examples/auto_scaling/delete_group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/identity/list.py` & `otcextensions-0.9.1/examples/identity/list.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/key_manager/create.py` & `otcextensions-0.9.1/examples/key_manager/create.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/key_manager/get.py` & `otcextensions-0.9.1/examples/key_manager/get.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/key_manager/list.py` & `otcextensions-0.9.1/examples/key_manager/list.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/list_keys.py` & `otcextensions-0.9.1/examples/kms/list_keys.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/create_key.py` & `otcextensions-0.9.1/examples/kms/create_key.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/create_datakey.py` & `otcextensions-0.9.1/examples/kms/create_datakey.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/encrypt_datakey.py` & `otcextensions-0.9.1/examples/kms/encrypt_datakey.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/enable_key.py` & `otcextensions-0.9.1/examples/kms/enable_key.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/get_key.py` & `otcextensions-0.9.1/examples/kms/get_key.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/create_datakey_without_plaintext.py` & `otcextensions-0.9.1/examples/kms/create_datakey_without_plaintext.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/generate_random_data.py` & `otcextensions-0.9.1/examples/kms/generate_random_data.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/schedule_key_deletion.py` & `otcextensions-0.9.1/examples/kms/schedule_key_deletion.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/cancel_key_deletion.py` & `otcextensions-0.9.1/examples/kms/cancel_key_deletion.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/disable_key.py` & `otcextensions-0.9.1/examples/kms/disable_key.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/list_quotas.py` & `otcextensions-0.9.1/examples/kms/list_quotas.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/find_key.py` & `otcextensions-0.9.1/examples/kms/find_key.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/get_instance_number.py` & `otcextensions-0.9.1/examples/kms/get_instance_number.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/kms/decrypt_datakey.py` & `otcextensions-0.9.1/examples/kms/decrypt_datakey.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/vpc/create_peering.py` & `otcextensions-0.9.1/examples/vpc/create_peering.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/vpc/find_peering.py` & `otcextensions-0.9.1/examples/vpc/find_peering.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/vpc/get_peering.py` & `otcextensions-0.9.1/examples/vpc/get_peering.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/vpc/get_route.py` & `otcextensions-0.9.1/examples/vpc/get_route.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/vpc/list_peerings.py` & `otcextensions-0.9.1/examples/vpc/list_peerings.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/vpc/add_route.py` & `otcextensions-0.9.1/examples/vpc/add_route.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/vpc/set_peering.py` & `otcextensions-0.9.1/examples/vpc/set_peering.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/vpc/list_routes.py` & `otcextensions-0.9.1/examples/vpc/list_routes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/vpc/update_peering.py` & `otcextensions-0.9.1/examples/vpc/update_peering.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/vpc/delete_route.py` & `otcextensions-0.9.1/examples/vpc/delete_route.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/vpc/delete_peering.py` & `otcextensions-0.9.1/examples/vpc/delete_peering.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/network/create.py` & `otcextensions-0.9.1/examples/network/create.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/network/delete.py` & `otcextensions-0.9.1/examples/network/delete.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/network/find.py` & `otcextensions-0.9.1/examples/network/find.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/network/list.py` & `otcextensions-0.9.1/examples/network/list.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/network/security_group_rules.py` & `otcextensions-0.9.1/examples/network/security_group_rules.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/baremetal/provisioning.py` & `otcextensions-0.9.1/examples/baremetal/provisioning.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/baremetal/list.py` & `otcextensions-0.9.1/examples/baremetal/list.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/anti_ddos/update_floating_ip_policies.py` & `otcextensions-0.9.1/examples/anti_ddos/update_floating_ip_policies.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/anti_ddos/list_floating_ip_stat_day.py` & `otcextensions-0.9.1/examples/anti_ddos/list_floating_ip_stat_day.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/anti_ddos/list_floating_ip_events.py` & `otcextensions-0.9.1/examples/anti_ddos/list_floating_ip_events.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/anti_ddos/list_configs.py` & `otcextensions-0.9.1/examples/anti_ddos/list_configs.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/anti_ddos/get_floating_ip_status.py` & `otcextensions-0.9.1/examples/anti_ddos/get_floating_ip_status.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/anti_ddos/protect_floating_ip.py` & `otcextensions-0.9.1/examples/anti_ddos/protect_floating_ip.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/anti_ddos/get_floating_ip_policies.py` & `otcextensions-0.9.1/examples/anti_ddos/get_floating_ip_policies.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/anti_ddos/unprotect_floating_ip.py` & `otcextensions-0.9.1/examples/anti_ddos/unprotect_floating_ip.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/anti_ddos/list_floating_ips.py` & `otcextensions-0.9.1/examples/anti_ddos/list_floating_ips.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/anti_ddos/list_floating_ip_stat_week.py` & `otcextensions-0.9.1/examples/anti_ddos/list_floating_ip_stat_week.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/image/create.py` & `otcextensions-0.9.1/examples/image/create.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/image/delete.py` & `otcextensions-0.9.1/examples/image/delete.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/image/download.py` & `otcextensions-0.9.1/examples/image/download.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/image/list.py` & `otcextensions-0.9.1/examples/image/list.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/deh/create.py` & `otcextensions-0.9.1/examples/deh/create.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/deh/list.py` & `otcextensions-0.9.1/examples/deh/list.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/deh/list_types.py` & `otcextensions-0.9.1/examples/deh/list_types.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/deh/list_servers.py` & `otcextensions-0.9.1/examples/deh/list_servers.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/get_dnat_rule.py` & `otcextensions-0.9.1/examples/nat/get_dnat_rule.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/create_snat_rule.py` & `otcextensions-0.9.1/examples/nat/create_snat_rule.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/create_gateway.py` & `otcextensions-0.9.1/examples/nat/create_gateway.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/update_gateway.py` & `otcextensions-0.9.1/examples/nat/update_gateway.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/delete_snat_rule.py` & `otcextensions-0.9.1/examples/nat/delete_snat_rule.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/get_snat_rule.py` & `otcextensions-0.9.1/examples/nat/get_snat_rule.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/find_gateway.py` & `otcextensions-0.9.1/examples/nat/find_gateway.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/delete_dnat_rule.py` & `otcextensions-0.9.1/examples/nat/delete_dnat_rule.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/create_dnat_rule.py` & `otcextensions-0.9.1/examples/nat/create_dnat_rule.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/list_gateways.py` & `otcextensions-0.9.1/examples/nat/list_gateways.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/delete_gateway.py` & `otcextensions-0.9.1/examples/nat/delete_gateway.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/list_dnat_rules.py` & `otcextensions-0.9.1/examples/nat/list_dnat_rules.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/list_snat_rules.py` & `otcextensions-0.9.1/examples/nat/list_snat_rules.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/nat/get_gateway.py` & `otcextensions-0.9.1/examples/nat/get_gateway.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/examples/connect.py` & `otcextensions-0.9.1/examples/connect.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/ChangeLog` & `otcextensions-0.9.1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 CHANGES
 =======
 
+0.9.1
+-----
+
+* change parameter state to status to fit Ansible playbooks (#113)
+* rollback credential OSC due to conflicts (#112)
+* Documentation added for CES (SDK + OSC), Identity Credential (OSC) and rework of README.rst (#111)
+* Agency support (#108)
+* add some project cleanup functions (#109)
+* Cloudeye (#101)
+* add SDK support for Identity Credentials (#106)
+
 0.9.0
 -----
 
 * drop maas service, since doesnt exist anymore (#105)
 * add support for waf domains (#104)
 
 0.8.0
```

### Comparing `otcextensions-0.9.0/README.rst` & `otcextensions-0.9.1/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -17,35 +17,39 @@
 * `python-openstackclient`
 
 packages.
 
 Documentation
 -------------
 
-* `Documentation <http://python-otcextensions.readthedocs.io/en/latest/>`
+`Documentation Overview <http://python-otcextensions.readthedocs.io/en/latest/>`_
 
 Installation
 ------------
 
+`Installation Page <https://python-otcextensions.readthedocs.io/en/latest/install/index.html>`_
+
 The OTC Extensions are hosted as the package `otcextensions` on PyPI
 and can be installed by pip as
 
 .. code-block: console
+
    $ pip install otcextensions
 
 There are several options
 to do that including but not limited to pip userland installation, system wide
 installation as well as installation from operating system packets or directly
 from source. Refer to the installation instructions_ in the projects
 documentation.
 
-
 Configuration
 -------------
 
+`Configuration Page <https://python-otcextensions.readthedocs.io/en/latest/install/configuration.html>`_
+
 Acessing the Open Telekom Cloud APIs requires authentication and
 authorization. For both there are several options available:
 
 * **Configuration files** (recommended): A file called `clouds.yaml`
   holds all necessary configuration parameters. The file can be placed
   either in the local directory, below the user home directory in
   `.config/openstack` or in the system-wide directory
@@ -54,46 +58,47 @@
   credentials. For more details see the section `configuration`_ in
   the official documentation.
 
   Minimal sample ``clouds.yaml`` file:
 
   .. code-block:: yaml
 
-      clouds:
-          otc:
-          profile: otc
-              auth:
-                  username: "*username*"
-                  password: "*password*"
-                  project_name: "eu-de"
-                  auth_url: "https://iam.eu-de.otc.t-systems.com:443/v3"
-                  user_domain_name: "*OTC00000000001000000xxx*"
-             interface: "public"
-             identity_api_version: 3
-             ak: "*40 digit access key*"
-             sk: "*20 digit secure key*"
+    clouds:
+      otc:
+        profile: otc
+        auth:
+          username: '<USER_NAME>'
+          password: '<PASSWORD>'
+          project_name: '<eu-de_project>'
+          # or project_id: '<123456_PROJECT_ID>'
+          user_domain_name: 'OTC00000000001000000xxx'
+          # or user_domain_id: '<123456_DOMAIN_ID>'
+          auth_url: 'https://iam.eu-de.otc.t-systems.com:443/v3'
+        interface: 'public'
+        identity_api_version: 3 # !Important
+        ak: '<AK_VALUE>' # AK/SK pair for access to OBS
+        sk: '<SK_VALUE>'
 
   With this configuration you can start using the CLI with ``openstack
   --os-cloud otc *command*`` or by ``export OS_CLOUD=otc; openstack
   *command*``.
 
 * **Environment variables:** Authentication using username/password is often
-  used:
+  used::
 
     export OS_AUTH_URL=<url-to-openstack-identity>
     export OS_IDENTITY_API_VERSION=3
     export OS_PROJECT_NAME=<project-name>
     export OS_PROJECT_DOMAIN_NAME=<project-domain-name>
     export OS_USERNAME=<username>
     export OS_USER_DOMAIN_NAME=<user-domain-name>
     export OS_PASSWORD=<password>  # (optional)
     export S3_ACCESS_KEY_ID=<access_key>
     export S3_SECRET_ACCESS_KEY=<secret_access_key>
 
-
 * **Command-Line Options:** The corresponding command-line options look
   very similar::
 
     --os-auth-url <url>
     --os-identity-api-version 3
     --os-project-name <project-name>
     --os-project-domain-name <project-domain-name>
@@ -107,37 +112,40 @@
 * **Existing Token:** Authentication may also be performed using an
   already-acquired token and a URL pointing directly to the service
   API that presumably was acquired from the Service Catalog::
 
     export OS_TOKEN=<token>
     export OS_URL=<url-to-openstack-service>
 
-The corresponding command-line options look very similar::
+* The corresponding command-line options look very similar::
 
     --os-token <token>
     --os-url <url-to-openstack-service>
 
 In addition to that a regular `clouds.yaml` configuration file can be used
 
 More information is available at
 https://docs.openstack.org/python-openstackclient/latest/cli/authentication.html
 or
 https://developer.openstack.org/sdks/python/openstacksdk/users/config
 
+OTC Extensions CLI Usage
+------------------------
+
+`OTCE CLI Command Overview <https://python-otcextensions.readthedocs.io/en/latest/cli/index.html>`_
 
-Writing Own Code
-----------------
+OTC Extensions SDK Guides
+-------------------------
 
-XXX Example XXXX
+`OTCE SDK Guides <https://python-otcextensions.readthedocs.io/en/latest/sdk/guides/index.html>`_
 
 Contributing
 ------------
 
-See CONTRIBUTING.rst
+* `Contribution Page <https://python-otcextensions.readthedocs.io/en/latest/contributor/index.html>`_
 
 Further Links
 -------------
 
 * `Issue Tracker <https://github.com/OpenTelekomCloud/python-otcextensions/issues>`_
 
 .. _instructions: http://python-otcextensions.readthedocs.io/en/latest/install/
-
```

### Comparing `otcextensions-0.9.0/spec/python-otcextensions.spec` & `otcextensions-0.9.1/spec/python-otcextensions.spec`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/conf.py` & `otcextensions-0.9.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/architecture.rst` & `otcextensions-0.9.1/doc/source/sdk/architecture.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/resources/cce/v3/cluster.rst` & `otcextensions-0.9.1/doc/source/sdk/resources/cce/v3/cluster.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/resources/auto_scaling/v1/quota.rst` & `otcextensions-0.9.1/doc/source/sdk/resources/auto_scaling/v1/quota.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/resources/dms/v1/misc.rst` & `otcextensions-0.9.1/doc/source/sdk/resources/dms/v1/misc`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/resources/dms/v1/misc` & `otcextensions-0.9.1/doc/source/sdk/resources/dms/v1/misc.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/resources/anti_ddos/v1/status.rst` & `otcextensions-0.9.1/doc/source/sdk/resources/anti_ddos/v1/status.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/resources/index.rst` & `otcextensions-0.9.1/doc/source/sdk/resources/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 
 .. toctree::
    :maxdepth: 1
 
    Anti DDoS Service (Anti-DDoS) <anti_ddos/index>
    AutoScaling Service (AS) <auto_scaling/index>
    Cloud Container Engine (CCE) <cce/index>
+   Cloud Eye Service (CES) <ces/index>
    Cloud Trace Service (CTS) <cts/index>
    Distributed Cache Service (DCS) <dcs/index>
    Dedicated Host Service (DeH) <deh/index>
    Distributed Message Service (DMS) <dms/index>
    Domain Name Service (DNS) <dns/index>
+   Identity Service (IAM) <identity/index>
    Key Management Service (KMS) <kms/index>
    Network Address Translation (NAT) <nat/index>
    Object Block Storage (OBS) <obs/index>
    Relational Database Service (RDS) <rds/index>
    Virtual Private Cloud (VPC) <vpc/index>
    Web Application Firewall (WAF) <waf/index>
```

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/cce_v1.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/cce_v1.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/rds_v1.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/rds_v1.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/kms.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/kms.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/dms.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/dms.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/rds_v3.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/rds_v3.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/volume_backup.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/volume_backup.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/dns.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/dns.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/dcs.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/dcs.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/vpc.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/vpc.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/deh.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/deh.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/anti_ddos.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/anti_ddos.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/auto_scaling.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/auto_scaling.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/nat.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/nat.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/waf.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/waf.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/index.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 .. toctree::
    :maxdepth: 1
 
    Anti DDoS Service (Anti-DDoS) <anti_ddos>
    AutoScaling Service (AS) <auto_scaling>
    Cloud Container Engine v1 (CCEv1) <cce_v1>
    Cloud Container Engine v2 (CCE) <cce_v3>
+   Cloud Eye Service (CES) <ces>
    Cloud Trace Service (CTS) <cts>
    Distributed Cache Service (DCS) <dcs>
    Dedicated Host Service (DeH) <deh>
    Distributed Message Service (DMS) <dms>
    Domain Name Server Service (DNS) <dns>
+   Identity Service (IAM) <identity_v3>
    Key Management Service (KMS) <kms>
    Network Address Translation (NAT) <nat>
    Object Block Storage (OBS) <obs>
    Relational Database Service RDS V1 (RDSv1) <rds_v1>
    Relational Database Service RDS V3 (RDS) <rds_v3>
    Volume Backup Service (VBS) <volume_backup>
    Virtual Private Cloud (VPC) <vpc>
```

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/cce_v3.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/cce_v3.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/obs.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/obs.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/proxies/cts.rst` & `otcextensions-0.9.1/doc/source/sdk/proxies/cts.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 CTS API
 =======
 
 .. automodule:: otcextensions.sdk.cts.v1._proxy
 
-The Distributed Message Service Class
--------------------------------------
+The Cloud Trace Service Class
+-----------------------------
 
 The CTS high-level interface is available through the ``cts``
 member of a :class:`~openstack.connection.Connection` object.  The
 ``cts`` member will only be added if the
 ``otcextensions.sdk.register_otc_extensions(conn)`` method is called.
 
 Trace Operations
```

### Comparing `otcextensions-0.9.0/doc/source/sdk/getting_started.rst` & `otcextensions-0.9.1/doc/source/sdk/getting_started.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/guides/kms.rst` & `otcextensions-0.9.1/doc/source/sdk/guides/kms.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/guides/dns.rst` & `otcextensions-0.9.1/doc/source/sdk/guides/dns.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/guides/dcs.rst` & `otcextensions-0.9.1/doc/source/sdk/guides/dcs.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/guides/vpc.rst` & `otcextensions-0.9.1/doc/source/sdk/guides/vpc.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/guides/deh.rst` & `otcextensions-0.9.1/doc/source/sdk/guides/deh.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/guides/rds.rst` & `otcextensions-0.9.1/doc/source/sdk/guides/rds.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/guides/anti_ddos.rst` & `otcextensions-0.9.1/doc/source/sdk/guides/anti_ddos.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/guides/auto_scaling.rst` & `otcextensions-0.9.1/doc/source/sdk/guides/auto_scaling.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/guides/nat.rst` & `otcextensions-0.9.1/doc/source/sdk/guides/nat.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/guides/cce.rst` & `otcextensions-0.9.1/doc/source/sdk/guides/cce.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/guides/logging.rst` & `otcextensions-0.9.1/doc/source/sdk/guides/logging.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/guides/index.rst` & `otcextensions-0.9.1/doc/source/sdk/guides/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 .. toctree::
    :maxdepth: 1
 
    anti_ddos
    auto_scaling
    cce
+   ces
    cts
    dcs
    deh
    dns
    kms
    nat
    rds
```

### Comparing `otcextensions-0.9.0/doc/source/sdk/guides/cts.rst` & `otcextensions-0.9.1/doc/source/sdk/guides/cts.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/sdk/index.rst` & `otcextensions-0.9.1/doc/source/sdk/index.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/dms.rst` & `otcextensions-0.9.1/doc/source/cli/dms.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/rds_v3.rst` & `otcextensions-0.9.1/doc/source/cli/rds_v3.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/volume_backup.rst` & `otcextensions-0.9.1/doc/source/cli/volume_backup.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/dns.rst` & `otcextensions-0.9.1/doc/source/cli/dns.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/dcs.rst` & `otcextensions-0.9.1/doc/source/cli/dcs.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/vpc.rst` & `otcextensions-0.9.1/doc/source/cli/vpc.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/deh.rst` & `otcextensions-0.9.1/doc/source/cli/deh.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/anti_ddos.rst` & `otcextensions-0.9.1/doc/source/cli/anti_ddos.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/auto_scaling.rst` & `otcextensions-0.9.1/doc/source/cli/auto_scaling.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/load_balancer.rst` & `otcextensions-0.9.1/doc/source/cli/load_balancer.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/nat.rst` & `otcextensions-0.9.1/doc/source/cli/nat.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/cce_v2.rst` & `otcextensions-0.9.1/doc/source/cli/cce_v2.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/index.rst` & `otcextensions-0.9.1/doc/source/cli/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -22,19 +22,21 @@
 
 .. toctree::
    :maxdepth: 1
 
    anti_ddos
    auto_scaling
    cce_v2
+   ces
    cts
    dcs
    deh
    dms
    dns
+   identity
    kms
    load_balancer
    nat
    obs
    rds_v3
    volume_backup
    vpc
```

### Comparing `otcextensions-0.9.0/doc/source/cli/obs.rst` & `otcextensions-0.9.1/doc/source/cli/obs.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/cli/cts.rst` & `otcextensions-0.9.1/doc/source/cli/cts.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/appendices/history.rst` & `otcextensions-0.9.1/doc/source/appendices/history.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/appendices/issues.rst` & `otcextensions-0.9.1/doc/source/appendices/issues.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/appendices/glossary.rst` & `otcextensions-0.9.1/doc/source/appendices/glossary.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/enforcer.py` & `otcextensions-0.9.1/doc/source/enforcer.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 
 def get_proxy_methods():
     """Return a set of public names on all proxies"""
     names = ["otcextensions.sdk.anti_ddos.v1._proxy",
              "otcextensions.sdk.auto_scaling.v1._proxy",
              "otcextensions.sdk.cce.v1._proxy",
+             "otcextensions.sdk.ces.v1._proxy",
              "otcextensions.sdk.cts.v1._proxy",
              "otcextensions.sdk.dcs.v1._proxy",
              "otcextensions.sdk.dms.v1._proxy",
              "otcextensions.sdk.dns.v2._proxy",
              "otcextensions.sdk.kms.v1._proxy",
              "otcextensions.sdk.obs.v1._proxy",
              "otcextensions.sdk.rds.v1._proxy",
```

### Comparing `otcextensions-0.9.0/doc/source/coverage.rst` & `otcextensions-0.9.1/doc/source/coverage.rst`

 * *Files 0% similar despite different names*

```diff
@@ -40,16 +40,16 @@
       - X
       - X
       - X
       -
     * - ces
       - Cloudeye
       - X
-      -
-      -
+      - X
+      - X
       -
     * - cts
       - Clout Trace Service
       - X
       - X
       - X
       -
```

### Comparing `otcextensions-0.9.0/doc/source/index.rst` & `otcextensions-0.9.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/install/source_install.rst` & `otcextensions-0.9.1/doc/source/install/source_install.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/install/configuration.rst` & `otcextensions-0.9.1/doc/source/install/configuration.rst`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 .. code-block:: yaml
 
   clouds:
     otc:
       profile: otc
       auth:
-       username: '<USER_NAME>'
+        username: '<USER_NAME>'
         password: '<PASSWORD>'
         project_name: '<eu-de_project>'
         # or project_id: '<123456_PROJECT_ID>'
         user_domain_name: 'OTC00000000001000000xxx'
         # or user_domain_id: '<123456_DOMAIN_ID>'
         auth_url: 'https://iam.eu-de.otc.t-systems.com:443/v3'
       interface: 'public'
@@ -69,15 +69,15 @@
 
 .. code-block:: yaml
 
   clouds:
     otcfirstproject:
       profile: otc
       auth:
-       username: '<USER_NAME>'
+        username: '<USER_NAME>'
         password: '<PASSWORD>'
         project_name: '<eu-de_project>'
         # or project_id: '<123456_PROJECT_ID>'
         user_domain_name: 'OTC00000000001000000xxx'
         # or user_domain_id: '<123456_DOMAIN_ID>'
         auth_url: 'https://iam.eu-de.otc.t-systems.com:443/v3'
       interface: 'public'
@@ -110,15 +110,15 @@
 
 .. code-block:: yaml
 
   clouds:
     otc:
       profile: otc
       auth:
-       username: '<USER_NAME>'
+        username: '<USER_NAME>'
         project_name: '<eu-de_project>'
         # or project_id: '<123456_PROJECT_ID>'
         user_domain_name: 'OTC00000000001000000xxx'
         # or user_domain_id: '<123456_DOMAIN_ID>'
         auth_url: 'https://iam.eu-de.otc.t-systems.com:443/v3'
       interface: 'public'
       identity_api_version: 3 # !Important
@@ -132,14 +132,41 @@
   clouds:
     otc:
       auth:
         password: '<PASSWORD>'
 
 .. _environment-variables:
 
+Agency based authorization
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Open Telekom Cloud supports a concept of agencies. One domain delegates access
+to resources to another domain. After trust relationship is established the
+following configuration can be used in ``clouds.yaml``:
+
+.. code-block:: yaml
+
+  clouds:
+    otc:
+      profile: otc
+      auth_type: agency
+      auth:
+        username: '<USER_NAME>'
+        project_name: '<eu-de_project>'
+        # or project_id: '<123456_PROJECT_ID>'
+        user_domain_name: 'OTC00000000001000000xxx'
+        # or user_domain_id: '<123456_DOMAIN_ID>'
+        auth_url: 'https://iam.eu-de.otc.t-systems.com:443/v3'
+        target_domain_id: '<123456_DOMAIN_ID>' # Domain where agency is created
+        # or target_domain_name: '<123456_DOMAIN_NAME'
+        target_agency_name: 'test_agency' # name of the agency
+        target_project_name: '<123456_PROJECT_NAME>' # project scoped operations
+        # or target_project_id: '<123456_PROJECT_ID>'
+        # When target_project_xx is not set - domain scope is selected
+
 Configuration of Environment Variables
 --------------------------------------
 
 Instead of using the clouds.yaml file, environmnt variables can be configured
 to connect to the Open Telekom Cloud. Create a simple file like ``.ostackrc``
 in the home directory and source the file to make the variables available. On
 Open Telekom Cloud servers this file exists on bootup and needs to be changed
```

### Comparing `otcextensions-0.9.0/doc/source/install/index.rst` & `otcextensions-0.9.1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/install/pip_install.rst` & `otcextensions-0.9.1/doc/source/install/pip_install.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/contributor/create/resource.rst` & `otcextensions-0.9.1/doc/source/contributor/create/resource.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/contributor/create/examples/resource/fake.py` & `otcextensions-0.9.1/doc/source/contributor/create/examples/resource/fake.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/contributor/setup.rst` & `otcextensions-0.9.1/doc/source/contributor/setup.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/contributor/testing.rst` & `otcextensions-0.9.1/doc/source/contributor/testing.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/contributor/local.conf` & `otcextensions-0.9.1/doc/source/contributor/local.conf`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/contributor/coding.rst` & `otcextensions-0.9.1/doc/source/contributor/coding.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/contributor/layout.rst` & `otcextensions-0.9.1/doc/source/contributor/layout.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/source/contributor/index.rst` & `otcextensions-0.9.1/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/rtfd_requirements.txt` & `otcextensions-0.9.1/doc/rtfd_requirements.txt`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/doc/requirements.txt` & `otcextensions-0.9.1/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/LICENSE` & `otcextensions-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/.travis.yml` & `otcextensions-0.9.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/_hacking.py` & `otcextensions-0.9.1/otcextensions/_hacking.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/__init__.py` & `otcextensions-0.9.1/otcextensions/__init__.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/plas/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/ecs/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/plas/plas_service.py` & `otcextensions-0.9.1/otcextensions/sdk/plas/plas_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/css/css_service.py` & `otcextensions-0.9.1/otcextensions/sdk/css/css_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/css/v1/flavor.py` & `otcextensions-0.9.1/otcextensions/sdk/css/v1/flavor.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/css/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/css/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/css/v1/cluster.py` & `otcextensions-0.9.1/otcextensions/sdk/css/v1/cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dns/v2/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/dns/v2/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dns/v2/zone.py` & `otcextensions-0.9.1/otcextensions/sdk/dns/v2/zone.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dns/v2/nameserver.py` & `otcextensions-0.9.1/otcextensions/sdk/dns/v2/nameserver.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dns/v2/floating_ip.py` & `otcextensions-0.9.1/otcextensions/sdk/dns/v2/floating_ip.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dns/v2/recordset.py` & `otcextensions-0.9.1/otcextensions/sdk/dns/v2/recordset.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dns/v2/_base.py` & `otcextensions-0.9.1/otcextensions/sdk/dns/v2/_base.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dns/dns_service.py` & `otcextensions-0.9.1/otcextensions/sdk/dns/dns_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/lts/v2/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/sdrs/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/lts/lts_service.py` & `otcextensions-0.9.1/otcextensions/sdk/lts/lts_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cts/v1/tracker.py` & `otcextensions-0.9.1/otcextensions/sdk/cts/v1/tracker.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cts/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/cts/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cts/v1/trace.py` & `otcextensions-0.9.1/otcextensions/sdk/cts/v1/trace.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cts/cts_service.py` & `otcextensions-0.9.1/otcextensions/sdk/cts/cts_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/mrs/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/plas/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/mrs/mrs_service.py` & `otcextensions-0.9.1/otcextensions/sdk/mrs/mrs_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/__init__.py` & `otcextensions-0.9.1/otcextensions/sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,20 @@
         'service_type': 'cce',
         'endpoint_service_type': 'ccev2.0',
     },
     'ces': {
         'service_type': 'ces',
         'append_project_id': True,
     },
+    # 'ces': {
+    #    'service_type': 'ces',
+    #    'endpoint_service_type': 'cesv1',
+    #    'set_endpoint_override': True
+    #    'append_project_id': False,
+    # },
     'cts': {
         'service_type': 'cts',
     },
     'css': {
         'service_type': 'css',
     },
     'dcaas': {
@@ -97,14 +103,18 @@
     'dws': {
         'service_type': 'dws',
         'endpoint_service_type': 'dwsv1'
     },
     'ecs': {
         'service_type': 'ecs',
     },
+    'identity': {
+        'service_type': 'identity',
+        'replace_system': True
+    },
     'kms': {
         'service_type': 'kms',
         'append_project_id': True,
     },
     'lts': {
         'service_type': 'lts'
     },
```

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/v1/flavor.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/v1/flavor.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/v1/configuration.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/v1/configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/v1/datastore.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/v1/datastore.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/v1/backup.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/v1/backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/v1/instance.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/v1/instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/v3/flavor.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/v3/flavor.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/v3/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/v3/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/v3/configuration.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/v3/configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/v3/_base.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/v3/_base.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/v3/datastore.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/v3/datastore.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/v3/backup.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/v3/backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/v3/instance.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/v3/instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/rds/rds_service.py` & `otcextensions-0.9.1/otcextensions/sdk/rds/rds_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/compute/v2/server.py` & `otcextensions-0.9.1/otcextensions/sdk/compute/v2/server.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cloud/rds.py` & `otcextensions-0.9.1/otcextensions/sdk/cloud/rds.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dws/dws_service.py` & `otcextensions-0.9.1/otcextensions/sdk/dws/dws_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dws/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/smn/v2/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cce/cce_service.py` & `otcextensions-0.9.1/otcextensions/sdk/cce/cce_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cce/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/cce/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cce/v1/cluster.py` & `otcextensions-0.9.1/otcextensions/sdk/cce/v1/cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cce/v1/cluster_node.py` & `otcextensions-0.9.1/otcextensions/sdk/cce/v1/cluster_node.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cce/v1/_base.py` & `otcextensions-0.9.1/otcextensions/sdk/cce/v1/_base.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cce/v3/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/cce/v3/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cce/v3/cluster.py` & `otcextensions-0.9.1/otcextensions/sdk/cce/v3/cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cce/v3/cluster_node.py` & `otcextensions-0.9.1/otcextensions/sdk/cce/v3/cluster_node.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cce/v3/cluster_cert.py` & `otcextensions-0.9.1/otcextensions/sdk/cce/v3/cluster_cert.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cce/v3/_base.py` & `otcextensions-0.9.1/otcextensions/sdk/cce/v3/_base.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/cce/v3/job.py` & `otcextensions-0.9.1/otcextensions/sdk/cce/v3/job.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dcs/v1/restore.py` & `otcextensions-0.9.1/otcextensions/sdk/dcs/v1/restore.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dcs/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/dcs/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dcs/v1/statistic.py` & `otcextensions-0.9.1/otcextensions/sdk/dcs/v1/statistic.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dcs/v1/config.py` & `otcextensions-0.9.1/otcextensions/sdk/dcs/v1/config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dcs/v1/backup.py` & `otcextensions-0.9.1/otcextensions/sdk/dcs/v1/backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dcs/v1/instance.py` & `otcextensions-0.9.1/otcextensions/sdk/dcs/v1/instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dcs/dcs_service.py` & `otcextensions-0.9.1/otcextensions/sdk/dcs/dcs_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/obs/obs_service.py` & `otcextensions-0.9.1/otcextensions/sdk/obs/obs_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/obs/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/obs/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/obs/v1/container.py` & `otcextensions-0.9.1/otcextensions/sdk/obs/v1/container.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/obs/v1/_base.py` & `otcextensions-0.9.1/otcextensions/sdk/obs/v1/_base.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/obs/v1/obj.py` & `otcextensions-0.9.1/otcextensions/sdk/obs/v1/obj.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/sdrs/sdrs_service.py` & `otcextensions-0.9.1/otcextensions/sdk/sdrs/sdrs_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/sdrs/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/dcaas/v2/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/auto_scaling/auto_scaling_service.py` & `otcextensions-0.9.1/otcextensions/sdk/auto_scaling/auto_scaling_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/__init__.py` & `otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,7 +464,20 @@
         if group:
             group = self._get_resource(_group.Group, group)
             return self._list(_quota.ScalingQuota,
                               paginated=False,
                               scaling_group_id=group.id)
         else:
             return self._list(_quota.Quota, paginated=False)
+
+    # ======== Project cleanup ========
+    def _get_cleanup_dependencies(self):
+        return {
+            'auto_scaling': {
+                'before': ['compute', 'block_storage']
+            }
+        }
+
+    def _service_cleanup(self, dry_run=True, client_status_queue=None,
+                         identified_resources=None,
+                         filters=None, resource_evaluation_fn=None):
+        pass
```

### Comparing `otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/activity.py` & `otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/activity.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/quota.py` & `otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/quota.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/_base.py` & `otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/_base.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/config.py` & `otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/group.py` & `otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/policy.py` & `otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/auto_scaling/v1/instance.py` & `otcextensions-0.9.1/otcextensions/sdk/auto_scaling/v1/instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/sdk_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/sdk_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dcaas/v2/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/dis/v2/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dcaas/dcaas_service.py` & `otcextensions-0.9.1/otcextensions/sdk/dcaas/dcaas_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dis/v2/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/mrs/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dis/dis_service.py` & `otcextensions-0.9.1/otcextensions/sdk/dis/dis_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/volume_backup/v2/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/volume_backup/v2/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/volume_backup/v2/backup_policy.py` & `otcextensions-0.9.1/otcextensions/sdk/volume_backup/v2/backup_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/volume_backup/v2/backup_task.py` & `otcextensions-0.9.1/otcextensions/sdk/volume_backup/v2/backup_task.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/volume_backup/v2/job.py` & `otcextensions-0.9.1/otcextensions/sdk/volume_backup/v2/job.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/volume_backup/volume_backup_service.py` & `otcextensions-0.9.1/otcextensions/sdk/volume_backup/volume_backup_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/ces/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/dws/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/ces/ces_service.py` & `otcextensions-0.9.1/otcextensions/sdk/ces/ces_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/smn/v2/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/dds/v3/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/smn/smn_service.py` & `otcextensions-0.9.1/otcextensions/sdk/smn/smn_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/kms/v1/data_key.py` & `otcextensions-0.9.1/otcextensions/sdk/kms/v1/data_key.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/kms/v1/misc.py` & `otcextensions-0.9.1/otcextensions/sdk/kms/v1/misc.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/kms/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/kms/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/kms/v1/key.py` & `otcextensions-0.9.1/otcextensions/sdk/kms/v1/key.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/kms/v1/_base.py` & `otcextensions-0.9.1/otcextensions/sdk/kms/v1/_base.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/kms/kms_service.py` & `otcextensions-0.9.1/otcextensions/sdk/kms/kms_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/vpc/v2/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/vpc/v2/_proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -179,7 +179,28 @@
         :returns: One :class:`~otcextensions.sdk.vpc.v2.route.Route`
 
         :raises: :class:`~openstack.exceptions.ResourceNotFound`
                  when no resource can be found.
         """
         self._override_endpoint()
         return self._get(_route.Route, route)
+
+    # ========== Project cleanup ==========
+    def _get_cleanup_dependencies(self):
+        return {
+            'vpc': {
+                'before': ['network']
+            }
+        }
+
+    def _service_cleanup(self, dry_run=True, client_status_queue=None,
+                         identified_resources=None,
+                         filters=None, resource_evaluation_fn=None):
+        for obj in self.peerings():
+            self._service_cleanup_del_res(
+                self.delete_peering,
+                obj,
+                dry_run=dry_run,
+                client_status_queue=client_status_queue,
+                identified_resources=identified_resources,
+                filters=filters,
+                resource_evaluation_fn=resource_evaluation_fn)
```

### Comparing `otcextensions-0.9.0/otcextensions/sdk/vpc/v2/route.py` & `otcextensions-0.9.1/otcextensions/sdk/vpc/v2/route.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/vpc/v2/peering.py` & `otcextensions-0.9.1/otcextensions/sdk/vpc/v2/peering.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/vpc/vpc_service.py` & `otcextensions-0.9.1/otcextensions/sdk/vpc/vpc_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dms/v1/queue.py` & `otcextensions-0.9.1/otcextensions/sdk/dms/v1/queue.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dms/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/dms/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dms/v1/topic.py` & `otcextensions-0.9.1/otcextensions/sdk/dms/v1/topic.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dms/v1/group_message.py` & `otcextensions-0.9.1/otcextensions/sdk/dms/v1/group_message.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dms/v1/quota.py` & `otcextensions-0.9.1/otcextensions/sdk/dms/v1/quota.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dms/v1/product.py` & `otcextensions-0.9.1/otcextensions/sdk/dms/v1/product.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dms/v1/maintenance_window.py` & `otcextensions-0.9.1/otcextensions/sdk/dms/v1/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dms/v1/_base.py` & `otcextensions-0.9.1/otcextensions/sdk/dms/v1/_base.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dms/v1/message.py` & `otcextensions-0.9.1/otcextensions/sdk/dms/v1/message.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dms/v1/group.py` & `otcextensions-0.9.1/otcextensions/sdk/dms/v1/group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dms/v1/az.py` & `otcextensions-0.9.1/otcextensions/sdk/dms/v1/az.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dms/v1/instance.py` & `otcextensions-0.9.1/otcextensions/sdk/dms/v1/instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dms/dms_service.py` & `otcextensions-0.9.1/otcextensions/sdk/dms/dms_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dds/dds_service.py` & `otcextensions-0.9.1/otcextensions/sdk/dds/dds_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/dds/v3/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/lts/v2/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/anti_ddos/anti_ddos_service.py` & `otcextensions-0.9.1/otcextensions/sdk/anti_ddos/anti_ddos_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/anti_ddos/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/anti_ddos/v1/_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,7 +150,20 @@
 
         :returns: A generator of FloatingIPWeekStat object
         :rtype:
             :class:`~otcextensions.sdk.anti_ddos.v1.status.FloatingIPWeekStat`
         """
         return self._get(_status.FloatingIPWeekStat, requires_id=False,
                          value=None, **query)
+
+    # ======== Project cleanup ========
+    def _get_cleanup_dependencies(self):
+        return {
+            'anti_ddos': {
+                'before': ['network']
+            }
+        }
+
+    def _service_cleanup(self, dry_run=True, client_status_queue=None,
+                         identified_resources=None,
+                         filters=None, resource_evaluation_fn=None):
+        pass
```

### Comparing `otcextensions-0.9.0/otcextensions/sdk/anti_ddos/v1/alert_config.py` & `otcextensions-0.9.1/otcextensions/sdk/anti_ddos/v1/alert_config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/anti_ddos/v1/status.py` & `otcextensions-0.9.1/otcextensions/sdk/anti_ddos/v1/status.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/anti_ddos/v1/floating_ip.py` & `otcextensions-0.9.1/otcextensions/sdk/anti_ddos/v1/floating_ip.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/anti_ddos/v1/config.py` & `otcextensions-0.9.1/otcextensions/sdk/anti_ddos/v1/config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/ecs/ecs_service.py` & `otcextensions-0.9.1/otcextensions/sdk/ecs/ecs_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/ecs/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/compute/v2/_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 from openstack import proxy
 
 
 class Proxy(proxy.Proxy):
-
-    skip_discovery = True
+    pass
```

### Comparing `otcextensions-0.9.0/otcextensions/sdk/deh/v1/host_type.py` & `otcextensions-0.9.1/otcextensions/sdk/deh/v1/host_type.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/deh/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/deh/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/deh/v1/server.py` & `otcextensions-0.9.1/otcextensions/sdk/deh/v1/server.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/deh/v1/host.py` & `otcextensions-0.9.1/otcextensions/sdk/deh/v1/host.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     allow_list = True
     allow_fetch = True
     allow_delete = True
     allow_commit = True
 
     _query_mapping = resource.QueryParameters(
         'id', 'name', 'host_type', 'host_type_name',
-        'flavor', 'state', 'tenant', 'availability_zone',
+        'flavor', 'status', 'tenant', 'availability_zone',
         'changes_since', 'tags', 'instance_uuid', 'released_at',
         changes_since='changes-since')
 
     #: Properties
     #: Specifies DeH ID
     id = resource.Body('dedicated_host_id', alternate_id=True)
     #: Time at which the DeH has been allocated
@@ -87,15 +87,15 @@
     project_id = resource.Body('project_id')
     #: Specifies the number of allocated DeHs (during creation).
     quantity = resource.Body('quantity', type=int)
     #: Time at which the DeH has been released
     released_at = resource.Body('released_at')
     #: Specifies the DeH status.
     #: The value can be available, fault or released
-    state = resource.Body('state')
+    status = resource.Body('state')
     #: Tag.
     tags = resource.Body('tags', type=list)
 
     def fetch_tags(self, session):
         """Lists tags set on the entity.
 
         :param session: The session to use for making this request.
```

### Comparing `otcextensions-0.9.0/otcextensions/sdk/deh/deh_service.py` & `otcextensions-0.9.1/otcextensions/sdk/deh/deh_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/nat/v2/snat.py` & `otcextensions-0.9.1/otcextensions/sdk/nat/v2/snat.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/nat/v2/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/nat/v2/_proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -203,7 +203,31 @@
 
         :param dict query: Optional query parameters to be sent to limit
             the resources being returned.
 
         :returns: A generator of Dnat objects.
         """
         return self._list(_dnat.Dnat, **query)
+
+    # ======== Project cleanup ========
+    def _get_cleanup_dependencies(self):
+        return {
+            'nat': {
+                'before': ['network']
+            }
+        }
+
+    def _service_cleanup(self, dry_run=True, client_status_queue=None,
+                         identified_resources=None,
+                         filters=None, resource_evaluation_fn=None):
+        for obj in self.gateways():
+            need_delete = self._service_cleanup_del_res(
+                self.delete_gateway,
+                obj,
+                dry_run=dry_run,
+                client_status_queue=client_status_queue,
+                identified_resources=identified_resources,
+                filters=filters,
+                resource_evaluation_fn=resource_evaluation_fn)
+            if dry_run and need_delete:
+                for port in self._connection.network.ports(device_id=obj.id):
+                    identified_resources[port.id] = port
```

### Comparing `otcextensions-0.9.0/otcextensions/sdk/nat/v2/gateway.py` & `otcextensions-0.9.1/otcextensions/sdk/nat/v2/gateway.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/nat/v2/dnat.py` & `otcextensions-0.9.1/otcextensions/sdk/nat/v2/dnat.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/nat/nat_service.py` & `otcextensions-0.9.1/otcextensions/sdk/nat/nat_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/job.py` & `otcextensions-0.9.1/otcextensions/sdk/job.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/waf/waf_service.py` & `otcextensions-0.9.1/otcextensions/sdk/waf/waf_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/waf/v1/_proxy.py` & `otcextensions-0.9.1/otcextensions/sdk/waf/v1/_proxy.py`

 * *Files 24% similar despite different names*

```diff
@@ -194,7 +194,38 @@
             to delete a nonexistent domain.
 
         :returns: ``None``
         """
         return self._find(_domain.Domain, name_or_id,
                           ignore_missing=ignore_missing,
                           **attrs)
+
+    # ======== Project cleanup ========
+    def _get_cleanup_dependencies(self):
+        return {
+            'waf': {
+                'before': []
+            }
+        }
+
+    def _service_cleanup(self, dry_run=True, client_status_queue=None,
+                         identified_resources=None,
+                         filters=None, resource_evaluation_fn=None):
+        for obj in self.domains():
+            self._service_cleanup_del_res(
+                self.delete_domain,
+                obj,
+                dry_run=dry_run,
+                client_status_queue=client_status_queue,
+                identified_resources=identified_resources,
+                filters=filters,
+                resource_evaluation_fn=resource_evaluation_fn)
+
+        for obj in self.certificates():
+            self._service_cleanup_del_res(
+                self.delete_certificate,
+                obj,
+                dry_run=dry_run,
+                client_status_queue=client_status_queue,
+                identified_resources=identified_resources,
+                filters=filters,
+                resource_evaluation_fn=resource_evaluation_fn)
```

### Comparing `otcextensions-0.9.0/otcextensions/sdk/waf/v1/certificate.py` & `otcextensions-0.9.1/otcextensions/sdk/waf/v1/certificate.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/waf/v1/domain.py` & `otcextensions-0.9.1/otcextensions/sdk/waf/v1/domain.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/waf/v1/_base.py` & `otcextensions-0.9.1/otcextensions/sdk/waf/v1/_base.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/ak_auth.py` & `otcextensions-0.9.1/otcextensions/sdk/ak_auth.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/sdk/sdk_resource.py` & `otcextensions-0.9.1/otcextensions/sdk/sdk_resource.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/i18n.py` & `otcextensions-0.9.1/otcextensions/i18n.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/common/utils.py` & `otcextensions-0.9.1/otcextensions/common/utils.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/common/exc.py` & `otcextensions-0.9.1/otcextensions/common/exc.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/common/sdk_utils.py` & `otcextensions-0.9.1/otcextensions/common/sdk_utils.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/common/format.py` & `otcextensions-0.9.1/otcextensions/common/format.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/common/errors.py` & `otcextensions-0.9.1/otcextensions/common/errors.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/plas/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/plas/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/css/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/css/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/test_openstacksdk_init.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/test_openstacksdk_init.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/dns/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/dns/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/lts/v2/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/lts/v2/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/cts/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/cts/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/mrs/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/mrs/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/rds/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/rds/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/dws/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/dws/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/cce/v1/test_cluster_nodes.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/cce/v1/test_cluster_nodes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/cce/v1/test_cluster.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/cce/v1/test_cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/cce/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/cce/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/dcs/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/dcs/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/obs/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/obs/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/sdrs/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/sdrs/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/auto_scaling/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/auto_scaling/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/dcaas/v2/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/dcaas/v2/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/dis/v2/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/dis/v2/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/volume_backup/v2/test_job.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/volume_backup/v2/test_job.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/volume_backup/v2/test_backup_policy.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/volume_backup/v2/test_backup_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/volume_backup/v2/test_backup.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/volume_backup/v2/test_backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/volume_backup/__init__.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/volume_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/ces/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/ces/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/smn/v2/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/smn/v2/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/kms/v1/test_key.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/kms/v1/test_key.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/kms/v1/test_data_key.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/kms/v1/test_data_key.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/kms/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/kms/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/kms/v1/test_misc.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/kms/v1/test_misc.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/vpc/v2/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/vpc/v2/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/dms/v1/test_message.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/dms/v1/test_message.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/dms/v1/test_instance.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/dms/v1/test_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/dms/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/dms/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/dms/v1/test_queue.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/dms/v1/test_queue.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/dms/v1/test_misc.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/dms/v1/test_misc.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/dds/v3/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/dds/v3/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/anti_ddos/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/anti_ddos/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/deh/v1/test_host.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/deh/v1/test_host.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/deh/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/deh/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/nat/v2/test_dnat.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/nat/v2/test_dnat.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/nat/v2/test_gateway.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/nat/v2/test_gateway.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/nat/v2/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/nat/v2/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/nat/v2/test_snat.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/nat/v2/test_snat.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/waf/__init__.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/waf/__init__.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/waf/v1/test_domain.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/waf/v1/test_domain.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/waf/v1/test_service.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/waf/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/sdk/waf/v1/test_certificate.py` & `otcextensions-0.9.1/otcextensions/tests/functional/sdk/waf/v1/test_certificate.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/base.py` & `otcextensions-0.9.1/otcextensions/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/dns/v2/test_zone.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/dns/v2/test_zone.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/rds/v3/test_configuration.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/rds/v3/test_configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/rds/v3/test_instance.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/rds/v3/test_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/rds/v3/test_datastore.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/rds/v3/test_datastore.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/rds/v3/test_flavor.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/rds/v3/test_flavor.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/obs/v1/test_obj.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/obs/v1/test_obj.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/obs/v1/test_container.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/obs/v1/test_container.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/volume_backup/v2/test_policy.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/volume_backup/v2/test_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/vpc/v2/common.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/vpc/v2/common.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/vpc/v2/test_peering.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/vpc/v2/test_peering.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/nat/v2/common.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/nat/v2/common.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/nat/v2/test_dnat.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/nat/v2/test_dnat.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/nat/v2/test_gateway.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/nat/v2/test_gateway.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/functional/osclient/nat/v2/test_snat.py` & `otcextensions-0.9.1/otcextensions/tests/functional/osclient/nat/v2/test_snat.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/plas/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/plas/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/css/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/css/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/css/v1/test_cluster.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/css/v1/test_cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/css/v1/test_flavor.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/css/v1/test_flavor.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/v2/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/v2/test_recordset.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/v2/test_recordset.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/v2/test_zone.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/v2/test_zone.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/v2/test_nameserver.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/v2/test_nameserver.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dns/v2/test_floating_ip.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dns/v2/test_floating_ip.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/lts/v2/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/lts/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/cts/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/cts/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/cts/v1/test_trace.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/cts/v1/test_trace.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/cts/v1/test_tracker.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/cts/v1/test_tracker.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/mrs/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/mrs/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/test_configuration.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/test_configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/test_instance.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/test_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/test_datastore.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/test_datastore.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/test_backup.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/test_backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v1/test_flavor.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v1/test_flavor.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_instance.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_base.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_base.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_datastore.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_datastore.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_config.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_backup.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/rds/v3/test_flavor.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/rds/v3/test_flavor.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/compute/v2/test_server.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/compute/v2/test_server.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/cloud/test_rds.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/cloud/test_rds.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dws/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dws/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v1/test_cluster.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v1/test_cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v1/test_cluster_node.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v1/test_cluster_node.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v3/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v3/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v3/test_job.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v3/test_job.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v3/test_cluster.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v3/test_cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v3/test_cluster_cert.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v3/test_cluster_cert.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/cce/v3/test_cluster_node.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/cce/v3/test_cluster_node.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/test_restore.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/test_restore.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/test_instance.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/test_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/test_statistic.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/test_statistic.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/test_config.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/test_config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcs/v1/test_backup.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcs/v1/test_backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/obs/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/obs/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/obs/v1/test_obj.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/obs/v1/test_obj.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/obs/v1/test_container.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/obs/v1/test_container.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/sdrs/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/sdrs/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_instance.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_policy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_activity.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_activity.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_config.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_group.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/auto_scaling/v1/test_quota.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/auto_scaling/v1/test_quota.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/base.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/base.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dcaas/v2/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dcaas/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dis/v2/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dis/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/test_job.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/test_job.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/test_backup_policy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/test_backup_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/get_backup.json` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/get_backup.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_backup_policies.json` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_backup_policies.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_backups.json` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_backups.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/link_resources.json` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/link_resources.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_backup_details.json` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_backup_details.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_tasks.json` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/data_files/list_tasks.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/volume_backup/v2/test_backup_policy_task.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/volume_backup/v2/test_backup_policy_task.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/ces/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dds/v3/test_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from otcextensions.sdk.ces.v1 import _proxy
+from otcextensions.sdk.dds.v3 import _proxy
 
 from openstack.tests.unit import test_proxy_base
 
 
-class TestCESProxy(test_proxy_base.TestProxyBase):
+class TestDdsProxy(test_proxy_base.TestProxyBase):
 
     def setUp(self):
-        super(TestCESProxy, self).setUp()
+        super(TestDdsProxy, self).setUp()
         self.proxy = _proxy.Proxy(self.session)
```

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/smn/v2/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/smn/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/kms/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/kms/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/kms/v1/test_key.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/kms/v1/test_key.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/kms/v1/test_data_key.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/kms/v1/test_data_key.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/kms/v1/test_misc.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/kms/v1/test_misc.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/vpc/v2/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/vpc/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/vpc/v2/test_peering.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/vpc/v2/test_peering.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/vpc/v2/test_route.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/vpc/v2/test_route.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_message.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_message.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_instance.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_product_spec.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_product_spec.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_mw.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_mw.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_topic.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_topic.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_az.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_az.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_group.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_queue.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_queue.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dms/v1/test_quota.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/dms/v1/test_quota.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/dds/v3/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
+#
 
-from otcextensions.sdk.dds.v3 import _proxy
+from openstack.tests.unit import base
 
-from openstack.tests.unit import test_proxy_base
+from otcextensions import sdk
 
 
-class TestDdsProxy(test_proxy_base.TestProxyBase):
+class TestCase(base.TestCase):
 
     def setUp(self):
-        super(TestDdsProxy, self).setUp()
-        self.proxy = _proxy.Proxy(self.session)
+        super(TestCase, self).setUp()
+        sdk.load(self.cloud)
```

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/anti_ddos/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/anti_ddos/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/anti_ddos/v1/test_status.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/anti_ddos/v1/test_status.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/anti_ddos/v1/test_config.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/anti_ddos/v1/test_config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/anti_ddos/v1/test_floating_ip.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/anti_ddos/v1/test_floating_ip.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/test_sdk_resource.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/test_sdk_resource.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/deh/v1/test_server.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/deh/v1/test_server.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/deh/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/deh/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/deh/v1/test_host_type.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/deh/v1/test_host_type.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/deh/v1/test_host.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/deh/v1/test_host.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                               'host_type_name': 'host_type_name',
                               'id': 'id',
                               'instance_uuid': 'instance_uuid',
                               'limit': 'limit',
                               'marker': 'marker',
                               'name': 'name',
                               'released_at': 'released_at',
-                              'state': 'state',
+                              'status': 'status',
                               'tags': 'tags',
                               'tenant': 'tenant'},
                              sot._query_mapping._mapping)
 
         self.assertTrue(sot.allow_list)
         self.assertTrue(sot.allow_fetch)
         self.assertTrue(sot.allow_create)
@@ -111,15 +111,15 @@
     def test_make_it(self):
 
         sot = host.Host(**EXAMPLE)
         self.assertEqual(EXAMPLE['dedicated_host_id'], FAKE_ID)
         self.assertEqual(EXAMPLE['name'], sot.name)
         self.assertEqual(EXAMPLE['auto_placement'], sot.auto_placement)
         self.assertEqual(EXAMPLE['availability_zone'], sot.availability_zone)
-        self.assertEqual(EXAMPLE['state'], sot.state)
+        self.assertEqual(EXAMPLE['state'], sot.status)
         self.assertEqual(EXAMPLE['project_id'], sot.project_id)
         self.assertEqual(EXAMPLE['available_vcpus'], sot.available_vcpus)
         self.assertEqual(EXAMPLE['available_memory'], sot.available_memory)
         self.assertEqual(EXAMPLE['instance_total'], sot.instance_total)
         self.assertEqual(EXAMPLE['released_at'], sot.released_at)
         ref = EXAMPLE['host_properties']
         actual = sot.host_properties
```

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/nat/v2/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/nat/v2/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/nat/v2/test_dnat.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/nat/v2/test_dnat.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-
-from openstack.tests.unit import base
-
-from otcextensions.sdk.nat.v2 import dnat
-
-
-INSTANCE_ID = '5b95c675-69c2-4656-ba06-58ff72e1d338'
-EXAMPLE = {
-    'floating_ip_id': 'bdc10a4c-d81a-41ec-adf7-de857f7c812a',
-    'status': 'ACTIVE',
-    'nat_gateway_id': 'a78fb3eb-1654-4710-8742-3fc49d5f04f8',
-    'admin_state_up': True,
-    'port_id': '9a469561-daac-4c94-88f5-39366e5ea193',
-    'internal_service_port': 993,
-    'protocol': 'TCP',
-    'project_id': '27e25061336f4af590faeabeb7fcd9a3',
-    'created_at': '2017-11-18 07:54:21.665430',
-    'id': INSTANCE_ID,
-    'floating_ip_address': '5.21.11.226',
-    'external_service_port': 242,
-    'private_ip': "",
-}
-
-
-class TestDnat(base.TestCase):
-
-    def test_basic(self):
-        sot = dnat.Dnat()
-        self.assertEqual('dnat_rule', sot.resource_key)
-        self.assertEqual('dnat_rules', sot.resources_key)
-        path = '/dnat_rules'
-        self.assertEqual(path, sot.base_path)
-        self.assertTrue(sot.allow_list)
-        self.assertTrue(sot.allow_create)
-        self.assertTrue(sot.allow_fetch)
-        self.assertFalse(sot.allow_commit)
-        self.assertTrue(sot.allow_delete)
-
-    def test_make_it(self):
-        sot = dnat.Dnat(**EXAMPLE)
-        self.assertEqual(EXAMPLE['floating_ip_id'], sot.floating_ip_id)
-        self.assertEqual(EXAMPLE['status'], sot.status)
-        self.assertEqual(EXAMPLE['nat_gateway_id'], sot.nat_gateway_id)
-        self.assertEqual(EXAMPLE['admin_state_up'], sot.admin_state_up)
-        self.assertEqual(EXAMPLE['port_id'], sot.port_id)
-        self.assertEqual(EXAMPLE['internal_service_port'],
-                         sot.internal_service_port)
-        self.assertEqual(EXAMPLE['protocol'], sot.protocol)
-        self.assertEqual(EXAMPLE['project_id'], sot.project_id)
-        self.assertEqual(EXAMPLE['created_at'], sot.created_at)
-        self.assertEqual(EXAMPLE['id'], sot.id)
-        self.assertEqual(EXAMPLE['floating_ip_address'],
-                         sot.floating_ip_address)
-        self.assertEqual(EXAMPLE['external_service_port'],
-                         sot.external_service_port)
-        self.assertEqual(EXAMPLE['private_ip'], sot.private_ip)
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+
+from openstack.tests.unit import base
+
+from otcextensions.sdk.nat.v2 import dnat
+
+
+INSTANCE_ID = '5b95c675-69c2-4656-ba06-58ff72e1d338'
+EXAMPLE = {
+    'floating_ip_id': 'bdc10a4c-d81a-41ec-adf7-de857f7c812a',
+    'status': 'ACTIVE',
+    'nat_gateway_id': 'a78fb3eb-1654-4710-8742-3fc49d5f04f8',
+    'admin_state_up': True,
+    'port_id': '9a469561-daac-4c94-88f5-39366e5ea193',
+    'internal_service_port': 993,
+    'protocol': 'TCP',
+    'project_id': '27e25061336f4af590faeabeb7fcd9a3',
+    'created_at': '2017-11-18 07:54:21.665430',
+    'id': INSTANCE_ID,
+    'floating_ip_address': '5.21.11.226',
+    'external_service_port': 242,
+    'private_ip': "",
+}
+
+
+class TestDnat(base.TestCase):
+
+    def test_basic(self):
+        sot = dnat.Dnat()
+        self.assertEqual('dnat_rule', sot.resource_key)
+        self.assertEqual('dnat_rules', sot.resources_key)
+        path = '/dnat_rules'
+        self.assertEqual(path, sot.base_path)
+        self.assertTrue(sot.allow_list)
+        self.assertTrue(sot.allow_create)
+        self.assertTrue(sot.allow_fetch)
+        self.assertFalse(sot.allow_commit)
+        self.assertTrue(sot.allow_delete)
+
+    def test_make_it(self):
+        sot = dnat.Dnat(**EXAMPLE)
+        self.assertEqual(EXAMPLE['floating_ip_id'], sot.floating_ip_id)
+        self.assertEqual(EXAMPLE['status'], sot.status)
+        self.assertEqual(EXAMPLE['nat_gateway_id'], sot.nat_gateway_id)
+        self.assertEqual(EXAMPLE['admin_state_up'], sot.admin_state_up)
+        self.assertEqual(EXAMPLE['port_id'], sot.port_id)
+        self.assertEqual(EXAMPLE['internal_service_port'],
+                         sot.internal_service_port)
+        self.assertEqual(EXAMPLE['protocol'], sot.protocol)
+        self.assertEqual(EXAMPLE['project_id'], sot.project_id)
+        self.assertEqual(EXAMPLE['created_at'], sot.created_at)
+        self.assertEqual(EXAMPLE['id'], sot.id)
+        self.assertEqual(EXAMPLE['floating_ip_address'],
+                         sot.floating_ip_address)
+        self.assertEqual(EXAMPLE['external_service_port'],
+                         sot.external_service_port)
+        self.assertEqual(EXAMPLE['private_ip'], sot.private_ip)
```

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/nat/v2/test_gateway.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/waf/v1/test_certificate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,65 @@
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-
-from openstack.tests.unit import base
-
-from otcextensions.sdk.nat.v2 import gateway
-
-
-INSTANCE_NAME = 'GATEWAYNAME'
-INSTANCE_ID = 'a78fb3eb-1654-4710-8742-3fc49d5f04f8'
-EXAMPLE = {
-    'router_id': 'd84f345c-80a1-4fa2-a39c-d0d397c3f09a',
-    'status': 'PENDING_CREATE',
-    'description': 'Test Gateway Response',
-    'admin_state_up': True,
-    'project_id': '27e25061336f4af590faeabeb7fcd9a3',
-    'created_at': '2017-11-18 07:34:32.203044',
-    'spec': '2',
-    'internal_network_id': '89d66639-aacb-4929-969d-07080b0f9fd9',
-    'id': INSTANCE_ID,
-    'name': INSTANCE_NAME
-}
-
-
-class TestGateway(base.TestCase):
-
-    def test_basic(self):
-        sot = gateway.Gateway()
-        self.assertEqual('nat_gateway', sot.resource_key)
-        self.assertEqual('nat_gateways', sot.resources_key)
-        path = '/nat_gateways'
-        self.assertEqual(path, sot.base_path)
-        self.assertTrue(sot.allow_list)
-        self.assertTrue(sot.allow_create)
-        self.assertTrue(sot.allow_fetch)
-        self.assertTrue(sot.allow_commit)
-        self.assertTrue(sot.allow_delete)
-
-    def test_make_it(self):
-        sot = gateway.Gateway(**EXAMPLE)
-        self.assertEqual(EXAMPLE['router_id'], sot.router_id)
-        self.assertEqual(EXAMPLE['status'], sot.status)
-        self.assertEqual(EXAMPLE['description'], sot.description)
-        self.assertEqual(EXAMPLE['admin_state_up'], sot.admin_state_up)
-        self.assertEqual(EXAMPLE['project_id'], sot.project_id)
-        self.assertEqual(EXAMPLE['created_at'], sot.created_at)
-        self.assertEqual(EXAMPLE['spec'], sot.spec)
-        self.assertEqual(EXAMPLE['internal_network_id'],
-                         sot.internal_network_id)
-        self.assertEqual(EXAMPLE['id'], sot.id)
-        self.assertEqual(EXAMPLE['name'], sot.name)
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+import mock
+
+from keystoneauth1 import adapter
+
+from openstack.tests.unit import base
+
+from otcextensions.sdk.waf.v1 import certificate
+
+
+FAKE_ID = "68d5745e-6af2-40e4-945d-fe449be00148"
+EXAMPLE = {
+    "id": FAKE_ID,
+    "name": "fake_name",
+    "content": "fake",
+    "key": "fake",
+    "timestamp": 1499817600,
+    "expire_time": 1499817600
+}
+
+
+class TestCertificate(base.TestCase):
+
+    def setUp(self):
+        super(TestCertificate, self).setUp()
+        self.sess = mock.Mock(spec=adapter.Adapter)
+        self.sess.post = mock.Mock()
+
+    def test_basic(self):
+        sot = certificate.Certificate()
+
+        self.assertEqual('/waf/certificate', sot.base_path)
+        self.assertEqual('items', sot.resources_key)
+        self.assertIsNone(sot.resource_key)
+
+        self.assertTrue(sot.allow_list)
+        self.assertTrue(sot.allow_fetch)
+        self.assertTrue(sot.allow_create)
+        self.assertTrue(sot.allow_delete)
+        self.assertTrue(sot.allow_commit)
+
+    def test_make_it(self):
+
+        sot = certificate.Certificate(**EXAMPLE)
+        self.assertEqual(EXAMPLE['id'], sot.id)
+        self.assertEqual(EXAMPLE['name'], sot.name)
+        self.assertEqual(EXAMPLE['expire_time'], sot.expire_time)
+        self.assertEqual(EXAMPLE['timestamp'], sot.timestamp)
+
+        self.assertDictEqual({
+            'limit': 'limit',
+            'marker': 'marker',
+            'offset': 'offset'},
+            sot._query_mapping._mapping
+        )
```

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/nat/v2/test_snat.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/nat/v2/test_snat.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-
-from openstack.tests.unit import base
-
-from otcextensions.sdk.nat.v2 import snat
-
-
-INSTANCE_ID = '5b95c675-69c2-4656-ba06-58ff72e1d338'
-EXAMPLE = {
-    'floating_ip_id': 'bdc10a4c-d81a-41ec-adf7-de857f7c812a',
-    'status': 'PENDING_CREATE',
-    'nat_gateway_id': 'a78fb3eb-1654-4710-8742-3fc49d5f04f8',
-    'admin_state_up': True,
-    'network_id': 'eaad9cd6-2372-4be1-9535-9bd37210ae7b',
-    'cidr': None,
-    'source_type': 0,
-    'project_id': '27e25061336f4af590faeabeb7fcd9a3',
-    'created_at': '2017-11-18 07:54:21.665430',
-    'id': INSTANCE_ID,
-    'floating_ip_address': '5.21.11.226'
-}
-
-
-class TestSnat(base.TestCase):
-
-    def test_basic(self):
-        sot = snat.Snat()
-        self.assertEqual('snat_rule', sot.resource_key)
-        self.assertEqual('snat_rules', sot.resources_key)
-        path = '/snat_rules'
-        self.assertEqual(path, sot.base_path)
-        self.assertTrue(sot.allow_list)
-        self.assertTrue(sot.allow_create)
-        self.assertTrue(sot.allow_fetch)
-        self.assertFalse(sot.allow_commit)
-        self.assertTrue(sot.allow_delete)
-
-    def test_make_it(self):
-        sot = snat.Snat(**EXAMPLE)
-        self.assertEqual(EXAMPLE['floating_ip_id'], sot.floating_ip_id)
-        self.assertEqual(EXAMPLE['status'], sot.status)
-        self.assertEqual(EXAMPLE['nat_gateway_id'], sot.nat_gateway_id)
-        self.assertEqual(EXAMPLE['admin_state_up'], sot.admin_state_up)
-        self.assertEqual(EXAMPLE['network_id'], sot.network_id)
-        self.assertIsNone(sot.cidr)
-        self.assertEqual(EXAMPLE['source_type'], sot.source_type)
-        self.assertEqual(EXAMPLE['project_id'], sot.project_id)
-        self.assertEqual(EXAMPLE['created_at'], sot.created_at)
-        self.assertEqual(EXAMPLE['id'], sot.id)
-        self.assertEqual(EXAMPLE['floating_ip_address'],
-                         sot.floating_ip_address)
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+
+from openstack.tests.unit import base
+
+from otcextensions.sdk.nat.v2 import snat
+
+
+INSTANCE_ID = '5b95c675-69c2-4656-ba06-58ff72e1d338'
+EXAMPLE = {
+    'floating_ip_id': 'bdc10a4c-d81a-41ec-adf7-de857f7c812a',
+    'status': 'PENDING_CREATE',
+    'nat_gateway_id': 'a78fb3eb-1654-4710-8742-3fc49d5f04f8',
+    'admin_state_up': True,
+    'network_id': 'eaad9cd6-2372-4be1-9535-9bd37210ae7b',
+    'cidr': None,
+    'source_type': 0,
+    'project_id': '27e25061336f4af590faeabeb7fcd9a3',
+    'created_at': '2017-11-18 07:54:21.665430',
+    'id': INSTANCE_ID,
+    'floating_ip_address': '5.21.11.226'
+}
+
+
+class TestSnat(base.TestCase):
+
+    def test_basic(self):
+        sot = snat.Snat()
+        self.assertEqual('snat_rule', sot.resource_key)
+        self.assertEqual('snat_rules', sot.resources_key)
+        path = '/snat_rules'
+        self.assertEqual(path, sot.base_path)
+        self.assertTrue(sot.allow_list)
+        self.assertTrue(sot.allow_create)
+        self.assertTrue(sot.allow_fetch)
+        self.assertFalse(sot.allow_commit)
+        self.assertTrue(sot.allow_delete)
+
+    def test_make_it(self):
+        sot = snat.Snat(**EXAMPLE)
+        self.assertEqual(EXAMPLE['floating_ip_id'], sot.floating_ip_id)
+        self.assertEqual(EXAMPLE['status'], sot.status)
+        self.assertEqual(EXAMPLE['nat_gateway_id'], sot.nat_gateway_id)
+        self.assertEqual(EXAMPLE['admin_state_up'], sot.admin_state_up)
+        self.assertEqual(EXAMPLE['network_id'], sot.network_id)
+        self.assertIsNone(sot.cidr)
+        self.assertEqual(EXAMPLE['source_type'], sot.source_type)
+        self.assertEqual(EXAMPLE['project_id'], sot.project_id)
+        self.assertEqual(EXAMPLE['created_at'], sot.created_at)
+        self.assertEqual(EXAMPLE['id'], sot.id)
+        self.assertEqual(EXAMPLE['floating_ip_address'],
+                         sot.floating_ip_address)
```

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/waf/v1/test_proxy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/waf/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/waf/v1/test_domain.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/waf/v1/test_domain.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/sdk/waf/v1/test_certificate.py` & `otcextensions-0.9.1/otcextensions/tests/unit/sdk/identity/v3/test_agency.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,61 +5,68 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
-import mock
-
-from keystoneauth1 import adapter
 
 from openstack.tests.unit import base
 
-from otcextensions.sdk.waf.v1 import certificate
+from otcextensions.sdk.identity.v3 import agency
 
 
-FAKE_ID = "68d5745e-6af2-40e4-945d-fe449be00148"
+FAKE_ID = "945d-fe449be00148"
 EXAMPLE = {
-    "id": FAKE_ID,
-    "name": "fake_name",
-    "content": "fake",
-    "key": "fake",
-    "timestamp": 1499817600,
-    "expire_time": 1499817600
+    "trust_domain_name": "exampledomain",
+    "description": " testsfdas ",
+    "trust_domain_id": "b3f266d0c08544a0859740de8b84e850",
+    "id": "afca8ddf2e92469a8fd26a635da5206f",
+    "duration": None,
+    "create_time": "2017-01-04T09:09:15.000000",
+    "expire_time": None,
+    "domain_id": "0ae9c6993a2e47bb8c4c7a9bb8278d61",
+    "name": "exampleagency"
 }
 
 
-class TestCertificate(base.TestCase):
+class TestAgency(base.TestCase):
 
     def setUp(self):
-        super(TestCertificate, self).setUp()
-        self.sess = mock.Mock(spec=adapter.Adapter)
-        self.sess.post = mock.Mock()
+        super(TestAgency, self).setUp()
 
     def test_basic(self):
-        sot = certificate.Certificate()
+        sot = agency.Agency()
 
-        self.assertEqual('/waf/certificate', sot.base_path)
-        self.assertEqual('items', sot.resources_key)
-        self.assertIsNone(sot.resource_key)
+        self.assertEqual('/v3.0/OS-AGENCY/agencies', sot.base_path)
+        self.assertEqual('agencies', sot.resources_key)
+        self.assertEqual('agency', sot.resource_key)
 
         self.assertTrue(sot.allow_list)
         self.assertTrue(sot.allow_fetch)
         self.assertTrue(sot.allow_create)
         self.assertTrue(sot.allow_delete)
         self.assertTrue(sot.allow_commit)
 
-    def test_make_it(self):
-
-        sot = certificate.Certificate(**EXAMPLE)
-        self.assertEqual(EXAMPLE['id'], sot.id)
-        self.assertEqual(EXAMPLE['name'], sot.name)
-        self.assertEqual(EXAMPLE['expire_time'], sot.expire_time)
-        self.assertEqual(EXAMPLE['timestamp'], sot.timestamp)
-
         self.assertDictEqual({
+            'domain_id': 'domain_id',
             'limit': 'limit',
             'marker': 'marker',
-            'offset': 'offset'},
+            'name': 'name',
+            'trust_domain_id': 'trust_domain_id'},
             sot._query_mapping._mapping
         )
+
+    def test_make_it(self):
+
+        sot = agency.Agency(connection=self.cloud, **EXAMPLE)
+        # Check how the override with "real" connection works
+        self.assertEqual(
+            'https://identity.example.com/v3.0/OS-AGENCY/agencies',
+            sot.base_path)
+
+        self.assertEqual(EXAMPLE['id'], sot.id)
+        self.assertEqual(EXAMPLE['description'], sot.description)
+        self.assertEqual(EXAMPLE['trust_domain_id'], sot.trust_domain_id)
+        self.assertEqual(EXAMPLE['create_time'], sot.created_at)
+        self.assertEqual(EXAMPLE['expire_time'], sot.expire_at)
+        self.assertEqual(EXAMPLE['domain_id'], sot.domain_id)
```

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/base.py` & `otcextensions-0.9.1/examples/deh/list_deh_hosts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
+#!/usr/bin/env python3
 # Licensed under the Apache License, Version 2.0 (the "License"); you may
 # not use this file except in compliance with the License. You may obtain
 # a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
-#
-
-from openstack.tests.unit import base
-
-from otcextensions import sdk
+"""
+List all allocated Dedicated hosts
+"""
+import openstack
 
 
-class TestCase(base.TestCase):
+openstack.enable_logging(True)
+conn = openstack.connect(cloud='otc')
 
-    def setUp(self):
-        super(TestCase, self).setUp()
-        sdk.load(self.cloud)
+for host in conn.deh.hosts():
+    print(host)
```

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/common/test_format.py` & `otcextensions-0.9.1/otcextensions/tests/unit/common/test_format.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dns/v2/test_recordset.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dns/v2/test_recordset.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dns/v2/test_zone.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dns/v2/test_zone.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dns/v2/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dns/v2/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dns/v2/test_ptr.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dns/v2/test_ptr.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/cts/v1/test_trace.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/cts/v1/test_trace.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/cts/v1/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/cts/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/cts/v1/test_tracker.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/cts/v1/test_tracker.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v1/test_configuration.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v1/test_configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v1/test_instance.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v1/test_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v1/test_datastore.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v1/test_datastore.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v1/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v1/test_backup.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v1/test_backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v1/test_flavor.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v1/test_flavor.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/test_configuration.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/test_configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/test_instance.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/test_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/test_datastore.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/test_datastore.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/test_backup.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/test_backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/rds/v3/test_flavor.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/rds/v3/test_flavor.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/test_health_monitor.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/test_health_monitor.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/test_load_balancer.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/test_load_balancer.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/test_pool.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/test_pool.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/test_listener.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/test_listener.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/test_pool_member.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/test_pool_member.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/load_balancer/v1/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/load_balancer/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v2/test_cluster.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v2/test_cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v2/test_cluster_node.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v2/test_cluster_node.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v2/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v2/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v1/test_cluster.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v1/test_cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v1/test_cluster_node.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v1/test_cluster_node.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/cce/v1/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/cce/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/test_restore.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/test_restore.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/test_instance.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/test_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/test_statistic.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/test_statistic.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/test_config.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/test_config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dcs/v1/test_backup.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dcs/v1/test_backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/obs/v1/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/obs/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/test_instance.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/test_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/test_policy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/test_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/test_activity.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/test_activity.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/test_config.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/test_config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/test_group.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/test_group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/auto_scaling/v1/test_quota.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/auto_scaling/v1/test_quota.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/test_base.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/test_base.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/volume_backup/v2/test_policy.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/volume_backup/v2/test_policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/volume_backup/v2/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/volume_backup/v2/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/kms/v1/test_cmk.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/kms/v1/test_cmk.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/kms/v1/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/kms/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/vpc/v2/test_peering.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/vpc/v2/test_peering.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/vpc/v2/test_route.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/vpc/v2/test_route.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/vpc/v2/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/vpc/v2/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/test_instance.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/test_instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/test_topic.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/test_topic.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/test_group.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/test_group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/test_queue.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/test_queue.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/dms/v1/test_quota.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/dms/v1/test_quota.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/anti_ddos/v1/test_status.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/anti_ddos/v1/test_status.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/anti_ddos/v1/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/anti_ddos/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/anti_ddos/v1/test_config.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/anti_ddos/v1/test_config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/anti_ddos/v1/test_floating_ip.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/anti_ddos/v1/test_floating_ip.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/deh/v1/test_host.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/deh/v1/test_host.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,29 +64,29 @@
     def test_default_query(self):
         arglist = [
             '--id', 'some_id',
             '--name', 'some_name',
             '--host_type', 'some_type',
             '--host_type_name', 'some_type_name',
             '--flavor', 'some_flavor',
-            '--state', 'available',
+            '--status', 'available',
             '--tenant', 'all',
             '--availability_zone', 'some_az',
             '--limit', '1',
             '--marker', 'some_marker',
             '--changes_since', '2200-01-01T00:00:00+00:00'
         ]
 
         verifylist = [
             ('id', 'some_id'),
             ('name', 'some_name'),
             ('host_type', 'some_type'),
             ('host_type_name', 'some_type_name'),
             ('flavor', 'some_flavor'),
-            ('state', 'available'),
+            ('status', 'available'),
             ('tenant', 'all'),
             ('availability_zone', 'some_az'),
             ('limit', 1),
             ('marker', 'some_marker'),
             ('changes_since', '2200-01-01T00:00:00+00:00')
         ]
 
@@ -107,30 +107,30 @@
             flavor='some_flavor',
             host_type='some_type',
             host_type_name='some_type_name',
             id='some_id',
             limit=1,
             marker='some_marker',
             name='some_name',
-            state='available',
+            status='available',
             tenant='all'
         )
 
         self.assertEqual(self.columns, columns)
         self.assertEqual(self.data, list(data))
 
 
 class TestShowHost(fakes.TestDeH):
 
     _data = fakes.FakeHost.create_one()
 
     columns = (
         'allocated_at', 'auto_placement', 'availability_zone',
         'available_memory', 'available_vcpus', 'host_properties', 'id',
-        'instance_total', 'name', 'project_id', 'released_at', 'state', 'tags'
+        'instance_total', 'name', 'project_id', 'released_at', 'status', 'tags'
     )
 
     data = fakes.gen_data(_data, columns)
 
     def setUp(self):
         super(TestShowHost, self).setUp()
 
@@ -264,15 +264,15 @@
 class TestSetHost(fakes.TestDeH):
 
     _fake = fakes.FakeHost.create_one()
 
     columns = (
         'allocated_at', 'auto_placement', 'availability_zone',
         'available_memory', 'available_vcpus', 'host_properties', 'id',
-        'instance_total', 'name', 'project_id', 'released_at', 'state', 'tags'
+        'instance_total', 'name', 'project_id', 'released_at', 'status', 'tags'
     )
 
     data = fakes.gen_data(_fake, columns)
 
     def setUp(self):
         super(TestSetHost, self).setUp()
 
@@ -412,15 +412,15 @@
 class TestUnsetHost(fakes.TestDeH):
 
     _fake = fakes.FakeHost.create_one()
 
     columns = (
         'allocated_at', 'auto_placement', 'availability_zone',
         'available_memory', 'available_vcpus', 'host_properties', 'id',
-        'instance_total', 'name', 'project_id', 'released_at', 'state', 'tags'
+        'instance_total', 'name', 'project_id', 'released_at', 'status', 'tags'
     )
 
     data = fakes.gen_data(_fake, columns)
 
     def setUp(self):
         super(TestUnsetHost, self).setUp()
```

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/deh/v1/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/deh/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/nat/v2/test_dnat.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/nat/v2/test_dnat.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/nat/v2/test_gateway.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/nat/v2/test_gateway.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/nat/v2/test_snat.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/nat/v2/test_snat.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/tests/unit/osclient/nat/v2/fakes.py` & `otcextensions-0.9.1/otcextensions/tests/unit/osclient/nat/v2/fakes.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dns/v2/ptr.py` & `otcextensions-0.9.1/otcextensions/osclient/dns/v2/ptr.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dns/v2/zone.py` & `otcextensions-0.9.1/otcextensions/osclient/dns/v2/zone.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dns/v2/recordset.py` & `otcextensions-0.9.1/otcextensions/osclient/dns/v2/recordset.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dns/client.py` & `otcextensions-0.9.1/otcextensions/osclient/dns/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/cts/client.py` & `otcextensions-0.9.1/otcextensions/osclient/cts/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/cts/v1/tracker.py` & `otcextensions-0.9.1/otcextensions/osclient/cts/v1/tracker.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/cts/v1/trace.py` & `otcextensions-0.9.1/otcextensions/osclient/cts/v1/trace.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/rds/client.py` & `otcextensions-0.9.1/otcextensions/osclient/rds/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/rds/v1/flavor.py` & `otcextensions-0.9.1/otcextensions/osclient/rds/v1/flavor.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/rds/v1/configuration.py` & `otcextensions-0.9.1/otcextensions/osclient/rds/v1/configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/rds/v1/datastore.py` & `otcextensions-0.9.1/otcextensions/osclient/rds/v1/datastore.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/rds/v1/backup.py` & `otcextensions-0.9.1/otcextensions/osclient/rds/v1/backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/rds/v1/instance.py` & `otcextensions-0.9.1/otcextensions/osclient/rds/v1/instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/rds/v3/flavor.py` & `otcextensions-0.9.1/otcextensions/osclient/rds/v3/flavor.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/rds/v3/configuration.py` & `otcextensions-0.9.1/otcextensions/osclient/rds/v3/configuration.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/rds/v3/datastore.py` & `otcextensions-0.9.1/otcextensions/osclient/rds/v3/datastore.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/rds/v3/backup.py` & `otcextensions-0.9.1/otcextensions/osclient/rds/v3/backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/rds/v3/instance.py` & `otcextensions-0.9.1/otcextensions/osclient/rds/v3/instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/load_balancer/client.py` & `otcextensions-0.9.1/otcextensions/osclient/load_balancer/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/load_balancer/v1/load_balancer.py` & `otcextensions-0.9.1/otcextensions/osclient/load_balancer/v1/load_balancer.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/load_balancer/v1/health_monitor.py` & `otcextensions-0.9.1/otcextensions/osclient/load_balancer/v1/health_monitor.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/load_balancer/v1/pool.py` & `otcextensions-0.9.1/otcextensions/osclient/load_balancer/v1/pool.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/load_balancer/v1/pool_member.py` & `otcextensions-0.9.1/otcextensions/osclient/load_balancer/v1/pool_member.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/load_balancer/v1/listener.py` & `otcextensions-0.9.1/otcextensions/osclient/load_balancer/v1/listener.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/compute/v2/server.py` & `otcextensions-0.9.1/otcextensions/osclient/compute/v2/server.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/cce/v2/cluster.py` & `otcextensions-0.9.1/otcextensions/osclient/cce/v2/cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/cce/v2/cluster_node.py` & `otcextensions-0.9.1/otcextensions/osclient/cce/v2/cluster_node.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/cce/client.py` & `otcextensions-0.9.1/otcextensions/osclient/cce/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/cce/v1/cluster.py` & `otcextensions-0.9.1/otcextensions/osclient/cce/v1/cluster.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/cce/v1/cluster_node.py` & `otcextensions-0.9.1/otcextensions/osclient/cce/v1/cluster_node.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dcs/client.py` & `otcextensions-0.9.1/otcextensions/osclient/dcs/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dcs/v1/restore.py` & `otcextensions-0.9.1/otcextensions/osclient/dcs/v1/restore.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dcs/v1/statistic.py` & `otcextensions-0.9.1/otcextensions/osclient/dcs/v1/statistic.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dcs/v1/config.py` & `otcextensions-0.9.1/otcextensions/osclient/dcs/v1/config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dcs/v1/backup.py` & `otcextensions-0.9.1/otcextensions/osclient/dcs/v1/backup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dcs/v1/instance.py` & `otcextensions-0.9.1/otcextensions/osclient/dcs/v1/instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/obs/client.py` & `otcextensions-0.9.1/otcextensions/osclient/obs/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/obs/v1/utils.py` & `otcextensions-0.9.1/otcextensions/osclient/obs/v1/utils.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/obs/v1/container.py` & `otcextensions-0.9.1/otcextensions/osclient/obs/v1/container.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/obs/v1/object.py` & `otcextensions-0.9.1/otcextensions/osclient/obs/v1/object.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/auto_scaling/client.py` & `otcextensions-0.9.1/otcextensions/osclient/auto_scaling/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/activity.py` & `otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/activity.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/quota.py` & `otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/quota.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/config.py` & `otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/group.py` & `otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/policy.py` & `otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/auto_scaling/v1/instance.py` & `otcextensions-0.9.1/otcextensions/osclient/auto_scaling/v1/instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/volume_backup/v2/policy.py` & `otcextensions-0.9.1/otcextensions/osclient/volume_backup/v2/policy.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/volume_backup/client.py` & `otcextensions-0.9.1/otcextensions/osclient/volume_backup/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/kms/client.py` & `otcextensions-0.9.1/otcextensions/osclient/kms/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/kms/v1/cmk.py` & `otcextensions-0.9.1/otcextensions/osclient/kms/v1/cmk.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/vpc/v2/route.py` & `otcextensions-0.9.1/otcextensions/osclient/vpc/v2/route.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/vpc/v2/peering.py` & `otcextensions-0.9.1/otcextensions/osclient/vpc/v2/peering.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/vpc/client.py` & `otcextensions-0.9.1/otcextensions/osclient/vpc/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dms/client.py` & `otcextensions-0.9.1/otcextensions/osclient/dms/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dms/v1/queue.py` & `otcextensions-0.9.1/otcextensions/osclient/dms/v1/queue.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dms/v1/topic.py` & `otcextensions-0.9.1/otcextensions/osclient/dms/v1/topic.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dms/v1/quota.py` & `otcextensions-0.9.1/otcextensions/osclient/dms/v1/quota.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dms/v1/product.py` & `otcextensions-0.9.1/otcextensions/osclient/dms/v1/product.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dms/v1/maintenance_window.py` & `otcextensions-0.9.1/otcextensions/osclient/dms/v1/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dms/v1/group.py` & `otcextensions-0.9.1/otcextensions/osclient/dms/v1/group.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dms/v1/az.py` & `otcextensions-0.9.1/otcextensions/osclient/dms/v1/az.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/dms/v1/instance.py` & `otcextensions-0.9.1/otcextensions/osclient/dms/v1/instance.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/anti_ddos/client.py` & `otcextensions-0.9.1/otcextensions/osclient/anti_ddos/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/anti_ddos/v1/status.py` & `otcextensions-0.9.1/otcextensions/osclient/anti_ddos/v1/status.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/anti_ddos/v1/floating_ip.py` & `otcextensions-0.9.1/otcextensions/osclient/anti_ddos/v1/floating_ip.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/anti_ddos/v1/config.py` & `otcextensions-0.9.1/otcextensions/osclient/anti_ddos/v1/config.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/deh/client.py` & `otcextensions-0.9.1/otcextensions/osclient/deh/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/deh/v1/host.py` & `otcextensions-0.9.1/otcextensions/osclient/deh/v1/host.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,19 +87,19 @@
         )
         parser.add_argument(
             '--flavor',
             metavar='<flavor>',
             help=_('Flavor ID.')
         )
         parser.add_argument(
-            '--state',
+            '--status',
             metavar='{' + ','.join(HOST_STATES) + '}',
             type=lambda s: s.lower(),
             choices=HOST_STATES,
-            help=_('Host state filter.')
+            help=_('Host status filter.')
         )
         parser.add_argument(
             '--tenant',
             metavar='<tenant>',
             help=_('Tenant ID or "all".')
         )
         parser.add_argument(
@@ -138,16 +138,16 @@
             query['name'] = parsed_args.name
         if parsed_args.host_type:
             query['host_type'] = parsed_args.host_type
         if parsed_args.host_type_name:
             query['host_type_name'] = parsed_args.host_type_name
         if parsed_args.flavor:
             query['flavor'] = parsed_args.flavor
-        if parsed_args.state:
-            query['state'] = parsed_args.state
+        if parsed_args.status:
+            query['status'] = parsed_args.status
         if parsed_args.tenant:
             query['tenant'] = parsed_args.tenant
         if parsed_args.availability_zone:
             query['availability_zone'] = parsed_args.availability_zone
         if parsed_args.limit:
             query['limit'] = parsed_args.limit
         if parsed_args.marker:
```

### Comparing `otcextensions-0.9.0/otcextensions/osclient/nat/v2/snat.py` & `otcextensions-0.9.1/otcextensions/osclient/nat/v2/snat.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/nat/v2/gateway.py` & `otcextensions-0.9.1/otcextensions/osclient/nat/v2/gateway.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/nat/v2/dnat.py` & `otcextensions-0.9.1/otcextensions/osclient/nat/v2/dnat.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions/osclient/nat/client.py` & `otcextensions-0.9.1/otcextensions/osclient/nat/client.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/CONTRIBUTING.rst` & `otcextensions-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/openstack/tests/unit/fixtures/catalog-v3.json` & `otcextensions-0.9.1/openstack/tests/unit/fixtures/catalog-v3.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/openstack/tests/unit/fixtures/catalog-v3-suburl.json` & `otcextensions-0.9.1/openstack/tests/unit/fixtures/catalog-v3-suburl.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/openstack/tests/unit/fixtures/image-version-v2.json` & `otcextensions-0.9.1/openstack/tests/unit/fixtures/image-version-v2.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/openstack/tests/unit/fixtures/image-version-suburl.json` & `otcextensions-0.9.1/openstack/tests/unit/fixtures/image-version-suburl.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/openstack/tests/unit/fixtures/clouds/clouds_cache.yaml` & `otcextensions-0.9.1/openstack/tests/unit/fixtures/clouds/clouds_cache.yaml`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/openstack/tests/unit/fixtures/clouds/clouds.yaml` & `otcextensions-0.9.1/openstack/tests/unit/fixtures/clouds/clouds.yaml`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/openstack/tests/unit/fixtures/image-version.json` & `otcextensions-0.9.1/openstack/tests/unit/fixtures/image-version.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/openstack/tests/unit/fixtures/dns.json` & `otcextensions-0.9.1/openstack/tests/unit/fixtures/dns.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/openstack/tests/unit/fixtures/discovery.json` & `otcextensions-0.9.1/openstack/tests/unit/fixtures/discovery.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/openstack/tests/unit/fixtures/baremetal.json` & `otcextensions-0.9.1/openstack/tests/unit/fixtures/baremetal.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/openstack/tests/unit/fixtures/image-version-broken.json` & `otcextensions-0.9.1/openstack/tests/unit/fixtures/image-version-broken.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/openstack/tests/unit/fixtures/catalog-v2.json` & `otcextensions-0.9.1/openstack/tests/unit/fixtures/catalog-v2.json`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/PKG-INFO` & `otcextensions-0.9.1/otcextensions.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: otcextensions
-Version: 0.9.0
+Version: 0.9.1
 Summary: Open Telekom Cloud specific extensions for the OpenStack Client CLI and OpenStack SDK
 Home-page: http://python-otcextensions.readthedocs.io/
 Author: Artem Goncharov
 Author-email: artem.goncharov@gmail.com
 License: UNKNOWN
 Description: OTC Extensions
         ==============
@@ -25,35 +25,39 @@
         * `python-openstackclient`
         
         packages.
         
         Documentation
         -------------
         
-        * `Documentation <http://python-otcextensions.readthedocs.io/en/latest/>`
+        `Documentation Overview <http://python-otcextensions.readthedocs.io/en/latest/>`_
         
         Installation
         ------------
         
+        `Installation Page <https://python-otcextensions.readthedocs.io/en/latest/install/index.html>`_
+        
         The OTC Extensions are hosted as the package `otcextensions` on PyPI
         and can be installed by pip as
         
         .. code-block: console
+        
            $ pip install otcextensions
         
         There are several options
         to do that including but not limited to pip userland installation, system wide
         installation as well as installation from operating system packets or directly
         from source. Refer to the installation instructions_ in the projects
         documentation.
         
-        
         Configuration
         -------------
         
+        `Configuration Page <https://python-otcextensions.readthedocs.io/en/latest/install/configuration.html>`_
+        
         Acessing the Open Telekom Cloud APIs requires authentication and
         authorization. For both there are several options available:
         
         * **Configuration files** (recommended): A file called `clouds.yaml`
           holds all necessary configuration parameters. The file can be placed
           either in the local directory, below the user home directory in
           `.config/openstack` or in the system-wide directory
@@ -62,46 +66,47 @@
           credentials. For more details see the section `configuration`_ in
           the official documentation.
         
           Minimal sample ``clouds.yaml`` file:
         
           .. code-block:: yaml
         
-              clouds:
-                  otc:
-                  profile: otc
-                      auth:
-                          username: "*username*"
-                          password: "*password*"
-                          project_name: "eu-de"
-                          auth_url: "https://iam.eu-de.otc.t-systems.com:443/v3"
-                          user_domain_name: "*OTC00000000001000000xxx*"
-                     interface: "public"
-                     identity_api_version: 3
-                     ak: "*40 digit access key*"
-                     sk: "*20 digit secure key*"
+            clouds:
+              otc:
+                profile: otc
+                auth:
+                  username: '<USER_NAME>'
+                  password: '<PASSWORD>'
+                  project_name: '<eu-de_project>'
+                  # or project_id: '<123456_PROJECT_ID>'
+                  user_domain_name: 'OTC00000000001000000xxx'
+                  # or user_domain_id: '<123456_DOMAIN_ID>'
+                  auth_url: 'https://iam.eu-de.otc.t-systems.com:443/v3'
+                interface: 'public'
+                identity_api_version: 3 # !Important
+                ak: '<AK_VALUE>' # AK/SK pair for access to OBS
+                sk: '<SK_VALUE>'
         
           With this configuration you can start using the CLI with ``openstack
           --os-cloud otc *command*`` or by ``export OS_CLOUD=otc; openstack
           *command*``.
         
         * **Environment variables:** Authentication using username/password is often
-          used:
+          used::
         
             export OS_AUTH_URL=<url-to-openstack-identity>
             export OS_IDENTITY_API_VERSION=3
             export OS_PROJECT_NAME=<project-name>
             export OS_PROJECT_DOMAIN_NAME=<project-domain-name>
             export OS_USERNAME=<username>
             export OS_USER_DOMAIN_NAME=<user-domain-name>
             export OS_PASSWORD=<password>  # (optional)
             export S3_ACCESS_KEY_ID=<access_key>
             export S3_SECRET_ACCESS_KEY=<secret_access_key>
         
-        
         * **Command-Line Options:** The corresponding command-line options look
           very similar::
         
             --os-auth-url <url>
             --os-identity-api-version 3
             --os-project-name <project-name>
             --os-project-domain-name <project-domain-name>
@@ -115,36 +120,40 @@
         * **Existing Token:** Authentication may also be performed using an
           already-acquired token and a URL pointing directly to the service
           API that presumably was acquired from the Service Catalog::
         
             export OS_TOKEN=<token>
             export OS_URL=<url-to-openstack-service>
         
-        The corresponding command-line options look very similar::
+        * The corresponding command-line options look very similar::
         
             --os-token <token>
             --os-url <url-to-openstack-service>
         
         In addition to that a regular `clouds.yaml` configuration file can be used
         
         More information is available at
         https://docs.openstack.org/python-openstackclient/latest/cli/authentication.html
         or
         https://developer.openstack.org/sdks/python/openstacksdk/users/config
         
+        OTC Extensions CLI Usage
+        ------------------------
+        
+        `OTCE CLI Command Overview <https://python-otcextensions.readthedocs.io/en/latest/cli/index.html>`_
         
-        Writing Own Code
-        ----------------
+        OTC Extensions SDK Guides
+        -------------------------
         
-        XXX Example XXXX
+        `OTCE SDK Guides <https://python-otcextensions.readthedocs.io/en/latest/sdk/guides/index.html>`_
         
         Contributing
         ------------
         
-        See CONTRIBUTING.rst
+        * `Contribution Page <https://python-otcextensions.readthedocs.io/en/latest/contributor/index.html>`_
         
         Further Links
         -------------
         
         * `Issue Tracker <https://github.com/OpenTelekomCloud/python-otcextensions/issues>`_
         
         .. _instructions: http://python-otcextensions.readthedocs.io/en/latest/install/
```

### Comparing `otcextensions-0.9.0/setup.cfg` & `otcextensions-0.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -22,20 +22,23 @@
 	OpenStack, openstackclient, openstacksdk, Open Telekom Cloud, otc, T-Systems, Telekom
 
 [files]
 packages = 
 	otcextensions
 
 [entry_points]
+keystoneauth1.plugin = 
+	agency = otcextensions.common.agency_auth:AgencyLoader
 openstack.cli.extension = 
 	obs = otcextensions.osclient.obs.client
 	rds = otcextensions.osclient.rds.client
 	auto_scaling = otcextensions.osclient.auto_scaling.client
 	kms = otcextensions.osclient.kms.client
 	cce = otcextensions.osclient.cce.client
+	ces = otcextensions.osclient.ces.client
 	load_balancer = otcextensions.osclient.load_balancer.client
 	volume_backup = otcextensions.osclient.volume_backup.client
 	dms = otcextensions.osclient.dms.client
 	dcs = otcextensions.osclient.dcs.client
 	cts = otcextensions.osclient.cts.client
 	anti_ddos = otcextensions.osclient.anti_ddos.client
 	dns = otcextensions.osclient.dns.client
@@ -190,14 +193,23 @@
 	cce_cluster_show = otcextensions.osclient.cce.v2.cluster:ShowCCECluster
 	cce_cluster_create = otcextensions.osclient.cce.v2.cluster:CreateCCECluster
 	cce_cluster_delete = otcextensions.osclient.cce.v2.cluster:DeleteCCECluster
 	cce_cluster_node_list = otcextensions.osclient.cce.v2.cluster_node:ListCCEClusterNode
 	cce_cluster_node_show = otcextensions.osclient.cce.v2.cluster_node:ShowCCEClusterNode
 	cce_cluster_node_create = otcextensions.osclient.cce.v2.cluster_node:CreateCCEClusterNode
 	cce_cluster_node_delete = otcextensions.osclient.cce.v2.cluster_node:DeleteCCEClusterNode
+openstack.ces.v1 = 
+	ces_alarm_list = otcextensions.osclient.ces.v1.alarm:ListAlarms
+	ces_alarm_show = otcextensions.osclient.ces.v1.alarm:ShowAlarm
+	ces_alarm_create = otcextensions.osclient.ces.v1.alarm:CreateAlarm
+	ces_alarm_switch_state = otcextensions.osclient.ces.v1.alarm:SetAlarm
+	ces_alarm_delete = otcextensions.osclient.ces.v1.alarm:DeleteAlarm
+	ces_metric_list = otcextensions.osclient.ces.v1.metric:ListMetrics
+	ces_quota_list = otcextensions.osclient.ces.v1.quota:ListQuotas
+	ces_event_data_list = otcextensions.osclient.ces.v1.event_data:ListEventData
 openstack.load_balancer.v1 = 
 	loadbalancer_list = otcextensions.osclient.load_balancer.v1.load_balancer:ListLoadBalancer
 	loadbalancer_show = otcextensions.osclient.load_balancer.v1.load_balancer:ShowLoadBalancer
 	loadbalancer_create = otcextensions.osclient.load_balancer.v1.load_balancer:CreateLoadBalancer
 	loadbalancer_set = otcextensions.osclient.load_balancer.v1.load_balancer:SetLoadBalancer
 	loadbalancer_delete = otcextensions.osclient.load_balancer.v1.load_balancer:DeleteLoadBalancer
 	loadbalancer_listener_list = otcextensions.osclient.load_balancer.v1.listener:ListListener
```

### Comparing `otcextensions-0.9.0/setup.py` & `otcextensions-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/test-requirements.txt` & `otcextensions-0.9.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/AUTHORS` & `otcextensions-0.9.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `otcextensions-0.9.0/otcextensions.egg-info/SOURCES.txt` & `otcextensions-0.9.1/otcextensions.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,21 @@
 doc/source/appendices/history.rst
 doc/source/appendices/index.rst
 doc/source/appendices/issues.rst
 doc/source/appendices/releasenotes.rst
 doc/source/cli/anti_ddos.rst
 doc/source/cli/auto_scaling.rst
 doc/source/cli/cce_v2.rst
+doc/source/cli/ces.rst
 doc/source/cli/cts.rst
 doc/source/cli/dcs.rst
 doc/source/cli/deh.rst
 doc/source/cli/dms.rst
 doc/source/cli/dns.rst
+doc/source/cli/identity.rst
 doc/source/cli/index.rst
 doc/source/cli/kms.rst
 doc/source/cli/load_balancer.rst
 doc/source/cli/nat.rst
 doc/source/cli/obs.rst
 doc/source/cli/rds_v3.rst
 doc/source/cli/volume_backup.rst
@@ -61,33 +63,36 @@
 doc/source/sdk/architecture.rst
 doc/source/sdk/examples
 doc/source/sdk/getting_started.rst
 doc/source/sdk/index.rst
 doc/source/sdk/guides/anti_ddos.rst
 doc/source/sdk/guides/auto_scaling.rst
 doc/source/sdk/guides/cce.rst
+doc/source/sdk/guides/ces.rst
 doc/source/sdk/guides/cts.rst
 doc/source/sdk/guides/dcs.rst
 doc/source/sdk/guides/deh.rst
 doc/source/sdk/guides/dns.rst
 doc/source/sdk/guides/index.rst
 doc/source/sdk/guides/kms.rst
 doc/source/sdk/guides/logging.rst
 doc/source/sdk/guides/nat.rst
 doc/source/sdk/guides/rds.rst
 doc/source/sdk/guides/vpc.rst
 doc/source/sdk/proxies/anti_ddos.rst
 doc/source/sdk/proxies/auto_scaling.rst
 doc/source/sdk/proxies/cce_v1.rst
 doc/source/sdk/proxies/cce_v3.rst
+doc/source/sdk/proxies/ces.rst
 doc/source/sdk/proxies/cts.rst
 doc/source/sdk/proxies/dcs.rst
 doc/source/sdk/proxies/deh.rst
 doc/source/sdk/proxies/dms.rst
 doc/source/sdk/proxies/dns.rst
+doc/source/sdk/proxies/identity_v3.rst
 doc/source/sdk/proxies/index.rst
 doc/source/sdk/proxies/kms.rst
 doc/source/sdk/proxies/nat.rst
 doc/source/sdk/proxies/obs.rst
 doc/source/sdk/proxies/rds_v1.rst
 doc/source/sdk/proxies/rds_v3.rst
 doc/source/sdk/proxies/volume_backup.rst
@@ -106,14 +111,20 @@
 doc/source/sdk/resources/auto_scaling/v1/policy.rst
 doc/source/sdk/resources/auto_scaling/v1/quota.rst
 doc/source/sdk/resources/cce/index.rst
 doc/source/sdk/resources/cce/v1/cluster.rst
 doc/source/sdk/resources/cce/v1/cluster_node.rst
 doc/source/sdk/resources/cce/v3/cluster.rst
 doc/source/sdk/resources/cce/v3/cluster_node.rst
+doc/source/sdk/resources/ces/index.rst
+doc/source/sdk/resources/ces/v1/alarm.rst
+doc/source/sdk/resources/ces/v1/event_data.rst
+doc/source/sdk/resources/ces/v1/metric.rst
+doc/source/sdk/resources/ces/v1/metric_data.rst
+doc/source/sdk/resources/ces/v1/quota.rst
 doc/source/sdk/resources/cts/index.rst
 doc/source/sdk/resources/cts/v1/trace.rst
 doc/source/sdk/resources/cts/v1/tracker.rst
 doc/source/sdk/resources/dcs/index.rst
 doc/source/sdk/resources/dcs/v1/backup.rst
 doc/source/sdk/resources/dcs/v1/config.rst
 doc/source/sdk/resources/dcs/v1/instance.rst
@@ -132,14 +143,25 @@
 doc/source/sdk/resources/dms/v1/queue.rst
 doc/source/sdk/resources/dms/v1/topic.rst
 doc/source/sdk/resources/dns/index.rst
 doc/source/sdk/resources/dns/v2/floating_ip.rst
 doc/source/sdk/resources/dns/v2/nameserver.rst
 doc/source/sdk/resources/dns/v2/recordset.rst
 doc/source/sdk/resources/dns/v2/zone.rst
+doc/source/sdk/resources/identity/index.rst
+doc/source/sdk/resources/identity/v3/agency.rst
+doc/source/sdk/resources/identity/v3/agency_role.rst
+doc/source/sdk/resources/identity/v3/credential.rst
+doc/source/sdk/resources/identity/v3/domain.rst
+doc/source/sdk/resources/identity/v3/endpoint.rst
+doc/source/sdk/resources/identity/v3/group.rst
+doc/source/sdk/resources/identity/v3/policy.rst
+doc/source/sdk/resources/identity/v3/project.rst
+doc/source/sdk/resources/identity/v3/service.rst
+doc/source/sdk/resources/identity/v3/user.rst
 doc/source/sdk/resources/kms/index.rst
 doc/source/sdk/resources/kms/v1/data_key.rst
 doc/source/sdk/resources/kms/v1/key.rst
 doc/source/sdk/resources/nat/index.rst
 doc/source/sdk/resources/nat/v2/dnat.rst
 doc/source/sdk/resources/nat/v2/gateway.rst
 doc/source/sdk/resources/nat/v2/snat.rst
@@ -210,14 +232,25 @@
 examples/cce/find_cluster_node.py
 examples/cce/get_cluster.py
 examples/cce/get_cluster_node.py
 examples/cce/get_job.py
 examples/cce/list_cluster_nodes.py
 examples/cce/list_clusters.py
 examples/cce/wait_for_job.py
+examples/ces/create_alarm.py
+examples/ces/create_metric_data.py
+examples/ces/delete_alarm.py
+examples/ces/find_alarm.py
+examples/ces/get_alarm.py
+examples/ces/list_alarms.py
+examples/ces/list_event_data.py
+examples/ces/list_metric_data.py
+examples/ces/list_metrics.py
+examples/ces/list_quotas.py
+examples/ces/switch_alarm_state.py
 examples/cloud/cleanup-servers.py
 examples/cloud/create-server-dict.py
 examples/cloud/create-server-name-or-id.py
 examples/cloud/debug-logging.py
 examples/cloud/find-an-image.py
 examples/cloud/http-debug-logging.py
 examples/cloud/munch-dict-object.py
@@ -267,14 +300,16 @@
 examples/dcs/start_instance.py
 examples/dcs/stop_instance.py
 examples/dcs/update_instance.py
 examples/dcs/update_instance_params.py
 examples/deh/__init__.py
 examples/deh/create.py
 examples/deh/list.py
+examples/deh/list_deh_hosts.py
+examples/deh/list_deh_servers.py
 examples/deh/list_servers.py
 examples/deh/list_types.py
 examples/dns/add_router_to_zone.py
 examples/dns/create_recordset.py
 examples/dns/create_zone.py
 examples/dns/delete_recordset.py
 examples/dns/delete_zone.py
@@ -290,15 +325,21 @@
 examples/dns/remove_router_from_zone.py
 examples/dns/set_floating_ip.py
 examples/dns/unset_floating_ip.py
 examples/dns/update_floating_ip.py
 examples/dns/update_recordset.py
 examples/dns/update_zone.py
 examples/identity/__init__.py
+examples/identity/create_credential.py
+examples/identity/delete_credential.py
+examples/identity/find_credential.py
+examples/identity/get_credential.py
 examples/identity/list.py
+examples/identity/list_credentials.py
+examples/identity/update_credential.py
 examples/image/__init__.py
 examples/image/create.py
 examples/image/delete.py
 examples/image/download.py
 examples/image/list.py
 examples/key_manager/__init__.py
 examples/key_manager/create.py
@@ -394,14 +435,15 @@
 otcextensions.egg-info/dependency_links.txt
 otcextensions.egg-info/entry_points.txt
 otcextensions.egg-info/not-zip-safe
 otcextensions.egg-info/pbr.json
 otcextensions.egg-info/requires.txt
 otcextensions.egg-info/top_level.txt
 otcextensions/common/__init__.py
+otcextensions/common/agency_auth.py
 otcextensions/common/errors.py
 otcextensions/common/exc.py
 otcextensions/common/format.py
 otcextensions/common/sdk_utils.py
 otcextensions/common/utils.py
 otcextensions/osclient/__init__.py
 otcextensions/osclient/anti_ddos/__init__.py
@@ -423,14 +465,22 @@
 otcextensions/osclient/cce/client.py
 otcextensions/osclient/cce/v1/__init__.py
 otcextensions/osclient/cce/v1/cluster.py
 otcextensions/osclient/cce/v1/cluster_node.py
 otcextensions/osclient/cce/v2/__init__.py
 otcextensions/osclient/cce/v2/cluster.py
 otcextensions/osclient/cce/v2/cluster_node.py
+otcextensions/osclient/ces/__init__.py
+otcextensions/osclient/ces/client.py
+otcextensions/osclient/ces/v1/__init__.py
+otcextensions/osclient/ces/v1/alarm.py
+otcextensions/osclient/ces/v1/event_data.py
+otcextensions/osclient/ces/v1/metric.py
+otcextensions/osclient/ces/v1/metric_data.py
+otcextensions/osclient/ces/v1/quota.py
 otcextensions/osclient/compute/__init__.py
 otcextensions/osclient/compute/v2/__init__.py
 otcextensions/osclient/compute/v2/server.py
 otcextensions/osclient/cts/__init__.py
 otcextensions/osclient/cts/client.py
 otcextensions/osclient/cts/v1/__init__.py
 otcextensions/osclient/cts/v1/trace.py
@@ -460,14 +510,18 @@
 otcextensions/osclient/dms/v1/topic.py
 otcextensions/osclient/dns/__init__.py
 otcextensions/osclient/dns/client.py
 otcextensions/osclient/dns/v2/__init__.py
 otcextensions/osclient/dns/v2/ptr.py
 otcextensions/osclient/dns/v2/recordset.py
 otcextensions/osclient/dns/v2/zone.py
+otcextensions/osclient/identity/__init__.py
+otcextensions/osclient/identity/client.py
+otcextensions/osclient/identity/v3/__init__.py
+otcextensions/osclient/identity/v3/credential.py
 otcextensions/osclient/kms/__init__.py
 otcextensions/osclient/kms/client.py
 otcextensions/osclient/kms/v1/__init__.py
 otcextensions/osclient/kms/v1/cmk.py
 otcextensions/osclient/load_balancer/__init__.py
 otcextensions/osclient/load_balancer/client.py
 otcextensions/osclient/load_balancer/v1/__init__.py
@@ -549,14 +603,19 @@
 otcextensions/sdk/cce/v3/cluster_cert.py
 otcextensions/sdk/cce/v3/cluster_node.py
 otcextensions/sdk/cce/v3/job.py
 otcextensions/sdk/ces/__init__.py
 otcextensions/sdk/ces/ces_service.py
 otcextensions/sdk/ces/v1/__init__.py
 otcextensions/sdk/ces/v1/_proxy.py
+otcextensions/sdk/ces/v1/alarm.py
+otcextensions/sdk/ces/v1/event_data.py
+otcextensions/sdk/ces/v1/metric.py
+otcextensions/sdk/ces/v1/metric_data.py
+otcextensions/sdk/ces/v1/quota.py
 otcextensions/sdk/cloud/__init__.py
 otcextensions/sdk/cloud/rds.py
 otcextensions/sdk/compute/__init__.py
 otcextensions/sdk/compute/v2/__init__.py
 otcextensions/sdk/compute/v2/_proxy.py
 otcextensions/sdk/compute/v2/server.py
 otcextensions/sdk/css/__init__.py
@@ -627,14 +686,22 @@
 otcextensions/sdk/dws/dws_service.py
 otcextensions/sdk/dws/v1/__init__.py
 otcextensions/sdk/dws/v1/_proxy.py
 otcextensions/sdk/ecs/__init__.py
 otcextensions/sdk/ecs/ecs_service.py
 otcextensions/sdk/ecs/v1/__init__.py
 otcextensions/sdk/ecs/v1/_proxy.py
+otcextensions/sdk/identity/__init__.py
+otcextensions/sdk/identity/identity_service.py
+otcextensions/sdk/identity/v3/__init__.py
+otcextensions/sdk/identity/v3/_bad_base.py
+otcextensions/sdk/identity/v3/_proxy.py
+otcextensions/sdk/identity/v3/agency.py
+otcextensions/sdk/identity/v3/agency_role.py
+otcextensions/sdk/identity/v3/credential.py
 otcextensions/sdk/kms/__init__.py
 otcextensions/sdk/kms/kms_service.py
 otcextensions/sdk/kms/v1/__init__.py
 otcextensions/sdk/kms/v1/_base.py
 otcextensions/sdk/kms/v1/_proxy.py
 otcextensions/sdk/kms/v1/data_key.py
 otcextensions/sdk/kms/v1/key.py
@@ -682,14 +749,15 @@
 otcextensions/sdk/rds/v3/datastore.py
 otcextensions/sdk/rds/v3/flavor.py
 otcextensions/sdk/rds/v3/instance.py
 otcextensions/sdk/sdrs/__init__.py
 otcextensions/sdk/sdrs/sdrs_service.py
 otcextensions/sdk/sdrs/v1/__init__.py
 otcextensions/sdk/sdrs/v1/_proxy.py
+otcextensions/sdk/smn/__init_.py
 otcextensions/sdk/smn/__init__.py
 otcextensions/sdk/smn/smn_service.py
 otcextensions/sdk/smn/v2/__init__.py
 otcextensions/sdk/smn/v2/_proxy.py
 otcextensions/sdk/volume_backup/__init__.py
 otcextensions/sdk/volume_backup/volume_backup_service.py
 otcextensions/sdk/volume_backup/v2/__init__.py
@@ -836,14 +904,15 @@
 otcextensions/tests/functional/sdk/waf/v1/__init__.py
 otcextensions/tests/functional/sdk/waf/v1/test_certificate.py
 otcextensions/tests/functional/sdk/waf/v1/test_domain.py
 otcextensions/tests/functional/sdk/waf/v1/test_service.py
 otcextensions/tests/unit/__init__.py
 otcextensions/tests/unit/base.py
 otcextensions/tests/unit/common/__init__.py
+otcextensions/tests/unit/common/test_agency_auth.py
 otcextensions/tests/unit/common/test_format.py
 otcextensions/tests/unit/osclient/__init__.py
 otcextensions/tests/unit/osclient/test_base.py
 otcextensions/tests/unit/osclient/anti_ddos/__init__.py
 otcextensions/tests/unit/osclient/anti_ddos/v1/__init__.py
 otcextensions/tests/unit/osclient/anti_ddos/v1/fakes.py
 otcextensions/tests/unit/osclient/anti_ddos/v1/test_config.py
@@ -894,14 +963,18 @@
 otcextensions/tests/unit/osclient/dms/v1/test_topic.py
 otcextensions/tests/unit/osclient/dns/__init__.py
 otcextensions/tests/unit/osclient/dns/v2/__init__.py
 otcextensions/tests/unit/osclient/dns/v2/fakes.py
 otcextensions/tests/unit/osclient/dns/v2/test_ptr.py
 otcextensions/tests/unit/osclient/dns/v2/test_recordset.py
 otcextensions/tests/unit/osclient/dns/v2/test_zone.py
+otcextensions/tests/unit/osclient/identity/__init__.py
+otcextensions/tests/unit/osclient/identity/v3/__init__.py
+otcextensions/tests/unit/osclient/identity/v3/fakes.py
+otcextensions/tests/unit/osclient/identity/v3/test_credential.py
 otcextensions/tests/unit/osclient/kms/__init__.py
 otcextensions/tests/unit/osclient/kms/v1/__init__.py
 otcextensions/tests/unit/osclient/kms/v1/fakes.py
 otcextensions/tests/unit/osclient/kms/v1/test_cmk.py
 otcextensions/tests/unit/osclient/load_balancer/__init__.py
 otcextensions/tests/unit/osclient/load_balancer/v1/__init__.py
 otcextensions/tests/unit/osclient/load_balancer/v1/fakes.py
@@ -968,15 +1041,21 @@
 otcextensions/tests/unit/sdk/cce/v3/__init__.py
 otcextensions/tests/unit/sdk/cce/v3/test_cluster.py
 otcextensions/tests/unit/sdk/cce/v3/test_cluster_cert.py
 otcextensions/tests/unit/sdk/cce/v3/test_cluster_node.py
 otcextensions/tests/unit/sdk/cce/v3/test_job.py
 otcextensions/tests/unit/sdk/cce/v3/test_proxy.py
 otcextensions/tests/unit/sdk/ces/__init__.py
+otcextensions/tests/unit/sdk/ces/v1/__init__.py
+otcextensions/tests/unit/sdk/ces/v1/test_alarm.py
+otcextensions/tests/unit/sdk/ces/v1/test_event_data.py
+otcextensions/tests/unit/sdk/ces/v1/test_metric.py
+otcextensions/tests/unit/sdk/ces/v1/test_metric_data.py
 otcextensions/tests/unit/sdk/ces/v1/test_proxy.py
+otcextensions/tests/unit/sdk/ces/v1/test_quota.py
 otcextensions/tests/unit/sdk/cloud/__init__.py
 otcextensions/tests/unit/sdk/cloud/test_rds.py
 otcextensions/tests/unit/sdk/compute/__init__.py
 otcextensions/tests/unit/sdk/compute/v2/__init__.py
 otcextensions/tests/unit/sdk/compute/v2/test_server.py
 otcextensions/tests/unit/sdk/css/__init__.py
 otcextensions/tests/unit/sdk/css/v1/__init__.py
@@ -1025,14 +1104,20 @@
 otcextensions/tests/unit/sdk/dns/v2/test_floating_ip.py
 otcextensions/tests/unit/sdk/dns/v2/test_nameserver.py
 otcextensions/tests/unit/sdk/dns/v2/test_proxy.py
 otcextensions/tests/unit/sdk/dns/v2/test_recordset.py
 otcextensions/tests/unit/sdk/dns/v2/test_zone.py
 otcextensions/tests/unit/sdk/dws/__init__.py
 otcextensions/tests/unit/sdk/dws/v1/test_proxy.py
+otcextensions/tests/unit/sdk/identity/__init__.py
+otcextensions/tests/unit/sdk/identity/v3/__init__.py
+otcextensions/tests/unit/sdk/identity/v3/test_agency.py
+otcextensions/tests/unit/sdk/identity/v3/test_agency_role.py
+otcextensions/tests/unit/sdk/identity/v3/test_credential.py
+otcextensions/tests/unit/sdk/identity/v3/test_proxy.py
 otcextensions/tests/unit/sdk/kms/__init__.py
 otcextensions/tests/unit/sdk/kms/v1/__init__.py
 otcextensions/tests/unit/sdk/kms/v1/test_data_key.py
 otcextensions/tests/unit/sdk/kms/v1/test_key.py
 otcextensions/tests/unit/sdk/kms/v1/test_misc.py
 otcextensions/tests/unit/sdk/kms/v1/test_proxy.py
 otcextensions/tests/unit/sdk/lts/__init__.py
```

### Comparing `otcextensions-0.9.0/otcextensions.egg-info/entry_points.txt` & `otcextensions-0.9.1/otcextensions.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[keystoneauth1.plugin]
+agency = otcextensions.common.agency_auth:AgencyLoader
+
 [openstack.anti_ddos.v1]
 antiddos_config_list = otcextensions.osclient.anti_ddos.v1.config:ListConfig
 antiddos_floatip_events = otcextensions.osclient.anti_ddos.v1.status:ListFloatingIPEvents
 antiddos_floatip_list = otcextensions.osclient.anti_ddos.v1.floating_ip:ListFloatingIP
 antiddos_floatip_show = otcextensions.osclient.anti_ddos.v1.floating_ip:ShowFloatingIP
 antiddos_floatip_stat_day = otcextensions.osclient.anti_ddos.v1.status:ListFloatingIPStatDay
 antiddos_floatip_stat_week = otcextensions.osclient.anti_ddos.v1.status:ListFloatingIPStatWeek
@@ -48,18 +51,29 @@
 cce_cluster_list = otcextensions.osclient.cce.v2.cluster:ListCCECluster
 cce_cluster_node_create = otcextensions.osclient.cce.v2.cluster_node:CreateCCEClusterNode
 cce_cluster_node_delete = otcextensions.osclient.cce.v2.cluster_node:DeleteCCEClusterNode
 cce_cluster_node_list = otcextensions.osclient.cce.v2.cluster_node:ListCCEClusterNode
 cce_cluster_node_show = otcextensions.osclient.cce.v2.cluster_node:ShowCCEClusterNode
 cce_cluster_show = otcextensions.osclient.cce.v2.cluster:ShowCCECluster
 
+[openstack.ces.v1]
+ces_alarm_create = otcextensions.osclient.ces.v1.alarm:CreateAlarm
+ces_alarm_delete = otcextensions.osclient.ces.v1.alarm:DeleteAlarm
+ces_alarm_list = otcextensions.osclient.ces.v1.alarm:ListAlarms
+ces_alarm_show = otcextensions.osclient.ces.v1.alarm:ShowAlarm
+ces_alarm_switch_state = otcextensions.osclient.ces.v1.alarm:SetAlarm
+ces_event_data_list = otcextensions.osclient.ces.v1.event_data:ListEventData
+ces_metric_list = otcextensions.osclient.ces.v1.metric:ListMetrics
+ces_quota_list = otcextensions.osclient.ces.v1.quota:ListQuotas
+
 [openstack.cli.extension]
 anti_ddos = otcextensions.osclient.anti_ddos.client
 auto_scaling = otcextensions.osclient.auto_scaling.client
 cce = otcextensions.osclient.cce.client
+ces = otcextensions.osclient.ces.client
 cts = otcextensions.osclient.cts.client
 dcs = otcextensions.osclient.dcs.client
 deh = otcextensions.osclient.deh.client
 dms = otcextensions.osclient.dms.client
 dns = otcextensions.osclient.dns.client
 kms = otcextensions.osclient.kms.client
 load_balancer = otcextensions.osclient.load_balancer.client
```

### Comparing `otcextensions-0.9.0/otcextensions.egg-info/PKG-INFO` & `otcextensions-0.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: otcextensions
-Version: 0.9.0
+Version: 0.9.1
 Summary: Open Telekom Cloud specific extensions for the OpenStack Client CLI and OpenStack SDK
 Home-page: http://python-otcextensions.readthedocs.io/
 Author: Artem Goncharov
 Author-email: artem.goncharov@gmail.com
 License: UNKNOWN
 Description: OTC Extensions
         ==============
@@ -25,35 +25,39 @@
         * `python-openstackclient`
         
         packages.
         
         Documentation
         -------------
         
-        * `Documentation <http://python-otcextensions.readthedocs.io/en/latest/>`
+        `Documentation Overview <http://python-otcextensions.readthedocs.io/en/latest/>`_
         
         Installation
         ------------
         
+        `Installation Page <https://python-otcextensions.readthedocs.io/en/latest/install/index.html>`_
+        
         The OTC Extensions are hosted as the package `otcextensions` on PyPI
         and can be installed by pip as
         
         .. code-block: console
+        
            $ pip install otcextensions
         
         There are several options
         to do that including but not limited to pip userland installation, system wide
         installation as well as installation from operating system packets or directly
         from source. Refer to the installation instructions_ in the projects
         documentation.
         
-        
         Configuration
         -------------
         
+        `Configuration Page <https://python-otcextensions.readthedocs.io/en/latest/install/configuration.html>`_
+        
         Acessing the Open Telekom Cloud APIs requires authentication and
         authorization. For both there are several options available:
         
         * **Configuration files** (recommended): A file called `clouds.yaml`
           holds all necessary configuration parameters. The file can be placed
           either in the local directory, below the user home directory in
           `.config/openstack` or in the system-wide directory
@@ -62,46 +66,47 @@
           credentials. For more details see the section `configuration`_ in
           the official documentation.
         
           Minimal sample ``clouds.yaml`` file:
         
           .. code-block:: yaml
         
-              clouds:
-                  otc:
-                  profile: otc
-                      auth:
-                          username: "*username*"
-                          password: "*password*"
-                          project_name: "eu-de"
-                          auth_url: "https://iam.eu-de.otc.t-systems.com:443/v3"
-                          user_domain_name: "*OTC00000000001000000xxx*"
-                     interface: "public"
-                     identity_api_version: 3
-                     ak: "*40 digit access key*"
-                     sk: "*20 digit secure key*"
+            clouds:
+              otc:
+                profile: otc
+                auth:
+                  username: '<USER_NAME>'
+                  password: '<PASSWORD>'
+                  project_name: '<eu-de_project>'
+                  # or project_id: '<123456_PROJECT_ID>'
+                  user_domain_name: 'OTC00000000001000000xxx'
+                  # or user_domain_id: '<123456_DOMAIN_ID>'
+                  auth_url: 'https://iam.eu-de.otc.t-systems.com:443/v3'
+                interface: 'public'
+                identity_api_version: 3 # !Important
+                ak: '<AK_VALUE>' # AK/SK pair for access to OBS
+                sk: '<SK_VALUE>'
         
           With this configuration you can start using the CLI with ``openstack
           --os-cloud otc *command*`` or by ``export OS_CLOUD=otc; openstack
           *command*``.
         
         * **Environment variables:** Authentication using username/password is often
-          used:
+          used::
         
             export OS_AUTH_URL=<url-to-openstack-identity>
             export OS_IDENTITY_API_VERSION=3
             export OS_PROJECT_NAME=<project-name>
             export OS_PROJECT_DOMAIN_NAME=<project-domain-name>
             export OS_USERNAME=<username>
             export OS_USER_DOMAIN_NAME=<user-domain-name>
             export OS_PASSWORD=<password>  # (optional)
             export S3_ACCESS_KEY_ID=<access_key>
             export S3_SECRET_ACCESS_KEY=<secret_access_key>
         
-        
         * **Command-Line Options:** The corresponding command-line options look
           very similar::
         
             --os-auth-url <url>
             --os-identity-api-version 3
             --os-project-name <project-name>
             --os-project-domain-name <project-domain-name>
@@ -115,36 +120,40 @@
         * **Existing Token:** Authentication may also be performed using an
           already-acquired token and a URL pointing directly to the service
           API that presumably was acquired from the Service Catalog::
         
             export OS_TOKEN=<token>
             export OS_URL=<url-to-openstack-service>
         
-        The corresponding command-line options look very similar::
+        * The corresponding command-line options look very similar::
         
             --os-token <token>
             --os-url <url-to-openstack-service>
         
         In addition to that a regular `clouds.yaml` configuration file can be used
         
         More information is available at
         https://docs.openstack.org/python-openstackclient/latest/cli/authentication.html
         or
         https://developer.openstack.org/sdks/python/openstacksdk/users/config
         
+        OTC Extensions CLI Usage
+        ------------------------
+        
+        `OTCE CLI Command Overview <https://python-otcextensions.readthedocs.io/en/latest/cli/index.html>`_
         
-        Writing Own Code
-        ----------------
+        OTC Extensions SDK Guides
+        -------------------------
         
-        XXX Example XXXX
+        `OTCE SDK Guides <https://python-otcextensions.readthedocs.io/en/latest/sdk/guides/index.html>`_
         
         Contributing
         ------------
         
-        See CONTRIBUTING.rst
+        * `Contribution Page <https://python-otcextensions.readthedocs.io/en/latest/contributor/index.html>`_
         
         Further Links
         -------------
         
         * `Issue Tracker <https://github.com/OpenTelekomCloud/python-otcextensions/issues>`_
         
         .. _instructions: http://python-otcextensions.readthedocs.io/en/latest/install/
```

### Comparing `otcextensions-0.9.0/tox.ini` & `otcextensions-0.9.1/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     coverage combine
     coverage html -d cover
     coverage xml -o cover/coverage.xml
 
 [testenv:docs]
 deps =
     -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
-    -r{toxinidir}/requirements.txt
+#    -r{toxinidir}/requirements.txt
     -r{toxinidir}/doc/requirements.txt
 commands =
     sphinx-build -W -d doc/build/doctrees --keep-going -b html doc/source/ doc/build/html
 
 [testenv:releasenotes]
 deps =
     -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
```

