# Comparing `tmp/darshan-3.4.2.0.tar.gz` & `tmp/darshan-3.4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darshan-3.4.2.0.tar", last modified: Fri Dec 16 20:32:18 2022, max compression
+gzip compressed data, was "darshan-3.4.3.0.tar", last modified: Mon Jun 12 20:20:56 2023, max compression
```

## Comparing `darshan-3.4.2.0.tar` & `darshan-3.4.3.0.tar`

### file list

```diff
@@ -1,151 +1,156 @@
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.812943 darshan-3.4.2.0/
--rw-rw-r--   0 shane     (1000) shane     (1000)      213 2022-10-26 18:33:05.000000 darshan-3.4.2.0/MANIFEST.in
--rw-rw-r--   0 shane     (1000) shane     (1000)     3542 2022-12-16 20:32:18.812943 darshan-3.4.2.0/PKG-INFO
--rw-rw-r--   0 shane     (1000) shane     (1000)     2879 2022-12-02 20:53:39.000000 darshan-3.4.2.0/README.rst
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.768942 darshan-3.4.2.0/darshan/
--rw-rw-r--   0 shane     (1000) shane     (1000)     1221 2022-12-15 22:54:06.000000 darshan-3.4.2.0/darshan/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)       64 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/__main__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.768942 darshan-3.4.2.0/darshan/backend/
--rw-rw-r--   0 shane     (1000) shane     (1000)      227 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/backend/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     4480 2022-11-29 19:58:53.000000 darshan-3.4.2.0/darshan/backend/api_def_c.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3694 2022-05-04 14:43:41.000000 darshan-3.4.2.0/darshan/backend/apmpi.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1928 2022-05-04 14:43:41.000000 darshan-3.4.2.0/darshan/backend/apss.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2305 2022-05-04 14:43:41.000000 darshan-3.4.2.0/darshan/backend/apxc.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    17361 2022-11-29 19:58:53.000000 darshan-3.4.2.0/darshan/backend/cffi_backend.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.772942 darshan-3.4.2.0/darshan/cli/
--rw-rw-r--   0 shane     (1000) shane     (1000)     5545 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/cli/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)       73 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/cli/__main__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2112 2022-11-29 19:58:53.000000 darshan-3.4.2.0/darshan/cli/base.html
--rw-rw-r--   0 shane     (1000) shane     (1000)      966 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/cli/info.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1028 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/cli/name_records.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     7131 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/cli/style.css
--rw-rw-r--   0 shane     (1000) shane     (1000)    22607 2022-11-29 19:58:53.000000 darshan-3.4.2.0/darshan/cli/summary.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      920 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/cli/to_json.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.772942 darshan-3.4.2.0/darshan/datatypes/
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/datatypes/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3814 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/datatypes/heatmap.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     7609 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/discover_darshan.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.772942 darshan-3.4.2.0/darshan/examples/
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.776942 darshan-3.4.2.0/darshan/examples/darshan-graph/
--rw-rw-r--   0 shane     (1000) shane     (1000)      279 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/darshan-graph/Makefile
--rw-rw-r--   0 shane     (1000) shane     (1000)     1676 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/darshan-graph/app.c
--rw-rw-r--   0 shane     (1000) shane     (1000)     3882 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/darshan-graph/app_rw_mpiio.c
--rw-rw-r--   0 shane     (1000) shane     (1000)     2498 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/darshan-graph/pq_app_readAB_writeC_id71326_7-31-5658-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1070 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/darshan-graph/pq_app_read_id71317_7-31-5657-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1079 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/darshan-graph/pq_app_read_id71344_7-31-5658-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1068 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/darshan-graph/pq_app_write_id71296_7-31-5657-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1069 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/darshan-graph/pq_app_write_id71303_7-31-5657-2037904274838284930_55623.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1072 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/darshan-graph/pq_app_write_id71310_7-31-5657-2037904274838284930_55623.darshan
--rwxrwxr-x   0 shane     (1000) shane     (1000)      717 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/darshan-graph/run.sh
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.776942 darshan-3.4.2.0/darshan/examples/example_logs/
--rw-rw-r--   0 shane     (1000) shane     (1000)      286 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/example_logs/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    98998 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/example_logs/dxt.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    11472 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/example_logs/example.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     3967 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/example_logs/ior_hdf5_example.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    16073 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/example_logs/noposix.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)   459650 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/example_logs/sample-badost.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1992 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/example_logs/shane_macsio_id29959_5-22-32552-7035573431850780836_1590156158.darshan
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.780942 darshan-3.4.2.0/darshan/examples/tutorial/
--rw-rw-r--   0 shane     (1000) shane     (1000)      103 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/tutorial/hello.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      216 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/tutorial/plot.py
--rwxrwxr-x   0 shane     (1000) shane     (1000)      596 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/examples/tutorial/tojson.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.780942 darshan-3.4.2.0/darshan/experimental/
--rw-rw-r--   0 shane     (1000) shane     (1000)      134 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/experimental/__init__.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.784942 darshan-3.4.2.0/darshan/experimental/aggregators/
--rw-rw-r--   0 shane     (1000) shane     (1000)      407 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/experimental/aggregators/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     4560 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/experimental/aggregators/agg_ioops.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2950 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/experimental/aggregators/create_dxttimeline.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1749 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/experimental/aggregators/create_sankey.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1335 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/experimental/aggregators/create_time_summary.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     5726 2022-11-02 17:48:53.000000 darshan-3.4.2.0/darshan/experimental/aggregators/create_timeline.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1476 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/experimental/aggregators/mod_agg_iohist.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      637 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/experimental/aggregators/name_records_summary.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     6951 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/experimental/aggregators/print_module_records.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1211 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/experimental/aggregators/records_as_dict.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      516 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/experimental/aggregators/summarize.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.784942 darshan-3.4.2.0/darshan/experimental/operations/
--rw-rw-r--   0 shane     (1000) shane     (1000)     2303 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/experimental/operations/filter.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2405 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/experimental/operations/merge.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     3187 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/experimental/operations/reduce.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.788942 darshan-3.4.2.0/darshan/experimental/plots/
--rw-rw-r--   0 shane     (1000) shane     (1000)      186 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/experimental/plots/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    26454 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/experimental/plots/data_access_by_filesystem.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    14135 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/experimental/plots/heatmap_handling.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2627 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/experimental/plots/plot_access_histogram.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     4340 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/experimental/plots/plot_common_access_table.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    14584 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/experimental/plots/plot_dxt_heatmap.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     4145 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/experimental/plots/plot_dxt_heatmap2.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     5939 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/experimental/plots/plot_io_cost.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     6501 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/experimental/plots/plot_opcounts.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.788942 darshan-3.4.2.0/darshan/experimental/transforms/
--rw-rw-r--   0 shane     (1000) shane     (1000)     5626 2022-10-26 18:33:05.000000 darshan-3.4.2.0/darshan/experimental/transforms/dxt2png.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2901 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/log_utils.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    35752 2022-11-29 19:59:00.000000 darshan-3.4.2.0/darshan/report.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.800943 darshan-3.4.2.0/darshan/tests/
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      533 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/conftest.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.804943 darshan-3.4.2.0/darshan/tests/input/
--rw-rw-r--   0 shane     (1000) shane     (1000)      313 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/input/__init__.py
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/input/match_dotout.dot
--rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/input/match_jsonout.json
--rw-rw-r--   0 shane     (1000) shane     (1000)    16073 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/input/noposix.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     1441 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/input/noposixopens.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)   459650 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/input/sample-badost.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     6631 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/input/sample-dxt-simple.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    10717 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/input/sample-goodost.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)    11472 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/input/sample.darshan
--rw-rw-r--   0 shane     (1000) shane     (1000)     6594 2022-12-01 17:04:20.000000 darshan-3.4.2.0/darshan/tests/test_cffi_misc.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    33345 2022-12-01 17:04:20.000000 darshan-3.4.2.0/darshan/tests/test_data_access_by_filesystem.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      567 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/test_error.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    22010 2022-12-01 17:04:20.000000 darshan-3.4.2.0/darshan/tests/test_heatmap_handling.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     2064 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/test_log_utils.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1653 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/test_moddxt.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1116 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/test_modmpiio.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1107 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/test_modposix.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     1144 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/test_modstdio.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     8550 2022-12-01 17:04:20.000000 darshan-3.4.2.0/darshan/tests/test_plot_common_access_table.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    16837 2022-12-01 17:04:20.000000 darshan-3.4.2.0/darshan/tests/test_plot_dxt_heatmap.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    12811 2022-12-01 17:04:20.000000 darshan-3.4.2.0/darshan/tests/test_plot_exp_common.py
--rw-rw-r--   0 shane     (1000) shane     (1000)     8933 2022-12-01 17:04:20.000000 darshan-3.4.2.0/darshan/tests/test_plot_io_cost.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    24120 2022-12-01 17:04:20.000000 darshan-3.4.2.0/darshan/tests/test_report.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      563 2022-11-22 21:37:27.000000 darshan-3.4.2.0/darshan/tests/test_report_copy.py
--rw-rw-r--   0 shane     (1000) shane     (1000)    24067 2022-12-01 17:04:20.000000 darshan-3.4.2.0/darshan/tests/test_summary.py
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.768942 darshan-3.4.2.0/darshan.egg-info/
--rw-rw-r--   0 shane     (1000) shane     (1000)     3542 2022-12-16 20:32:18.000000 darshan-3.4.2.0/darshan.egg-info/PKG-INFO
--rw-rw-r--   0 shane     (1000) shane     (1000)     4874 2022-12-16 20:32:18.000000 darshan-3.4.2.0/darshan.egg-info/SOURCES.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        1 2022-12-16 20:32:18.000000 darshan-3.4.2.0/darshan.egg-info/dependency_links.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        1 2022-12-16 20:32:18.000000 darshan-3.4.2.0/darshan.egg-info/not-zip-safe
--rw-rw-r--   0 shane     (1000) shane     (1000)       42 2022-12-16 20:32:18.000000 darshan-3.4.2.0/darshan.egg-info/requires.txt
--rw-rw-r--   0 shane     (1000) shane     (1000)        8 2022-12-16 20:32:18.000000 darshan-3.4.2.0/darshan.egg-info/top_level.txt
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.808943 darshan-3.4.2.0/docs/
--rw-rw-r--   0 shane     (1000) shane     (1000)      610 2022-10-26 18:33:05.000000 darshan-3.4.2.0/docs/Makefile
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.764942 darshan-3.4.2.0/docs/api/
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.812943 darshan-3.4.2.0/docs/api/pydarshan/
--rw-rw-r--   0 shane     (1000) shane     (1000)      501 2022-12-02 20:55:32.000000 darshan-3.4.2.0/docs/api/pydarshan/darshan.backend.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      740 2022-12-02 20:55:32.000000 darshan-3.4.2.0/docs/api/pydarshan/darshan.cli.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      328 2022-12-02 20:55:32.000000 darshan-3.4.2.0/docs/api/pydarshan/darshan.datatypes.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      179 2022-12-02 20:55:32.000000 darshan-3.4.2.0/docs/api/pydarshan/darshan.examples.example_logs.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      227 2022-12-02 20:55:32.000000 darshan-3.4.2.0/docs/api/pydarshan/darshan.examples.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     2573 2022-12-02 20:55:32.000000 darshan-3.4.2.0/docs/api/pydarshan/darshan.experimental.aggregators.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     2015 2022-12-02 20:55:32.000000 darshan-3.4.2.0/docs/api/pydarshan/darshan.experimental.plots.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      272 2022-12-02 20:55:32.000000 darshan-3.4.2.0/docs/api/pydarshan/darshan.experimental.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      742 2022-12-02 20:55:31.000000 darshan-3.4.2.0/docs/api/pydarshan/darshan.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      147 2022-12-02 20:55:32.000000 darshan-3.4.2.0/docs/api/pydarshan/darshan.tests.input.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     3341 2022-12-02 20:55:32.000000 darshan-3.4.2.0/docs/api/pydarshan/darshan.tests.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)       62 2022-12-02 20:55:32.000000 darshan-3.4.2.0/docs/api/pydarshan/modules.rst
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.764942 darshan-3.4.2.0/docs/build/
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.764942 darshan-3.4.2.0/docs/build/html/
-drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2022-12-16 20:32:18.812943 darshan-3.4.2.0/docs/build/html/_static/
--rw-rw-r--   0 shane     (1000) shane     (1000)      286 2022-12-02 17:37:07.000000 darshan-3.4.2.0/docs/build/html/_static/file.png
--rw-rw-r--   0 shane     (1000) shane     (1000)       90 2022-12-02 17:37:07.000000 darshan-3.4.2.0/docs/build/html/_static/minus.png
--rw-rw-r--   0 shane     (1000) shane     (1000)       90 2022-12-02 17:37:07.000000 darshan-3.4.2.0/docs/build/html/_static/plus.png
--rwxrwxr-x   0 shane     (1000) shane     (1000)     5230 2022-10-26 18:33:05.000000 darshan-3.4.2.0/docs/conf.py
--rw-rw-r--   0 shane     (1000) shane     (1000)      528 2022-12-01 18:54:09.000000 darshan-3.4.2.0/docs/index.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     1184 2022-12-02 20:53:39.000000 darshan-3.4.2.0/docs/install.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)      771 2022-10-26 18:33:05.000000 darshan-3.4.2.0/docs/make.bat
--rw-rw-r--   0 shane     (1000) shane     (1000)       27 2022-12-01 18:54:58.000000 darshan-3.4.2.0/docs/readme.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     2151 2022-12-02 20:53:39.000000 darshan-3.4.2.0/docs/usage.rst
--rw-rw-r--   0 shane     (1000) shane     (1000)     1279 2022-11-22 21:37:27.000000 darshan-3.4.2.0/pyproject.toml
--rw-rw-r--   0 shane     (1000) shane     (1000)      480 2022-12-16 20:32:18.812943 darshan-3.4.2.0/setup.cfg
--rw-rw-r--   0 shane     (1000) shane     (1000)     2773 2022-12-15 22:54:35.000000 darshan-3.4.2.0/setup.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.316522 darshan-3.4.3.0/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      213 2022-10-26 18:33:05.000000 darshan-3.4.3.0/MANIFEST.in
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2830 2023-06-12 20:20:56.316522 darshan-3.4.3.0/PKG-INFO
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2115 2023-06-12 18:17:58.000000 darshan-3.4.3.0/README.rst
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.276521 darshan-3.4.3.0/darshan/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1221 2023-06-12 14:45:06.000000 darshan-3.4.3.0/darshan/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)       64 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/__main__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.280521 darshan-3.4.3.0/darshan/backend/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      227 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/backend/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6193 2023-02-08 22:31:13.000000 darshan-3.4.3.0/darshan/backend/api_def_c.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3694 2022-05-04 14:43:41.000000 darshan-3.4.3.0/darshan/backend/apmpi.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1928 2022-05-04 14:43:41.000000 darshan-3.4.3.0/darshan/backend/apss.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2305 2022-05-04 14:43:41.000000 darshan-3.4.3.0/darshan/backend/apxc.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    22874 2023-04-19 16:40:28.000000 darshan-3.4.3.0/darshan/backend/cffi_backend.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.284521 darshan-3.4.3.0/darshan/cli/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5545 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/cli/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)       73 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/cli/__main__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2313 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/cli/base.html
+-rw-rw-r--   0 shane     (1000) shane     (1000)      966 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/cli/info.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1028 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/cli/name_records.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     7563 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/cli/style.css
+-rw-rw-r--   0 shane     (1000) shane     (1000)    29267 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/cli/summary.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      920 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/cli/to_json.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.284521 darshan-3.4.3.0/darshan/datatypes/
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/datatypes/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3814 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/datatypes/heatmap.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     7635 2023-04-13 22:44:27.000000 darshan-3.4.3.0/darshan/discover_darshan.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.284521 darshan-3.4.3.0/darshan/examples/
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.284521 darshan-3.4.3.0/darshan/examples/darshan-graph/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      279 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/Makefile
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1676 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/app.c
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3882 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/app_rw_mpiio.c
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2498 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_readAB_writeC_id71326_7-31-5658-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1070 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_read_id71317_7-31-5657-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1079 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_read_id71344_7-31-5658-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1068 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_write_id71296_7-31-5657-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1069 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_write_id71303_7-31-5657-2037904274838284930_55623.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1072 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_write_id71310_7-31-5657-2037904274838284930_55623.darshan
+-rwxrwxr-x   0 shane     (1000) shane     (1000)      717 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/darshan-graph/run.sh
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.288521 darshan-3.4.3.0/darshan/examples/example_logs/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      286 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    98998 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/dxt.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    11472 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/example.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3967 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/ior_hdf5_example.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    16073 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/noposix.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)   459650 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/sample-badost.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1992 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/example_logs/shane_macsio_id29959_5-22-32552-7035573431850780836_1590156158.darshan
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.288521 darshan-3.4.3.0/darshan/examples/tutorial/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      103 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/tutorial/hello.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      216 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/tutorial/plot.py
+-rwxrwxr-x   0 shane     (1000) shane     (1000)      596 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/examples/tutorial/tojson.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.288521 darshan-3.4.3.0/darshan/experimental/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      134 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/__init__.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.292521 darshan-3.4.3.0/darshan/experimental/aggregators/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      407 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4560 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/experimental/aggregators/agg_ioops.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2950 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/experimental/aggregators/create_dxttimeline.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1749 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/create_sankey.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1335 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/create_time_summary.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5726 2022-11-02 17:48:53.000000 darshan-3.4.3.0/darshan/experimental/aggregators/create_timeline.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1476 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/experimental/aggregators/mod_agg_iohist.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      637 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/name_records_summary.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6951 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/print_module_records.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1211 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/records_as_dict.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      516 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/aggregators/summarize.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.292521 darshan-3.4.3.0/darshan/experimental/operations/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2303 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/operations/filter.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2405 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/operations/merge.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3187 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/operations/reduce.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.296521 darshan-3.4.3.0/darshan/experimental/plots/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      251 2023-04-19 16:40:28.000000 darshan-3.4.3.0/darshan/experimental/plots/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    26333 2023-04-14 19:27:35.000000 darshan-3.4.3.0/darshan/experimental/plots/data_access_by_filesystem.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    14559 2023-04-13 22:44:27.000000 darshan-3.4.3.0/darshan/experimental/plots/heatmap_handling.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2765 2023-04-14 19:27:35.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_access_histogram.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4340 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_common_access_table.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    14759 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_dxt_heatmap.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     4145 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_dxt_heatmap2.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6297 2023-04-14 19:27:35.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_io_cost.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6638 2023-04-14 19:27:35.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_opcounts.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1982 2023-04-19 16:40:28.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_posix_access_pattern.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5204 2022-12-19 21:37:30.000000 darshan-3.4.3.0/darshan/experimental/plots/plot_posix_io_pattern.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.296521 darshan-3.4.3.0/darshan/experimental/transforms/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5626 2022-10-26 18:33:05.000000 darshan-3.4.3.0/darshan/experimental/transforms/dxt2png.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.300521 darshan-3.4.3.0/darshan/lib/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3741 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/lib/accum.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2901 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/log_utils.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    35880 2023-02-15 21:55:53.000000 darshan-3.4.3.0/darshan/report.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.304521 darshan-3.4.3.0/darshan/tests/
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      533 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/conftest.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.308521 darshan-3.4.3.0/darshan/tests/input/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      313 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/__init__.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/match_dotout.dot
+-rw-rw-r--   0 shane     (1000) shane     (1000)        0 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/match_jsonout.json
+-rw-rw-r--   0 shane     (1000) shane     (1000)    16073 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/noposix.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1441 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/noposixopens.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)   459650 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/sample-badost.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)     6631 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/sample-dxt-simple.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    10717 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/sample-goodost.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    11472 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/input/sample.darshan
+-rw-rw-r--   0 shane     (1000) shane     (1000)    11523 2023-02-15 21:55:53.000000 darshan-3.4.3.0/darshan/tests/test_cffi_misc.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    32921 2023-04-14 19:27:35.000000 darshan-3.4.3.0/darshan/tests/test_data_access_by_filesystem.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      567 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_error.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    22010 2022-12-01 17:04:20.000000 darshan-3.4.3.0/darshan/tests/test_heatmap_handling.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     8314 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/tests/test_lib_accum.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2064 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_log_utils.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1653 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_moddxt.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1116 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_modmpiio.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1107 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_modposix.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1144 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_modstdio.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)     8550 2022-12-01 17:04:20.000000 darshan-3.4.3.0/darshan/tests/test_plot_common_access_table.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    16837 2022-12-01 17:04:20.000000 darshan-3.4.3.0/darshan/tests/test_plot_dxt_heatmap.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    13048 2023-04-14 19:27:35.000000 darshan-3.4.3.0/darshan/tests/test_plot_exp_common.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    10752 2023-02-15 21:55:53.000000 darshan-3.4.3.0/darshan/tests/test_plot_io_cost.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    24120 2022-12-01 17:04:20.000000 darshan-3.4.3.0/darshan/tests/test_report.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      563 2022-11-22 21:37:27.000000 darshan-3.4.3.0/darshan/tests/test_report_copy.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)    25957 2023-05-31 18:10:46.000000 darshan-3.4.3.0/darshan/tests/test_summary.py
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.276521 darshan-3.4.3.0/darshan.egg-info/
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2830 2023-06-12 20:20:56.000000 darshan-3.4.3.0/darshan.egg-info/PKG-INFO
+-rw-rw-r--   0 shane     (1000) shane     (1000)     5035 2023-06-12 20:20:56.000000 darshan-3.4.3.0/darshan.egg-info/SOURCES.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        1 2023-06-12 20:20:56.000000 darshan-3.4.3.0/darshan.egg-info/dependency_links.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        1 2023-06-12 20:20:56.000000 darshan-3.4.3.0/darshan.egg-info/not-zip-safe
+-rw-rw-r--   0 shane     (1000) shane     (1000)       51 2023-06-12 20:20:56.000000 darshan-3.4.3.0/darshan.egg-info/requires.txt
+-rw-rw-r--   0 shane     (1000) shane     (1000)        8 2023-06-12 20:20:56.000000 darshan-3.4.3.0/darshan.egg-info/top_level.txt
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.312521 darshan-3.4.3.0/docs/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      610 2022-10-26 18:33:05.000000 darshan-3.4.3.0/docs/Makefile
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.272521 darshan-3.4.3.0/docs/api/
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.312521 darshan-3.4.3.0/docs/api/pydarshan/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      951 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.backend.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      740 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.cli.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      328 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.datatypes.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      179 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.examples.example_logs.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      227 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.examples.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2573 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.experimental.aggregators.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2015 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.experimental.plots.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      272 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.experimental.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      742 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      147 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.tests.input.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3341 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/darshan.tests.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)       62 2022-12-16 21:58:31.000000 darshan-3.4.3.0/docs/api/pydarshan/modules.rst
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.272521 darshan-3.4.3.0/docs/build/
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.272521 darshan-3.4.3.0/docs/build/html/
+drwxrwxr-x   0 shane     (1000) shane     (1000)        0 2023-06-12 20:20:56.316522 darshan-3.4.3.0/docs/build/html/_static/
+-rw-rw-r--   0 shane     (1000) shane     (1000)      286 2023-06-06 18:59:29.000000 darshan-3.4.3.0/docs/build/html/_static/file.png
+-rw-rw-r--   0 shane     (1000) shane     (1000)       90 2023-06-06 18:59:29.000000 darshan-3.4.3.0/docs/build/html/_static/minus.png
+-rw-rw-r--   0 shane     (1000) shane     (1000)       90 2023-06-06 18:59:29.000000 darshan-3.4.3.0/docs/build/html/_static/plus.png
+-rwxrwxr-x   0 shane     (1000) shane     (1000)     5230 2022-10-26 18:33:05.000000 darshan-3.4.3.0/docs/conf.py
+-rw-rw-r--   0 shane     (1000) shane     (1000)      669 2023-05-31 18:10:46.000000 darshan-3.4.3.0/docs/index.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2097 2023-05-31 18:10:46.000000 darshan-3.4.3.0/docs/install.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)      771 2022-10-26 18:33:05.000000 darshan-3.4.3.0/docs/make.bat
+-rw-rw-r--   0 shane     (1000) shane     (1000)       27 2022-12-01 18:54:58.000000 darshan-3.4.3.0/docs/readme.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     3682 2023-05-31 18:10:46.000000 darshan-3.4.3.0/docs/usage.rst
+-rw-rw-r--   0 shane     (1000) shane     (1000)     1353 2023-02-16 19:35:59.000000 darshan-3.4.3.0/pyproject.toml
+-rw-rw-r--   0 shane     (1000) shane     (1000)      480 2023-06-12 20:20:56.316522 darshan-3.4.3.0/setup.cfg
+-rw-rw-r--   0 shane     (1000) shane     (1000)     2850 2023-06-12 14:45:06.000000 darshan-3.4.3.0/setup.py
```

### Comparing `darshan-3.4.2.0/darshan/__init__.py` & `darshan-3.4.3.0/darshan/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 PyDarshan provides direct log access for reading binary Darshan logs.
 PyDarshan also provides a suite of analysis utilities.
 """
 
-__version__ = '3.4.2.0'
-__darshanutil_version__ = '3.4.2'
+__version__ = '3.4.3.0'
+__darshanutil_version__ = '3.4.3'
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 options = {} # type: ignore
```

### Comparing `darshan-3.4.2.0/darshan/backend/apmpi.py` & `darshan-3.4.3.0/darshan/backend/apmpi.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/backend/apss.py` & `darshan-3.4.3.0/darshan/backend/apss.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/backend/apxc.py` & `darshan-3.4.3.0/darshan/backend/apxc.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/backend/cffi_backend.py` & `darshan-3.4.3.0/darshan/backend/cffi_backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 import cffi
 import ctypes
 
 import numpy as np
 import pandas as pd
 
+from collections import namedtuple
+
 import logging
 logger = logging.getLogger(__name__)
 
 
 from darshan.backend.api_def_c import load_darshan_header
 from darshan.discover_darshan import find_utils
 from darshan.discover_darshan import check_version
@@ -47,14 +49,34 @@
 
 libdutil = None
 libdutil = find_utils(ffi, libdutil)
 
 check_version(ffi, libdutil)
 
 
+_mod_names = [
+    "NULL",
+    "POSIX",
+    "MPI-IO",
+    "H5F",
+    "H5D",
+    "PNETCDF_FILE",
+    "PNETCDF_VAR",
+    "BG/Q",
+    "LUSTRE",
+    "STDIO",
+    "DXT_POSIX",
+    "DXT_MPIIO",
+    "MDHIM",
+    "APXC",
+    "APMPI",
+    "HEATMAP",
+]
+def mod_name_to_idx(mod_name):
+    return _mod_names.index(mod_name)
 
 _structdefs = {
     "BG/Q": "struct darshan_bgq_record **",
     "DXT_MPIIO": "struct dxt_file_record **",
     "DXT_POSIX": "struct dxt_file_record **",
     "HEATMAP": "struct darshan_heatmap_record **",
     "H5F": "struct darshan_hdf5_file **",
@@ -344,29 +366,37 @@
 
     """
     modules = log_get_modules(log)
     if mod_name not in modules:
         return None
     mod_type = _structdefs[mod_name]
 
