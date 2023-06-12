# Comparing `tmp/quickstats-0.6.8.4.tar.gz` & `tmp/quickstats-0.6.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.6.8.4.tar", last modified: Mon Jun  5 21:18:20 2023, max compression
+gzip compressed data, was "quickstats-0.6.8.6.tar", last modified: Mon Jun 12 09:05:55 2023, max compression
```

## Comparing `quickstats-0.6.8.4.tar` & `quickstats-0.6.8.6.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.8.4/README.md
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:11.000000 quickstats-0.6.8.4/bin/
--rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1651 2023-05-11 20:22:22.000000 quickstats-0.6.8.4/bin/quickstats
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:11.000000 quickstats-0.6.8.4/quickstats/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-05-31 15:23:38.000000 quickstats-0.6.8.4/quickstats/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-06-05 21:17:07.000000 quickstats-0.6.8.4/quickstats/_version.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:11.000000 quickstats-0.6.8.4/quickstats/analysis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.8.4/quickstats/analysis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.8.4/quickstats/analysis/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.8.4/quickstats/analysis/analysis_path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.8.4/quickstats/analysis/config_format_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    41649 2023-05-20 03:33:19.000000 quickstats-0.6.8.4/quickstats/analysis/data_loading.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.8.4/quickstats/analysis/data_preprocessing.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    85935 2023-05-20 03:34:59.000000 quickstats-0.6.8.4/quickstats/analysis/event_categorization.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.8.4/quickstats/analysis/multi_class_boundary_tree.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9286 2023-05-20 03:35:21.000000 quickstats-0.6.8.4/quickstats/analysis/ntuple_conversion_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    32052 2023-06-03 14:05:32.000000 quickstats-0.6.8.4/quickstats/analysis/ntuple_process_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8856 2023-05-20 03:36:01.000000 quickstats-0.6.8.4/quickstats/analysis/sample_poly_param_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:12.000000 quickstats-0.6.8.4/quickstats/analysis/systematics/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.8.4/quickstats/analysis/systematics/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29550 2023-05-20 03:37:08.000000 quickstats-0.6.8.4/quickstats/analysis/systematics/base_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.8.4/quickstats/analysis/systematics/gaussian_shape_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.8.4/quickstats/analysis/systematics/normalization_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11815 2023-05-20 03:31:54.000000 quickstats-0.6.8.4/quickstats/analysis/systematics/systematics_evaluation_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:12.000000 quickstats-0.6.8.4/quickstats/clis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.8.4/quickstats/clis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    35299 2023-05-31 19:41:46.000000 quickstats-0.6.8.4/quickstats/clis/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.8.4/quickstats/clis/inspect_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.8.4/quickstats/clis/inspect_ws.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16785 2023-06-05 09:37:42.000000 quickstats-0.6.8.4/quickstats/clis/likelihood_fit.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7818 2023-01-04 09:02:54.000000 quickstats-0.6.8.4/quickstats/clis/likelihood_scan.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.8.4/quickstats/clis/limit_setting.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1327 2023-02-14 22:29:19.000000 quickstats-0.6.8.4/quickstats/clis/processor_cli.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15178 2023-05-11 20:21:35.000000 quickstats-0.6.8.4/quickstats/clis/workspace_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:14.000000 quickstats-0.6.8.4/quickstats/components/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      849 2023-05-30 19:49:31.000000 quickstats-0.6.8.4/quickstats/components/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3152 2023-05-27 07:22:07.000000 quickstats-0.6.8.4/quickstats/components/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13395 2023-05-27 02:29:45.000000 quickstats-0.6.8.4/quickstats/components/analysis_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8656 2023-04-05 18:11:38.000000 quickstats-0.6.8.4/quickstats/components/asimov_generator.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    30804 2023-05-20 02:55:29.000000 quickstats-0.6.8.4/quickstats/components/asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.8.4/quickstats/components/basics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31916 2023-05-31 14:47:47.000000 quickstats-0.6.8.4/quickstats/components/extended_minimizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    98139 2023-05-31 20:12:21.000000 quickstats-0.6.8.4/quickstats/components/extended_model.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5539 2023-05-20 03:03:29.000000 quickstats-0.6.8.4/quickstats/components/extended_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15647 2023-05-25 18:13:48.000000 quickstats-0.6.8.4/quickstats/components/likelihood.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:14.000000 quickstats-0.6.8.4/quickstats/components/modelling/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.8.4/quickstats/components/modelling/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.8.4/quickstats/components/modelling/component_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20157 2023-05-20 03:06:27.000000 quickstats-0.6.8.4/quickstats/components/modelling/data_modelling.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.8.4/quickstats/components/modelling/model_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.8.4/quickstats/components/modelling/parameter_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-05-20 03:07:18.000000 quickstats-0.6.8.4/quickstats/components/modelling/pdf_fit_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3532 2023-05-20 03:07:28.000000 quickstats-0.6.8.4/quickstats/components/modelling/tree_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10839 2022-04-07 03:18:15.000000 quickstats-0.6.8.4/quickstats/components/nuisance_parameter_harmonizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17291 2023-05-31 18:05:59.000000 quickstats-0.6.8.4/quickstats/components/nuisance_parameter_pull.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12390 2023-05-31 15:55:13.000000 quickstats-0.6.8.4/quickstats/components/nuisance_parameter_ranking.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:14.000000 quickstats-0.6.8.4/quickstats/components/processors/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.8.4/quickstats/components/processors/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:15.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2066 2023-05-19 15:52:58.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/auxiliary.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2660 2023-05-21 22:51:18.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_base_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-05-21 22:53:11.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_declare.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      870 2023-05-23 18:53:54.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1154 2023-06-03 14:06:41.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_export.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_filter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1076 2022-08-29 06:56:49.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1121 2023-05-21 22:55:55.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_load_macro.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_max.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_mean.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_min.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_redefine.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1677 2023-05-22 21:51:19.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_report.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2129 2023-06-03 16:04:25.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_save.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      645 2023-06-03 14:13:00.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_stat.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_sum.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_treename.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8953 2023-05-28 22:27:10.000000 quickstats-0.6.8.4/quickstats/components/processors/builtin_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6504 2023-05-21 22:51:45.000000 quickstats-0.6.8.4/quickstats/components/processors/roo_config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6772 2023-06-03 19:25:34.000000 quickstats-0.6.8.4/quickstats/components/processors/roo_processor.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.8.4/quickstats/components/pvalue_toys.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3519 2023-05-20 03:04:57.000000 quickstats-0.6.8.4/quickstats/components/roo_inspector.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3083 2023-05-20 03:04:47.000000 quickstats-0.6.8.4/quickstats/components/root_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21336 2023-05-20 03:06:10.000000 quickstats-0.6.8.4/quickstats/components/toy_limit_calculator.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:16.000000 quickstats-0.6.8.4/quickstats/components/workspaces/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2023-05-11 12:58:08.000000 quickstats-0.6.8.4/quickstats/components/workspaces/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2023-05-20 03:10:01.000000 quickstats-0.6.8.4/quickstats/components/workspaces/asimov_handler.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2023-05-20 03:10:09.000000 quickstats-0.6.8.4/quickstats/components/workspaces/core_argument_sets.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.8.4/quickstats/components/workspaces/sample.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.8.4/quickstats/components/workspaces/settings.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8295 2023-05-20 03:10:27.000000 quickstats-0.6.8.4/quickstats/components/workspaces/systematic.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.8.4/quickstats/components/workspaces/systematics_domain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    53138 2023-05-20 03:11:16.000000 quickstats-0.6.8.4/quickstats/components/workspaces/ws_comparer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8837 2023-05-20 03:11:35.000000 quickstats-0.6.8.4/quickstats/components/workspaces/ws_decomposer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.8.4/quickstats/components/workspaces/ws_modifier_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10859 2023-05-20 03:12:06.000000 quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    87030 2023-05-20 03:16:06.000000 quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    76213 2023-05-20 03:19:36.000000 quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    45866 2023-05-20 03:21:08.000000 quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_combiner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    48960 2023-05-20 03:23:15.000000 quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_modifier.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:16.000000 quickstats-0.6.8.4/quickstats/concurrent/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      306 2023-05-31 15:27:50.000000 quickstats-0.6.8.4/quickstats/concurrent/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3064 2023-05-31 15:10:38.000000 quickstats-0.6.8.4/quickstats/concurrent/abstract_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.8.4/quickstats/concurrent/logging.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5239 2023-05-31 16:02:49.000000 quickstats-0.6.8.4/quickstats/concurrent/nuisance_parameter_ranking_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5891 2023-05-31 15:28:21.000000 quickstats-0.6.8.4/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-05-31 15:28:38.000000 quickstats-0.6.8.4/quickstats/concurrent/parameterised_likelihood.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3963 2023-05-31 15:27:15.000000 quickstats-0.6.8.4/quickstats/concurrent/parameterised_runner.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:16.000000 quickstats-0.6.8.4/quickstats/core/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.8.4/quickstats/core/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.8.4/quickstats/core/abstract_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20587 2023-05-20 03:28:17.000000 quickstats-0.6.8.4/quickstats/core/configs.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.8.4/quickstats/core/configurable_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.8.4/quickstats/core/dataclass_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      971 2023-05-20 03:27:42.000000 quickstats-0.6.8.4/quickstats/core/decorators.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2296 2023-05-23 21:10:32.000000 quickstats-0.6.8.4/quickstats/core/enums.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.8.4/quickstats/core/methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.8.4/quickstats/core/path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.8.4/quickstats/core/virtual_trees.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:16.000000 quickstats-0.6.8.4/quickstats/interface/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2023-05-31 15:27:05.000000 quickstats-0.6.8.4/quickstats/interface/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:16.000000 quickstats-0.6.8.4/quickstats/interface/cppyy/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.6.8.4/quickstats/interface/cppyy/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.8.4/quickstats/interface/cppyy/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12546 2023-05-28 20:56:33.000000 quickstats-0.6.8.4/quickstats/interface/cppyy/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.8.4/quickstats/interface/cppyy/vectorize.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:17.000000 quickstats-0.6.8.4/quickstats/interface/root/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.8.4/quickstats/interface/root/RooAbsData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9855 2023-05-20 12:12:25.000000 quickstats-0.6.8.4/quickstats/interface/root/RooAbsPdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.8.4/quickstats/interface/root/RooArgSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.8.4/quickstats/interface/root/RooCategory.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    44679 2023-05-20 12:08:58.000000 quickstats-0.6.8.4/quickstats/interface/root/RooDataSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.8.4/quickstats/interface/root/RooMsgService.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5451 2023-05-11 15:17:32.000000 quickstats-0.6.8.4/quickstats/interface/root/RooRealVar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.8.4/quickstats/interface/root/TArrayData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.8.4/quickstats/interface/root/TF1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.8.4/quickstats/interface/root/TFile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-05-20 12:06:46.000000 quickstats-0.6.8.4/quickstats/interface/root/TH1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5707 2023-05-03 13:36:36.000000 quickstats-0.6.8.4/quickstats/interface/root/TH2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.8.4/quickstats/interface/root/TObject.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.8.4/quickstats/interface/root/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.8.4/quickstats/interface/root/helper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.8.4/quickstats/interface/root/inspection.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.8.4/quickstats/interface/root/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19576 2023-05-11 13:39:17.000000 quickstats-0.6.8.4/quickstats/interface/root/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5637 2023-05-27 06:13:47.000000 quickstats-0.6.8.4/quickstats/interface/root/roofit_extension.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:11.000000 quickstats-0.6.8.4/quickstats/macros/
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:17.000000 quickstats-0.6.8.4/quickstats/macros/AsymptoticCLsTool/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.8.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.8.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:17.000000 quickstats-0.6.8.4/quickstats/macros/FlexibleInterpVarMkII/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.8.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.8.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:18.000000 quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:18.000000 quickstats-0.6.8.4/quickstats/macros/ResponseFunction/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13755 2023-04-25 19:09:18.000000 quickstats-0.6.8.4/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.6.8.4/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:18.000000 quickstats-0.6.8.4/quickstats/macros/RooTwoSidedCBShape/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.8.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.8.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:18.000000 quickstats-0.6.8.4/quickstats/maths/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.8.4/quickstats/maths/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1130 2023-03-10 17:21:22.000000 quickstats-0.6.8.4/quickstats/maths/interpolation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.8.4/quickstats/maths/numerics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25719 2023-06-05 15:09:16.000000 quickstats-0.6.8.4/quickstats/maths/statistics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2023-05-15 01:04:06.000000 quickstats-0.6.8.4/quickstats/maths/statistics_jitted.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.8.4/quickstats/maths/symbolics.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:18.000000 quickstats-0.6.8.4/quickstats/parsers/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.8.4/quickstats/parsers/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.8.4/quickstats/parsers/config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15883 2023-05-31 15:27:08.000000 quickstats-0.6.8.4/quickstats/parsers/param_parser.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/quickstats/plots/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.8.4/quickstats/plots/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12818 2023-04-27 22:46:00.000000 quickstats-0.6.8.4/quickstats/plots/abstract_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.8.4/quickstats/plots/bidirectional_bar_chart.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.8.4/quickstats/plots/collective_data_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.8.4/quickstats/plots/color_schemes.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5180 2023-05-17 15:59:58.000000 quickstats-0.6.8.4/quickstats/plots/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4007 2023-05-17 16:00:48.000000 quickstats-0.6.8.4/quickstats/plots/correlation_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5968 2023-03-22 14:09:34.000000 quickstats-0.6.8.4/quickstats/plots/general_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.8.4/quickstats/plots/general_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.8.4/quickstats/plots/histo_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.8.4/quickstats/plots/hypotest_inverter_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5834 2023-05-25 20:07:07.000000 quickstats-0.6.8.4/quickstats/plots/likelihood_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9916 2023-04-10 17:13:17.000000 quickstats-0.6.8.4/quickstats/plots/likelihood_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.8.4/quickstats/plots/likelihood_scan_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29009 2023-05-31 19:45:49.000000 quickstats-0.6.8.4/quickstats/plots/np_ranking_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25696 2023-04-18 01:26:39.000000 quickstats-0.6.8.4/quickstats/plots/pdf_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.8.4/quickstats/plots/sample_purity_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.8.4/quickstats/plots/score_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.8.4/quickstats/plots/stat_plot_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-04-02 13:33:12.000000 quickstats-0.6.8.4/quickstats/plots/template.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.8.4/quickstats/plots/test_statistic_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.8.4/quickstats/plots/upper_limit_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2023-04-14 12:19:16.000000 quickstats-0.6.8.4/quickstats/plots/upper_limit_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.8.4/quickstats/plots/upper_limit_3D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5069 2022-08-24 13:05:29.000000 quickstats-0.6.8.4/quickstats/plots/upper_limit_benchmark_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29805 2023-06-05 15:07:31.000000 quickstats-0.6.8.4/quickstats/plots/variable_distribution_plot.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/quickstats/resources/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.8.4/quickstats/resources/default_workspace_extensions.json
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.8.4/quickstats/root_checker.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/quickstats/stylesheets/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.8.4/quickstats/stylesheets/quick_default.mplstyle
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/quickstats/utils/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.8.4/quickstats/utils/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10988 2023-06-03 14:56:07.000000 quickstats-0.6.8.4/quickstats/utils/common_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.8.4/quickstats/utils/condor_tasks.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17089 2023-06-04 03:39:00.000000 quickstats-0.6.8.4/quickstats/utils/data_conversion.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.8.4/quickstats/utils/hep_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6812 2023-05-31 13:27:25.000000 quickstats-0.6.8.4/quickstats/utils/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.8.4/quickstats/utils/process_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    26227 2023-05-20 21:07:10.000000 quickstats-0.6.8.4/quickstats/utils/roofit_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.8.4/quickstats/utils/roostats_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12379 2023-05-20 03:26:53.000000 quickstats-0.6.8.4/quickstats/utils/root_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1347 2023-05-21 21:45:53.000000 quickstats-0.6.8.4/quickstats/utils/string_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15011 2023-03-14 18:38:57.000000 quickstats-0.6.8.4/quickstats/utils/xml_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-05 21:18:11.000000 quickstats-0.6.8.4/quickstats.egg-info/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-06-05 21:18:10.000000 quickstats-0.6.8.4/quickstats.egg-info/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9079 2023-06-05 21:18:10.000000 quickstats-0.6.8.4/quickstats.egg-info/SOURCES.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-06-05 21:18:10.000000 quickstats-0.6.8.4/quickstats.egg-info/dependency_links.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-06-05 21:18:10.000000 quickstats-0.6.8.4/quickstats.egg-info/requires.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-06-05 21:18:10.000000 quickstats-0.6.8.4/quickstats.egg-info/top_level.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-06-05 21:18:20.000000 quickstats-0.6.8.4/setup.cfg
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.8.4/setup.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.8.6/README.md
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/bin/
+-rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1651 2023-05-11 20:22:22.000000 quickstats-0.6.8.6/bin/quickstats
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-05-31 15:23:38.000000 quickstats-0.6.8.6/quickstats/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-06-12 08:48:07.000000 quickstats-0.6.8.6/quickstats/_version.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/analysis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.8.6/quickstats/analysis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.8.6/quickstats/analysis/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.8.6/quickstats/analysis/analysis_path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.8.6/quickstats/analysis/config_format_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    41649 2023-05-20 03:33:19.000000 quickstats-0.6.8.6/quickstats/analysis/data_loading.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.8.6/quickstats/analysis/data_preprocessing.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    85935 2023-05-20 03:34:59.000000 quickstats-0.6.8.6/quickstats/analysis/event_categorization.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.8.6/quickstats/analysis/multi_class_boundary_tree.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9286 2023-05-20 03:35:21.000000 quickstats-0.6.8.6/quickstats/analysis/ntuple_conversion_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    32052 2023-06-03 14:05:32.000000 quickstats-0.6.8.6/quickstats/analysis/ntuple_process_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8897 2023-06-07 14:20:37.000000 quickstats-0.6.8.6/quickstats/analysis/sample_poly_param_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/analysis/systematics/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.8.6/quickstats/analysis/systematics/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29550 2023-05-20 03:37:08.000000 quickstats-0.6.8.6/quickstats/analysis/systematics/base_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.8.6/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.8.6/quickstats/analysis/systematics/normalization_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11815 2023-05-20 03:31:54.000000 quickstats-0.6.8.6/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/clis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.8.6/quickstats/clis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    35406 2023-06-08 10:16:18.000000 quickstats-0.6.8.6/quickstats/clis/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.8.6/quickstats/clis/inspect_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.8.6/quickstats/clis/inspect_ws.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16785 2023-06-05 09:37:42.000000 quickstats-0.6.8.6/quickstats/clis/likelihood_fit.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7818 2023-01-04 09:02:54.000000 quickstats-0.6.8.6/quickstats/clis/likelihood_scan.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.8.6/quickstats/clis/limit_setting.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1327 2023-02-14 22:29:19.000000 quickstats-0.6.8.6/quickstats/clis/processor_cli.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15178 2023-05-11 20:21:35.000000 quickstats-0.6.8.6/quickstats/clis/workspace_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/components/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      849 2023-05-30 19:49:31.000000 quickstats-0.6.8.6/quickstats/components/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3152 2023-05-27 07:22:07.000000 quickstats-0.6.8.6/quickstats/components/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13357 2023-06-09 12:55:20.000000 quickstats-0.6.8.6/quickstats/components/analysis_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7333 2023-06-08 10:12:47.000000 quickstats-0.6.8.6/quickstats/components/asimov_generator.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    30804 2023-05-20 02:55:29.000000 quickstats-0.6.8.6/quickstats/components/asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.8.6/quickstats/components/basics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31916 2023-06-07 11:32:50.000000 quickstats-0.6.8.6/quickstats/components/extended_minimizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)   102368 2023-06-10 22:20:54.000000 quickstats-0.6.8.6/quickstats/components/extended_model.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5539 2023-05-20 03:03:29.000000 quickstats-0.6.8.6/quickstats/components/extended_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14934 2023-06-07 13:15:59.000000 quickstats-0.6.8.6/quickstats/components/likelihood.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/components/modelling/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.8.6/quickstats/components/modelling/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.8.6/quickstats/components/modelling/component_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20157 2023-05-20 03:06:27.000000 quickstats-0.6.8.6/quickstats/components/modelling/data_modelling.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.8.6/quickstats/components/modelling/model_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.8.6/quickstats/components/modelling/parameter_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-05-20 03:07:18.000000 quickstats-0.6.8.6/quickstats/components/modelling/pdf_fit_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3532 2023-05-20 03:07:28.000000 quickstats-0.6.8.6/quickstats/components/modelling/tree_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10839 2022-04-07 03:18:15.000000 quickstats-0.6.8.6/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17291 2023-05-31 18:05:59.000000 quickstats-0.6.8.6/quickstats/components/nuisance_parameter_pull.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12390 2023-05-31 15:55:13.000000 quickstats-0.6.8.6/quickstats/components/nuisance_parameter_ranking.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/components/processors/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.8.6/quickstats/components/processors/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2066 2023-05-19 15:52:58.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/auxiliary.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2660 2023-05-21 22:51:18.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-05-21 22:53:11.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_declare.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      870 2023-05-23 18:53:54.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1154 2023-06-03 14:06:41.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_export.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_filter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1076 2022-08-29 06:56:49.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1121 2023-05-21 22:55:55.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_load_macro.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_max.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_mean.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_min.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1677 2023-05-22 21:51:19.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_report.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2129 2023-06-03 16:04:25.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_save.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      645 2023-06-03 14:13:00.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_stat.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_sum.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_treename.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9969 2023-06-05 23:09:50.000000 quickstats-0.6.8.6/quickstats/components/processors/builtin_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6504 2023-05-21 22:51:45.000000 quickstats-0.6.8.6/quickstats/components/processors/roo_config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6772 2023-06-03 19:25:34.000000 quickstats-0.6.8.6/quickstats/components/processors/roo_processor.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.8.6/quickstats/components/pvalue_toys.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3519 2023-05-20 03:04:57.000000 quickstats-0.6.8.6/quickstats/components/roo_inspector.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3083 2023-05-20 03:04:47.000000 quickstats-0.6.8.6/quickstats/components/root_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21336 2023-05-20 03:06:10.000000 quickstats-0.6.8.6/quickstats/components/toy_limit_calculator.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/components/workspaces/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2023-05-11 12:58:08.000000 quickstats-0.6.8.6/quickstats/components/workspaces/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2023-05-20 03:10:01.000000 quickstats-0.6.8.6/quickstats/components/workspaces/asimov_handler.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2023-05-20 03:10:09.000000 quickstats-0.6.8.6/quickstats/components/workspaces/core_argument_sets.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.8.6/quickstats/components/workspaces/sample.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.8.6/quickstats/components/workspaces/settings.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8295 2023-05-20 03:10:27.000000 quickstats-0.6.8.6/quickstats/components/workspaces/systematic.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.8.6/quickstats/components/workspaces/systematics_domain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    53162 2023-06-06 14:20:25.000000 quickstats-0.6.8.6/quickstats/components/workspaces/ws_comparer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8837 2023-05-20 03:11:35.000000 quickstats-0.6.8.6/quickstats/components/workspaces/ws_decomposer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.8.6/quickstats/components/workspaces/ws_modifier_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10859 2023-05-20 03:12:06.000000 quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    87030 2023-05-20 03:16:06.000000 quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    76213 2023-05-20 03:19:36.000000 quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    45866 2023-05-20 03:21:08.000000 quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    48960 2023-05-20 03:23:15.000000 quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_modifier.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/concurrent/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      306 2023-05-31 15:27:50.000000 quickstats-0.6.8.6/quickstats/concurrent/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3064 2023-05-31 15:10:38.000000 quickstats-0.6.8.6/quickstats/concurrent/abstract_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.8.6/quickstats/concurrent/logging.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5239 2023-05-31 16:02:49.000000 quickstats-0.6.8.6/quickstats/concurrent/nuisance_parameter_ranking_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5891 2023-06-10 22:16:28.000000 quickstats-0.6.8.6/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-05-31 15:28:38.000000 quickstats-0.6.8.6/quickstats/concurrent/parameterised_likelihood.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3963 2023-05-31 15:27:15.000000 quickstats-0.6.8.6/quickstats/concurrent/parameterised_runner.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/core/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.8.6/quickstats/core/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.8.6/quickstats/core/abstract_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20587 2023-05-20 03:28:17.000000 quickstats-0.6.8.6/quickstats/core/configs.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.8.6/quickstats/core/configurable_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.8.6/quickstats/core/dataclass_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      971 2023-05-20 03:27:42.000000 quickstats-0.6.8.6/quickstats/core/decorators.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2296 2023-05-23 21:10:32.000000 quickstats-0.6.8.6/quickstats/core/enums.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.8.6/quickstats/core/methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.8.6/quickstats/core/path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.8.6/quickstats/core/virtual_trees.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/interface/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2023-05-31 15:27:05.000000 quickstats-0.6.8.6/quickstats/interface/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/interface/cppyy/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.6.8.6/quickstats/interface/cppyy/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.8.6/quickstats/interface/cppyy/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12546 2023-05-28 20:56:33.000000 quickstats-0.6.8.6/quickstats/interface/cppyy/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.8.6/quickstats/interface/cppyy/vectorize.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/interface/root/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.8.6/quickstats/interface/root/RooAbsData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9855 2023-05-20 12:12:25.000000 quickstats-0.6.8.6/quickstats/interface/root/RooAbsPdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.8.6/quickstats/interface/root/RooArgSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.8.6/quickstats/interface/root/RooCategory.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    44679 2023-05-20 12:08:58.000000 quickstats-0.6.8.6/quickstats/interface/root/RooDataSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.8.6/quickstats/interface/root/RooMsgService.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5451 2023-05-11 15:17:32.000000 quickstats-0.6.8.6/quickstats/interface/root/RooRealVar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.8.6/quickstats/interface/root/TArrayData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.8.6/quickstats/interface/root/TF1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.8.6/quickstats/interface/root/TFile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-05-20 12:06:46.000000 quickstats-0.6.8.6/quickstats/interface/root/TH1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5707 2023-05-03 13:36:36.000000 quickstats-0.6.8.6/quickstats/interface/root/TH2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.8.6/quickstats/interface/root/TObject.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.8.6/quickstats/interface/root/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.8.6/quickstats/interface/root/helper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.8.6/quickstats/interface/root/inspection.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.8.6/quickstats/interface/root/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19576 2023-05-11 13:39:17.000000 quickstats-0.6.8.6/quickstats/interface/root/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5637 2023-05-27 06:13:47.000000 quickstats-0.6.8.6/quickstats/interface/root/roofit_extension.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats/macros/
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/macros/AsymptoticCLsTool/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.8.6/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.8.6/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/macros/FlexibleInterpVarMkII/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.8.6/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.8.6/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/macros/ResponseFunction/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13755 2023-04-25 19:09:18.000000 quickstats-0.6.8.6/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.6.8.6/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/macros/RooTwoSidedCBShape/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.8.6/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.8.6/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/maths/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.8.6/quickstats/maths/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1785 2023-06-10 18:00:53.000000 quickstats-0.6.8.6/quickstats/maths/interpolation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.8.6/quickstats/maths/numerics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25719 2023-06-05 15:09:16.000000 quickstats-0.6.8.6/quickstats/maths/statistics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2023-05-15 01:04:06.000000 quickstats-0.6.8.6/quickstats/maths/statistics_jitted.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.8.6/quickstats/maths/symbolics.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:54.000000 quickstats-0.6.8.6/quickstats/parsers/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.8.6/quickstats/parsers/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.8.6/quickstats/parsers/config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15883 2023-05-31 15:27:08.000000 quickstats-0.6.8.6/quickstats/parsers/param_parser.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/quickstats/plots/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.8.6/quickstats/plots/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12868 2023-06-10 17:38:08.000000 quickstats-0.6.8.6/quickstats/plots/abstract_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.8.6/quickstats/plots/bidirectional_bar_chart.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.8.6/quickstats/plots/collective_data_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.8.6/quickstats/plots/color_schemes.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5180 2023-05-17 15:59:58.000000 quickstats-0.6.8.6/quickstats/plots/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4007 2023-05-17 16:00:48.000000 quickstats-0.6.8.6/quickstats/plots/correlation_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5968 2023-03-22 14:09:34.000000 quickstats-0.6.8.6/quickstats/plots/general_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.8.6/quickstats/plots/general_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.8.6/quickstats/plots/histo_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.8.6/quickstats/plots/hypotest_inverter_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8153 2023-06-10 15:01:45.000000 quickstats-0.6.8.6/quickstats/plots/likelihood_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11993 2023-06-10 17:40:53.000000 quickstats-0.6.8.6/quickstats/plots/likelihood_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.8.6/quickstats/plots/likelihood_scan_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29009 2023-05-31 19:45:49.000000 quickstats-0.6.8.6/quickstats/plots/np_ranking_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25696 2023-04-18 01:26:39.000000 quickstats-0.6.8.6/quickstats/plots/pdf_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.8.6/quickstats/plots/sample_purity_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.8.6/quickstats/plots/score_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.8.6/quickstats/plots/stat_plot_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-04-02 13:33:12.000000 quickstats-0.6.8.6/quickstats/plots/template.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.8.6/quickstats/plots/test_statistic_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.8.6/quickstats/plots/upper_limit_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2023-04-14 12:19:16.000000 quickstats-0.6.8.6/quickstats/plots/upper_limit_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.8.6/quickstats/plots/upper_limit_3D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5069 2022-08-24 13:05:29.000000 quickstats-0.6.8.6/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29805 2023-06-05 15:07:31.000000 quickstats-0.6.8.6/quickstats/plots/variable_distribution_plot.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/quickstats/resources/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.8.6/quickstats/resources/default_workspace_extensions.json
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.8.6/quickstats/root_checker.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/quickstats/stylesheets/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.8.6/quickstats/stylesheets/quick_default.mplstyle
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/quickstats/utils/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.8.6/quickstats/utils/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10988 2023-06-03 14:56:07.000000 quickstats-0.6.8.6/quickstats/utils/common_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.8.6/quickstats/utils/condor_tasks.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17089 2023-06-04 03:39:00.000000 quickstats-0.6.8.6/quickstats/utils/data_conversion.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.8.6/quickstats/utils/hep_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6812 2023-05-31 13:27:25.000000 quickstats-0.6.8.6/quickstats/utils/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.8.6/quickstats/utils/process_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    26262 2023-06-07 15:13:35.000000 quickstats-0.6.8.6/quickstats/utils/roofit_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.8.6/quickstats/utils/roostats_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12379 2023-05-20 03:26:53.000000 quickstats-0.6.8.6/quickstats/utils/root_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1347 2023-05-21 21:45:53.000000 quickstats-0.6.8.6/quickstats/utils/string_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15011 2023-06-07 03:21:08.000000 quickstats-0.6.8.6/quickstats/utils/xml_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-06-12 09:05:53.000000 quickstats-0.6.8.6/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-06-12 09:05:52.000000 quickstats-0.6.8.6/quickstats.egg-info/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9079 2023-06-12 09:05:52.000000 quickstats-0.6.8.6/quickstats.egg-info/SOURCES.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-06-12 09:05:52.000000 quickstats-0.6.8.6/quickstats.egg-info/dependency_links.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-06-12 09:05:52.000000 quickstats-0.6.8.6/quickstats.egg-info/requires.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-06-12 09:05:52.000000 quickstats-0.6.8.6/quickstats.egg-info/top_level.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-06-12 09:05:55.000000 quickstats-0.6.8.6/setup.cfg
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.8.6/setup.py
```

### Comparing `quickstats-0.6.8.4/PKG-INFO` & `quickstats-0.6.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.8.4
+Version: 0.6.8.6
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.8.4/README.md` & `quickstats-0.6.8.6/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/bin/quickstats` & `quickstats-0.6.8.6/bin/quickstats`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/__init__.py` & `quickstats-0.6.8.6/quickstats/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/analysis/analysis_base.py` & `quickstats-0.6.8.6/quickstats/analysis/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.6.8.6/quickstats/analysis/analysis_path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/analysis/config_format_templates.py` & `quickstats-0.6.8.6/quickstats/analysis/config_format_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/analysis/data_loading.py` & `quickstats-0.6.8.6/quickstats/analysis/data_loading.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/analysis/data_preprocessing.py` & `quickstats-0.6.8.6/quickstats/analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/analysis/event_categorization.py` & `quickstats-0.6.8.6/quickstats/analysis/event_categorization.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.6.8.6/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.6.8.6/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/analysis/ntuple_process_tool.py` & `quickstats-0.6.8.6/quickstats/analysis/ntuple_process_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.6.8.6/quickstats/analysis/sample_poly_param_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Dict, Optional, Union
 
-from quickstats import AbstractObject
+from quickstats import AbstractObject, semistaticmethod
 
 from quickstats.maths.numerics import to_rounded_float, str_encode_value
 from quickstats.utils.common_utils import in_notebook
 
 class SamplePolyParamTool(AbstractObject):
     
     def __init__(self, verbosity:Optional[Union[int, str]]="INFO"):
@@ -23,14 +23,15 @@
         for coefficient in coefficients:
             coefficient_symbols[coefficient] = Symbol(latex_map.get(coefficient, coefficient))
         basis_symbols = {}
         for basis in bases:
             basis_symbols[basis] = Symbol(basis)
         return parameter_symbols, coefficient_symbols, basis_symbols
     
+    @semistaticmethod
     def initialize_formula(self, formula_str:str, parameters:Dict, coefficients:Dict,
                            latex_map:Optional[Dict]=None):
         from sympy import simplify
         formula = simplify(formula_str)
         if latex_map is None:
             return formula
         symbols = list(formula.free_symbols)
@@ -132,15 +133,15 @@
         self.stdout.info("Formula:", bare=True)
         self.display_expression(formula_expr)
         self.stdout.info("Parameters:", bare=True)
         self.display_sets(*parameter_symbols.values())
         self.stdout.info("Coefficients:", bare=True)
         self.display_sets(*coefficient_symbols.values())
         solutions = self.solve_coefficients(formula_expr, parameter_symbols, coefficient_symbols,
-                                           basis_symbols, basis_value_map)
+                                            basis_symbols, basis_value_map)
         if len(solutions) == 0:
             raise RuntimeError("unable to solve the system of linear equations")
         elif len(solutions) > 1:
             raise RuntimeError("system of linear equations gives non-unique solutions")
         solution = solutions[0]
         self.stdout.info("Solutions:", bare=True)
         for coefficient in coefficient_symbols.values():
```