-    rec = {}
     buf = ffi.new("void **")
     r = libdutil.darshan_log_get_record(log['handle'], modules[mod_name]['idx'], buf)
     if r < 1:
         return None
     rbuf = ffi.cast(mod_type, buf)
 
+    rec = _make_generic_record(rbuf, mod_name, dtype)
+    libdutil.darshan_free(buf[0])
+
+    return rec
+
+def _make_generic_record(rbuf, mod_name, dtype='numpy'):
+    """
+    Returns a record dictionary for an input record buffer for a given module.
+    """
+    rec = {}
     rec['id'] = rbuf[0].base_rec.id
     rec['rank'] = rbuf[0].base_rec.rank
     if mod_name == 'H5D' or mod_name == 'PNETCDF_VAR':
         rec['file_rec_id'] = rbuf[0].file_rec_id
 
     clst = np.copy(np.frombuffer(ffi.buffer(rbuf[0].counters), dtype=np.int64))
     flst = np.copy(np.frombuffer(ffi.buffer(rbuf[0].fcounters), dtype=np.float64))
-    libdutil.darshan_free(buf[0])
 
     c_cols = counter_names(mod_name)
     fc_cols = fcounter_names(mod_name)
 
     if dtype == "numpy":
         rec['counters'] = clst
         rec['fcounters'] = flst
@@ -392,15 +422,14 @@
         df_c['id'] = rec_id
         df_fc['id'] = rec_id
         # assign the dataframes to the record
         rec['counters'] = df_c
         rec['fcounters'] = df_fc
     return rec
 
-
 @functools.lru_cache(maxsize=32)
 def counter_names(mod_name, fcnts=False, special=''):
     """
     Returns a list of available counter names for the module.
     By default only integer counter names are listed, unless fcnts is set to
     true in which case only the floating point counter names are listed.
 
@@ -653,7 +682,117 @@
     rec['write_bins'] = write_bins
 
     read_bins = np.copy(np.frombuffer(ffi.buffer(filerec[0].read_bins, sizeof_64*nbins), dtype = np.int64))
     rec['read_bins'] = read_bins
     libdutil.darshan_free(buf[0])
     
     return rec
+
+
+def _df_to_rec(rec_dict, mod_name, rec_index_of_interest=None):
+    """
+    Pack the DataFrames-format PyDarshan data back into
+    a C buffer of records that can be consumed by darshan-util
+    C code.
+
+    Parameters
+    ----------
+    rec_dict: dict
+        Dictionary containing the counter and fcounter dataframes.
+
+    mod_name: str
+        Name of the darshan module.
+
+    rec_index_of_interest: int or None
+        If ``None``, use all records in the dataframe. Otherwise,
+        repack only the the record at the provided integer index.
+
+    Returns
+    -------
+    buf: Raw char array containing a buffer of record(s) or a single record.
+    """
+    counters_df = rec_dict["counters"]
+    fcounters_df = rec_dict["fcounters"]
+    counters_n_cols = counters_df.shape[1]
+    fcounters_n_cols = fcounters_df.shape[1]
+    id_col = counters_df.columns.get_loc("id")
+    rank_col = counters_df.columns.get_loc("rank")
+    if rec_index_of_interest is None:
+        num_recs = counters_df.shape[0]
+        # newer pandas versions can support ...
+        # but we use a slice for now
+        rec_index_of_interest = slice(0, counters_df.shape[0])
+    else:
+        num_recs = 1
+    # id and rank columns are duplicated
+    # in counters and fcounters
+    rec_arr = np.recarray(shape=(num_recs), dtype=[("id", "<u8", (1,)),
+                                                   ("rank", "<i8", (1,)),
+                                                   ("counters", "<i8", (counters_n_cols - 2,)),
+                                                   ("fcounters", "<f8", (fcounters_n_cols - 2,))])
+    rec_arr.fcounters = fcounters_df.iloc[rec_index_of_interest, 2:].to_numpy()
+    rec_arr.counters = counters_df.iloc[rec_index_of_interest, 2:].to_numpy()
+    if num_recs > 1:
+        rec_arr.id = counters_df.iloc[rec_index_of_interest, id_col].to_numpy().reshape((num_recs, 1))
+        rec_arr.rank = counters_df.iloc[rec_index_of_interest, rank_col].to_numpy().reshape((num_recs, 1))
+    else:
+        rec_arr.id = counters_df.iloc[rec_index_of_interest, id_col]
+        rec_arr.rank = counters_df.iloc[rec_index_of_interest, rank_col]
+    buf = rec_arr.tobytes()
+    return buf
+
+
+def accumulate_records(rec_dict, mod_name, nprocs):
+    """
+    Passes a set of records (in pandas format) to the Darshan accumulator
+    interface, and returns the corresponding derived metrics struct and
+    summary record.
+
+    Parameters:
+        rec_dict: Dictionary containing the counter and fcounter dataframes.
+        mod_name: Name of the Darshan module.
+        nprocs: Number of processes participating in accumulation.
+
+    Returns:
+        namedtuple containing derived_metrics (cdata object) and
+        summary_record (dict).
+    """
+    mod_idx = mod_name_to_idx(mod_name)
+    darshan_accumulator = ffi.new("darshan_accumulator *")
+    r = libdutil.darshan_accumulator_create(mod_idx, nprocs, darshan_accumulator)
+    if r != 0:
+        raise RuntimeError("A nonzero exit code was received from "
+                           "darshan_accumulator_create() at the C level. "
+                           f"This could mean that the {mod_name} module does not "
+                           "support derived metric calculation, or that "
+                           "another kind of error occurred. It may be possible "
+                           "to retrieve additional information from the stderr "
+                           "stream.")
+
+    num_recs = rec_dict["fcounters"].shape[0]
+    record_array = _df_to_rec(rec_dict, mod_name)
+
+    r_i = libdutil.darshan_accumulator_inject(darshan_accumulator[0], record_array, num_recs)
+    if r_i != 0:
+        raise RuntimeError("A nonzero exit code was received from "
+                           "darshan_accumulator_inject() at the C level. "
+                           "It may be possible "
+                           "to retrieve additional information from the stderr "
+                           "stream.")
+    derived_metrics = ffi.new("struct darshan_derived_metrics *")
+    summary_rbuf = ffi.new(_structdefs[mod_name].replace("**", "*"))
+    r = libdutil.darshan_accumulator_emit(darshan_accumulator[0],
+                                          derived_metrics,
+                                          summary_rbuf)
+    libdutil.darshan_accumulator_destroy(darshan_accumulator[0])
+    if r != 0:
+        raise RuntimeError("A nonzero exit code was received from "
+                           "darshan_accumulator_emit() at the C level. "
+                           "It may be possible "
+                           "to retrieve additional information from the stderr "
+                           "stream.")
+
+    summary_rec = _make_generic_record(summary_rbuf, mod_name, dtype='pandas')
+
+    # create namedtuple type to hold return values
+    AccumulatedRecords = namedtuple("AccumulatedRecords", ['derived_metrics', 'summary_record'])
+    return AccumulatedRecords(derived_metrics, summary_rec)
```

### Comparing `darshan-3.4.2.0/darshan/cli/__init__.py` & `darshan-3.4.3.0/darshan/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/cli/base.html` & `darshan-3.4.3.0/darshan/cli/base.html`

 * *Files 14% similar despite different names*

```diff
@@ -36,24 +36,29 @@
           % if len(report_data.sections[sect_title]) > 1:
             <!-- if more than 1 figure in section, use grid wrapper class -->
             <div class="grid-wrapper">
           % else:
             <div>
           % endif
 
-          % for fig_title, fig in report_data.sections[sect_title].items():
-            <div>
-            <h3>${fig_title}</h3>
+          % for fig in report_data.sections[sect_title]:
+            % if not fig.fig_grid_area:
+                <div>
+            % else:
+                <div class="${fig.fig_grid_area}">
+            % endif
+            <h3>${fig.fig_title}</h3>
             <figure style="width: ${fig.fig_width}px;">
             % if fig.fig_html:
               ${fig.fig_html}
               <figcaption>${fig.fig_description}</figcaption>
             % else:
               <!-- temporary handling for DXT-disabled cases -->
-              <figcaption style="font-weight: bold; color: red; width: 400px;">
+              <!-- now also handles the bandwidth text... -->
+              <figcaption style="font-weight: bold; color: ${fig.text_only_color}; width: 400px;">
                 ${fig.fig_description}
               </figcaption>
             % endif
           </figure>
           </div>
           % endfor
         </div>
```

#### html2text {}

```diff
@@ -6,16 +6,19 @@
 **** Job Summary ****
 ${report_data.metadata_table}
 **** Darshan Log Information ****
 ${report_data.module_table}   % for sect_title in report_data.sections:
 ***** ${sect_title} *****
 % if len(report_data.sections[sect_title]) > 1:
 % else:
-% endif % for fig_title, fig in report_data.sections[sect_title].items():
-**** ${fig_title} ****
- % if fig.fig_html: ${fig.fig_html} ${fig.fig_description} % else:   $
+% endif % for fig in report_data.sections[sect_title]: % if not
+fig.fig_grid_area:
+% else:
+% endif
+**** ${fig.fig_title} ****
+ % if fig.fig_html: ${fig.fig_html} ${fig.fig_description} % else:    $
 {fig.fig_description}  % endif
 % endfor
  % endfor
 ${report_data.footer}
 For more information visit the
 Darshan_website
```

### Comparing `darshan-3.4.2.0/darshan/cli/info.py` & `darshan-3.4.3.0/darshan/cli/info.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/cli/name_records.py` & `darshan-3.4.3.0/darshan/cli/name_records.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/cli/style.css` & `darshan-3.4.3.0/darshan/cli/style.css`

 * *Files 4% similar despite different names*

```diff
@@ -342,17 +342,16 @@
 
 figure img {
   background: white;
   padding: 0.25em;
 }
 
 figcaption {
-  font-style: italic;
   font-size: 0.75em;
-  font-weight: 200;
+  font-weight: 300;
   margin: 0;
 }
 
 abbr[title] {
   border-bottom: none;
   text-decoration: underline;
   text-decoration: underline dotted;
@@ -524,13 +523,30 @@
 }
 .fixed-header{
     top: 0;
 }
 .fixed-footer{
     bottom: 0;
 }
+
+.overview { grid-area: overview; font-weight: bold; }
+.file_tbl { grid-area: file_tbl; }
+.op_counts { grid-area: op_counts; }
+.acc_hist { grid-area: acc_hist; }
+.common_acc_tbl { grid-area: common_acc_tbl; }
+
+.overview tr:last-child td {
+   color: blue;
+}
+
 .grid-wrapper {
   display: grid;
-  /* set 2-column-wide grid with auto width scaling*/
+  /* set 2-column-wide grid with auto width scaling */
   grid-template-columns: repeat(2, auto);
+  /* explicit grid areas to control placement of module figures */
+  grid-template-areas:
+    'overview   overview'
+    'file_tbl   file_tbl'
+    'op_counts  .'
+    'acc_hist   common_acc_tbl';
   gap: 5px;
-}
+}
```

### Comparing `darshan-3.4.2.0/darshan/cli/summary.py` & `darshan-3.4.3.0/darshan/cli/summary.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import sys
 import os
 import io
 import base64
 import argparse
 import datetime
 from collections import OrderedDict
-if sys.version_info >= (3, 7):
-    import importlib.resources as importlib_resources
-else:
-    import importlib_resources
+import importlib.resources as importlib_resources
 
 from typing import Any, Union, Callable
 
 import pandas as pd
 from mako.template import Template
 
 import darshan
 import darshan.cli
+from darshan.backend.cffi_backend import accumulate_records
+from darshan.lib.accum import log_file_count_summary_table, log_module_overview_table
 from darshan.experimental.plots import (
     plot_dxt_heatmap,
     plot_io_cost,
     plot_common_access_table,
     plot_access_histogram,
     plot_opcounts,
+    plot_posix_access_pattern,
     data_access_by_filesystem,
 )
 
 darshan.enable_experimental()
 
 
 class ReportFigure:
@@ -43,36 +43,54 @@
 
     fig_args : the keyword arguments used for `fig_func`
 
     fig_description : description of the figure, typically used as the caption.
 
     fig_width : the width of the figure in pixels.
 
+    fig_grid_area : figure name corresponding to grid-area definitions specified in the CSS.
+
     """
     def __init__(
         self,
         section_title: str,
         fig_title: str,
         fig_func: Union[Callable, None],
         fig_args: dict,
         fig_description: str = "",
         fig_width: int = 500,
+        fig_grid_area: str = "",
+        # when there is no HTML data generated
+        # for the figure (i.e., no image/plot),
+        # we have the option of changing the caption
+        # text color for a warning/important standalone text
+        text_only_color: str = "red",
     ):
         self.section_title = section_title
         if not fig_title:
             fig_title = "&nbsp;"
         self.fig_title = fig_title
         self.fig_func = fig_func
         self.fig_args = fig_args
         self.fig_description = fig_description
         self.fig_width = fig_width