### Comparing `quickstats-0.6.8.4/quickstats/analysis/systematics/base_systematics.py` & `quickstats-0.6.8.6/quickstats/analysis/systematics/base_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/analysis/systematics/gaussian_shape_systematics.py` & `quickstats-0.6.8.6/quickstats/analysis/systematics/gaussian_shape_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/analysis/systematics/normalization_systematics.py` & `quickstats-0.6.8.6/quickstats/analysis/systematics/normalization_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/analysis/systematics/systematics_evaluation_tool.py` & `quickstats-0.6.8.6/quickstats/analysis/systematics/systematics_evaluation_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/clis/core.py` & `quickstats-0.6.8.6/quickstats/clis/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,15 @@
               help='Path to the input workspace file.')
 @click.option('-o', '--output_file', 'outname', required=True, 
               help='Name of the output workspace containing the '
                    'generated asimov dataset.')
 @click.option('-d', '--data', 'data_name', default='combData', show_default=True,
               help='Name of the dataset used in NP profiling.')
 @click.option('-p', '--poi', 'poi_name', required=True, 
-              help='Name of the parameter of interest (POI).')
+              help='Name of the parameter of interest (POI). Multiple POIs are separated by commas.')
 @click.option('-s', '--poi_scale', type=float, default=1.0, show_default=True,
               help='Scale factor applied to the poi value')
 @click.option('-f', '--fix', 'fix_param', default="", show_default=True,
               help='Parameters to fix')
 @click.option('-r', '--profile', 'profile_param', default="", show_default=True,
               help='Parameters to profile')
 @click.option('-s', '--snapshot', 'snapshot_name', default=None, show_default=True,
@@ -488,14 +488,15 @@
     profile_param = kwargs.pop('profile_param')
     snapshot_name = kwargs.pop('snapshot_name')
     poi_scale = kwargs.pop("poi_scale")
     asimov_names = kwargs.pop("asimov_names")
     asimov_snapshots = kwargs.pop("asimov_snapshots")
     verbosity = kwargs.pop("verbosity")
     rebuild = kwargs.pop("rebuild")
+    kwargs['poi_name'] = split_str(kwargs.pop('poi_name'), sep=",")
     config = {
         'fix_param': fix_param,
         'profile_param': profile_param,
         'snapshot_name': snapshot_name
     }
     from quickstats.utils.string_utils import split_str
     if asimov_names is not None:
```

### Comparing `quickstats-0.6.8.4/quickstats/clis/inspect_rfile.py` & `quickstats-0.6.8.6/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/clis/inspect_ws.py` & `quickstats-0.6.8.6/quickstats/clis/inspect_ws.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/clis/likelihood_fit.py` & `quickstats-0.6.8.6/quickstats/clis/likelihood_fit.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/clis/likelihood_scan.py` & `quickstats-0.6.8.6/quickstats/clis/likelihood_scan.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/clis/limit_setting.py` & `quickstats-0.6.8.6/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/clis/processor_cli.py` & `quickstats-0.6.8.6/quickstats/clis/processor_cli.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/clis/workspace_tools.py` & `quickstats-0.6.8.6/quickstats/clis/workspace_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/__init__.py` & `quickstats-0.6.8.6/quickstats/components/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/analysis_base.py` & `quickstats-0.6.8.6/quickstats/components/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/analysis_object.py` & `quickstats-0.6.8.6/quickstats/components/analysis_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,46 +104,49 @@
     def minimizer_options(self):
         return self.minimizer.config
     
     @property
     def nll_commands(self):
         return self.minimizer.nll_commands
     
+    @property
+    def get_poi(self):
+        return self.model.get_poi
+    
     # black magic
     def _inherit_init(self, init_func, **kwargs):
         import inspect
         this_parameters = list(inspect.signature(AnalysisObject.__init__).parameters)
         if "self" in this_parameters:
             this_parameters.remove("self")
         that_parameters = list(inspect.signature(init_func).parameters)
         is_calling_this = set(this_parameters) == set(that_parameters)
         if is_calling_this:
             init_func(**kwargs)
         else:
             that_kwargs = {k:v for k,v in kwargs.items() if k in that_parameters}
             this_kwargs = {k:v for k,v in kwargs.items() if k not in that_parameters}
             init_func(config=this_kwargs, **that_kwargs)
-
+        
     def set_poi(self, poi_name:Optional[Union[str, List[str]]]=None):
-        # multi POI case
-        if isinstance(poi_name, list):
-            self.poi = ROOT.RooArgSet()
-            true_poi_names = []
-            # remove duplicates
-            poi_name = list(set(poi_name))
-            for pname in poi_name:
-                poi = self.model.get_poi(pname)
-                self.poi.add(poi)
-                true_poi_names.append(poi.GetName())
-            if true_poi_names:
-                self.stdout.info('POIs set to {}'.format(", ".join([f"\"{name}\"" for name in true_poi_names])))
+        pois = self.get_poi(poi_name)
+        if isinstance(pois, ROOT.RooRealVar):
+            poi_text = f'"{pois.GetName()}"'
+            n_poi = 1
+        elif isinstance(pois, ROOT.RooArgSet) and (len(pois) > 0):
+            poi_text = ", ".join([f'"{poi.GetName()}"' for poi in pois])
+            n_poi = len(pois)
         else:
-            self.poi = self.model.get_poi(poi_name)
-            if poi_name is not None:
-                self.stdout.info(f'POI set to "{poi_name}"')
+            poi_text = None
+            n_poi = 0
+        if n_poi == 1:
+            self.stdout.info(f'POI set to {poi_text}')
+        elif n_poi > 1:
+            self.stdout.info(f'POIs set to {poi_text}')
+        self.poi = pois
         
     def setup_model(self, **kwargs):
         model = ExtendedModel(**kwargs, verbosity=self.stdout.verbosity)
         self.model = model
     
     def setup_parameters(self, fix_param:str='', profile_param:str='', update_snapshot:bool=True):
         if not self.model:
```

### Comparing `quickstats-0.6.8.4/quickstats/components/asimov_generator.py` & `quickstats-0.6.8.6/quickstats/components/asimov_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -104,45 +104,14 @@
         config['poi_name']  = poi_name
         config['data_name'] = data_name
         config['verbosity'] = verbosity
         if 'preset_param' not in config:
             config['preset_param'] = True
         self._inherit_init(super(AsimovGenerator, self).__init__, **config)
         
-    def generate_asimov(self, poi_val:Optional[float]=None, 
-                        poi_profile:Optional[float]=None,
-                        do_fit:bool=True,
-                        modify_globs:bool=True,
-                        do_import:bool=True,
-                        asimov_name:Optional[str]=None,
-                        asimov_snapshot:Optional[str]=None,
-                        channel_asimov_name:Optional[str]=None,
-                        dataset:Optional["ROOT.RooDataSet"]=None,
-                        constraint_option:int=0,
-                        restore_states:int=0,
-                        snapshot_names:Optional[Dict]=None):
-        kwargs = {
-            "poi_name"            : self.poi.GetName(),
-            "poi_val"             : poi_val,
-            "poi_profile"         : poi_profile,
-            "do_fit"              : do_fit,
-            "modify_globs"        : modify_globs,
-            "do_import"           : do_import,
-            "asimov_name"         : asimov_name,
-            "asimov_snapshot"     : asimov_snapshot,
-            "channel_asimov_name" : channel_asimov_name,
-            "dataset"             : dataset,
-            "constraint_option"   : constraint_option,
-            "restore_states"      : restore_states,
-            "minimizer_options"   : self.minimizer_options,
-            "nll_options"         : self.nll_commands,
-            "snapshot_names"      : snapshot_names
-        }
-        return self.model.generate_asimov(**kwargs)
-        
     def generate_standard_asimov(self, asimov_types:Optional[Union[List[AsimovType], List[int], List[str]]]=None,
                                  asimov_names:Optional[Union[List[str], str]]=None,
                                  asimov_snapshots:Optional[Union[List[str], str]]=None,
                                  poi_scale:Optional[float]=None, do_import:bool=True):
         single_asimov = False
         if asimov_types is None:
             asimov_types = self.DEFAULT_ASIMOV_TYPES
@@ -158,19 +127,24 @@
         if asimov_snapshots is not None:
             if isinstance(asimov_snapshots, str):
                 asimov_snapshots = [asimov_snapshots]
             assert len(asimov_snapshots) == len(asimov_types)            
         if poi_scale is None:
             poi_scale = 1.0
             
-        poi_name = self.poi.GetName()
-        self.save_snapshot("temp", WSArgument.MUTABLE)
+        import ROOT
+        if isinstance(self.poi, ROOT.RooArgSet):
+            poi_name = [poi.GetName() for poi in self.poi]
+        else:
+            poi_name = self.poi.GetName()
+            
+        self.save_snapshot(self.kTempSnapshotName, WSArgument.MUTABLE)
         asimov_datasets = []
         for i, asimov_type in enumerate(asimov_types):
-            self.load_snapshot("temp")
+            self.load_snapshot(self.kTempSnapshotName)
             kwargs = copy.deepcopy(self.ASIMOV_SETTINGS[asimov_type])
             if kwargs is None:
                 continue
             kwargs['poi_name'] = poi_name
             for key in ['poi_val', 'poi_profile']:
                 if kwargs[key] is not None:
                     kwargs[key] *= poi_scale
```

### Comparing `quickstats-0.6.8.4/quickstats/components/asymptotic_cls.py` & `quickstats-0.6.8.6/quickstats/components/asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/basics.py` & `quickstats-0.6.8.6/quickstats/components/basics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/extended_minimizer.py` & `quickstats-0.6.8.6/quickstats/components/extended_minimizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/extended_model.py` & `quickstats-0.6.8.6/quickstats/components/extended_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ROOT.RooPrintable import (kName, kClassName, kValue, kArgs, kExtras, kAddress,
                                kTitle, kCollectionHeader, kSingleLine)
 
 import quickstats
 from quickstats import semistaticmethod, AbstractObject
 from quickstats.maths.numerics import is_integer, pretty_value, get_bins_given_edges, array_issubset
 from quickstats.utils.root_utils import load_macro
-from quickstats.utils.common_utils import str_list_filter
+from quickstats.utils.common_utils import str_list_filter, combine_dict
 from quickstats.utils.roofit_utils import (get_variable_attributes, variable_collection_to_dataframe,
                                            get_relevant_components)
 from quickstats.utils.string_utils import split_str, remove_whitespace
 from quickstats.interface.root import TH1, RooDataSet, RooArgSet, RooMsgService, RooAbsPdf
 from quickstats.interface.root import roofit_extension as rf_ext
 from quickstats.interface.root.roofit_extension import get_str_data
 from quickstats.components.basics import WSArgument, SetValueMode
@@ -37,14 +37,15 @@
     
     _DEFAULT_NAMES_ = {
         'conditional_globs': 'conditionalGlobs_{mu}',
         'conditional_nuis': 'conditionalNuis_{mu}',
         'nominal_globs': 'nominalGlobs',
         'nominal_nuis': 'nominalNuis',
         'nominal_vars': 'nominalVars',
+        'nominal_pois': 'nominalPOIs',
         'weight': 'weightVar',
         'dataset_args': 'obsAndWeight',
         'asimov': 'asimovData_{mu}',
         'asimov_no_poi': 'asimovData',
         'channel_asimov': 'combAsimovData_{label}',
         'nll_snapshot': '{nll_name}_{mu}',
         'range_sideband_low': 'SBLo',
@@ -353,31 +354,75 @@
         
     def fix_parameters(self, param_setup_expr:Optional[str]=None, source:Optional["ROOT.RooArgSet"]=None):
         return self.set_parameters_with_expression(param_setup_expr, source, mode=SetValueMode.FIX)
     
     def profile_parameters(self, param_setup_expr:Optional[str]=None, source:Optional["ROOT.RooArgSet"]=None):
         return self.set_parameters_with_expression(param_setup_expr, source, mode=SetValueMode.FREE)
     
-    def _set_parameters(self, source:"ROOT.RooArgSet", param_setup:Dict, 
-                        mode:Union[str, SetValueMode]=SetValueMode.UNCHANGED):
+    @semistaticmethod
+    def _parse_param_setup(self, source:"ROOT.RooArgSet",
+                           param_setup:Optional[Union[float, Dict, Sequence]]=None,
+                           fill_missing:bool=False,
+                           strict_match:bool=True):
+        if isinstance(source, ROOT.RooRealVar):
+            source = ROOT.RooArgSet(source)
+        assert isinstance(source, ROOT.RooArgSet)
+        if isinstance(param_setup, (float, int)):
+            param_value = param_setup
+            param_setup = {param.GetName(): param_value for param in source}
+        elif isinstance(param_setup, Sequence):
+            if len(source) != len(param_setup):
+                raise ValueError('number of parameters do not match the number of setup values')
+            param_names = [param.GetName() for param in source]
+            param_setup = {param_name: value for param_name, value in zip(param_names, param_setup)}
+        elif isinstance(param_setup, dict):
+            if strict_match:
+                param_setup_cpy = combine_dict(param_setup)
+                param_setup = {}
+                for param in source:
+                    param_name = param.GetName()
+                    if param_name in param_setup_cpy:
+                        param_setup[param_name] = param_setup_cpy[param_name]
+                    elif fill_missing:
+                        param_setup[param_name] = param.getVal()
+            else:
+                param_setup = combine_dict(param_setup)
+        elif param_setup is None:
+            param_setup = {}
+            if fill_missing:
+                param_setup = {param.GetName(): param.getVal() for param in source}
+        else:
+            raise ValueError('invalid param_setup format')
+        return param_setup
+    
+    def _set_parameters(self, source:"ROOT.RooArgSet", param_setup:Union[Dict, Sequence], 
+                        mode:Union[str, SetValueMode]=SetValueMode.UNCHANGED,
+                        strict:bool=False):
+        if isinstance(source, ROOT.RooRealVar):
+            source = ROOT.RooArgSet(source)
         selected_parameters = []
         source_names = [param.GetName() for param in source]
+        param_setup = self._parse_param_setup(source, param_setup, strict_match=False)
         for param_name in param_setup:
             # resolve variable set
             if param_name.startswith("<") and param_name.endswith(">"):
                 selected_params = self.get_variables(param_name.strip("<>"))
             else:
                 selected_params = [sname for sname in source_names if fnmatch.fnmatch(sname, param_name)]
-            if not selected_params:
-                # check the possibility that the parameter is not a variable
-                param = self.workspace.obj(param_name)
-                if param:
-                    selected_params = [param]
+            if (not selected_params):
+                if (not strict):
+                    # check the possibility that the parameter is not a variable
+                    param = self.workspace.obj(param_name)
+                    if param:
+                        selected_params = [param]
+                    else:
+                        self.stdout.warning(f'Parameter "{param_name}" does not exist. No modification will be made.')
                 else:
-                    self.stdout.warning(f'Parameter "{param_name}" does not exist. No modification will be made.', "red")
+                    self.stdout.warning(f'Parameter "{param_name}" do not belong to the given '
+                                        'parameter set. No modification will be made.')
             for param in selected_params:
                 if isinstance(param, str):
                     param = source[param]
                 self._set_parameter(param, param_setup[param_name], mode=mode)
                 selected_parameters.append(param)
         return selected_parameters
 
@@ -762,33 +807,43 @@
             prefit_variation, constraint_type, _ = self.inspect_constrained_nuisance_parameter(nuis, all_constraints)
             if constraint_type=='gaus':
                 self.stdout.info(f'Changing error of {nuis_name} from {nuis.getError()} to {prefit_variation}')
                 nuis.setError(prefit_variation)
                 nuis.removeRange()    
         return None
     
-    def get_poi(self, poi_name:Optional[str]=None, strict:bool=False):
+    def get_poi(self, poi_name:Optional[Union[str, List[str]]]=None, strict:bool=False):
         """Get POI variable by name
         
         Arguments
-            poi_name: str
-                name of POI to retrieve
+            poi_name: (optional) str, list of str
+                Name of POI to retrieve. A list of names can be given to retrieve multiple POIs.
+                If None, the first POI defined in the model config will be returned.
             strict: bool
                 require the variable to be defined in the POI list, throw error otherwise
         """
         if poi_name is None:
             poi = self.pois.first()
             self.stdout.info(f'POI name not specified. The first POI "{poi.GetName()}" is used by default.')
-        else:
-            poi = self.workspace.var(poi_name)
-        if not poi:
-            raise RuntimeError(f'workspace does not contain the variable "{poi_name}"')
-        if strict and (poi not in list(self.pois)):
-            raise RuntimeError(f'workspace variable "{poi_name}" is not part of the POIs')
-        return poi
+            return poi
+        if isinstance(poi_name, str):
+            poi_names = [poi_name]
+        else:
+            poi_names = list(poi_name)
+        pois = ROOT.RooArgSet()
+        for name in poi_names:
+            poi = self.workspace.var(name)
+            if not poi:
+                raise RuntimeError(f'workspace does not contain the variable "{name}"')
+            if strict and (poi not in list(self.pois)):
+                raise RuntimeError(f'workspace variable "{name}" is not part of the POIs')
+            pois.add(poi)
+        if isinstance(poi_name, str):
+            return pois.first()
+        return pois
     
     def _load_obs_and_weight(self, obs_and_weight:Optional[Union["ROOT.RooArgSet",str]]=None, 
                              weight_var:Optional[Union["ROOT.RooRealVar",str]]=None):
         # get the weight variable
         if weight_var is None:
             weight_name = self._DEFAULT_NAMES_['weight']
             weight_var = self.workspace.var(weight_name)
@@ -939,23 +994,24 @@
                 are saved as "conditionalNuis_{mu}" and "conditionalGlobs_{mu}" irrespective of
                 whether nuisance parameter profiling is performed and whether conditional mle
                 is used for the profiling. This is to faciliate the use case of Asymptotic limit
                 calculation. The names of these snahpshots can be customized via the
                 `snapshot_names` option.
         
             Arguments:
-                poi_name: str
-                    Name of the parameter of interest (POI).
-                poi_val: (Optional) float
-                    Generate asimov data with POI set at the specified value. If None, POI will be kept
-                    at the post-fit value if a fitting is performed or the pre-fit value if no fitting
+                poi_name: (optional) str, list of str
+                    Name of POI to retrieve. A list of names can be given to retrieve multiple POIs.
+                If None, the first POI defined in the model config will be returned.
+                poi_val: (Optional) float, list of float
+                    Generate asimov data with POI(s) set at the specified value(s). If None, POI(s) will be kept
+                    at the post-fit value(s) if a fitting is performed or the pre-fit value if no fitting
                     is performed.
-                poi_profile: (Optional) float
-                    Perform nuisance parameter profiling with POI set at the specified value. This option
-                    is only effective if do_fit is set to True. If None, POI is set floating 
+                poi_profile: (Optional) float, list of float
+                    Perform nuisance parameter profiling with POI(s) set at the specified value(s). This option
+                    is only effective if do_fit is set to True. If None, POI(s) is set floating 
                     (i.e. unconditional maximum likelihood estimate). 
                 do_fit: bool, default=True    
                     Perform nuisance parameter profiling with a fit to the given dataset.
                 modify_globs: bool, default=True
                     Match the values of nuisance parameters and the corresponding global observables when
                     generating the asimov data. This is important for making sure the asimov data has the 
                     (conditional) minimal NLL.
@@ -969,15 +1025,17 @@
                     Case 0: All variable states will be restored.
                     Case 1: Only global observable states will be restored.
                 do_import: bool, default=True
                     Import the generated asimov data to the current workspace.
                 asimov_name: (Optional) str
                     Name of the generated asimov dataset. If None, defaults to "asimovData_{mu}" where
                     `{mu}` will be replaced by the value of `poi_val`. Other keywords are: `{mu_cond}`
-                    which is the the value of `poi_profile`.
+                    which is the the value of `poi_profile`. If multiple POIs are defined, `{mu}`
+                    will be replaced by `<poi_name_i>_<mu_i>_<poi_name_j>_<mu_j>...` and similarly for
+                    `{mu_cond}`
                 asimov_snapshot: (Optional) str
                     Name of the snapshot taken right after asimov data generation. If None, no snapshot
                     will be saved.
                 channel_asimov_name: (Optional) str
                     Name of the asimov dataset in each category of a simultaneous pdf. If None,
                     defaults to "combAsimovData_{label}" where `{label}` will be replaced by the
                 dataset: (Optional) ROOT.RooDataSet
@@ -995,95 +1053,118 @@
         """
         # define simplified ws variable names
         ws = self.workspace
         all_globs = self.global_observables
         all_nuis  = self.nuisance_parameters
         
         # define names used for various objects
-        names = copy.deepcopy(self._DEFAULT_NAMES_)
+        names = combine_dict(self._DEFAULT_NAMES_)
         if snapshot_names is not None:
             names.update(snapshot_names)
         if asimov_name is not None:
             names['asimov'] = asimov_name
             names['asimov_no_poi'] = asimov_name
         if channel_asimov_name is not None:
             names['channel_asimov'] = channel_asimov_name
         nom_vars_name = names['nominal_vars']
         nom_glob_name = names['nominal_globs']
         nom_nuis_name = names['nominal_nuis']
         con_glob_name = names['conditional_globs']
         con_nuis_name = names['conditional_nuis']
 
         if poi_name is None:
-            poi = None
+            poi_set = None
         else:
-            poi = self.get_poi(poi_name)
+            poi_set = self.get_poi(poi_name)
+            
+        poi_const_state = {}
+        if poi_set is not None:
+            if isinstance(poi_set, ROOT.RooRealVar):
+                poi_const_state[poi_set] = poi_set.isConstant()
+            else:
+                for poi in poi_set:
+                    poi_const_state[poi] = poi.isConstant()
         
         # take snapshot of initial states of all variables
         mutable_vars = self.get_variables(WSArgument.MUTABLE)
-        ws.saveSnapshot(nom_vars_name, mutable_vars)
+        self.save_snapshot(nom_vars_name, mutable_vars)
         if not ws.getSnapshot(nom_glob_name):
-            self.stdout.info(f'Saving snapshot "{nom_glob_name}"')
-            ws.saveSnapshot(nom_glob_name, all_globs)
+            self.save_snapshot(nom_glob_name, all_globs)
         if not ws.getSnapshot(nom_nuis_name):
-            self.stdout.info(f'Saving snapshot "{nom_nuis_name}"')
-            ws.saveSnapshot(nom_nuis_name, all_nuis)
+            self.save_snapshot(nom_nuis_name, all_nuis)
         
         if do_fit:
             if dataset is None:
                 dataset = self.data
             minimizer = self.minimizer_cls("Minimizer", self.pdf, dataset, workspace=self.workspace)
             if minimizer_options is None:
-                minimizer_options = copy.deepcopy(minimizer._DEFAULT_MINIMIZER_OPTION_)
+                minimizer_options = combine_dict(minimizer._DEFAULT_MINIMIZER_OPTION_)
             if nll_options is None:
-                nll_options = copy.deepcopy(minimizer._DEFAULT_NLL_OPTION_)
+                nll_options = combine_dict(minimizer._DEFAULT_NLL_OPTION_)
             minimizer.configure(**minimizer_options)
             if constraint_option == 0:
                 pass
             elif constraint_option == 1:
                 self.set_constrained_nuisance_parameters_to_nominal()
             else:
                 raise ValueError(f"unsupported constraint option: {constraint_option}")
             if isinstance(nll_options, dict):
                 minimizer.configure_nll(**nll_options)
             elif isinstance(nll_options, list):
                 minimizer.set_nll_commands(nll_options)
             else:
                 raise ValueError(f"unsupported nll options format")
-            if poi:
-                if poi_profile is not None:
-                    # conditional mle
-                    poi.setVal(poi_profile)
-                    poi.setConstant(1)
-                else:
+                
+            if poi_set is not None:
+                uncond_fit = poi_profile is None
+                poi_profile = self._parse_param_setup(poi_set, poi_profile, fill_missing=True)
+                if uncond_fit:
                     # unconditional mle
-                    poi.setConstant(0)
+                    self._set_parameters(poi_set, poi_profile, mode=SetValueMode.FREE)
+                else:
+                    # conditional mle
+                    self._set_parameters(poi_set, poi_profile, mode=SetValueMode.FIX)
+                    
             status = minimizer.minimize()
             self.last_fit_status = status
+        else:
+            poi_profile = self._parse_param_setup(poi_set, poi_profile, fill_missing=True)
+            
+        if poi_set is not None:
+            poi_val = self._parse_param_setup(poi_set, poi_val)
+            self._set_parameters(poi_set, poi_val)
+            
+        # restore the constant state of the pois
+        for poi, const_state in poi_const_state.items():
+            poi.setConstant(const_state)
             
-        if poi:
-            if poi_val is not None:
-                poi.setVal(poi_val)
-            poi.setConstant(0)
-            poi_val = poi.getVal()
-
         # match values of global observables to the corresponding NPs
         if modify_globs:
             self.match_globs()
+            
+        def format_mu_str(poi_setup):
+            npoi = len(poi_setup)
+            assert npoi > 0
+            if (npoi == 1):
+                return pretty_value(list(poi_setup.values())[0])
+            components = []
+            for poi_name, value in poi_setup.items():
+                    components.append(f"{poi_name}_{pretty_value(value)}")
+            return "_".join(components)
 
-        if poi:
+        if poi_set is not None:
             if do_fit:
-                ws.saveSnapshot(con_glob_name.format(mu=pretty_value(poi_profile)), all_globs)
-                ws.saveSnapshot(con_nuis_name.format(mu=pretty_value(poi_profile)), all_nuis)
+                self.save_snapshot(con_glob_name.format(mu=format_mu_str(poi_profile)), all_globs)
+                self.save_snapshot(con_nuis_name.format(mu=format_mu_str(poi_profile)), all_nuis)
             else:
-                ws.saveSnapshot(con_glob_name.format(mu=pretty_value(poi_val)), all_globs)
-                ws.saveSnapshot(con_nuis_name.format(mu=pretty_value(poi_val)), all_nuis)
+                self.save_snapshot(con_glob_name.format(mu=format_mu_str(poi_val)), all_globs)
+                self.save_snapshot(con_nuis_name.format(mu=format_mu_str(poi_val)), all_nuis)
 
-            asimov_data_name = names['asimov'].format(mu=pretty_value(poi_val),
-                                                      mu_cond=pretty_value(poi_profile))
+            asimov_data_name = names['asimov'].format(mu=format_mu_str(poi_val),
+                                                      mu_cond=format_mu_str(poi_profile))
         else:
             asimov_data_name = names['asimov_no_poi']
             
         channel_asimov_data_name = names['channel_asimov']
         sim_pdf = self.pdf
         if not isinstance(sim_pdf, ROOT.RooSimultaneous):
             asimov_data = self.generate_asimov_from_pdf(asimov_data_name, sim_pdf)
@@ -1104,32 +1185,31 @@
                                           ROOT.RooArgSet(obs_and_weight, channel_cat),
                                           ROOT.RooFit.Index(channel_cat),
                                           ROOT.RooFit.Import(dataset_map),
                                           ROOT.RooFit.WeightVar(weight_var))
 
         if do_import:
             if ws.data(asimov_data_name):
-                self.stdout.warning(f"[WARNING] Dataset with name {asimov_data_name} already exists in the "
+                self.stdout.warning(f"Dataset with name {asimov_data_name} already exists in the "
                                     "workspace. The newly generated dataset will not overwrite the original "
                                     "dataset.")
-            getattr(ws, "import")(asimov_data)
+            ws.Import(asimov_data)
             self.stdout.info(f'Generated Asimov Dataset "{asimov_data_name}"')
             
         if asimov_snapshot is not None:
-            snapshot_name = asimov_snapshot.format(mu=pretty_value(poi_val),
-                                                   mu_cond=pretty_value(poi_profile))
-            self.stdout.info(f'Saving snapshot "{snapshot_name}"')
-            ws.saveSnapshot(snapshot_name, mutable_vars)
+            snapshot_name = asimov_snapshot.format(mu=format_mu_str(poi_val),
+                                                   mu_cond=format_mu_str(poi_profile))
+            self.save_snapshot(snapshot_name, mutable_vars)
     
         if restore_states == 0:
             # load back a snapshot of all variable's initial states
-            ws.loadSnapshot(nom_vars_name)
+            self.load_snapshot(nom_vars_name)
         elif restore_states == 1:
             # load back a snapshot of the initial global observable states
-            ws.loadSnapshot(nom_glob_name)
+            self.load_snapshot(nom_glob_name)
         elif restore_states == 2:
             pass
         else:
             raise ValueError(f'unsupported restore state option "{restore_states}"')
         
         return asimov_data
     
@@ -1953,19 +2033,19 @@
     def load_snapshot(self, snapshot_name:Optional[str]=None):
         if snapshot_name is not None:
             snapshot = self.workspace.getSnapshot(snapshot_name)
             if (not snapshot) and ('0x(nil)' in snapshot.__repr__()):
                 self.stdout.warning(f'Snapshot "{snapshot_name}" does not exist.')
             else:
                 self.workspace.loadSnapshot(snapshot_name)
-                self.stdout.debug(f'Loaded snapshot "{snapshot_name}"')
+                self.stdout.info(f'Loaded snapshot "{snapshot_name}"')
                 
     def save_snapshot(self, snapshot_name:Optional[str]=None, 
                       variables:Optional[Union[ROOT.RooArgSet, str, WSArgument]]=None):
         if snapshot_name is not None:
             if variables is None:
                 self.workspace.saveSnapshot(snapshot_name, self.workspace.allVars())
             else:
                 if isinstance(variables, (str, WSArgument)):
                     variables = self.get_variables(variables)
                 self.workspace.saveSnapshot(snapshot_name, variables)
-            self.stdout.debug(f'Saved snapshot "{snapshot_name}"')
+            self.stdout.info(f'Saved snapshot "{snapshot_name}"')
```

### Comparing `quickstats-0.6.8.4/quickstats/components/extended_rfile.py` & `quickstats-0.6.8.6/quickstats/components/extended_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/likelihood.py` & `quickstats-0.6.8.6/quickstats/components/likelihood.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,33 +34,14 @@
         config['verbosity'] = verbosity
         if 'preset_param' not in config:
             config['preset_param'] = True
         self._inherit_init(super().__init__, **config)
         self.roofit_result = None
     
     @staticmethod
-    def _parse_poi_val(pois:"ROOT.RooArgSet", poi_val:Optional[Union[Dict[str, float], float]]=None):
-        if poi_val is None:
-            poi_val = {}
-            for poi in pois:
-                poi_val[poi.GetName()] = poi.getVal()
-        elif not isinstance(poi_val, dict):
-            poi_val_tmp = poi_val
-            poi_val = {}
-            for poi in pois:
-                poi_val[poi.GetName()] = poi_val_tmp
-        else:
-            # fill in missing values
-            for poi in pois:
-                poi_name = poi.GetName()
-                if poi_name not in poi_val:
-                    poi_val[poi_name] = poi.getVal()
-        return poi_val
-    
-    @staticmethod
     def get_combined_fit_result(uncond_fit_result:Dict, cond_fit_result:Dict):
         combined_fit_result = {}
         nll_uncond = uncond_fit_result['nll']
         nll_cond = cond_fit_result['nll']
         pnll = nll_cond - nll_uncond
         qmu  = 2 * pnll
         combined_fit_result['pnll'] = pnll
@@ -141,18 +122,15 @@
         if "cond" not in snapshot_name:
             snapshot_name["cond"] = self.kCurrentSnapshotName
             self.stdout.info(f'No snapshot given for conditional fit. The snapshot "{self.kCurrentSnapshotName}" '
                              'will be used by default')
         if set(snapshot_name.keys()) != set(["uncond", "cond"]):
             raise ValueError('when snapshot name is given as a dictionary, it must be of the '
             'form {"cond": <conditional_fit_snapshot>, "uncond": <unconditional_fit_snapshot>}')
-        
-        self.load_snapshot(snapshot_name["cond"])
-        poi_val = self._parse_poi_val(pois, poi_val)
-        
+
         nll_uncond = None
         nll_cond   = None
         muhat      = None
         
         tmp_do_minos = self.minimizer.config['minos']
         
         self.minimizer.config['minos'] = do_minos
@@ -201,14 +179,15 @@
                 muhat_errlo[poi_name] = poi.getErrorLo()
                 muhat_errhi[poi_name] = poi.getErrorHi()
         fit_time_uncond = time.time() - start_time
         # conditional nll
         if mode in [FitMode.HYBRID, FitMode.COND]:
             # restore initial parameter values after each fit
             self.load_snapshot(snapshot_name["cond"])
+            poi_val = self.model._parse_param_setup(pois, poi_val, fill_missing=True)
             # fix other pois if they are not studied
             for poi in self.model.pois:
                 poi.setConstant(1)
             for poi in pois:
                 val = poi_val[poi.GetName()]
                 # profiled poi
                 if val is None:
@@ -235,15 +214,15 @@
                 'nll': nll_uncond,
                 'status': fit_status_uncond,
                 'time': fit_time_uncond
             }
         if mode in [FitMode.HYBRID, FitMode.COND]:
             mu = {name:pretty_value(value) for name, value in poi_val.items()}
             mu_str = ", ".join([f"{name} = {pretty_value(value)}" for name, value in poi_val.items()])
-            self.stdout.info("mu : ".rjust(15) + f"{mu_str}", bare=True)
+            self.stdout.info("cond value : ".rjust(15) + f"{mu_str}", bare=True)
             # also add the best-fit value for profiled POIs
             for name, value in poi_val.items():
                 if value == None:
                     muhat[name] = self.model.workspace.var(name).getVal()
             self.stdout.info("cond NLL = ".rjust(15)+f"{nll_cond:.5f}", bare=True)
             fit_result['cond_fit'] = {
                 'mu': mu,
```

### Comparing `quickstats-0.6.8.4/quickstats/components/modelling/component_source.py` & `quickstats-0.6.8.6/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/modelling/data_modelling.py` & `quickstats-0.6.8.6/quickstats/components/modelling/data_modelling.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/modelling/model_source.py` & `quickstats-0.6.8.6/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.6.8.6/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.6.8.6/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.6.8.6/quickstats/components/modelling/tree_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.6.8.6/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.6.8.6/quickstats/components/nuisance_parameter_pull.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/nuisance_parameter_ranking.py` & `quickstats-0.6.8.6/quickstats/components/nuisance_parameter_ranking.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/__init__.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_declare.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_define.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_export.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_export.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_filter.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_filter.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_load_macro.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_load_macro.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_report.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_safe_alias.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_safe_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_save.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/actions/rooproc_treename.py` & `quickstats-0.6.8.6/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/builtin_methods.py` & `quickstats-0.6.8.6/quickstats/components/processors/builtin_methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -188,20 +188,41 @@
     RVec<LorentzVector<T>> SortLVByPT(const RVec<LorentzVector<T>> &lv_vec, const bool descending=true){
         if (descending)
             return Sort(lv_vec, [](LorentzVector<T> x, LorentzVector<T> y){return x.Pt() > y.Pt();});
         return Sort(lv_vec, [](LorentzVector<T> x, LorentzVector<T> y){return x.Pt() < y.Pt();});
     }
     
     template<typename T>
-    RVec< typename RVec< T >::size_type > ArgSortLVByPT(const RVec<LorentzVector<T>> &lv_vec, const bool descending=true){
+    RVec< typename RVec< T >::size_type > ArgSortLVByPT(const RVec<LorentzVector<T>> &lv_vec, const bool &descending=true){
         if (descending)
             return Argsort(lv_vec, [](LorentzVector<T> x, LorentzVector<T> y){return x.Pt() > y.Pt();});
         return Argsort(lv_vec, [](LorentzVector<T> x, LorentzVector<T> y){return x.Pt() < y.Pt();});
     }
     
+    template<typename T>
+    RVec< typename RVec< T >::size_type > GetP4RankedByPT(const RVec<LorentzVector<T>> &p4_vec, const size_t &rank, const bool descending=true){
+        auto sort_indices = ArgSortLVByPT(p4_vec, descending);
+        
+    }
+    
+    template<typename T>
+    LorentzVector<T> GetP4RankedByPT(const RVec<LorentzVector<T>> &p4_vec, const RVec< typename RVec< T >::size_type > &sort_indices, const size_t &rank){
+        if (p4_vec.size() != sort_indices.size())
+            throw std::runtime_error("size mismatch between p4 vectors and sort indices");
+        if (rank >= p4_vec.size())
+            return LorentzVector<T>{};
+        return p4_vec[sort_indices[rank]];
+    }
+
+    template<typename T>
+    LorentzVector<T> GetP4RankedByPT(const RVec<LorentzVector<T>> &p4_vec, const size_t &rank, const bool descending=true){
+         RVec< typename RVec< T >::size_type > sort_indices = ArgSortLVByPT(p4_vec, descending);
+        return GetP4RankedByPT(p4_vec, sort_indices, rank);
+    }
+    
     template<typename T1, typename T2>
     T1 PairFirst(const std::pair<T1, T2> &p){
         return p.first;
     }
     
     template<typename T1, typename T2>
     T2 PairSecond(const std::pair<T1, T2> &p){
```

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/roo_config_parser.py` & `quickstats-0.6.8.6/quickstats/components/processors/roo_config_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/processors/roo_processor.py` & `quickstats-0.6.8.6/quickstats/components/processors/roo_processor.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/pvalue_toys.py` & `quickstats-0.6.8.6/quickstats/components/pvalue_toys.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/roo_inspector.py` & `quickstats-0.6.8.6/quickstats/components/roo_inspector.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/root_object.py` & `quickstats-0.6.8.6/quickstats/components/root_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/toy_limit_calculator.py` & `quickstats-0.6.8.6/quickstats/components/toy_limit_calculator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/__init__.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/asimov_handler.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/core_argument_sets.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/sample.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/settings.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/settings.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/systematic.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/systematic.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/ws_comparer.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,16 +258,16 @@
         df_merge = self.df_1.merge(self.df_2, on="name", how='outer', indicator=True, sort=True,
                                    suffixes=('_left', '_right'), validate="one_to_one")
         df_merge['same_definition'] = df_merge['definition_left'] == df_merge['definition_right']
         columns = ["name", "definition_left", "definition_right", "class_left", "class_right"]
         import pandas as pd
         df_merge[columns] = df_merge[columns].astype(str)
         regex = re.compile(r"([a-zA-Z_][a-zA-Z0-9_]*)")
-        expression_left  = df_merge['definition_left'].str.replace(regex, "")
-        expression_right = df_merge['definition_right'].str.replace(regex, "")
+        expression_left  = df_merge['definition_left'].str.replace(regex, "", regex=True)
+        expression_right = df_merge['definition_right'].str.replace(regex, "", regex=True)
         df_merge['same_expression'] = expression_left == expression_right
         df_merge['category'] = df_merge['_merge']
         new_categories = ["identical", "redefined", "reconstituted", "renamed", "remapped", "splitted", "merged"]
         df_merge['category'] = df_merge['category'].cat.add_categories(new_categories)
         mask_identical = (df_merge['_merge'] == "both") & (df_merge['same_definition'])
         mask_redefined = (df_merge['_merge'] == "both") & (~df_merge['same_definition'])
         df_merge.loc[mask_identical, ['category']] = 'identical'
```

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/ws_decomposer.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/ws_decomposer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.6.8.6/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/concurrent/abstract_runner.py` & `quickstats-0.6.8.6/quickstats/concurrent/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/concurrent/logging.py` & `quickstats-0.6.8.6/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/concurrent/nuisance_parameter_ranking_runner.py` & `quickstats-0.6.8.6/quickstats/concurrent/nuisance_parameter_ranking_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.6.8.6/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.6.8.6/quickstats/concurrent/parameterised_likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.6.8.6/quickstats/concurrent/parameterised_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/core/abstract_object.py` & `quickstats-0.6.8.6/quickstats/core/abstract_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/core/configs.py` & `quickstats-0.6.8.6/quickstats/core/configs.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/core/configurable_object.py` & `quickstats-0.6.8.6/quickstats/core/configurable_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/core/dataclass_object.py` & `quickstats-0.6.8.6/quickstats/core/dataclass_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/core/decorators.py` & `quickstats-0.6.8.6/quickstats/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/core/enums.py` & `quickstats-0.6.8.6/quickstats/core/enums.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/core/methods.py` & `quickstats-0.6.8.6/quickstats/core/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/core/path_manager.py` & `quickstats-0.6.8.6/quickstats/core/path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/core/virtual_trees.py` & `quickstats-0.6.8.6/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/cppyy/core.py` & `quickstats-0.6.8.6/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/cppyy/macros.py` & `quickstats-0.6.8.6/quickstats/interface/cppyy/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.6.8.6/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/RooAbsData.py` & `quickstats-0.6.8.6/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/RooAbsPdf.py` & `quickstats-0.6.8.6/quickstats/interface/root/RooAbsPdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/RooCategory.py` & `quickstats-0.6.8.6/quickstats/interface/root/RooCategory.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/RooDataSet.py` & `quickstats-0.6.8.6/quickstats/interface/root/RooDataSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/RooMsgService.py` & `quickstats-0.6.8.6/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/RooRealVar.py` & `quickstats-0.6.8.6/quickstats/interface/root/RooRealVar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/TF1.py` & `quickstats-0.6.8.6/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/TFile.py` & `quickstats-0.6.8.6/quickstats/interface/root/TFile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/TH1.py` & `quickstats-0.6.8.6/quickstats/interface/root/TH1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/TH2.py` & `quickstats-0.6.8.6/quickstats/interface/root/TH2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/TObject.py` & `quickstats-0.6.8.6/quickstats/interface/root/TObject.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/__init__.py` & `quickstats-0.6.8.6/quickstats/interface/root/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/helper.py` & `quickstats-0.6.8.6/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/inspection.py` & `quickstats-0.6.8.6/quickstats/interface/root/inspection.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/macros.py` & `quickstats-0.6.8.6/quickstats/interface/root/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/interface/root/roofit_extension.py` & `quickstats-0.6.8.6/quickstats/interface/root/roofit_extension.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.6.8.6/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.6.8.6/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.6.8.6/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.6.8.6/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.6.8.6/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.6.8.6/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.6.8.6/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.6.8.6/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.6.8.6/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/maths/numerics.py` & `quickstats-0.6.8.6/quickstats/maths/numerics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/maths/statistics.py` & `quickstats-0.6.8.6/quickstats/maths/statistics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/maths/statistics_jitted.py` & `quickstats-0.6.8.6/quickstats/maths/statistics_jitted.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/maths/symbolics.py` & `quickstats-0.6.8.6/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/parsers/param_parser.py` & `quickstats-0.6.8.6/quickstats/parsers/param_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/__init__.py` & `quickstats-0.6.8.6/quickstats/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/abstract_plot.py` & `quickstats-0.6.8.6/quickstats/plots/abstract_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,30 +44,32 @@
         self.styles = combine_dict(self.STYLES, styles)
         self.styles = parse_styles(self.styles)
         
         if analysis_label_options is None:
             self.analysis_label_options = None
         else:
             self.analysis_label_options = parse_analysis_label_options(analysis_label_options)
-            
-        self.legend_order = self.get_default_legend_order()
-        
-        self.legend_data = {}
-        self.legend_data_sec = {}
-        self.legend_data_ext = {}
+
+        self.reset_legend_data()
         
         self.figure_index = figure_index
         
         self.config = combine_dict(AbstractPlot.CONFIG, self.CONFIG)
         if config is not None:
             self.config = combine_dict(self.config, config)
 
         self.set_color_cycle(color_cycle)
             
         self.annotation_list = []
+    
+    def reset_legend_data(self):
+        self.legend_data = {}
+        self.legend_data_sec = {}
+        self.legend_data_ext = {}
+        self.legend_order = self.get_default_legend_order()
         
     def add_annotation(self, text:str, **kwargs):
         self.annotation_list.append({"text": text, **kwargs})
         
     def set_color_cycle(self, color_cycle:Optional[Union[List, str, "ListedColorMap"]]=None):
         if color_cycle is None:
             color_cycle = self.COLOR_CYCLE
```

### Comparing `quickstats-0.6.8.4/quickstats/plots/bidirectional_bar_chart.py` & `quickstats-0.6.8.6/quickstats/plots/bidirectional_bar_chart.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/collective_data_plot.py` & `quickstats-0.6.8.6/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/color_schemes.py` & `quickstats-0.6.8.6/quickstats/plots/color_schemes.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/core.py` & `quickstats-0.6.8.6/quickstats/plots/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/correlation_plot.py` & `quickstats-0.6.8.6/quickstats/plots/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/general_1D_plot.py` & `quickstats-0.6.8.6/quickstats/plots/general_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/general_distribution_plot.py` & `quickstats-0.6.8.6/quickstats/plots/general_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/histo_1D_plot.py` & `quickstats-0.6.8.6/quickstats/plots/histo_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.6.8.6/quickstats/plots/hypotest_inverter_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/likelihood_2D_plot.py` & `quickstats-0.6.8.6/quickstats/plots/likelihood_2D_plot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,90 @@
-from typing import Dict, Optional, Union, List
+from typing import Dict, Optional, Union, List, Sequence
+
+from itertools import repeat
+
 import numpy as np
 import pandas as pd
 
 from quickstats.plots import AbstractPlot
 from quickstats.plots.template import create_transform
 from quickstats.utils.common_utils import combine_dict
+from quickstats.maths.interpolation import get_regular_meshgrid
 from matplotlib.lines import Line2D
 
 
 class Likelihood2DPlot(AbstractPlot):
 
     CONFIG = {
-        'sigma_levels': ('1sigma', '2sigma', '3sigma'),
-        'sigma_pos': 0.93,
-        'sigma_names': ('1 $\sigma$', '2 $\sigma$', '3 $\sigma$'),
-        'sigma_colors': ("hh:darkblue", "#F2385A", "#FDC536"),
+        # intervals to include in the plot
+        "interval_formats": {
+            "68_95"               : ('0.68', '0.95'),
+            "one_two_sigma"       : ('1sigma', '2sigma'),
+            "68_95_99"            : ('0.68', '0.95', '0.99'),
+            "one_two_three_sigma" : ('1sigma', '2sigma', '3sigma')
+        },
         'highlight_styles': {
             'linewidth': 0,
             'marker': '*',
             'markersize': 20,
             'color': '#E9F1DF',
             'markeredgecolor': 'black'
         },
         'bestfit_styles':{
             'marker': 'P',
             'linewidth': 0,
             'markersize': 15
         },
+        'contour_styles': {
+            'linestyles': 'solid',
+            'linewidths': 3
+        },
         'bestfit_label': "Best fit ({x:.2f}, {y:.2f})",
         'cmap': 'GnBu',
         'interpolation': 'cubic',
         'num_grid_points': 500,
     }
-    # https://pdg.lbl.gov/2018/reviews/rpp2018-rev-statistics.pdf#page=31
-    likelihood_label_threshold = {
-        '0.68': 2.30,
-        '1sigma': 2.30, # 68.2%
-        '0.90': 4.61,
-        '0.95': 5.99,
-        '2sigma': 6.18, # 95.45%
-        '0.99': 9.21,
-        '3sigma': 11.83, #  99.73%
+    
+    # qmu from https://pdg.lbl.gov/2018/reviews/rpp2018-rev-statistics.pdf#page=31
+    coverage_proba_data = {
+        '0.68': {
+            'qmu': 2.30,
+            'label': '68% CL',
+            'color': "hh:darkblue"
+        },
+        '1sigma': {  
+            'qmu': 2.30, # 68.2%
+            'label': '1 $\sigma$',
+            'color': "hh:darkblue"
+        },
+        '0.90': {
+            'qmu': 4.61,
+            'label': '90% CL',
+            'color': "#36b1bf"
+        },
+        '0.95': {
+            'qmu': 5.99,
+            'label': '95% CL',
+            'color': "#F2385A"
+        },
+        '2sigma': {
+            'qmu': 6.18, # 95.45%
+            'label': '2 $\sigma$',
+            'color': "#F2385A"
+        },
+        '0.99': {
+            'qmu': 9.21,
+            'label': '99% CL',
+            'color': "#FDC536"
+        },
+        '3sigma': {
+            'qmu': 11.83, # 99.73%
+            'label': '3 $\sigma$',
+            'color': "#FDC536"
+        }
     }
 
     def __init__(self, data_map: Union[pd.DataFrame, Dict[str, pd.DataFrame]],
                  label_map: Optional[Dict] = None,
                  styles_map: Optional[Dict] = None,
                  config_map: Optional[Dict] = None,
                  color_cycle=None,
@@ -53,94 +93,119 @@
                  config: Optional[Dict] = None):
 
         self.data_map = data_map
         self.label_map = label_map
         self.styles_map = styles_map
         self.config_map = config_map
         self.highlight_data = []
-        self.legend_order = []
         self.contours = None
 
         super().__init__(color_cycle=color_cycle,
                          styles=styles,
                          analysis_label_options=analysis_label_options,
                          config=config)
-
-    def get_default_legend_order(self):
-        if not isinstance(self.data_map, dict):
-            return self.legend_order
-        else:
-            return list(self.data_map)
+        
+    def get_sigma_levels(self, interval_format:str="one_two_three_sigma"):
+        if interval_format not in self.config['interval_formats']:
+            choices = ','.join([f'"{choice}"' for choice in self.config['interval_formats']])
+            raise ValueError(f'undefined sigma interval format: {interval_format} (choose from {choices})')
+        sigma_levels = self.config['interval_formats'][interval_format]
+        return sigma_levels
 
     def draw_single_data(self, ax, data: pd.DataFrame,
-                         xattrib: str, yattrib: str, zattrib: str = 'qmu',
+                         xattrib: str, yattrib: str,
+                         zattrib: str = 'qmu',
                          styles: Optional[Dict] = None,
-                         config: Optional[Dict] = None,
-                         clabel_size=None, show_colormesh=False):
-        if config is None:
-            config = self.config
-        colors = list(config['sigma_colors'])
-        if 'sigma_linestyles' not in config:
-            config['sigma_linestyles'] = ['solid'] * \
-                len(list(config['sigma_colors']))
-        linestyles = list(config['sigma_linestyles'])
-        levels = [self.likelihood_label_threshold[key]
-                        for key in config['sigma_levels']]
-        if config['interpolation'] is not None:
+                         clabel_size=None, show_colormesh=False,
+                         interval_format:str="one_two_three_sigma"):
+        config = combine_dict(self.config)
+        sigma_levels = self.get_sigma_levels(interval_format=interval_format)
+        sigma_values = [self.coverage_proba_data[level]['qmu'] for level in sigma_levels]
+        sigma_labels = [self.coverage_proba_data[level]['label'] for level in sigma_levels]
+        sigma_colors = [self.coverage_proba_data[level]['color'] for level in sigma_levels]
+
+        interpolate_method = config.get('interpolation', None)
+        if interpolate_method is not None:
             from scipy import interpolate
-            x = data[xattrib]
-            y = data[yattrib]
-            z = data[zattrib]
-
-            def get_grid(X_range, Y_range, num_grid_points):
-                X_points = np.linspace(*X_range, num_grid_points)
-                Y_points = np.linspace(*Y_range, num_grid_points)
-                X_grid, Y_grid = np.meshgrid(X_points, Y_points)
-                return X_grid, Y_grid
-            X, Y = get_grid(X_range=(x.min(), x.max()), Y_range=(
-                y.min(), y.max()), num_grid_points=config['num_grid_points'])
-            Z = interpolate.griddata(
-                np.stack((x, y), axis=1), z, (X, Y), method=config['interpolation'])
-        else:  # buggy for [dict]
-            X_unique = np.sort(self.data_map[xattrib].unique())
-            Y_unique = np.sort(self.data_map[yattrib].unique())
+            x, y, z = data[xattrib], data[yattrib], data[zattrib]
+            n = config.get('num_grid_points', 500)
+            X, Y = get_regular_meshgrid(x, y, n=n)
+            Z = interpolate.griddata(np.stack((x, y), axis=1), z, (X, Y), interpolate_method)
+        else:
+            X_unique = np.sort(data[xattrib].unique())
+            Y_unique = np.sort(data[yattrib].unique())
             X, Y = np.meshgrid(X_unique, Y_unique)
-            Z = self.data_map.pivot_table(
-                index=xattrib, columns=yattrib, values=zattrib).T.values - self.data_map[zattrib].min()
-
+            Z = (data.pivot_table(index=xattrib, columns=yattrib, values=zattrib).T.values
+                 - data[zattrib].min())
+            
         if show_colormesh:
             cmap = config['cmap']
             im = ax.pcolormesh(X, Y, Z, cmap=cmap, shading='auto')
             import matplotlib.pyplot as plt
             self.cbar = plt.colorbar(im, ax=ax, **config['colorbar'])
             self.cbar.set_label(**config['colorbar_label'])
-        if levels:
-            cp = ax.contour(X, Y, Z, levels=levels, colors=colors,
-                        linestyles=linestyles, linewidths=3)
+            
+        if sigma_values:
+            cp = ax.contour(X, Y, Z, levels=sigma_values, colors=sigma_colors,
+                            **config['contour_styles'])
             if clabel_size is not None:
                 ax.clabel(cp, inline=True, fontsize=clabel_size)
-        custom_handles = [Line2D([0], [0], color=color, linestyle=linestyle, lw=3, label=label) \
-                          for color, key, label, linestyle in \
-                          zip(config['sigma_colors'], config['sigma_levels'], config['sigma_names'], config['sigma_linestyles'])]
-        self.update_legend_handles(
-            dict(zip(config['sigma_names'], custom_handles)))
-        self.legend_order.extend(config['sigma_names'])
+                
+        line_styles = self._get_line_styles(config['contour_styles'])
+        custom_handles = [Line2D([0], [0], color=color, label=label, **styles) \
+                          for color, label, styles in zip(sigma_colors, sigma_labels, line_styles)]
+        self.update_legend_handles(dict(zip(sigma_labels, custom_handles)))
+        self.legend_order.extend(sigma_labels)
         return custom_handles
+    
+    def _get_line_styles(self, styles:Dict):
+        style_key_map = {
+            'linestyles': 'linestyle',
+            'linewidths': 'linewidth'
+        }
+        new_styles = {new_name: styles[old_name] for old_name, new_name \
+                      in style_key_map.items() if old_name in styles}
+        sizes = []
+        for style in new_styles.values():
+            if (isinstance(style, Sequence)) and (not isinstance(style, str)):
+                sizes.append(len(style))
+            else:
+                sizes.append(1)
+        if not sizes:
+            return repeat({})
+        if not len(np.unique(sizes)) == 1:
+            raise ValueError('contour line styles have inconsistent sizes')
+        size = np.unique(sizes)[0]
+        if size == 1:
+            return repeat(new_styles)
+        list_styles = []
+        for i in range(size):
+            styles_i = {key: value[i] for key, value in new_styles.items()}
+            list_styles.append(styles_i)
+        return list_styles
 
-    def draw(self, xattrib: str, yattrib: str, zattrib: str = 'qmu', xlabel: Optional[str] = "",
+    def draw(self, xattrib:str, yattrib:str, zattrib:str='qmu', xlabel: Optional[str] = "",
              ylabel: Optional[str] = "", zlabel: Optional[str] = "$-2\Delta ln(L)$",
-             ymax: float = 5, ymin: float = -5, xmin: Optional[float] = -10, xmax: Optional[float] = 10,
+             ymax:Optional[float]=None, ymin:Optional[float]=None,
+             xmin:Optional[float]=None, xmax:Optional[float]=None,
              clabel_size=None, draw_sm_line: bool = False, draw_bestfit:bool=True,
-             show_colormesh=False, show_legend=True):
+             show_colormesh=False, show_legend=True,
+             interval_format:str="one_two_three_sigma"):
+        self.reset_legend_data()
         ax = self.draw_frame()
         self.contours = {'keys': [], 'contours': [], 'levels': []}
         if isinstance(self.data_map, pd.DataFrame):
             self.draw_single_data(ax, self.data_map, xattrib=xattrib, yattrib=yattrib,
-                                  zattrib=zattrib, styles=self.styles_map, config=self.config,
-                                  clabel_size=clabel_size, show_colormesh=show_colormesh)
+                                  zattrib=zattrib, styles=self.styles_map,
+                                  clabel_size=clabel_size, show_colormesh=show_colormesh,
+                                  interval_format=interval_format)
+        else:
+            raise ValueError("invalid data format")
+            
+        """
         elif isinstance(self.data_map, dict):
             if self.styles_map is None:
                 styles_map = {k: None for k in self.data_map}
             else:
                 styles_map = self.styles_map
             if self.label_map is None:
                 label_map = {k: k for k in self.data_map}
@@ -161,16 +226,16 @@
                 handle = self.draw_single_data(ax, data,
                                                xattrib=xattrib,
                                                yattrib=yattrib,
                                                zattrib=zattrib,
                                                styles=styles,
                                                config=config,
                                                show_colormesh=show_colormesh)
-        else:
-            raise ValueError("invalid data format")
+                         
+        """
         
         highlight_index = 0
         
         if draw_bestfit and isinstance(self.data_map, pd.DataFrame):
             bestfit_idx = np.argmin(self.data_map[zattrib].values)
             bestfit_x   = self.data_map.iloc[bestfit_idx][xattrib]
             bestfit_y   = self.data_map.iloc[bestfit_idx][yattrib]
```

### Comparing `quickstats-0.6.8.4/quickstats/plots/np_ranking_plot.py` & `quickstats-0.6.8.6/quickstats/plots/np_ranking_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.6.8.6/quickstats/plots/pdf_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/sample_purity_plot.py` & `quickstats-0.6.8.6/quickstats/plots/sample_purity_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/score_distribution_plot.py` & `quickstats-0.6.8.6/quickstats/plots/score_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/stat_plot_config.py` & `quickstats-0.6.8.6/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/template.py` & `quickstats-0.6.8.6/quickstats/plots/template.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.6.8.6/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.6.8.6/quickstats/plots/upper_limit_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.6.8.6/quickstats/plots/upper_limit_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/upper_limit_3D_plot.py` & `quickstats-0.6.8.6/quickstats/plots/upper_limit_3D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/upper_limit_benchmark_plot.py` & `quickstats-0.6.8.6/quickstats/plots/upper_limit_benchmark_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/plots/variable_distribution_plot.py` & `quickstats-0.6.8.6/quickstats/plots/variable_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/root_checker.py` & `quickstats-0.6.8.6/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/utils/common_utils.py` & `quickstats-0.6.8.6/quickstats/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/utils/data_conversion.py` & `quickstats-0.6.8.6/quickstats/utils/data_conversion.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/utils/hep_utils.py` & `quickstats-0.6.8.6/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/utils/io.py` & `quickstats-0.6.8.6/quickstats/utils/io.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/utils/roofit_utils.py` & `quickstats-0.6.8.6/quickstats/utils/roofit_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,16 @@
     if len(expressions) != 1:
         raise RuntimeError("invalid RooFit factory expression")
     expression = expressions[0]
     variables_regex = re.compile(r"\('.*?',(.*)\)")
     variables = variables_regex.findall(formula)
     if len(variables) != 1:
         raise RuntimeError("invalid RooFit factory expression")
-    variables = split_str(variables[0], sep=',', remove_empty=True)
+    variable_regex = re.compile(f"([a-zA-Z]\w*)")
+    variables = variable_regex.findall(variables[0])
     recovered_formula = expression
     for i, variable in enumerate(variables):
         recovered_formula = re.sub(f"@{i}(?![0-9])", variable, recovered_formula)
     return recovered_formula
 
 def get_nuis_beta_terms(nuis_name:str, components):
     nuis_term = None
```

### Comparing `quickstats-0.6.8.4/quickstats/utils/roostats_utils.py` & `quickstats-0.6.8.6/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/utils/root_utils.py` & `quickstats-0.6.8.6/quickstats/utils/root_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/utils/string_utils.py` & `quickstats-0.6.8.6/quickstats/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats/utils/xml_tools.py` & `quickstats-0.6.8.6/quickstats/utils/xml_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/quickstats.egg-info/PKG-INFO` & `quickstats-0.6.8.6/quickstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.8.4
+Version: 0.6.8.6
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.8.4/quickstats.egg-info/SOURCES.txt` & `quickstats-0.6.8.6/quickstats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.4/setup.py` & `quickstats-0.6.8.6/setup.py`

 * *Files identical despite different names*