+        # grid areas should correspond to defintions of a grid-area
+        # in the CSS code (style.css)
+        # use of grid areas is optional -- if not specified,
+        # figures are placed in insertion order into first available
+        # open grid spaces in the default grid
+        self.fig_grid_area = fig_grid_area
         # temporary handling for DXT disabled cases
         # so special error message can be passed
         # in place of an encoded image
+        # NOTE: this code path is now also
+        # being used for adding the bandwidth
+        # text, which doesn't really have an image...
         self.fig_html = None
+        self.text_only_color = text_only_color
         if self.fig_func:
             self.generate_fig()
 
     @staticmethod
     def get_encoded_fig(mpl_fig: Any):
         """
         Encode a `matplotlib` figure using base64 encoding.
@@ -114,21 +132,30 @@
     """
     Collects all of the metadata, tables, and figures
     required to generate a Darshan Summary Report.
 
     Parameters
     ----------
     log_path: path to a darshan log file.
+    enable_dxt_heatmap: flag indicating whether DXT heatmaps should be enabled
 
     """
-    def __init__(self, log_path: str):
+    def __init__(self, log_path: str, enable_dxt_heatmap: bool = False):
         # store the log path and use it to generate the report
         self.log_path = log_path
+        self.enable_dxt_heatmap = enable_dxt_heatmap
         # store the report
-        self.report = darshan.DarshanReport(log_path, read_all=True)
+        self.report = darshan.DarshanReport(log_path, read_all=False)
+        # read only generic module data and heatmap data by default
+        self.report.read_all_generic_records()
+        if "HEATMAP" in self.report.data['modules']:
+            self.report.read_all_heatmap_records()
+        # if DXT heatmaps requested, additionally read-in DXT data
+        if self.enable_dxt_heatmap:
+            self.report.read_all_dxt_records()
         # create the header/footer
         self.get_header()
         self.get_footer()
         # create the metadata and module tables
         self.get_metadata_table()
         self.get_module_table()
         # register the report figures
@@ -320,14 +347,30 @@
         The order of the sections and figures is based on the order in which
         they are placed in `self.figures`. Since the DXT figure(s) are added
         first, they show up at the very top of the figure list.
 
         """
         self.figures = []
 
+        if not self.report.modules:
+            # no data in report to summarize, print warning and that's it
+            no_data_message = (
+                "This Darshan log file has no instrumentation records, "
+                "there is no data to plot. Did this app do any I/O?"
+            )
+            fig = ReportFigure(
+                section_title="",
+                fig_title="",
+                fig_func=None,
+                fig_args=None,
+                fig_description=no_data_message,
+            )
+            self.figures.append(fig)
+            return
+
         #########################################
         ## Add the runtime and/or DXT heat map(s)
         #########################################
         # if either or both modules are present, register their figures
         hmap_description = (
             "Heat map of I/O (in bytes) over time broken down by MPI rank. "
             "Bins are populated based on the number of bytes read/written in "
@@ -355,22 +398,38 @@
                                 fig_title=f"Heat Map: {mod} {possible_submodule}",
                                 fig_func=plot_dxt_heatmap.plot_heatmap,
                                 fig_args=dict(report=self.report, mod=mod, submodule=possible_submodule),
                                 fig_description=hmap_description,
                             )
                             hmap_grid[f"HEATMAP_{possible_submodule}"] = heatmap_fig
                     else:
-                        heatmap_fig = ReportFigure(
-                            section_title="I/O Summary",
-                            fig_title=f"Heat Map: {mod}",
-                            fig_func=plot_dxt_heatmap.plot_heatmap,
-                            fig_args=dict(report=self.report, mod=mod),
-                            fig_description=hmap_description,
-                        )
-                        hmap_grid[mod] = heatmap_fig
+                        if self.enable_dxt_heatmap:
+                            heatmap_fig = ReportFigure(
+                                section_title="I/O Summary",
+                                fig_title=f"Heat Map: {mod}",
+                                fig_func=plot_dxt_heatmap.plot_heatmap,
+                                fig_args=dict(report=self.report, mod=mod),
+                                fig_description=hmap_description,
+                            )
+                            hmap_grid[mod] = heatmap_fig
+                        else:
+                            temp_message = (
+                                f"{mod} trace data available, but DXT-based heatmaps are "
+                                "not currently generated by default by the job summary tool. "
+                                "To force generation of heatmaps based on DXT trace data, users "
+                                "can specify the '--enable_dxt_heatmap' option."
+                            )
+                            fig = ReportFigure(
+                                section_title="I/O Summary",
+                                fig_title=f"Heat Map: {mod}",
+                                fig_func=None,
+                                fig_args=None,
+                                fig_description=temp_message,
+                            )
+                            hmap_grid[mod] = fig
             for heatmap_fig in hmap_grid.values():
                 if heatmap_fig:
                     self.figures.append(heatmap_fig)
         else:
             url = (
                 "https://www.mcs.anl.gov/research/projects/darshan/docs/darshan"
                 "-runtime.html#_using_the_darshan_extended_tracing_dxt_module"
@@ -401,15 +460,16 @@
         # add the I/O cost stacked bar graph
         url = "https://www.mcs.anl.gov/research/projects/darshan/docs/darshan-util.html"
 
         io_cost_description = (
             "Average (across all ranks) amount of run time that each process "
             "spent performing I/O, broken down by access type. See the right "
             "edge bar graph on heat maps in preceding section to indicate if "
-            "I/O activity was balanced across processes."
+            "I/O activity was balanced across processes. The 'Wait' category "
+            "is only meaningful for PNETCDF asynchronous I/O operations."
         )
         io_cost_params = {
             "section_title": "Cross-Module Comparisons",
             "fig_title": "I/O Cost",
             "fig_func": plot_io_cost,
             "fig_args": dict(report=self.report),
             "fig_description": io_cost_description,
@@ -441,27 +501,83 @@
             if "H5" in mod:
                 sect_title = "Per-Module Statistics: HDF5"
             elif "PNETCDF" in mod:
                 sect_title = "Per-Module Statistics: PNETCDF"
             else:
                 sect_title = f"Per-Module Statistics: {mod}"
 
+            try:
+                if mod in ["POSIX", "MPI-IO", "STDIO"]:
+                    # get the module's record dataframe and then pass to
+                    # Darshan accumulator interface to generate a cumulative
+                    # record and derived metrics
+                    rec_dict = self.report.records[mod].to_df()
+                    acc = accumulate_records(rec_dict, mod, self.report.metadata['job']['nprocs'])
+
+                    mod_overview_fig = ReportFigure(
+                            section_title=sect_title,
+                            fig_title=f"Overview",
+                            fig_func=log_module_overview_table,
+                            fig_args=dict(derived_metrics=acc.derived_metrics,
+                                          mod_name=mod),
+                            fig_width=805,
+                            fig_description="",
+                            fig_grid_area="overview")
+                    self.figures.append(mod_overview_fig)
+
+                    file_count_summary_fig = ReportFigure(
+                            section_title=sect_title,
+                            fig_title=f"File Count Summary <br> (estimated by {mod} I/O access offsets)",
+                            fig_func=log_file_count_summary_table,
+                            fig_args=dict(derived_metrics=acc.derived_metrics,
+                                          mod_name=mod),
+                            fig_width=805,
+                            fig_description="",
+                            fig_grid_area="file_tbl")
+                    self.figures.append(file_count_summary_fig)
+
+                    if mod == "POSIX":
+                        access_pattern_fig = ReportFigure(
+                            section_title=sect_title,
+                            fig_title="Access Pattern",
+                            fig_func=plot_posix_access_pattern,
+                            fig_args=dict(record=acc.summary_record),
+                            fig_description="Sequential (offset greater than previous offset) vs. "
+                                            "consecutive (offset immediately following previous offset) "
+                                            "file operations. Note that, by definition, the sequential "
+                                            "operations are inclusive of consecutive operations.",
+                            fig_width=350
+                        )
+                        self.figures.append(access_pattern_fig)
+
+            except (RuntimeError, KeyError):
+                # the module probably doesn't support derived metrics
+                # calculations, but the C code doesn't distinguish other
+                # types of errors
+
+                # the KeyError appears to be needed for a subset of logs
+                # for which _structdefs lacks APMPI or APXC entries;
+                # for example `e3sm_io_heatmap_only.darshan` in logs
+                # repo
+                pass
+
             if mod in ["POSIX", "MPI-IO", "H5D", "PNETCDF_VAR"]:
                 access_hist_description = (
                     "Histogram of read and write access sizes. The specific values "
                     "of the most frequently occurring access sizes can be found in "
                     "the <i>Common Access Sizes</i> table."
                 )
                 access_hist_fig = ReportFigure(
                     section_title=sect_title,
                     fig_title="Access Sizes",
                     fig_func=plot_access_histogram,
                     fig_args=dict(report=self.report, mod=mod),
                     fig_description=access_hist_description,
                     fig_width=350,
+                    fig_grid_area="acc_hist"
                 )
                 self.figures.append(access_hist_fig)
                 if mod == "MPI-IO":
                     com_acc_tbl_description = (
                         "NOTE: MPI-IO accesses are given in "
                         "terms of aggregate datatype size."
                     )
@@ -470,29 +586,32 @@
                 com_acc_tbl_fig = ReportFigure(
                     section_title=sect_title,
                     fig_title="Common Access Sizes",
                     fig_func=plot_common_access_table.plot_common_access_table,
                     fig_args=dict(report=self.report, mod=mod),
                     fig_description=com_acc_tbl_description,
                     fig_width=350,
+                    fig_grid_area="common_acc_tbl"
                 )
                 self.figures.append(com_acc_tbl_fig)
 
             # add the operation counts figure
             if mod in opcounts_mods:
                 opcount_fig = ReportFigure(
                     section_title=sect_title,
                     fig_title="Operation Counts",
                     fig_func=plot_opcounts,
                     fig_args=dict(report=self.report, mod=mod),
                     fig_description="Histogram of I/O operation frequency.",
                     fig_width=350,
+                    fig_grid_area="op_counts"
                 )
                 self.figures.append(opcount_fig)
 
+
         #########################
         # Data Access by Category
         if not {"POSIX", "STDIO"}.isdisjoint(set(self.report.modules)):
             data_access_by_cat_fig = ReportFigure(
                 section_title="Data Access by Category",
                 fig_title="",
                 fig_func=data_access_by_filesystem.plot_with_report,
@@ -511,20 +630,20 @@
         """
         Uses figure info to generate the unique sections
         and places the figures in their sections.
         """
         self.sections = {}
         for fig in self.figures:
             # if a section title is not already in sections, add
-            # the section title and a corresponding empty dictionary
+            # the section title and a corresponding empty list
             # to store its figures
             if fig.section_title not in self.sections:
-                self.sections[fig.section_title] = {}
+                self.sections[fig.section_title] = []
             # add the image to its corresponding section
-            self.sections[fig.section_title][fig.fig_title] = fig
+            self.sections[fig.section_title].append(fig)
 
 
 def setup_parser(parser: argparse.ArgumentParser):
     """
     Configures the command line arguments.
 
     Parameters
@@ -535,15 +654,25 @@
     parser.description = "Generates a Darshan Summary Report"
 
     parser.add_argument(
         "log_path",
         type=str,
         help="Specify path to darshan log.",
     )
-    parser.add_argument("--output", type=str, help="Specify output filename.")
+    parser.add_argument(
+        "--output",
+        type=str,
+        help="Specify output filename."
+    )
+    # DXT-based heatmap generation can be expensive, so it is opt-in for now
+    parser.add_argument(
+        "--enable_dxt_heatmap",
+        action="store_true",
+        help="Enable DXT-based versions of I/O activity heatmaps."
+    )
 
 
 def main(args: Union[Any, None] = None):
     """
     Generates a Darshan Summary Report.
 
     Parameters
@@ -553,25 +682,29 @@
     """
     if args is None:
         parser = argparse.ArgumentParser(description="")
         setup_parser(parser)
         args = parser.parse_args()
 
     log_path = args.log_path
+    enable_dxt_heatmap = args.enable_dxt_heatmap
 
     if args.output is None:
         # if no output is provided, use the log file
         # name to create the output filename
         log_filename = os.path.splitext(os.path.basename(log_path))[0]
         report_filename = f"{log_filename}_report.html"
     else:
         report_filename = args.output
 
     # collect the report data to feed into the template
-    report_data = ReportData(log_path=log_path)
+    report_data = ReportData(
+        log_path=log_path,
+        enable_dxt_heatmap=enable_dxt_heatmap
+    )
 
     with importlib_resources.path(darshan.cli, "base.html") as base_path:
         # load a template object using the base template
         template = Template(filename=str(base_path))
         # render the base template
         stream = template.render(report_data=report_data)
         with open(report_filename, "w") as f:
```

### Comparing `darshan-3.4.2.0/darshan/cli/to_json.py` & `darshan-3.4.3.0/darshan/cli/to_json.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/datatypes/heatmap.py` & `darshan-3.4.3.0/darshan/datatypes/heatmap.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/discover_darshan.py` & `darshan-3.4.3.0/darshan/discover_darshan.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,23 +82,23 @@
     path to a shared object for use with Python's CFFI.
 
     :return: Path to a darshan-util installation.
     """
 
     import subprocess
 
-    args = ['pkg-config', '--path', 'darshan-util']
+    args = ['pkg-config', '--variable=prefix', 'darshan-util']
     p = subprocess.Popen(args, shell=False, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd='.')
     out,err = p.communicate()
     retval = p.wait()
 
-    path = os.path.dirname(out.decode('ascii').strip())
+    path = out.decode('ascii').strip()
 
     if path:
-        return os.path.realpath(path + '/../../')
+        return os.path.realpath(path)
     else:
         raise RuntimeError('Could not discover darshan! Is darshan-util installed?')
 
 
 def discover_darshan_shutil():
     """
     Discovers an existing darshan-util installation and returns the appropriate
@@ -159,14 +159,28 @@
 
     Args:
         ffi: existing ffi instance to use
         libdutil: reference to libdutil to populate
 
     """
     if libdutil is None:
+        # prefer wheel library discovery method
+        try:
+            darshan_path = discover_darshan_wheel()
+            import glob
+            library_path = glob.glob(f'{darshan_path}/libdarshan-util*.so*')[0]
+            logger.debug(f"Attempting library_path={library_path} in case of binary wheel.")
+            save = os.getcwd()
+            os.chdir(darshan_path)
+            libdutil = ffi.dlopen(library_path)
+            os.chdir(save)
+        except:
+            libdutil = None
+
+    if libdutil is None:
         try:
             libdutil = ffi.dlopen("libdarshan-util.so")
         except:
             libdutil = None
 
     if libdutil is None:
         try:
@@ -188,27 +202,14 @@
             logger.debug(f"Attempting library_path={library_path} via pkgconfig discovery.")
             libdutil = ffi.dlopen(library_path + "/lib/libdarshan-util.so")
         except:
             libdutil = None
 
     if libdutil is None:
         try:
-            darshan_path = discover_darshan_wheel()
-            import glob
-            library_path = glob.glob(f'{darshan_path}/libdarshan-util*.so*')[0]
-            logger.debug(f"Attempting library_path={library_path} in case of binary wheel.")
-            save = os.getcwd()
-            os.chdir(darshan_path)
-            libdutil = ffi.dlopen(library_path)
-            os.chdir(save)
-        except:
-            libdutil = None
-    
-    if libdutil is None:
-        try:
             darshan_path = discover_darshan_pyinstaller()
             import glob
             library_path = glob.glob(f'{darshan_path}/libdarshan-util*.so*')[0]
             logger.debug(f"Attempting library_path={library_path} for pyinstaller bundles.")
             save = os.getcwd()
             os.chdir(darshan_path)
             libdutil = ffi.dlopen(library_path)
```

### Comparing `darshan-3.4.2.0/darshan/examples/darshan-graph/app.c` & `darshan-3.4.3.0/darshan/examples/darshan-graph/app.c`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/darshan-graph/app_rw_mpiio.c` & `darshan-3.4.3.0/darshan/examples/darshan-graph/app_rw_mpiio.c`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/darshan-graph/pq_app_readAB_writeC_id71326_7-31-5658-2037904274838284930_55623.darshan` & `darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_readAB_writeC_id71326_7-31-5658-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/darshan-graph/pq_app_read_id71317_7-31-5657-2037904274838284930_55623.darshan` & `darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_read_id71317_7-31-5657-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/darshan-graph/pq_app_read_id71344_7-31-5658-2037904274838284930_55623.darshan` & `darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_read_id71344_7-31-5658-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/darshan-graph/pq_app_write_id71296_7-31-5657-2037904274838284930_55623.darshan` & `darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_write_id71296_7-31-5657-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/darshan-graph/pq_app_write_id71303_7-31-5657-2037904274838284930_55623.darshan` & `darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_write_id71303_7-31-5657-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/darshan-graph/pq_app_write_id71310_7-31-5657-2037904274838284930_55623.darshan` & `darshan-3.4.3.0/darshan/examples/darshan-graph/pq_app_write_id71310_7-31-5657-2037904274838284930_55623.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/darshan-graph/run.sh` & `darshan-3.4.3.0/darshan/examples/darshan-graph/run.sh`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/example_logs/dxt.darshan` & `darshan-3.4.3.0/darshan/examples/example_logs/dxt.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/example_logs/example.darshan` & `darshan-3.4.3.0/darshan/examples/example_logs/example.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/example_logs/ior_hdf5_example.darshan` & `darshan-3.4.3.0/darshan/examples/example_logs/ior_hdf5_example.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/example_logs/noposix.darshan` & `darshan-3.4.3.0/darshan/examples/example_logs/noposix.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/example_logs/sample-badost.darshan` & `darshan-3.4.3.0/darshan/examples/example_logs/sample-badost.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/example_logs/shane_macsio_id29959_5-22-32552-7035573431850780836_1590156158.darshan` & `darshan-3.4.3.0/darshan/examples/example_logs/shane_macsio_id29959_5-22-32552-7035573431850780836_1590156158.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/examples/tutorial/tojson.py` & `darshan-3.4.3.0/darshan/examples/tutorial/tojson.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/aggregators/agg_ioops.py` & `darshan-3.4.3.0/darshan/experimental/aggregators/agg_ioops.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/aggregators/create_dxttimeline.py` & `darshan-3.4.3.0/darshan/experimental/aggregators/create_dxttimeline.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/aggregators/create_sankey.py` & `darshan-3.4.3.0/darshan/experimental/aggregators/create_sankey.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/aggregators/create_time_summary.py` & `darshan-3.4.3.0/darshan/experimental/aggregators/create_time_summary.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/aggregators/create_timeline.py` & `darshan-3.4.3.0/darshan/experimental/aggregators/create_timeline.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/aggregators/mod_agg_iohist.py` & `darshan-3.4.3.0/darshan/experimental/aggregators/mod_agg_iohist.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/aggregators/name_records_summary.py` & `darshan-3.4.3.0/darshan/experimental/aggregators/name_records_summary.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/aggregators/print_module_records.py` & `darshan-3.4.3.0/darshan/experimental/aggregators/print_module_records.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/aggregators/records_as_dict.py` & `darshan-3.4.3.0/darshan/experimental/aggregators/records_as_dict.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/aggregators/summarize.py` & `darshan-3.4.3.0/darshan/experimental/aggregators/summarize.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/operations/filter.py` & `darshan-3.4.3.0/darshan/experimental/operations/filter.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/operations/merge.py` & `darshan-3.4.3.0/darshan/experimental/operations/merge.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/operations/reduce.py` & `darshan-3.4.3.0/darshan/experimental/operations/reduce.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/plots/data_access_by_filesystem.py` & `darshan-3.4.3.0/darshan/experimental/plots/data_access_by_filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import numpy as np
 import pandas as pd
 import darshan
 import matplotlib
 matplotlib.use('Agg')
 import matplotlib.pyplot as plt
-
+import humanize
 
 def process_byte_counts(df_reads, df_writes):
     """
     Given separate dataframes for read/write IO activity,
     returns separate pandas Series objects with the counts
     of bytes read or written per filesystem root.
 
@@ -501,25 +501,26 @@
     counts of bytes written
 
     filesystem_roots: a sequence of strings containing unique filesystem root paths
 
     num_cats: an integer representing the number of categories
     to plot; default ``None`` plots all categories
     """
+    fontsize = 18
     list_byte_axes: list = []
     list_count_axes: list = []
     # use log10 scale if range exceeds
     # two orders of magnitude in a column
     use_log = [False, False]
-    for idx, series_pair in enumerate([[bytes_rd_series, bytes_wr_series, 1048576],
-                                       [file_rd_series, file_wr_series, 1]]):
+    for idx, series_pair in enumerate([[bytes_rd_series, bytes_wr_series],
+                                       [file_rd_series, file_wr_series]]):
         maxval = max(series_pair[0].max(), series_pair[1].max())
         minval = max(min(series_pair[0].min(), series_pair[1].min()), 1)
         # adjust ratio to MiB when needed
-        ratio = ((maxval / series_pair[2]) / (minval / series_pair[2]))
+        ratio = (maxval / minval)
         if ratio > 100:
             use_log[idx] = True
 
     if num_cats is None:
         num_cats = len(filesystem_roots)
 
     for row, filesystem in enumerate(bytes_rd_series.index[:num_cats]):
@@ -536,72 +537,63 @@
             ax_filesystem_counts.sharex(list_count_axes[row - 1])
             if use_log[1]:
                 ax_filesystem_counts.set_xscale('symlog')
 
         list_byte_axes.append(ax_filesystem_bytes)
         list_count_axes.append(ax_filesystem_counts)
 
-        # convert to MiB using 1048576 (ie: 2**20)
-        bytes_read = bytes_rd_series[filesystem]/1048576
-        bytes_written = bytes_wr_series[filesystem]/1048576
-        files_written = file_wr_series[filesystem]
-        files_read = file_rd_series[filesystem]
-
-        # scale to fit longer filesystem
-        # strings on the left side of the plots
-        # NOTE: may need more sophisticated scaling
-        # eventually
-        if len(filesystem) <= 8 and not '<STD' in filesystem:
-            fontsize = 18
-        else:
-            fontsize = 12
+        bytes_read = bytes_rd_series[filesystem]
+        bytes_written = bytes_wr_series[filesystem]
+        files_written = int(file_wr_series[filesystem])
+        files_read = int(file_rd_series[filesystem])
 
         # anonymized STD.. streams have associated integers
         # that are stored in the filesystem data field
         # but that are confusing to display, so strip them
         if filesystem.startswith('anonymized'):
             ax_filesystem_bytes.annotate('anonymized',
-                                         (-0.3, 0.5),
+                                         (-0.1, 0.5),
                                          fontsize=fontsize,
                                          xycoords='axes fraction',
+                                         ha="right",
                                          va="center")
         else:
             ax_filesystem_bytes.annotate(filesystem,
-                                         (-0.3, 0.5),
+                                         (-0.1, 0.5),
                                          fontsize=fontsize,
                                          xycoords='axes fraction',
+                                         ha="right",
                                          va="center")
 
         ax_filesystem_counts.barh(0, files_written, color='red', alpha=0.3)
         ax_filesystem_counts.barh(1, files_read, color='blue', alpha=0.3)
 
-        ax_filesystem_bytes.text(0, 0.75, f' # bytes read ({bytes_read:.2E} MiB)',
+        bytes_read_str = humanize.naturalsize(bytes_read,
+                                              binary=True,
+                                              format="%.2f")
+        ax_filesystem_bytes.text(0, 0.75, f' bytes read: {bytes_read_str}',
                                  transform=ax_filesystem_bytes.transAxes,
+                                 fontsize=fontsize,
                                  va="center")
-        ax_filesystem_bytes.text(0, 0.25, f' # bytes written ({bytes_written:.2E} MiB)',
+        bytes_written_str = humanize.naturalsize(bytes_written,
+                                                 binary=True,
+                                                 format="%.2f")
+        ax_filesystem_bytes.text(0, 0.25, f' bytes written: {bytes_written_str}',
                                  transform=ax_filesystem_bytes.transAxes,
+                                 fontsize=fontsize,
                                  va="center")
 
-        if files_read == 0:
-            ax_filesystem_counts.text(0, 0.75, ' 0 files read',
-                                      transform=ax_filesystem_counts.transAxes,
-                                      va="center")
-        else:
-            ax_filesystem_counts.text(0, 0.75, f' # files read ({files_read:.2E})',
-                                      transform=ax_filesystem_counts.transAxes,
-                                      va="center")
-
-        if files_written == 0:
-            ax_filesystem_counts.text(0, 0.25, ' 0 files written',
-                                      transform=ax_filesystem_counts.transAxes,
-                                      va="center")
-        else:
-            ax_filesystem_counts.text(0, 0.25, f' # files written ({files_written:.2E})',
-                                      transform=ax_filesystem_counts.transAxes,
-                                      va="center")
+        ax_filesystem_counts.text(0, 0.75, f' files read: {files_read}',
+                                  transform=ax_filesystem_counts.transAxes,
+                                  fontsize=fontsize,
+                                  va="center")
+        ax_filesystem_counts.text(0, 0.25, f' files written: {files_written}',
+                                  transform=ax_filesystem_counts.transAxes,
+                                  fontsize=fontsize,
+                                  va="center")
 
         ax_filesystem_bytes.barh(0, bytes_written, color='red', alpha=0.3)
         ax_filesystem_bytes.barh(1, bytes_read, color='blue', alpha=0.3)
 
         for axis in fig.axes:
             # hide the right side plot frame (spine) so that
             # the value labels don't overlap with the plot frame
@@ -692,11 +684,12 @@
               filesystem_roots,
               num_cats=num_cats)
 
     # at least this much height seems to
     # produce a decent aspect ratio
     if height < 16:
         height = 16
-
+    # add additional padding to left margin for annotations
+    fig.subplots_adjust(left=0.2)
     fig.set_size_inches(12, height)
     plt.close(fig)
     return fig
```

### Comparing `darshan-3.4.2.0/darshan/experimental/plots/heatmap_handling.py` & `darshan-3.4.3.0/darshan/experimental/plots/heatmap_handling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Module of data pre-processing functions for constructing the heatmap figure.
 """
 
-from typing import Dict, Any, Tuple, Sequence, TYPE_CHECKING
+from typing import Dict, Any, Tuple, Sequence, TYPE_CHECKING, Optional
 
 import sys
 
 if sys.version_info >= (3, 8):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -269,15 +269,18 @@
         agg_df = pd.concat(df_list, ignore_index=True)
     else:
         raise ValueError("No data available for selected module(s) and operation(s).")
 
     return agg_df
 
 
-def get_heatmap_df(agg_df: pd.DataFrame, xbins: int, nprocs: int) -> pd.DataFrame:
+def get_heatmap_df(agg_df: pd.DataFrame,
+                   xbins: int,
+                   nprocs: int,
+                   max_time: Optional[float] = None) -> pd.DataFrame:
     """
     Builds an array similar to a 2D-histogram, where the y data is the unique
     ranks and the x data is time. Each bin is populated with the data sum
     and/or proportionate data sum for all IO events read/written during the
     time spanned by the bin.
 
     Parameters
@@ -286,14 +289,17 @@
     agg_df: a ``pd.DataFrame`` containing the aggregated data determined
     by the input modules and operations.
 
     xbins: the number of x-axis bins to create.
 
     nprocs: the number of MPI ranks/processes used at runtime.
 
+    max_time: the maximum time, since input DXT data is not necessarily
+              bounded by wallclock duration
+
     Returns
     -------
 
     hmap_df: dataframe with time intervals for columns and rank
     index (0, 1, etc.) for rows, where each element contains the data
     read/written by the corresponding rank in the given time interval.
 
@@ -308,20 +314,25 @@
         1                   3.746313e+05
         2                   6.350999e+05
         3                   1.048576e+06
 
     """
     # generate the bin edges by generating an array of length n_bins+1, then
     # taking pairs of data points as the min/max bin value
-    max_time = agg_df["end_time"].max()
+    if max_time is None:
+        max_time = agg_df["end_time"].max()
     bin_edge_data = np.linspace(0.0, max_time, xbins + 1)
     # create dummy variables for start/end time data, where dataframe columns
     # are the x-axis bin ranges
+    # pin dtype here because of pandas 2.0+ change--see:
+    # gh-909 and
+    # https://github.com/pandas-dev/pandas/pull/48022#issuecomment-1448755561
     cats_start = pd.get_dummies(
-        pd.cut(agg_df["start_time"], bin_edge_data, precision=16)
+        pd.cut(agg_df["start_time"], bin_edge_data, precision=16),
+        dtype=np.uint8,
     )
     cats_end = pd.get_dummies(pd.cut(agg_df["end_time"], bin_edge_data, precision=16))
     # get series for the elapsed times for each dxt segment
     elapsed_times_dxt_segments = agg_df["end_time"] - agg_df["start_time"]
     # calculate the time interval spanned by each bin
     bin_size = bin_edge_data[1] - bin_edge_data[0]
     # get the ratio of the bin time interval over the dxt segment elapsed times
```

### Comparing `darshan-3.4.2.0/darshan/experimental/plots/plot_access_histogram.py` & `darshan-3.4.3.0/darshan/experimental/plots/plot_access_histogram.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
 def autolabel(ax, rects):
     """Attach a text label above each bar in *rects*, displaying its value."""
     for rect in rects:
         height = rect.get_height()
-        ax.annotate(
-            '{}'.format(height),
-            xy=(rect.get_x() + rect.get_width() / 2, height),
-            xytext=(0, 3),  # 3 points vertical offset
-            textcoords="offset points",
-            ha='center',
-            va='bottom',
-            rotation=0,
-        )
+        if height > 0:
+            ax.annotate(
+                '{}'.format(height),
+                xy=(rect.get_x() + rect.get_width() / 2, height),
+                xytext=(0, 3),  # 3 points vertical offset
+                textcoords="offset points",
+                ha='center',
+                va='bottom',
+                rotation=45,
+            )
 
 def plot_access_histogram(report, mod, ax=None):
     """
     Plots a histogram of access sizes for specified module.
 
 	Args:
 		report (darshan.DarshanReport): report to generate plot from
@@ -77,16 +78,19 @@
     rects2 = ax.bar(x + width/2, write_vals, width, label='Write')
 
     # Add some text for labels, title and custom x-axis tick labels, etc.
     ax.set_ylabel('Count')
     ax.set_xlabel('Access Sizes')
     ax.set_xticks(x)
     ax.set_xticklabels(labels, rotation=45, ha='right')
+    ax.set_ylim(ymin = 0)
     ax.legend()
 
+    ax.spines[['right', 'top']].set_visible(False)
+
     autolabel(ax=ax, rects=rects1)
     autolabel(ax=ax, rects=rects2)
 
     plt.tight_layout()
 
     if fig is not None:
         plt.close()
```

### Comparing `darshan-3.4.2.0/darshan/experimental/plots/plot_common_access_table.py` & `darshan-3.4.3.0/darshan/experimental/plots/plot_common_access_table.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/plots/plot_dxt_heatmap.py` & `darshan-3.4.3.0/darshan/experimental/plots/plot_dxt_heatmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 """
 Module for creating the ranks vs. time IO intensity
 heatmap figure for the Darshan job summary.
 """
 
+from __future__ import annotations
 import functools
 from typing import (Any, List, Sequence, Union,
                     TYPE_CHECKING, Tuple, Optional)
 
 import numpy as np
 
 if TYPE_CHECKING:
     import numpy.typing as npt
 
-# we can't use PEP563 delayed type
-# evaluations while we have to support
-# Python 3.6 because the __future__ import is not
-# available yet;
-# TODO: delete the mocking and restore the
-# from __future__ import annotations
-from unittest.mock import MagicMock
-npt = MagicMock()
-
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 from matplotlib.colors import LogNorm
 
 import darshan
 from darshan.experimental.plots import heatmap_handling
@@ -49,16 +41,16 @@
     A tuple containing `tmax`, `runtime` floats.
 
     """
     # get the elapsed runtime
     runtime = report.metadata["job"]["run_time"]
     # leverage higher resolution DXT timing
     # data if available
-    if ("DXT_POSIX" in report.modules or
-        "DXT_MPIIO" in report.modules):
+    if ("DXT_POSIX" in report.records or
+        "DXT_MPIIO" in report.records):
         tmax = 0.0
         for mod in report.modules:
             if "DXT" in mod:
                 agg_df = heatmap_handling.get_aggregate_data(report=report,
                                                              mod=mod,
                                                              ops=["read", "write"])
                 tmax_dxt = float(agg_df["end_time"].max())
@@ -360,20 +352,28 @@
     if "DXT" not in mod and "HEATMAP" not in mod:
         raise NotImplementedError("Only DXT and HEATMAP modules are supported.")
 
     if mod not in report.modules:
         raise ValueError(f"Module {mod} not found in DarshanReport.")
 
     nprocs = report.metadata["job"]["nprocs"]
+    tmax, runtime = determine_hmap_runtime(report=report)
 
     if "DXT" in mod:
         # aggregate the data according to the selected modules and operations
         agg_df = heatmap_handling.get_aggregate_data(report=report, mod=mod, ops=ops)
         # get the heatmap data array
-        hmap_df = heatmap_handling.get_heatmap_df(agg_df=agg_df, xbins=xbins, nprocs=nprocs)
+        # NOTE: the darshan runtime does not collect empty DXT records,
+        # so we are not guaranteed to have data for all time spans
+        # as a result, we force the upper time bound for the heatmap data
+        # to be the wallclock time
+        hmap_df = heatmap_handling.get_heatmap_df(agg_df=agg_df,
+                                                  xbins=xbins,
+                                                  nprocs=nprocs,
+                                                  max_time=runtime)
     elif mod == "HEATMAP":
         hmap_df = report.heatmaps[submodule].to_df(ops=ops)
         # mirror the DXT approach to heatmaps by
         # adding all-zero rows for inactive ranks
         hmap_df = hmap_df.reindex(index=range(nprocs), fill_value=0.0)
         xbins = hmap_df.shape[1]
 
@@ -431,15 +431,14 @@
     jgrid.ax_marg_x.bar(
         x=np.arange(xbins),
         height=hmap_df.sum(axis=0),
         facecolor="black",
         align="edge",
     )
 
-    tmax, runtime = determine_hmap_runtime(report=report)
     # scale the x-axis to span the calculated run time
     xbin_max = xbins * (runtime / tmax)
     jgrid.ax_joint.set_xlim(0.0, xbin_max)
     # set the x and y tick locations and labels using the runtime
     set_x_axis_ticks_and_labels(jointgrid=jgrid, tmax=runtime, bin_max=xbin_max, n_xlabels=4)
     set_y_axis_ticks_and_labels(jointgrid=jgrid, n_ylabels=6)
```

### Comparing `darshan-3.4.2.0/darshan/experimental/plots/plot_dxt_heatmap2.py` & `darshan-3.4.3.0/darshan/experimental/plots/plot_dxt_heatmap2.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/experimental/plots/plot_io_cost.py` & `darshan-3.4.3.0/darshan/experimental/plots/plot_io_cost.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,28 +26,33 @@
     bar graph for (i.e. "POSIX", "MPI-IO", "STDIO").
 
     nprocs: the number of MPI ranks used for the log of interest.
 
     Returns
     -------
     by_avg_series: a ``pd.Series`` containing the
-    average read, write, and meta times.
+    average read, write, meta, and wait times.
 
     """
     # filter out all except the following columns
     cols = [
         f"{mod_key}_F_READ_TIME",
         f"{mod_key}_F_WRITE_TIME",
         f"{mod_key}_F_META_TIME",
     ]
+    if "PNETCDF_FILE" in mod_key:
+        cols.append("PNETCDF_FILE_F_WAIT_TIME")
+    else:
+        cols.append("Wait")
     by_avg_series = df.filter(cols, axis=1).sum(axis=0) / nprocs
     # reindex to ensure 3 rows are always created
     by_avg_series = by_avg_series.reindex(cols, fill_value=0.0)
     # rename the columns so the labels are automatically generated when plotting
     name_dict = {cols[0]: "Read", cols[1]: "Write", cols[2]: "Meta"}
+    name_dict[cols[3]] = "Wait"
     by_avg_series.rename(index=name_dict, inplace=True)
     return by_avg_series
 
 
 def combine_hdf5_modules(df: Any) -> Any:
     """
     Combines the "H5F" and "H5D" rows in the input dataframe into
@@ -169,12 +174,17 @@
     n_ticks = len(ax_norm.get_yticks())
     yticks = np.linspace(0, runtime, n_ticks)
     ax_raw.set_yticks(yticks)
     # add the legend and appropriate labels
     ax_raw.set_ylabel("Runtime (s)")
     handles, labels = ax_raw.get_legend_handles_labels()
     ax_norm.legend(handles[::-1], labels[::-1], loc="upper left", bbox_to_anchor=(1.22, 1.02))
+    ax_norm.set_ylabel("Runtime (%)")
+    # rotate the xticklabels so they don't overlap
+    for ax in [ax_raw, ax_norm]:
+        for label in ax.get_xticklabels():
+            label.set_rotation(90)
     # adjust the figure to reduce white space
     io_cost_fig.subplots_adjust(right=0.59)
     io_cost_fig.tight_layout()
     plt.close()
     return io_cost_fig
```

### Comparing `darshan-3.4.2.0/darshan/experimental/plots/plot_opcounts.py` & `darshan-3.4.3.0/darshan/experimental/plots/plot_opcounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 import numpy as np
 
 
 def autolabel(ax, rects):
     """Attach a text label above each bar in *rects*, displaying its height."""
     for rect in rects:
         height = rect.get_height()
-        ax.annotate(
-            '{}'.format(height),
-            xy=(rect.get_x() + rect.get_width() / 2, height),
-            xytext=(0, 3),  # 3 points vertical offset
-            textcoords="offset points",
-            ha='center',
-            va='bottom',
-            rotation=45,
-        )
+        if height > 0:
+            ax.annotate(
+                '{}'.format(height),
+                xy=(rect.get_x() + rect.get_width() / 2, height),
+                xytext=(0, 3),  # 3 points vertical offset
+                textcoords="offset points",
+                ha='center',
+                va='bottom',
+                rotation=45,
+            )
 
 def gather_count_data(report, mod):
     """
     Collect the module counts and labels
     for the I/O Operation Count plot.
     """
     # TODO: change to report.summary
@@ -180,14 +181,17 @@
     x = np.arange(len(labels))  # the label locations
     rects = ax.bar(x, counts)
 
     # Add some text for labels, title and custom x-axis tick labels, etc.
     ax.set_ylabel('Count')
     ax.set_xticks(x)
     ax.set_xticklabels(labels, rotation=90)
+    ax.set_ylim(ymin = 0)
+
+    ax.spines[['right', 'top']].set_visible(False)
 
     autolabel(ax=ax, rects=rects)
 
     plt.tight_layout()
 
     if fig is not None:
         plt.close()
```

### Comparing `darshan-3.4.2.0/darshan/experimental/transforms/dxt2png.py` & `darshan-3.4.3.0/darshan/experimental/transforms/dxt2png.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/log_utils.py` & `darshan-3.4.3.0/darshan/log_utils.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/report.py` & `darshan-3.4.3.0/darshan/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -657,14 +657,17 @@
         dtype = dtype if dtype else self.dtype
 
 
         self.records[mod] = DarshanRecordCollection(mod=mod, report=self)
         cn = backend.counter_names(mod)
         fcn = backend.fcounter_names(mod)
 
+        if mod not in self._modules:
+            raise ValueError(f"mod {mod} is not available in this DarshanReport object.")
+
         # update module metadata
         self._modules[mod]['num_records'] = 0
         if mod not in self.counters:
             self.counters[mod] = {}
             self.counters[mod]['counters'] = cn 
             self.counters[mod]['fcounters'] = fcn
```

### Comparing `darshan-3.4.2.0/darshan/tests/conftest.py` & `darshan-3.4.3.0/darshan/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/input/noposix.darshan` & `darshan-3.4.3.0/darshan/tests/input/noposix.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/input/noposixopens.darshan` & `darshan-3.4.3.0/darshan/tests/input/noposixopens.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/input/sample-badost.darshan` & `darshan-3.4.3.0/darshan/tests/input/sample-badost.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/input/sample-dxt-simple.darshan` & `darshan-3.4.3.0/darshan/tests/input/sample-dxt-simple.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/input/sample-goodost.darshan` & `darshan-3.4.3.0/darshan/tests/input/sample-goodost.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/input/sample.darshan` & `darshan-3.4.3.0/darshan/tests/input/sample.darshan`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/test_data_access_by_filesystem.py` & `darshan-3.4.3.0/darshan/tests/test_data_access_by_filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,16 +264,16 @@
 
     # accumulate text added via ax.text()
     # by the function
     for child in children:
         if isinstance(child, matplotlib.text.Text):
             actual_list_text_in_fig.append(child.get_text())
 
-    for expected_text_entry in [matplotlib.text.Text(0, 1, ' # files read (3.00E+00)'),
-                                matplotlib.text.Text(0, 0, ' # files written (1.40E+01)')]:
+    for expected_text_entry in [matplotlib.text.Text(0, 1, ' files read: 3'),
+                                matplotlib.text.Text(0, 0, ' files written: 14')]:
         assert expected_text_entry.get_text() in actual_list_text_in_fig
 
     # enforce invisibile right-side spine so that
     # there is no overlap between value labels and
     # the plot frame on the right side
     for ax in fig.axes:
         spines = ax.spines
@@ -294,18 +294,15 @@
     # adjusted based on the length of the strings
     axes = actual_fig.axes
     for ax in axes:
         for child in ax.get_children():
             if isinstance(child, matplotlib.text.Annotation):
                 actual_text = child.get_text()
                 actual_fontsize = child.get_fontsize()
-                if len(actual_text) <= 8:
-                    assert actual_fontsize == 18
-                else:
-                    assert actual_fontsize == 12
+                assert actual_fontsize == 18
 
 @pytest.mark.parametrize("log_file_name, expected_text_labels", [
     ('noposixopens.darshan', ['/global', 'anonymized']),
     ('sample.darshan', ['/scratch2', '<STDERR>', '<STDOUT>']),
     # test case for gh-678
     ('mpi-io-test.darshan', ['/global', '<STDOUT>']),
     ])
@@ -320,18 +317,14 @@
         actual_fig = data_access_by_filesystem.plot_with_report(report=report)
     axes = actual_fig.axes
     for ax in axes:
         for child in ax.get_children():
             if isinstance(child, matplotlib.text.Annotation):
                 actual_text = child.get_text()
                 actual_text_labels.append(actual_text)
-                if 'STD' in actual_text:
-                    # format the STD.. streams properly
-                    actual_fontsize = child.get_fontsize()
-                    assert actual_fontsize == 12
 
     assert actual_text_labels == expected_text_labels
 
 def test_empty_data_posix_text_position():
     # the bytes and files read/written text labels
     # were observed to be too far to the right in the
     # subplots for a log file lacking POSIX activity
@@ -405,18 +398,16 @@
     # https://github.com/darshan-hpc/darshan/pull/397#pullrequestreview-717403104
     # https://github.com/darshan-hpc/darshan/pull/397#issuecomment-889504530
     filesystem_roots = ['/usr', '/yellow', '/green', '/global']
     rd_bytes = [1e7, 1e8, 1e9, 1e10]
     wr_bytes = [1e8, 1e9, 1e10, 1e11]
     rd_file_cts = [1e3, 1e4, 1e5, 1e6]
     wr_file_cts = [1e2, 1e3, 1e4, 1e5]
-    # multiply by the MiB conversion factor
-    factor = 1048576
-    bytes_rd_series = pd.Series(data=rd_bytes, index=filesystem_roots) * factor
-    bytes_wr_series = pd.Series(data=wr_bytes, index=filesystem_roots) * factor
+    bytes_rd_series = pd.Series(data=rd_bytes, index=filesystem_roots)
+    bytes_wr_series = pd.Series(data=wr_bytes, index=filesystem_roots)
     file_rd_series = pd.Series(data=rd_file_cts, index=filesystem_roots)
     file_wr_series = pd.Series(data=wr_file_cts, index=filesystem_roots)
     fig = plt.figure()
     data_access_by_filesystem.plot_data(fig,
                                        file_rd_series,
                                        file_wr_series,
                                        bytes_rd_series,
```

### Comparing `darshan-3.4.2.0/darshan/tests/test_error.py` & `darshan-3.4.3.0/darshan/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/test_heatmap_handling.py` & `darshan-3.4.3.0/darshan/tests/test_heatmap_handling.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/test_log_utils.py` & `darshan-3.4.3.0/darshan/tests/test_log_utils.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/test_moddxt.py` & `darshan-3.4.3.0/darshan/tests/test_moddxt.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/test_modmpiio.py` & `darshan-3.4.3.0/darshan/tests/test_modmpiio.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/test_modposix.py` & `darshan-3.4.3.0/darshan/tests/test_modposix.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/test_modstdio.py` & `darshan-3.4.3.0/darshan/tests/test_modstdio.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/test_plot_common_access_table.py` & `darshan-3.4.3.0/darshan/tests/test_plot_common_access_table.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/test_plot_dxt_heatmap.py` & `darshan-3.4.3.0/darshan/tests/test_plot_dxt_heatmap.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/test_plot_exp_common.py` & `darshan-3.4.3.0/darshan/tests/test_plot_exp_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,20 @@
     actual_xticks = ax.get_xticks()
     actual_xticklabels = [tl.get_text() for tl in ax.get_xticklabels()]
 
     expected_xticks = range(len(expected_xticklabels))
 
     assert_array_equal(actual_xticks, expected_xticks)
     assert_array_equal(actual_xticklabels, expected_xticklabels)
+    # see Argonne formatting reqs in gh-910
+    spines = ax.spines
+    assert not spines["top"].get_visible()
+    assert not spines["right"].get_visible()
+    assert spines["bottom"].get_visible()
+    assert spines["left"].get_visible()
 
 
 @pytest.mark.parametrize(
     "filename, mod, fig_func, expected_heights",
     [
         (
             "dxt.darshan",
```

### Comparing `darshan-3.4.2.0/darshan/tests/test_plot_io_cost.py` & `darshan-3.4.3.0/darshan/tests/test_plot_io_cost.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from packaging import version
 import pytest
 import numpy as np
 from numpy.testing import assert_allclose, assert_array_equal
 import pandas as pd
 from pandas.testing import assert_frame_equal, assert_series_equal
+import matplotlib
 
 import darshan
 from darshan.log_utils import get_log_path
 from darshan.experimental.plots.plot_io_cost import (
     get_by_avg_series,
     get_io_cost_df,
     plot_io_cost,
@@ -17,45 +19,45 @@
 @pytest.mark.parametrize(
     "logname, expected_df",
     [
         (
             "ior_hdf5_example.darshan",
             pd.DataFrame(
                 np.array([
-                    [0.0196126699, 0.1342029571533203, 0.0074423551],
-                    [0.0196372866, 0.13425052165985107, 0.0475],
-                    [0.016869, 0.086689, 0.097160],
-                    [0.0, 2.5570392608642578e-05, 0.0],
+                    [0.0196126699, 0.1342029571533203, 0.0074423551, 0.0],
+                    [0.0196372866, 0.13425052165985107, 0.0475, 0.0],
+                    [0.016869, 0.086689, 0.097160, 0.0],
+                    [0.0, 2.5570392608642578e-05, 0.0, 0.0],
                 ]),
                 ["POSIX", "MPIIO", "HDF5", "STDIO"],
-                ["Read", "Write", "Meta"],
+                ["Read", "Write", "Meta", "Wait"],
             ),
         ),
         (
             "sample-badost.darshan",
             pd.DataFrame(
                 np.array([
-                    [0.0, 33.48587587394286, 0.5547398688504472],
-                    [0.011203573201783001, 4.632166e-07, 0.135187],
+                    [0.0, 33.48587587394286, 0.5547398688504472, 0.0],
+                    [0.011203573201783001, 4.632166e-07, 0.135187, 0.0],
                 ]),
                 ["POSIX", "STDIO"],
-                ["Read", "Write", "Meta"],
+                ["Read", "Write", "Meta", "Wait"],
             ),
         ),
         (
             "shane_ior-PNETCDF_id438100-438100_11-9-41525-10280033558448664385_1.darshan",
             pd.DataFrame(
                 np.array([
-                [0.000378787518, 0.002514898777, 0.000068306923],
-                [0.000397562981, 0.002540826797, 0.001559376717],
-                [0.000402510166, 0.002579867840, 0.001994967461],
-                [0.000000000000, 0.000120997429, 0.000000000000],
+                [0.000378787518, 0.002514898777, 0.000068306923, 0.0],
+                [0.000397562981, 0.002540826797, 0.001559376717, 0.0],
+                [0.000402510166, 0.002579867840, 0.001994967461, 0.0],
+                [0.000000000000, 0.000120997429, 0.000000000000, 0.0],
                 ]),
                 ["POSIX", "MPIIO", "PNETCDF", "STDIO"],
-                ["Read", "Write", "Meta"],
+                ["Read", "Write", "Meta", "Wait"],
             ),
         ),
     ],
 )
 def test_get_io_cost_df(logname, expected_df):
     # regression test for `plot_io_cost.get_io_cost_df()`
     with darshan.DarshanReport(get_log_path(logname)) as report:
@@ -154,16 +156,16 @@
             ],
             columns=[
                 "POSIX_F_READ_TIME", "POSIX_F_WRITE_TIME",
                 "POSIX_F_META_TIME", "TEST"
             ],
         ),
         pd.Series(
-            data=[1.2, .6, 3.0],
-            index=["Read", "Write", "Meta"],
+            data=[1.2, .6, 3.0, 0.0],
+            index=["Read", "Write", "Meta", "Wait"],
         ),
     ),
     (
         # generate a dataframe similar to a shared-record-enabled log
         # where there is a single entry that needs to be divided through
         # by `nprocs`
         "STDIO",
@@ -173,16 +175,16 @@
             ],
             columns=[
                 "STDIO_F_READ_TIME", "STDIO_F_WRITE_TIME",
                 "STDIO_F_META_TIME", "TEST"
             ],
         ),
         pd.Series(
-            data=[3000.0, 300.0, 30.0],
-            index=["Read", "Write", "Meta"],
+            data=[3000.0, 300.0, 30.0, 0.0],
+            index=["Read", "Write", "Meta", "Wait"],
         ),
     ),
     (
         # combine 2 previous cases to check if
         # calculations are being done appropriately
         "MPIIO",
         pd.DataFrame(
@@ -193,16 +195,16 @@
             ],
             columns=[
                 "MPIIO_F_READ_TIME", "MPIIO_F_WRITE_TIME",
                 "MPIIO_F_META_TIME", "TEST"
             ],
         ),
         pd.Series(
-            data=[3001.2, 300.6, 33.0],
-            index=["Read", "Write", "Meta"],
+            data=[3001.2, 300.6, 33.0, 0.0],
+            index=["Read", "Write", "Meta", "Wait"],
         ),
     )
 ])
 def test_get_by_avg_series(mod_key, input_df, expected_series):
     # unit test for `plot_io_cost.get_by_avg_series`
     actual_series = get_by_avg_series(df=input_df, mod_key=mod_key, nprocs=10)
     assert_series_equal(actual_series, expected_series)
@@ -211,19 +213,19 @@
 @pytest.mark.parametrize(
     "filename, expected_df",
     [
         (
             "nonmpi_dxt_anonymized.darshan",
             pd.DataFrame(
                 np.array([
-                    [0.281718, 0.504260, 0.170138],
-                    [0.232386, 0.165982, 0.072751],
+                    [0.281718, 0.504260, 0.170138, 0.0],
+                    [0.232386, 0.165982, 0.072751, 0.0],
                 ]),
                 ["POSIX", "STDIO"],
-                ["Read", "Write", "Meta"],
+                ["Read", "Write", "Meta", "Wait"],
             ),
         ),
     ])
 def test_issue_590(filename, expected_df):
     # regression test for issue #590
     # see: https://github.com/darshan-hpc/darshan/issues/590
     log_path = get_log_path(filename)
@@ -268,7 +270,48 @@
     for df in (input_df, expected_df):
         df.columns = ["Read", "Write", "Meta"]
 
     actual_df = combine_hdf5_modules(input_df)
 
     # check actual and expected dataframes are identical
     assert_frame_equal(actual_df, expected_df)
+
+
+@pytest.mark.parametrize(
+    "logname, expected_xticks, expected_xlabels", [
+        (
+            "shane_ior-PNETCDF_id438100-438100_11-9-41525-10280033558448664385_1.darshan",
+            range(4),
+            ["POSIX", "MPIIO", "PNETCDF", "STDIO"]
+        ),
+        (
+            "imbalanced-io.darshan",
+            range(3),
+            ["POSIX", "MPIIO", "STDIO"]
+        ),
+    ],
+)
+def test_plot_io_cost_x_ticks_and_labels(logname,
+                                         expected_xticks,
+                                         expected_xlabels):
+    # check the x-axis tick marks are at the appropriate
+    # locations and the labels are as expected
+
+    logpath = get_log_path(logname)
+    with darshan.DarshanReport(logpath) as report:
+        fig = plot_io_cost(report=report)
+    for i, ax in enumerate(fig.axes):
+        if i > 0 and version.parse(matplotlib.__version__) < version.parse("3.6.0"):
+            # the second (invisible/twinned) axis is effectively
+            # empty in older matplotlib versions
+            continue
+        # there are only 2 axes, the first being the "raw" data
+        # and the second being the normalized data (percent)
+        actual_xticks = ax.get_xticks()
+        xticklabels = ax.get_xticklabels()
+        actual_xticklabels = [tl.get_text() for tl in xticklabels]
+        assert_allclose(actual_xticks, expected_xticks)
+        assert_array_equal(actual_xticklabels, expected_xlabels)
+        # regression test for gh-881
+        expected_rotations = 90
+        x_rotations = [tl.get_rotation() for tl in xticklabels]
+        assert_allclose(x_rotations, expected_rotations)
```

### Comparing `darshan-3.4.2.0/darshan/tests/test_report.py` & `darshan-3.4.3.0/darshan/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/test_report_copy.py` & `darshan-3.4.3.0/darshan/tests/test_report_copy.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/darshan/tests/test_summary.py` & `darshan-3.4.3.0/darshan/tests/test_summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,30 @@
 try:
     import lxml
     has_lxml = True
 except ImportError:
     has_lxml = False
 
 
+def _enforce_html_report_aesthetics(report_str):
+    # formatting requirements, partly from Argonne
+    # feedback in gh-910
+    prog = re.compile(r"figcaption {\n.*\n.*\n.*\n}")
+    m = prog.search(report_str)
+    if m:
+        result = m.group(0)
+    assert "font-weight: 300" in result
+    assert "font-size: 0.75em" in result
+    assert not "italic" in result
+
+    # Argonne team doesn't like index label
+    # for File Count Summary table
+    assert not "<th>type</th>" in report_str
+
+
 @pytest.mark.parametrize(
     "argv", [
         ["./tests/input/sample.darshan"],
         ["./tests/input/sample.darshan", "--output=test.html"],
     ]
 )
 def test_setup_parser(argv):
@@ -77,20 +93,21 @@
 
         # verify the HTML file was generated
         assert os.path.exists(expected_save_path)
 
 
 @pytest.mark.parametrize(
     "argv, expected_img_count, expected_table_count", [
-        (["noposix.darshan"], 3, 2),
-        (["noposix.darshan", "--output=test.html"], 3, 2),
-        (["sample-dxt-simple.darshan"], 8, 4),
-        (["sample-dxt-simple.darshan", "--output=test.html"], 8, 4),
-        (["nonmpi_dxt_anonymized.darshan"], 6, 3),
-        (["ior_hdf5_example.darshan"], 11, 5),
+        (["noposix.darshan"], 3, 4),
+        (["noposix.darshan", "--output=test.html"], 3, 4),
+        (["sample-dxt-simple.darshan"], 7, 8),
+        (["sample-dxt-simple.darshan", "--output=test.html"], 7, 8),
+        (["sample-dxt-simple.darshan", "--enable_dxt_heatmap"], 9, 8),
+        (["nonmpi_dxt_anonymized.darshan"], 6, 7),
+        (["ior_hdf5_example.darshan"], 10, 11),
         ([None], 0, 0),
     ]
 )
 def test_main_without_args(tmpdir, argv, expected_img_count, expected_table_count):
     # test summary.main() by running it without a parser
     if argv[0] is not None:
         argv[0] = get_log_path(argv[0])
@@ -99,32 +116,40 @@
         if argv[0]:
             # if a log path is given, generate the summary report
             # in a temporary directory
             with tmpdir.as_cwd():
                 summary.main()
 
                 # get the path for the generated summary report
-                if len(argv) == 1:
+                if not any("--output" in arg for arg in argv):
                     log_fname = os.path.basename(argv[0])
                     output_fname = os.path.splitext(log_fname)[0] + "_report.html"
                 else:
                     output_fname = "test.html"
                 expected_save_path = os.path.abspath(output_fname)
 
                 # verify the HTML file was generated
                 assert os.path.exists(expected_save_path)
 
                 # verify DXT figures are present for each DXT module
                 with darshan.DarshanReport(filename=argv[0], read_all=False) as report:
                     with open(expected_save_path) as html_report:
                         report_str = html_report.read()
+                        _enforce_html_report_aesthetics(report_str=report_str)
                         if "DXT" in "\t".join(report.modules):
                             for dxt_mod in ["DXT_POSIX", "DXT_MPIIO"]:
                                 if dxt_mod in report.modules:
                                     assert f"Heat Map: {dxt_mod}" in report_str
+                                    if not any("--enable_dxt_heatmap" in arg for arg in argv):
+                                        warn_str = (
+                                            f"{dxt_mod} trace data available, but DXT-based "
+                                            "heatmaps are not currently generated by default "
+                                            "by the job summary tool."
+                                        )
+                                        assert warn_str in report_str
                         else:
                             # check that help message is present
                             assert "Heatmap data is not available for this job" in report_str
                             assert "Consider enabling the runtime heatmap module" in report_str
 
                         # check that expected number of figures are found
                         assert report_str.count("<img") == expected_img_count
@@ -205,17 +230,22 @@
                         # the 3-way check is only valid if all heatmap modules
                         # are present:
                         if (mpiio_position > -1 and
                             posix_position > -1 and
                             stdio_position > -1):
                             assert mpiio_position < posix_position < stdio_position
                     else:
-                        # check that help message is present
-                        assert "Heatmap data is not available for this job" in report_str
-                        assert "Consider enabling the runtime heatmap module" in report_str
+                        if not "empty_log" in log_filepath:
+                            # check that help message is present
+                            assert "Heatmap data is not available for this job" in report_str
+                            assert "Consider enabling the runtime heatmap module" in report_str
+                        else:
+                            # check empty log warning and return
+                            assert "This Darshan log file has no instrumentation records, " in report_str
+                            return
 
                     # check if I/O cost figure is present
                     for mod in report.modules:
                         if mod in ["POSIX", "MPI-IO", "STDIO"]:
                             assert "I/O Cost" in report_str
 
                     # check the number of opening section tags
@@ -232,14 +262,21 @@
                     elif ("runtime_and_dxt_heatmaps_diagonal_write_only" in log_filepath or
                           "treddy_runtime_heatmap_inactive_ranks" in log_filepath or
                           "h5d_no_h5f" in log_filepath):
                         assert actual_runtime_heatmap_titles == 1
                     else:
                         assert actual_runtime_heatmap_titles == 0
 
+                    # check for presence of bandwidth summary strings
+                    # (more detailed per-module probes are present
+                    # in test_derived_metrics_bytes_and_bandwidth())
+                    assert "I/O performance estimate" in report_str
+                    assert "color: blue" in report_str
+                    assert "File Count Summary" in report_str
+
 
 class TestReportData:
 
     @pytest.mark.parametrize(
         "log_path",
         [
             "sample.darshan",
```

### Comparing `darshan-3.4.2.0/darshan.egg-info/SOURCES.txt` & `darshan-3.4.3.0/darshan.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,21 +71,25 @@
 darshan/experimental/plots/heatmap_handling.py
 darshan/experimental/plots/plot_access_histogram.py
 darshan/experimental/plots/plot_common_access_table.py
 darshan/experimental/plots/plot_dxt_heatmap.py
 darshan/experimental/plots/plot_dxt_heatmap2.py
 darshan/experimental/plots/plot_io_cost.py
 darshan/experimental/plots/plot_opcounts.py
+darshan/experimental/plots/plot_posix_access_pattern.py
+darshan/experimental/plots/plot_posix_io_pattern.py
 darshan/experimental/transforms/dxt2png.py
+darshan/lib/accum.py
 darshan/tests/__init__.py
 darshan/tests/conftest.py
 darshan/tests/test_cffi_misc.py
 darshan/tests/test_data_access_by_filesystem.py
 darshan/tests/test_error.py
 darshan/tests/test_heatmap_handling.py
+darshan/tests/test_lib_accum.py
 darshan/tests/test_log_utils.py
 darshan/tests/test_moddxt.py
 darshan/tests/test_modmpiio.py
 darshan/tests/test_modposix.py
 darshan/tests/test_modstdio.py
 darshan/tests/test_plot_common_access_table.py
 darshan/tests/test_plot_dxt_heatmap.py
```

### Comparing `darshan-3.4.2.0/docs/Makefile` & `darshan-3.4.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/docs/api/pydarshan/darshan.cli.rst` & `darshan-3.4.3.0/docs/api/pydarshan/darshan.cli.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/docs/api/pydarshan/darshan.experimental.aggregators.rst` & `darshan-3.4.3.0/docs/api/pydarshan/darshan.experimental.aggregators.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/docs/api/pydarshan/darshan.experimental.plots.rst` & `darshan-3.4.3.0/docs/api/pydarshan/darshan.experimental.plots.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/docs/api/pydarshan/darshan.rst` & `darshan-3.4.3.0/docs/api/pydarshan/darshan.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/docs/api/pydarshan/darshan.tests.rst` & `darshan-3.4.3.0/docs/api/pydarshan/darshan.tests.rst`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/docs/conf.py` & `darshan-3.4.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/docs/make.bat` & `darshan-3.4.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `darshan-3.4.2.0/pyproject.toml` & `darshan-3.4.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 [build-system]
 requires = [
     "wheel",
-    "setuptools",
+    "setuptools<64.0.0",
 ]
 
+[project]
+requires-python = ">=3.7"
+
 [tool.cibuildwheel]
 environment = "PYDARSHAN_BUILD_EXT=1"
 skip = [
+    "cp36-*",
     "pp*",
     "*musllinux*",
     "*i686*",
     "*_ppc64le",
     "*_s390x"
 ]
 test-requires = [
     "packaging",
     "pytest",
     "lxml",
     "matplotlib",
-    "importlib_resources;python_version<'3.9'"
+    "importlib_resources;python_version<'3.9'",
+    "humanize"
 ]
 before-test = "pip install -U git+https://github.com/darshan-hpc/darshan-logs.git@main"
 test-command = "pytest {package}"
 
 [tool.cibuildwheel.linux]
 before-all = [
     "yum install -y blas-devel lapack-devel",
```

### Comparing `darshan-3.4.2.0/setup.py` & `darshan-3.4.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages, Extension
 import sys
 import os
 
+if sys.version_info[:2] < (3, 7):
+    raise RuntimeError("Python version >= 3.7 required.")
+
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 
-requirements = ["cffi", "numpy", "pandas", "matplotlib", "seaborn", "mako"]
-
-if sys.version_info == (3, 6):
-    requirements.append("importlib_resources")
+requirements = ["cffi", "numpy", "pandas", "matplotlib", "seaborn", "mako", "humanize"]
 
 setup_requirements = [
     "pytest-runner",
 ]
 test_requirements = ["pytest"]
 
 
@@ -58,31 +58,32 @@
     author_email="",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     description="Python tools to interact with darshan log records of HPC applications.",
     long_description=readme,
     ext_modules=ext_modules,
     install_requires=requirements,
     include_package_data=True,
     keywords="darshan",
     name="darshan",
     packages=find_packages(include=["darshan"]),
     setup_requires=setup_requirements,
     tests_require=test_requirements,
     url='https://www.mcs.anl.gov/research/projects/darshan/',
-    version='3.4.2.0',
+    version='3.4.3.0',
     zip_safe=False,
     package_data={"": ["*.darshan"],
                   "darshan": ["cli/style.css",
                               "cli/base.html",
                               "examples/example_logs/*",
                               "examples/darshan-graph/*",
                               "tests/input/*"]},
```

