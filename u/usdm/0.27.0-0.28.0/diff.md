# Comparing `tmp/usdm-0.27.0.tar.gz` & `tmp/usdm-0.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usdm-0.27.0.tar", last modified: Wed May 17 10:33:50 2023, max compression
+gzip compressed data, was "usdm-0.28.0.tar", last modified: Mon Jun 12 10:42:48 2023, max compression
```

## Comparing `usdm-0.27.0.tar` & `usdm-0.28.0.tar`

### file list

```diff
@@ -1,141 +1,144 @@
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.722452 usdm-0.27.0/
--rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.27.0/LICENSE
--rw-r--r--   0 daveih     (501) staff       (20)    21536 2023-05-17 10:33:50.722225 usdm-0.27.0/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)    21086 2023-05-16 13:32:48.000000 usdm-0.27.0/README.md
--rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.27.0/pyproject.toml
--rw-r--r--   0 daveih     (501) staff       (20)       38 2023-05-17 10:33:50.722509 usdm-0.27.0/setup.cfg
--rw-r--r--   0 daveih     (501) staff       (20)      932 2023-04-12 12:31:13.000000 usdm-0.27.0/setup.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.638826 usdm-0.27.0/src/
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.653855 usdm-0.27.0/src/usdm.egg-info/
--rw-r--r--   0 daveih     (501) staff       (20)    21536 2023-05-17 10:33:50.000000 usdm-0.27.0/src/usdm.egg-info/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)     4507 2023-05-17 10:33:50.000000 usdm-0.27.0/src/usdm.egg-info/SOURCES.txt
--rw-r--r--   0 daveih     (501) staff       (20)        1 2023-05-17 10:33:50.000000 usdm-0.27.0/src/usdm.egg-info/dependency_links.txt
--rw-r--r--   0 daveih     (501) staff       (20)       45 2023-05-17 10:33:50.000000 usdm-0.27.0/src/usdm.egg-info/requires.txt
--rw-r--r--   0 daveih     (501) staff       (20)       32 2023-05-17 10:33:50.000000 usdm-0.27.0/src/usdm.egg-info/top_level.txt
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.668920 usdm-0.27.0/src/usdm_excel/
--rw-r--r--   0 daveih     (501) staff       (20)     1611 2023-05-17 09:09:09.000000 usdm-0.27.0/src/usdm_excel/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      269 2023-03-31 14:50:16.000000 usdm-0.27.0/src/usdm_excel/alias.py
--rw-r--r--   0 daveih     (501) staff       (20)    10630 2023-05-17 09:48:28.000000 usdm-0.27.0/src/usdm_excel/base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4667 2023-05-01 12:04:14.000000 usdm-0.27.0/src/usdm_excel/cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      787 2023-03-31 14:50:16.000000 usdm-0.27.0/src/usdm_excel/cdisc_ct.py
--rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 15:59:49.000000 usdm-0.27.0/src/usdm_excel/cdisc_ct_library.py
--rw-r--r--   0 daveih     (501) staff       (20)     1564 2023-05-08 13:47:22.000000 usdm-0.27.0/src/usdm_excel/configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/cross_ref.py
--rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/ct_version_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.670521 usdm-0.27.0/src/usdm_excel/data/
--rw-r--r--   0 daveih     (501) staff       (20)      963 2023-04-14 12:14:15.000000 usdm-0.27.0/src/usdm_excel/data/cdisc_ct_config.yaml
--rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/data/iso_3166.json
--rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 15:59:49.000000 usdm-0.27.0/src/usdm_excel/data/missing_ct.yaml
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.672238 usdm-0.27.0/src/usdm_excel/errors/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-06 07:20:00.000000 usdm-0.27.0/src/usdm_excel/errors/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      933 2023-05-17 09:15:41.000000 usdm-0.27.0/src/usdm_excel/errors/error.py
--rw-r--r--   0 daveih     (501) staff       (20)      732 2023-05-17 09:15:52.000000 usdm-0.27.0/src/usdm_excel/errors/errors.py
--rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/id_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)      744 2023-04-13 09:34:38.000000 usdm-0.27.0/src/usdm_excel/iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      111 2023-04-03 10:43:35.000000 usdm-0.27.0/src/usdm_excel/logger.py
--rw-r--r--   0 daveih     (501) staff       (20)      309 2023-03-31 14:50:16.000000 usdm-0.27.0/src/usdm_excel/ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)     5161 2023-05-15 06:05:22.000000 usdm-0.27.0/src/usdm_excel/nodes_and_edges.py
--rw-r--r--   0 daveih     (501) staff       (20)      824 2023-05-08 13:47:22.000000 usdm-0.27.0/src/usdm_excel/option_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.673239 usdm-0.27.0/src/usdm_excel/study_design_activity_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-05-03 10:02:41.000000 usdm-0.27.0/src/usdm_excel/study_design_activity_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1570 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.675122 usdm-0.27.0/src/usdm_excel/study_design_arm_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.27.0/src/usdm_excel/study_design_arm_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1617 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.678503 usdm-0.27.0/src/usdm_excel/study_design_element_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_element_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2003 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.680194 usdm-0.27.0/src/usdm_excel/study_design_encounter_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2503 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.684651 usdm-0.27.0/src/usdm_excel/study_design_epoch_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.27.0/src/usdm_excel/study_design_epoch_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1289 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.686650 usdm-0.27.0/src/usdm_excel/study_design_estimands_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2794 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.689357 usdm-0.27.0/src/usdm_excel/study_design_ii_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_ii_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1991 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.690943 usdm-0.27.0/src/usdm_excel/study_design_objective_endpoint_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2475 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.693078 usdm-0.27.0/src/usdm_excel/study_design_population_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_population_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1778 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.694041 usdm-0.27.0/src/usdm_excel/study_design_procedure_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1645 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.694646 usdm-0.27.0/src/usdm_excel/study_design_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     6218 2023-05-17 09:41:38.000000 usdm-0.27.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.695169 usdm-0.27.0/src/usdm_excel/study_identifiers_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_identifiers_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3435 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.695942 usdm-0.27.0/src/usdm_excel/study_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     7892 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_sheet/study_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.701901 usdm-0.27.0/src/usdm_excel/study_soa_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-03 10:43:35.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/activities.py
--rw-r--r--   0 daveih     (501) staff       (20)     3498 2023-05-09 06:07:57.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 14:06:46.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/cycle.py
--rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 14:06:46.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/cycles.py
--rw-r--r--   0 daveih     (501) staff       (20)     1056 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/encounters.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
--rw-r--r--   0 daveih     (501) staff       (20)     4645 2023-04-13 09:55:50.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     5048 2023-04-13 04:26:45.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/timepoint.py
--rw-r--r--   0 daveih     (501) staff       (20)     2748 2023-04-13 04:26:45.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/timepoints.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.702326 usdm-0.27.0/src/usdm_info/
--rw-r--r--   0 daveih     (501) staff       (20)       59 2023-05-16 13:26:16.000000 usdm-0.27.0/src/usdm_info/__init__.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.715353 usdm-0.27.0/src/usdm_model/
--rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      545 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/address.py
--rw-r--r--   0 daveih     (501) staff       (20)      229 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/aliasCode.py
--rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/alias_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/analysis_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      844 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/api_base_model.py
--rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      315 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/biomedical_concept_category.py
--rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/biomedical_concept_property.py
--rw-r--r--   0 daveih     (501) staff       (20)      216 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/biomedical_concept_surrogate.py
--rw-r--r--   0 daveih     (501) staff       (20)      152 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/code.py
--rw-r--r--   0 daveih     (501) staff       (20)      642 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/encounter.py
--rw-r--r--   0 daveih     (501) staff       (20)      262 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/endpoint.py
--rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/estimand.py
--rw-r--r--   0 daveih     (501) staff       (20)      224 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/indication.py
--rw-r--r--   0 daveih     (501) staff       (20)      206 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/intercurrent_event.py
--rw-r--r--   0 daveih     (501) staff       (20)      260 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/investigational_intervention.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/objective.py
--rw-r--r--   0 daveih     (501) staff       (20)      347 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/organisation.py
--rw-r--r--   0 daveih     (501) staff       (20)      274 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/procedure.py
--rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/response_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      509 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/schedule_timeline.py
--rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/schedule_timeline_exit.py
--rw-r--r--   0 daveih     (501) staff       (20)      691 2023-04-13 04:26:45.000000 usdm-0.27.0/src/usdm_model/scheduled_instance.py
--rw-r--r--   0 daveih     (501) staff       (20)      677 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study.py
--rw-r--r--   0 daveih     (501) staff       (20)      296 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/study_arm.py
--rw-r--r--   0 daveih     (501) staff       (20)      380 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study_cell.py
--rw-r--r--   0 daveih     (501) staff       (20)     1583 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/study_design.py
--rw-r--r--   0 daveih     (501) staff       (20)      351 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study_design_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      359 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study_element.py
--rw-r--r--   0 daveih     (501) staff       (20)      401 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study_epoch.py
--rw-r--r--   0 daveih     (501) staff       (20)      583 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study_identifier.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study_protocol_version.py
--rw-r--r--   0 daveih     (501) staff       (20)      336 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/timing.py
--rw-r--r--   0 daveih     (501) staff       (20)      134 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/transition_rule.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.721753 usdm-0.27.0/tests/
--rw-r--r--   0 daveih     (501) staff       (20)    14241 2023-05-16 13:26:16.000000 usdm-0.27.0/tests/test_base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 14:43:30.000000 usdm-0.27.0/tests/test_cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)     1517 2023-05-08 13:47:22.000000 usdm-0.27.0/tests/test_configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      880 2023-05-17 09:18:36.000000 usdm-0.27.0/tests/test_error.py
--rw-r--r--   0 daveih     (501) staff       (20)     2234 2023-05-17 09:18:13.000000 usdm-0.27.0/tests/test_errors.py
--rw-r--r--   0 daveih     (501) staff       (20)      811 2023-05-16 13:26:16.000000 usdm-0.27.0/tests/test_integration.py
--rw-r--r--   0 daveih     (501) staff       (20)      971 2023-04-13 09:35:41.000000 usdm-0.27.0/tests/test_iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-05 14:06:46.000000 usdm-0.27.0/tests/test_ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)     1098 2023-05-08 13:47:22.000000 usdm-0.27.0/tests/test_option_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)     3199 2023-05-08 14:51:48.000000 usdm-0.27.0/tests/test_study_design_activity_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     3320 2023-04-14 12:14:15.000000 usdm-0.27.0/tests/test_study_design_arm_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     2716 2023-04-14 12:14:15.000000 usdm-0.27.0/tests/test_study_design_epoch_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4884 2023-05-16 13:26:16.000000 usdm-0.27.0/tests/test_study_identifiers_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.162775 usdm-0.28.0/
+-rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.28.0/LICENSE
+-rw-r--r--   0 daveih     (501) staff       (20)    22277 2023-06-12 10:42:48.156309 usdm-0.28.0/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)    21827 2023-06-12 10:01:21.000000 usdm-0.28.0/README.md
+-rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.28.0/pyproject.toml
+-rw-r--r--   0 daveih     (501) staff       (20)       38 2023-06-12 10:42:48.162956 usdm-0.28.0/setup.cfg
+-rw-r--r--   0 daveih     (501) staff       (20)      932 2023-04-12 12:31:13.000000 usdm-0.28.0/setup.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.012282 usdm-0.28.0/src/
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.016347 usdm-0.28.0/src/usdm.egg-info/
+-rw-r--r--   0 daveih     (501) staff       (20)    22277 2023-06-12 10:42:47.000000 usdm-0.28.0/src/usdm.egg-info/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)     4627 2023-06-12 10:42:48.000000 usdm-0.28.0/src/usdm.egg-info/SOURCES.txt
+-rw-r--r--   0 daveih     (501) staff       (20)        1 2023-06-12 10:42:47.000000 usdm-0.28.0/src/usdm.egg-info/dependency_links.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       45 2023-06-12 10:42:47.000000 usdm-0.28.0/src/usdm.egg-info/requires.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       32 2023-06-12 10:42:47.000000 usdm-0.28.0/src/usdm.egg-info/top_level.txt
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.057627 usdm-0.28.0/src/usdm_excel/
+-rw-r--r--   0 daveih     (501) staff       (20)     1611 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      269 2023-03-31 14:50:16.000000 usdm-0.28.0/src/usdm_excel/alias.py
+-rw-r--r--   0 daveih     (501) staff       (20)    10753 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4667 2023-05-01 12:04:14.000000 usdm-0.28.0/src/usdm_excel/cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      787 2023-03-31 14:50:16.000000 usdm-0.28.0/src/usdm_excel/cdisc_ct.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 15:59:49.000000 usdm-0.28.0/src/usdm_excel/cdisc_ct_library.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1564 2023-05-08 13:47:22.000000 usdm-0.28.0/src/usdm_excel/configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/cross_ref.py
+-rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/ct_version_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.068119 usdm-0.28.0/src/usdm_excel/data/
+-rw-r--r--   0 daveih     (501) staff       (20)      963 2023-04-14 12:14:15.000000 usdm-0.28.0/src/usdm_excel/data/cdisc_ct_config.yaml
+-rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/data/iso_3166.json
+-rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 15:59:49.000000 usdm-0.28.0/src/usdm_excel/data/missing_ct.yaml
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.070098 usdm-0.28.0/src/usdm_excel/errors/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-06 07:20:00.000000 usdm-0.28.0/src/usdm_excel/errors/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      933 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/errors/error.py
+-rw-r--r--   0 daveih     (501) staff       (20)      732 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/errors/errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/id_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)      744 2023-04-13 09:34:38.000000 usdm-0.28.0/src/usdm_excel/iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      883 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/iso_8601_duration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      111 2023-04-03 10:43:35.000000 usdm-0.28.0/src/usdm_excel/logger.py
+-rw-r--r--   0 daveih     (501) staff       (20)      309 2023-03-31 14:50:16.000000 usdm-0.28.0/src/usdm_excel/ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5641 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/nodes_and_edges.py
+-rw-r--r--   0 daveih     (501) staff       (20)      824 2023-05-08 13:47:22.000000 usdm-0.28.0/src/usdm_excel/option_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.071927 usdm-0.28.0/src/usdm_excel/study_design_activity_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-05-03 10:02:41.000000 usdm-0.28.0/src/usdm_excel/study_design_activity_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1570 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.073883 usdm-0.28.0/src/usdm_excel/study_design_arm_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.28.0/src/usdm_excel/study_design_arm_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1617 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.075313 usdm-0.28.0/src/usdm_excel/study_design_element_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_element_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2003 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.076968 usdm-0.28.0/src/usdm_excel/study_design_encounter_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2503 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.078554 usdm-0.28.0/src/usdm_excel/study_design_epoch_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.28.0/src/usdm_excel/study_design_epoch_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1289 2023-06-09 09:44:08.000000 usdm-0.28.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.079826 usdm-0.28.0/src/usdm_excel/study_design_estimands_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2794 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.080944 usdm-0.28.0/src/usdm_excel/study_design_ii_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_ii_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1991 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.083977 usdm-0.28.0/src/usdm_excel/study_design_objective_endpoint_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2475 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.085282 usdm-0.28.0/src/usdm_excel/study_design_population_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_population_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1778 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.086213 usdm-0.28.0/src/usdm_excel/study_design_procedure_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1645 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.087235 usdm-0.28.0/src/usdm_excel/study_design_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     6844 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.088829 usdm-0.28.0/src/usdm_excel/study_identifiers_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_identifiers_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3435 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.091987 usdm-0.28.0/src/usdm_excel/study_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     7910 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/study_sheet/study_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.104242 usdm-0.28.0/src/usdm_excel/study_soa_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-03 10:43:35.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/activities.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3498 2023-05-09 06:07:57.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 14:06:46.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/cycle.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 14:06:46.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/cycles.py
+-rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4620 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5070 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/timepoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2550 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/timepoint_type.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2748 2023-04-13 04:26:45.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/timepoints.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2008 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/window_type.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.104590 usdm-0.28.0/src/usdm_info/
+-rw-r--r--   0 daveih     (501) staff       (20)       59 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_info/__init__.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.143778 usdm-0.28.0/src/usdm_model/
+-rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      586 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 13:59:38.000000 usdm-0.28.0/src/usdm_model/address.py
+-rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/alias_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/analysis_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      844 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/api_base_model.py
+-rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      383 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/biomedical_concept_category.py
+-rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/biomedical_concept_property.py
+-rw-r--r--   0 daveih     (501) staff       (20)      243 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/biomedical_concept_surrogate.py
+-rw-r--r--   0 daveih     (501) staff       (20)      151 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      661 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/encounter.py
+-rw-r--r--   0 daveih     (501) staff       (20)      240 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/endpoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/estimand.py
+-rw-r--r--   0 daveih     (501) staff       (20)      195 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/indication.py
+-rw-r--r--   0 daveih     (501) staff       (20)      251 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/intercurrent_event.py
+-rw-r--r--   0 daveih     (501) staff       (20)      238 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/investigational_intervention.py
+-rw-r--r--   0 daveih     (501) staff       (20)      289 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/objective.py
+-rw-r--r--   0 daveih     (501) staff       (20)      346 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/organisation.py
+-rw-r--r--   0 daveih     (501) staff       (20)      339 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/procedure.py
+-rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/response_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      551 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/schedule_timeline.py
+-rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/schedule_timeline_exit.py
+-rw-r--r--   0 daveih     (501) staff       (20)      729 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/scheduled_instance.py
+-rw-r--r--   0 daveih     (501) staff       (20)      676 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study.py
+-rw-r--r--   0 daveih     (501) staff       (20)      294 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_arm.py
+-rw-r--r--   0 daveih     (501) staff       (20)      188 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_cell.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1820 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_design.py
+-rw-r--r--   0 daveih     (501) staff       (20)      398 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_design_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      356 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_element.py
+-rw-r--r--   0 daveih     (501) staff       (20)      328 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_epoch.py
+-rw-r--r--   0 daveih     (501) staff       (20)      250 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_identifier.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/study_protocol_version.py
+-rw-r--r--   0 daveih     (501) staff       (20)      492 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/timing.py
+-rw-r--r--   0 daveih     (501) staff       (20)      135 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/transition_rule.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.155436 usdm-0.28.0/tests/
+-rw-r--r--   0 daveih     (501) staff       (20)    14241 2023-05-16 13:26:16.000000 usdm-0.28.0/tests/test_base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 14:43:30.000000 usdm-0.28.0/tests/test_cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1517 2023-05-08 13:47:22.000000 usdm-0.28.0/tests/test_configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      880 2023-05-17 10:35:35.000000 usdm-0.28.0/tests/test_error.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2234 2023-05-17 10:35:35.000000 usdm-0.28.0/tests/test_errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2466 2023-06-12 09:18:24.000000 usdm-0.28.0/tests/test_integration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      971 2023-04-13 09:35:41.000000 usdm-0.28.0/tests/test_iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1763 2023-06-12 09:18:24.000000 usdm-0.28.0/tests/test_iso_8601_duration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-05 14:06:46.000000 usdm-0.28.0/tests/test_ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1098 2023-05-08 13:47:22.000000 usdm-0.28.0/tests/test_option_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3199 2023-05-08 14:51:48.000000 usdm-0.28.0/tests/test_study_design_activity_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3320 2023-04-14 12:14:15.000000 usdm-0.28.0/tests/test_study_design_arm_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2716 2023-04-14 12:14:15.000000 usdm-0.28.0/tests/test_study_design_epoch_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4884 2023-05-16 13:26:16.000000 usdm-0.28.0/tests/test_study_identifiers_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4167 2023-06-12 09:18:24.000000 usdm-0.28.0/tests/test_study_soa_sheet.py
```

### Comparing `usdm-0.27.0/LICENSE` & `usdm-0.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/PKG-INFO` & `usdm-0.28.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.27.0
+Version: 0.28.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -71,15 +71,15 @@
 - Study Design Objectives and Endpoints sheet
 - Study Design Estimands sheet
 - Study Design Procedures sheet
 - Study Design Encounters sheet
 - Study Design Elements sheet
 - Configuration sheet
 
-The content of each sheet is described below. Example workbooks can be found in the [CDISC Reference Architecture repo](https://github.com/cdisc-org/DDF-RA/tree/sprint-11/Deliverables/IG/examples). *Note: the link above points to the sprint 11 branch. This will be merged into the main branch prior to public review.*
+The content of each sheet is described below. Example workbooks can be found in the [CDISC Reference Architecture repo](https://github.com/cdisc-org/DDF-RA/tree/main/Deliverables/IG/examples).
 
 ### CDISC Terminology
 
 For those cells where CDISC codes are used the user can enter either the CDISC C Code, for example `C15602`, the CDISC submission value, for example `PHASE III TRIAL`, or the preferred term, for example `Phase III Trial`
 
 ### Multiple Values
 
@@ -95,14 +95,29 @@
 
 ### Identifiers and Cross References
 
 Some content defined within the sheets contain unique identifiers such that the content can be cross referenced in other sheets. This is done so as to link content or expand definitions. Identifiers are simple strings that need to be unique within the workbook. There is a single definition and one or more cross references.
 
 See the [infographic](https://github.com/data4knowledge/usdm/blob/main/docs/sheets.png) for further information.
 
+### Timing Values
+
+A number of fields specify timing values, either single relative values or ranges. These can be entered as
+a *Timing Value* of ```<value> <unit>``` or a *Timing Range* of ```<lower>..<upper> <unit>```. The unit can be entered as follows:
+
+- Years: 'Y', 'YRS', 'YR', 'YEARS', 'YEAR'
+- Months: 'MTHS', 'MTH', 'MONTHS', 'MONTH'
+- Weeks: 'W', 'WKS', 'WK', 'WEEKS', 'WEEK'
+- Days: 'D', 'DYS', 'DY', 'DAYS', 'DAY'
+- Hours: 'H', 'HRS', 'HR', 'HOURS', 'HOUR'
+- Minutes: 'M', 'MINS', 'MIN', 'MINUTES', 'MINUTE'
+- Seconds: 'S', 'SECS', 'SEC', 'SECONDS', 'SECOND'
+
+So ```3 Y```, ```3 YRS```, ```3 YR```, ```3 YEARS```, ```3 YEAR``` are all equivalent. Only a single value and unit should be entered, i.e. combination values are not supported.
+
 ### Study Sheet
 
 #### Sheet Name
 
 `study`
 
 #### Sheet Contents
@@ -255,29 +270,29 @@
 | Row | Row Name | Description | Format and Values |
 | :--- | :--- | :--- | :--- |
 | 1 | Epoch | The name of the epoch within which the timepoint falls. Note the cells in this row can be merged to link an epoch with many timepoints | Text string  |
 | 2 | Cycle | The cycle in which the "timepoint" exists. Can be empty or set to '-' (empty) | Text string |
 | 3 | First Cycle Start | The time at which the cycle starts. Should be specified. Empty if not part of a cycle | Text string |
 | 4 | Cycle Period | The cycle period. Shoudl be specified. Empty if not part of a cycle | Text string |
 | 5 | Cycle End Rule | The cycle end rule. Can be empty. Empty if not part of a cycle | Text string |
-| 6 | Timing | "Timepoint" timing.  | Text String |
-| 7 | Encounter xref | Cross reference tot he encounter in which the timepoint belongs. Can be empty | Text string |
-| 8 | Window | Timing window. Can be empty | Text string |
+| 6 | Timing | "Timepoint" timing.  | A timing string, see below |
+| 7 | Encounter xref | Cross reference to the encounter in which the timepoint belongs. Can be empty | Text string |
+| 8 | Window | Timing window. Can be empty | A *Timing Range* |
 
 The timepont timing takes the form defined as follows (using pseudo BNF). 
 
 ```
 <entry> ::= <type> [<count>] : [<relative timing>]
 <type> ::= N | P| A | C
 <count> ::= any positive integer (will default to 1)
-<relative timing> ::= string
+<relative timing> ::= A single Timing Value
 ```
 N = Next, P = Previous, A = Anchor and C = Cycle Start. The count when used with N or P indicates a relative to the Nth next or previous timepoint. When not specificed it defaults to 1.
 
-`P2: +14 Days` indicates the timepoiint is relative to the 2nd previous timepoint by 14 days.
+`P2: +14 Days` indicates the timepoiint is relative to the 2nd previous timepoint by 14 days. A plus or minus sign can be entered but will be ignored as times are absolute.
 `N1: 1 Day` is equivalent to `N: 1 Day` and indicates the timepoiint is relative to the next timepoint by 1 day.
 `A:` is an anchor
 
 ##### Activity
 
 The activity section consists of three columns, A to C, starting in row 10, row 9 being a title row. As many rows as needed can be added.
```

### Comparing `usdm-0.27.0/README.md` & `usdm-0.28.0/src/usdm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: usdm
+Version: 0.28.0
+Summary: A python package for using the CDISC TransCelerate USDM
+Author: D Iberson-Hurst
+Author-email: 
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CDISC / Transcelerate DDF USDM Package
 
 This package provides an implementation of the Digital Data Flow (DDF) CDISC / TransCelerate Unified Study Definitions Model (USDM). Two main parts are provided:
 
 - Within the `usdm_model` directory are a set of classes reflecting the USDM model as transported using the DDF USDM API 
 - Within the `usdm_excel` directory is a class, `USDMExcel`, that can be used to import an entire study definition from an excel file and build the equivalent json as defined by the API
 
@@ -57,15 +71,15 @@
 - Study Design Objectives and Endpoints sheet
 - Study Design Estimands sheet
 - Study Design Procedures sheet
 - Study Design Encounters sheet
 - Study Design Elements sheet
 - Configuration sheet
 
-The content of each sheet is described below. Example workbooks can be found in the [CDISC Reference Architecture repo](https://github.com/cdisc-org/DDF-RA/tree/sprint-11/Deliverables/IG/examples). *Note: the link above points to the sprint 11 branch. This will be merged into the main branch prior to public review.*
+The content of each sheet is described below. Example workbooks can be found in the [CDISC Reference Architecture repo](https://github.com/cdisc-org/DDF-RA/tree/main/Deliverables/IG/examples).
 
 ### CDISC Terminology
 
 For those cells where CDISC codes are used the user can enter either the CDISC C Code, for example `C15602`, the CDISC submission value, for example `PHASE III TRIAL`, or the preferred term, for example `Phase III Trial`
 
 ### Multiple Values
 
@@ -81,14 +95,29 @@
 
 ### Identifiers and Cross References
 
 Some content defined within the sheets contain unique identifiers such that the content can be cross referenced in other sheets. This is done so as to link content or expand definitions. Identifiers are simple strings that need to be unique within the workbook. There is a single definition and one or more cross references.
 
 See the [infographic](https://github.com/data4knowledge/usdm/blob/main/docs/sheets.png) for further information.
 
+### Timing Values
+
+A number of fields specify timing values, either single relative values or ranges. These can be entered as
+a *Timing Value* of ```<value> <unit>``` or a *Timing Range* of ```<lower>..<upper> <unit>```. The unit can be entered as follows:
+
+- Years: 'Y', 'YRS', 'YR', 'YEARS', 'YEAR'
+- Months: 'MTHS', 'MTH', 'MONTHS', 'MONTH'
+- Weeks: 'W', 'WKS', 'WK', 'WEEKS', 'WEEK'
+- Days: 'D', 'DYS', 'DY', 'DAYS', 'DAY'
+- Hours: 'H', 'HRS', 'HR', 'HOURS', 'HOUR'
+- Minutes: 'M', 'MINS', 'MIN', 'MINUTES', 'MINUTE'
+- Seconds: 'S', 'SECS', 'SEC', 'SECONDS', 'SECOND'
+
+So ```3 Y```, ```3 YRS```, ```3 YR```, ```3 YEARS```, ```3 YEAR``` are all equivalent. Only a single value and unit should be entered, i.e. combination values are not supported.
+
 ### Study Sheet
 
 #### Sheet Name
 
 `study`
 
 #### Sheet Contents
@@ -241,29 +270,29 @@
 | Row | Row Name | Description | Format and Values |
 | :--- | :--- | :--- | :--- |
 | 1 | Epoch | The name of the epoch within which the timepoint falls. Note the cells in this row can be merged to link an epoch with many timepoints | Text string  |
 | 2 | Cycle | The cycle in which the "timepoint" exists. Can be empty or set to '-' (empty) | Text string |
 | 3 | First Cycle Start | The time at which the cycle starts. Should be specified. Empty if not part of a cycle | Text string |
 | 4 | Cycle Period | The cycle period. Shoudl be specified. Empty if not part of a cycle | Text string |
 | 5 | Cycle End Rule | The cycle end rule. Can be empty. Empty if not part of a cycle | Text string |
-| 6 | Timing | "Timepoint" timing.  | Text String |
-| 7 | Encounter xref | Cross reference tot he encounter in which the timepoint belongs. Can be empty | Text string |
-| 8 | Window | Timing window. Can be empty | Text string |
+| 6 | Timing | "Timepoint" timing.  | A timing string, see below |
+| 7 | Encounter xref | Cross reference to the encounter in which the timepoint belongs. Can be empty | Text string |
+| 8 | Window | Timing window. Can be empty | A *Timing Range* |
 
 The timepont timing takes the form defined as follows (using pseudo BNF). 
 
 ```
 <entry> ::= <type> [<count>] : [<relative timing>]
 <type> ::= N | P| A | C
 <count> ::= any positive integer (will default to 1)
-<relative timing> ::= string
+<relative timing> ::= A single Timing Value
 ```
 N = Next, P = Previous, A = Anchor and C = Cycle Start. The count when used with N or P indicates a relative to the Nth next or previous timepoint. When not specificed it defaults to 1.
 
-`P2: +14 Days` indicates the timepoiint is relative to the 2nd previous timepoint by 14 days.
+`P2: +14 Days` indicates the timepoiint is relative to the 2nd previous timepoint by 14 days. A plus or minus sign can be entered but will be ignored as times are absolute.
 `N1: 1 Day` is equivalent to `N: 1 Day` and indicates the timepoiint is relative to the next timepoint by 1 day.
 `A:` is an anchor
 
 ##### Activity
 
 The activity section consists of three columns, A to C, starting in row 10, row 9 being a title row. As many rows as needed can be added.
 
@@ -465,8 +494,8 @@
 
 See the [github issues](https://github.com/data4knowledge/usdm/issues)
 
 # Build Notes
 
 Build with `python3 -m build --sdist --wheel`
 
-Upload to pypi using `twine upload dist/* `
+Upload to pypi using `twine upload dist/* `
```

### Comparing `usdm-0.27.0/setup.py` & `usdm-0.28.0/setup.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm.egg-info/PKG-INFO` & `usdm-0.28.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: usdm
-Version: 0.27.0
-Summary: A python package for using the CDISC TransCelerate USDM
-Author: D Iberson-Hurst
-Author-email: 
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CDISC / Transcelerate DDF USDM Package
 
 This package provides an implementation of the Digital Data Flow (DDF) CDISC / TransCelerate Unified Study Definitions Model (USDM). Two main parts are provided:
 
 - Within the `usdm_model` directory are a set of classes reflecting the USDM model as transported using the DDF USDM API 
 - Within the `usdm_excel` directory is a class, `USDMExcel`, that can be used to import an entire study definition from an excel file and build the equivalent json as defined by the API
 
@@ -71,15 +57,15 @@
 - Study Design Objectives and Endpoints sheet
 - Study Design Estimands sheet
 - Study Design Procedures sheet
 - Study Design Encounters sheet
 - Study Design Elements sheet
 - Configuration sheet
 
-The content of each sheet is described below. Example workbooks can be found in the [CDISC Reference Architecture repo](https://github.com/cdisc-org/DDF-RA/tree/sprint-11/Deliverables/IG/examples). *Note: the link above points to the sprint 11 branch. This will be merged into the main branch prior to public review.*
+The content of each sheet is described below. Example workbooks can be found in the [CDISC Reference Architecture repo](https://github.com/cdisc-org/DDF-RA/tree/main/Deliverables/IG/examples).
 
 ### CDISC Terminology
 
 For those cells where CDISC codes are used the user can enter either the CDISC C Code, for example `C15602`, the CDISC submission value, for example `PHASE III TRIAL`, or the preferred term, for example `Phase III Trial`
 
 ### Multiple Values
 
@@ -95,14 +81,29 @@
 
 ### Identifiers and Cross References
 
 Some content defined within the sheets contain unique identifiers such that the content can be cross referenced in other sheets. This is done so as to link content or expand definitions. Identifiers are simple strings that need to be unique within the workbook. There is a single definition and one or more cross references.
 
 See the [infographic](https://github.com/data4knowledge/usdm/blob/main/docs/sheets.png) for further information.
 
+### Timing Values
+
+A number of fields specify timing values, either single relative values or ranges. These can be entered as
+a *Timing Value* of ```<value> <unit>``` or a *Timing Range* of ```<lower>..<upper> <unit>```. The unit can be entered as follows:
+
+- Years: 'Y', 'YRS', 'YR', 'YEARS', 'YEAR'
+- Months: 'MTHS', 'MTH', 'MONTHS', 'MONTH'
+- Weeks: 'W', 'WKS', 'WK', 'WEEKS', 'WEEK'
+- Days: 'D', 'DYS', 'DY', 'DAYS', 'DAY'
+- Hours: 'H', 'HRS', 'HR', 'HOURS', 'HOUR'
+- Minutes: 'M', 'MINS', 'MIN', 'MINUTES', 'MINUTE'
+- Seconds: 'S', 'SECS', 'SEC', 'SECONDS', 'SECOND'
+
+So ```3 Y```, ```3 YRS```, ```3 YR```, ```3 YEARS```, ```3 YEAR``` are all equivalent. Only a single value and unit should be entered, i.e. combination values are not supported.
+
 ### Study Sheet
 
 #### Sheet Name
 
 `study`
 
 #### Sheet Contents
@@ -255,29 +256,29 @@
 | Row | Row Name | Description | Format and Values |
 | :--- | :--- | :--- | :--- |
 | 1 | Epoch | The name of the epoch within which the timepoint falls. Note the cells in this row can be merged to link an epoch with many timepoints | Text string  |
 | 2 | Cycle | The cycle in which the "timepoint" exists. Can be empty or set to '-' (empty) | Text string |
 | 3 | First Cycle Start | The time at which the cycle starts. Should be specified. Empty if not part of a cycle | Text string |
 | 4 | Cycle Period | The cycle period. Shoudl be specified. Empty if not part of a cycle | Text string |
 | 5 | Cycle End Rule | The cycle end rule. Can be empty. Empty if not part of a cycle | Text string |
-| 6 | Timing | "Timepoint" timing.  | Text String |
-| 7 | Encounter xref | Cross reference tot he encounter in which the timepoint belongs. Can be empty | Text string |
-| 8 | Window | Timing window. Can be empty | Text string |
+| 6 | Timing | "Timepoint" timing.  | A timing string, see below |
+| 7 | Encounter xref | Cross reference to the encounter in which the timepoint belongs. Can be empty | Text string |
+| 8 | Window | Timing window. Can be empty | A *Timing Range* |
 
 The timepont timing takes the form defined as follows (using pseudo BNF). 
 
 ```
 <entry> ::= <type> [<count>] : [<relative timing>]
 <type> ::= N | P| A | C
 <count> ::= any positive integer (will default to 1)
-<relative timing> ::= string
+<relative timing> ::= A single Timing Value
 ```
 N = Next, P = Previous, A = Anchor and C = Cycle Start. The count when used with N or P indicates a relative to the Nth next or previous timepoint. When not specificed it defaults to 1.
 
-`P2: +14 Days` indicates the timepoiint is relative to the 2nd previous timepoint by 14 days.
+`P2: +14 Days` indicates the timepoiint is relative to the 2nd previous timepoint by 14 days. A plus or minus sign can be entered but will be ignored as times are absolute.
 `N1: 1 Day` is equivalent to `N: 1 Day` and indicates the timepoiint is relative to the next timepoint by 1 day.
 `A:` is an anchor
 
 ##### Activity
 
 The activity section consists of three columns, A to C, starting in row 10, row 9 being a title row. As many rows as needed can be added.
 
@@ -479,8 +480,8 @@
 
 See the [github issues](https://github.com/data4knowledge/usdm/issues)
 
 # Build Notes
 
 Build with `python3 -m build --sdist --wheel`
 
-Upload to pypi using `twine upload dist/* `
+Upload to pypi using `twine upload dist/* `
```

### Comparing `usdm-0.27.0/src/usdm.egg-info/SOURCES.txt` & `usdm-0.28.0/src/usdm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/usdm_excel/cdisc_ct.py
 src/usdm_excel/cdisc_ct_library.py
 src/usdm_excel/configuration_sheet.py
 src/usdm_excel/cross_ref.py
 src/usdm_excel/ct_version_manager.py
 src/usdm_excel/id_manager.py
 src/usdm_excel/iso_3166.py
+src/usdm_excel/iso_8601_duration.py
 src/usdm_excel/logger.py
 src/usdm_excel/ncit.py
 src/usdm_excel/nodes_and_edges.py
 src/usdm_excel/option_manager.py
 src/usdm_excel/data/cdisc_ct_config.yaml
 src/usdm_excel/data/iso_3166.json
 src/usdm_excel/data/missing_ct.yaml
@@ -55,24 +56,24 @@
 src/usdm_excel/study_sheet/__init__.py
 src/usdm_excel/study_sheet/study_sheet.py
 src/usdm_excel/study_soa_sheet/__init__.py
 src/usdm_excel/study_soa_sheet/activities.py
 src/usdm_excel/study_soa_sheet/activity.py
 src/usdm_excel/study_soa_sheet/cycle.py
 src/usdm_excel/study_soa_sheet/cycles.py
-src/usdm_excel/study_soa_sheet/encounters.py
 src/usdm_excel/study_soa_sheet/soa_column_rows.py
 src/usdm_excel/study_soa_sheet/study_soa_sheet.py
 src/usdm_excel/study_soa_sheet/timepoint.py
+src/usdm_excel/study_soa_sheet/timepoint_type.py
 src/usdm_excel/study_soa_sheet/timepoints.py
+src/usdm_excel/study_soa_sheet/window_type.py
 src/usdm_info/__init__.py
 src/usdm_model/__init__.py
 src/usdm_model/activity.py
 src/usdm_model/address.py
-src/usdm_model/aliasCode.py
 src/usdm_model/alias_code.py
 src/usdm_model/analysis_population.py
 src/usdm_model/api_base_model.py
 src/usdm_model/biomedical_concept.py
 src/usdm_model/biomedical_concept_category.py
 src/usdm_model/biomedical_concept_property.py
 src/usdm_model/biomedical_concept_surrogate.py
@@ -104,13 +105,15 @@
 tests/test_base_sheet.py
 tests/test_cdisc_biomedical_concept.py
 tests/test_configuration_sheet.py
 tests/test_error.py
 tests/test_errors.py
 tests/test_integration.py
 tests/test_iso_3166.py
+tests/test_iso_8601_duration.py
 tests/test_ncit.py
 tests/test_option_manager.py
 tests/test_study_design_activity_sheet.py
 tests/test_study_design_arm_sheet.py
 tests/test_study_design_epoch_sheet.py
-tests/test_study_identifiers_sheet.py
+tests/test_study_identifiers_sheet.py
+tests/test_study_soa_sheet.py
```

### Comparing `usdm-0.27.0/src/usdm_excel/__init__.py` & `usdm-0.28.0/src/usdm_excel/__init__.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/base_sheet.py` & `usdm-0.28.0/src/usdm_excel/base_sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,17 @@
 
   def _general_error(self, message):
     error_manager.add(self.sheet_name, None, None, message)
 
   def _warning(self, row, column, message):
     error_manager.add(self.sheet_name, row + 1, column + 1, message, error_manager.WARNING)
 
+  def _general_warning(self, message):
+    error_manager.add(self.sheet_name, None, None, message, error_manager.WARNING)
+
   def _debug(self, row, column, message):
     error_manager.add(self.sheet_name, row + 1, column + 1, message, error_manager.DEBUG)
 
   def _traceback(self, message):
     package_logger.debug(message)
 
   def _format(self, row, column, message):
```

### Comparing `usdm-0.27.0/src/usdm_excel/cdisc_biomedical_concept.py` & `usdm-0.28.0/src/usdm_excel/cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/cdisc_ct.py` & `usdm-0.28.0/src/usdm_excel/cdisc_ct.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/cdisc_ct_library.py` & `usdm-0.28.0/src/usdm_excel/cdisc_ct_library.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/configuration_sheet.py` & `usdm-0.28.0/src/usdm_excel/configuration_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/data/cdisc_ct_config.yaml` & `usdm-0.28.0/src/usdm_excel/data/cdisc_ct_config.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/data/iso_3166.json` & `usdm-0.28.0/src/usdm_excel/data/iso_3166.json`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/data/missing_ct.yaml` & `usdm-0.28.0/src/usdm_excel/data/missing_ct.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/errors/error.py` & `usdm-0.28.0/src/usdm_excel/errors/error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/errors/errors.py` & `usdm-0.28.0/src/usdm_excel/errors/errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/id_manager.py` & `usdm-0.28.0/src/usdm_excel/id_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/iso_3166.py` & `usdm-0.28.0/src/usdm_excel/iso_3166.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/nodes_and_edges.py` & `usdm-0.28.0/src/usdm_excel/nodes_and_edges.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,53 +10,72 @@
     self.study = study
     self.nodes = []
     self.edges = []
     self.add_edges = []
     self.node_index = 1
     self.edge_index = 1
     self.id_node_index_map = {}
-    self.edge_attributes = [
-      'encounterIds',
-      'timepointActivityIds',
-      'timepointEncounterId',
-      'bcSurrogateIds',
-      'bcCategoryIds',
-      'biomedicalConceptIds',
-      'biomedicalConceptSurrogateId',
-      'relativeFromScheduledInstanceId',
-      'relativeToScheduledInstanceId',
-      'scheduledInstanceEncounterId',
-      'activityIds',
-      'scheduledDecisionInstanceId',
-      'treatment',
-      'variableOfInterest',
-      'conditionAssignments',
-      'activityTimelineId'
-    ]
+    self.edge_attributes = {
+      'ScheduledActivityInstance': [
+        'timepointActivityIds',
+        'scheduledActivityInstanceEncounterId',
+        'activityIds',
+        'epochId',
+        'defaultConditionId',
+      ],
+      'ScheduledDecisionInstance': [
+        'timepointActivityIds',
+        'epochId',
+        'defaultConditionId',
+        'conditionAssignments',
+      ],
+      'Activity': [
+        'bcSurrogateIds',
+        'bcCategoryIds',
+        'biomedicalConceptIds',
+      ],
+      'Timing': [
+        'relativeFromScheduledInstanceId',
+        'relativeToScheduledInstanceId',
+      ],
+      'Estimand': [
+        'treatment',
+        'variableOfInterest',
+      ],
+      'ScheduledTimeline': [
+        'activityTimelineId',
+      ],
+      'StudyCell': [
+        'studyArmId',
+        'studyEpochId',
+        'studyElementIds',
+      ]
+    }
     self.fix_id_name = {
       'scheduledActivityInstanceId': 'scheduledInstanceId',
       'scheduledDecisionInstanceId': 'scheduledInstanceId',
       'biomedicalConceptSurrogateId': 'bcSurrogateId',
       'biomedicalConceptPropertyId': 'bcPropertyId'
     }
     self.order_attributes = []
     self.ignore_klass = []
     self.collapse_klass = []
     if view == self.__class__.TIMELINE:
       self.ignore_klass = [
         'StudyProtocolVersion', 'StudyIdentifier', 'Indication', 
         'InvestigationalIntervention', 'Objective', 'StudyDesignPopulation', 
-        'Estimand', 'StudyCell', 'TransitionRule',
-        'BiomedicalConcept', 'BiomedicalConceptCategory', 'BiomedicalConceptSurrogate', 'Procedure', 'AliasCode'
+        'Estimand', 'StudyCell', 'TransitionRule', 'StudyArm', 'StudyEpoch', 'StudyElement',
+        'BiomedicalConcept', 'BiomedicalConceptCategory', 'BiomedicalConceptSurrogate', 
+        'Procedure', 'AliasCode'
       ]
       self.collapse_klass = ['Code']
-      self.order_attributes = [
-        'scheduleSequenceNumber'
-      ]
-    self.sequence_number_map = {}
+      #self.order_attributes = [
+      #  'scheduleSequenceNumber'
+      #]
+    #self.sequence_number_map = {}
       
   def nodes_and_edges(self):
     node = json.loads(self.study.to_json_with_type())
     self._process_node(node)
     for edge in self.add_edges:
       if edge['end'] in self.id_node_index_map:
         edge['id'] = self.edge_index
@@ -87,33 +106,34 @@
         return [self.id_node_index_map[node[id_field]]]
       this_node_index = self.node_index
       self.node_index += 1
       if klass in self.collapse_klass:
         return []
       for key, value in node.items():
         # Special case, get the ids for the sequence numbers but within scope of each timeline
-        if key == "scheduleTimelineInstances":
-          self.sequence_number_map = {}
-          for item in value:
-            self.sequence_number_map[item['scheduleSequenceNumber']] = item['scheduledInstanceId']
+        # if key == "scheduleTimelineInstances":
+        #   self.sequence_number_map = {}
+        #   for item in value:
+        #     self.sequence_number_map[item['scheduleSequenceNumber']] = item['scheduledInstanceId']
         # Link the sequence numbers
-        if key in self.order_attributes:
-          seq = value + 1
-          if seq in self.sequence_number_map:
-            self.add_edges.append( { 'start': this_node_index, 'end': self.sequence_number_map[seq], 'properties': { 'label': key, 'type': 'Order' }})
-        if key in self.edge_attributes:
+        # if key in self.order_attributes:
+        #   seq = value + 1
+        #   if seq in self.sequence_number_map:
+        #     self.add_edges.append( { 'start': this_node_index, 'end': self.sequence_number_map[seq], 'properties': { 'label': key, 'type': 'Order' }})
+        if klass in self.edge_attributes and key in self.edge_attributes[klass]:
           if key == "conditionAssignments":
             # Special case, array of arrays of condition and link id
             for item in value:
               self.add_edges.append( { 'start': this_node_index, 'end': item[1], 'properties': { 'label': key, 'type': 'Condition' }})
           elif type(value) == list:
             for item in value:
-              self.add_edges.append( { 'start': this_node_index, 'end': item, 'properties': { 'label': key, 'type': 'List' }})
+              if item:
+                self.add_edges.append( { 'start': this_node_index, 'end': item, 'properties': { 'label': key, 'type': 'List' }})
           else:
-            if not value == "":
+            if value:
               self.add_edges.append( { 'start': this_node_index, 'end': value, 'properties': { 'label': key, 'type': 'Other' }})
         else:
           indexes = self._process_node(value)
           if indexes == None:
             properties[key] = {}
           elif indexes == []:
             properties[key] = value
```

### Comparing `usdm-0.27.0/src/usdm_excel/option_manager.py` & `usdm-0.28.0/src/usdm_excel/option_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_design_sheet/study_design_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_design_sheet/study_design_sheet.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,29 +28,33 @@
 
   def __init__(self, file_path):
     try:
       super().__init__(file_path=file_path, sheet_name='studyDesign', header=None)
       self.name = "TEST"
       self.description = "An Microsoft Excel test study design"
       self.epochs = []
+      self.epoch_names = {}
       self.arms = []
+      self.arm_names = {}
       self.cells = []
+      self.elements = {}
       self.study_designs = []
       self.therapeutic_areas = []
       self.rationale = ""
       self.blinding = None
       self.trial_intents = []
       self.trial_types = []
       self.intervention_model = None
       self.main_timeline = None
       self.other_timelines = []
       self.process_sheet()
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
+      print(f"{traceback.format_exc()}")
 
   def process_sheet(self):
     for rindex, row in self.sheet.iterrows():
       if rindex == self.NAME_ROW:
         self.name = self.read_cell(rindex, self.PARAMS_DATA_COL)
       elif rindex == self.DESCRIPTION_ROW:
         self.description = self.read_cell(rindex, self.PARAMS_DATA_COL)
@@ -84,83 +88,94 @@
             if cindex != 0:
               resolved_epochs[epoch_index] = self._add_epoch(cell)
           else:
             arm_index = rindex - self.EPOCH_ARMS_START_ROW - 1
             if cindex == 0:
               resolved_arms[arm_index] = self._add_arm(cell)
             else:
-              elements = []
+              cell_elements = []
               element_names = self.read_cell_multiple(rindex, cindex)
               for name in element_names:
                 element = self._add_element(name)
                 if element is not None:
-                  elements.append(element)
-              arm = resolved_arms[arm_index]
-              epoch = resolved_epochs[epoch_index]
-              if arm is not None and epoch is not None:
-                self.cells.append(self._add_cell(arm=arm, epoch=epoch, elements=elements))
+                  cell_elements.append(element.studyElementId)
+              cell_arm = resolved_arms[arm_index].studyArmId
+              cell_epoch = resolved_epochs[epoch_index].studyEpochId
+              if cell_arm is not None and cell_epoch is not None:
+                self.cells.append(self._add_cell(arm=cell_arm, epoch=cell_epoch, elements=cell_elements))
               else:
-                self._general_error(f"Cannot resolve arms and/or epoch for cell [{arm_index + 1},{epoch_index + 1}]")
+                self._general_error(f"Cannot resolve arm and/or epoch for cell [{arm_index + 1},{epoch_index + 1}]")
               
-    
     self.double_link(self.epochs, 'studyEpochId', 'previousStudyEpochId', 'nextStudyEpochId')
 
     study_design = self._add_design(
       name=self.name,
       description=self.description,
-      cells=self.cells, 
+      cells=self.cells,
+      epochs=self.epochs,
+      arms=self.arms,
+      elements=list(self.elements.values()),
       intent_types=self.trial_intents, 
       trial_types=self.trial_types, 
       intervention_model=self.intervention_model,
       rationale=self.rationale, 
       blinding=self.blinding, 
       therapeutic_areas=self.therapeutic_areas
     )
     self.study_designs.append(study_design)
 
   def _add_arm(self, name):
     arm = cross_references.get(name)
     if arm is not None:
-      self.arms.append(arm)
+      if name not in self.arm_names:
+        self.arm_names[name] = True
+        self.arms.append(arm)
       return arm
     else:
       self._general_error(f"No arm definition found for arm '{name}'")
       return None
 
   def _add_epoch(self, name):
     epoch = cross_references.get(name)
     if epoch is not None:
-      self.epochs.append(epoch)
+      if name not in self.epoch_names:
+        self.epoch_names[name] = True
+        self.epochs.append(epoch)
       return epoch
     else:
       self._general_error(f"No epoch definition found for epoch '{name}'")
       return None
   
   def _add_element(self, name):
     element = cross_references.get(name)
     if element is not None:
+      if name not in self.elements:
+        self.elements[name] = element
       return element
     else:
       self._general_error(f"No element definition found for element '{name}'")
       return None
 
   def _add_cell(self, arm, epoch, elements):
     return StudyCell(
       studyCellId=id_manager.build_id(StudyCell), 
-      studyArm=arm,
-      studyEpoch=epoch,
-      studyElements=elements
+      studyArmId=arm,
+      studyEpochId=epoch,
+      studyElementIds=elements
     )
 
-  def _add_design(self, name, description, cells, intent_types, trial_types, intervention_model, rationale, blinding, therapeutic_areas):
+  def _add_design(self, name, description, epochs, arms, cells, elements, intent_types, trial_types, intervention_model, rationale, blinding, therapeutic_areas):
     return StudyDesign(
       studyDesignId=id_manager.build_id(StudyDesign), 
       studyDesignName=name,
       studyDesignDescription=description,
       trialIntentTypes=intent_types,
       trialType=trial_types,
       interventionModel=intervention_model,
       studyCells=cells,
+      studyArms=arms,
+      studyEpochs=epochs,
+      studyElements=elements,
       therapeuticAreas=therapeutic_areas,
       studyDesignRationale=rationale,
       studyDesignBlindingScheme=blinding
     )
```

### Comparing `usdm-0.27.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_sheet/study_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_sheet/study_sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,26 +64,26 @@
       self.epochs = StudyDesignEpochSheet(file_path)
       self.activities = StudyDesignActivitySheet(file_path)
       self.study_design = StudyDesignSheet(file_path)
       for timeline in self.study_design.other_timelines:
         tl = StudySoASheet(file_path, timeline)
         self.timelines[timeline] = tl
         cross_references.add(timeline, tl.timeline.scheduleTimelineId)
-      self.soa = StudySoASheet(file_path, self.study_design.main_timeline)
+      self.soa = StudySoASheet(file_path, self.study_design.main_timeline, True)
       self.ii = StudyDesignIISheet(file_path)
       self.study_populations = StudyDesignPopulationSheet(file_path)
       self.oe = StudyDesignObjectiveEndpointSheet(file_path)
       self.estimands = StudyDesignEstimandsSheet(file_path)
 
-      for epoch in self.study_design.epochs:
-        ids = self.soa.epoch_encounter_map(epoch.studyEpochName)
-        if ids is not None:
-          epoch.encounterIds = ids
-        else:
-          self._general_info(f"No encounters found for epoch '{epoch.studyEpochName}'")
+      # for epoch in self.study_design.epochs:
+      #   ids = self.soa.epoch_encounter_map(epoch.studyEpochName)
+      #   if ids is not None:
+      #     epoch.encounterIds = ids
+      #   else:
+      #     self._general_info(f"No encounters found for epoch '{epoch.studyEpochName}'")
 
       study_design = self.study_design.study_designs[0]
       study_design.studyScheduleTimelines.append(self.soa.timeline)
       study_design.encounters = self.encounters.items
       study_design.activities = self.soa.activities
       study_design.biomedicalConcepts = self.soa.biomedical_concepts
       study_design.bcSurrogates = self.soa.biomedical_concept_surrogates
```

### Comparing `usdm-0.27.0/src/usdm_excel/study_soa_sheet/activities.py` & `usdm-0.28.0/src/usdm_excel/study_soa_sheet/activities.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_soa_sheet/activity.py` & `usdm-0.28.0/src/usdm_excel/study_soa_sheet/activity.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_soa_sheet/cycle.py` & `usdm-0.28.0/src/usdm_excel/study_soa_sheet/cycle.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_soa_sheet/cycles.py` & `usdm-0.28.0/src/usdm_excel/study_soa_sheet/cycles.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py` & `usdm-0.28.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,74 @@
 from usdm_excel.study_soa_sheet.soa_column_rows import SoAColumnRows
 from usdm_excel.base_sheet import BaseSheet
 from usdm_excel.id_manager import id_manager
 from usdm_excel.study_soa_sheet.cycles import Cycles
 from usdm_excel.study_soa_sheet.timepoints import Timepoints
 from usdm_excel.study_soa_sheet.timepoint import Timepoint
-from usdm_excel.study_soa_sheet.encounters import Encounters
 from usdm_excel.study_soa_sheet.activities import Activities
 from usdm_model.scheduled_instance import ScheduledActivityInstance, ScheduledDecisionInstance
 from usdm_model.schedule_timeline import ScheduleTimeline
 from usdm_model.schedule_timeline_exit import ScheduleTimelineExit
 
 import traceback
-import pandas as pd
 
 class StudySoASheet(BaseSheet):
 
   NAME_ROW = 0
   DESCRIPTION_ROW = 1
   CONDITION_ROW = 2
   PARAMS_DATA_COL = 1
 
-  def __init__(self, file_path, sheet_name):
+  def __init__(self, file_path, sheet_name, main=False):
     try:
-      #super().__init__(pd.read_excel(open(file_path, 'rb'), sheet_name=sheet_name, header=None))
       super().__init__(file_path=file_path, sheet_name=sheet_name, header=None)
       self.name = ""
       self.description = ""
       self.condition = ""
       self.timeline = None
+      self.main_timeline = main
       self.encounters = []
       self.activities = []
       self.timelines = []
       self.biomedical_concept_surrogates = []
       self.biomedical_concepts = []
       self._process_sheet()
       self._raw_cycles = Cycles(self)
       self._raw_timepoints = Timepoints(self)
-      self._raw_encounters = Encounters(self)
+      #self._raw_encounters = Encounters(self)
       self._raw_activities = Activities(self)
 
       self._link_instance_to_activities()
       self._insert_cycles_into_timeline()
       self._raw_timepoints.set_condition_refs()
 
       instances = []
 
       for item in self._raw_activities.items:
         self.activities.append(item.usdm_activity)
         self.biomedical_concept_surrogates += item.usdm_biomedical_concept_surrogates
         self.biomedical_concepts += item.usdm_biomedical_concepts
       self.double_link(self.activities, 'activityId', 'previousActivityId', 'nextActivityId')
       
-      seq_number = 1
+      prev_instance = None
       for raw_timepoint in self._raw_timepoints.items:
         instance = raw_timepoint.usdm_timepoint
-        instance.scheduleSequenceNumber = seq_number
+        instance.defaultConditionId = None
         instances.append(instance)
-        seq_number += 1
+        if prev_instance is not None:
+          prev_instance.defaultConditionId = instance.scheduledInstanceId
+        prev_instance = instance
       exit = self._add_exit()
       self.timeline = self._add_timeline(self.name, self.description, self.condition, instances, exit)
 
     except Exception as e:
+      print(f"Exception [{e}] raised reading sheet")
       self._general_error(f"Exception [{e}] raised reading sheet")
       self._traceback(f"{traceback.format_exc()}")
 
-  def epoch_encounter_map(self, epoch):
-    return self._raw_encounters.epoch_encounter_map(epoch)
-
   def _process_sheet(self):
     for rindex in range(self.NAME_ROW, self.CONDITION_ROW + 1):
       if rindex == self.NAME_ROW:
         self.name = self.read_cell(rindex, self.PARAMS_DATA_COL)
       elif rindex == self.DESCRIPTION_ROW:
         self.description = self.read_cell(rindex, self.PARAMS_DATA_COL)
       elif rindex == self.CONDITION_ROW:
@@ -80,14 +78,15 @@
 
   def _add_exit(self):
     return ScheduleTimelineExit(scheduleTimelineExitId=id_manager.build_id(ScheduleTimelineExit))
 
   def _add_timeline(self, name, description, condition, instances, exit):
     return ScheduleTimeline(
       scheduleTimelineId=id_manager.build_id(ScheduleTimeline),
+      mainTimeline=self.main_timeline,
       scheduleTimelineName=name,
       scheduleTimelineDescription=description,
       entryCondition=condition,
       scheduleTimelineEntryId=instances[0].scheduledInstanceId,
       scheduleTimelineExits=[exit],
       scheduleTimelineInstances=instances
     )
```

### Comparing `usdm-0.27.0/src/usdm_excel/study_soa_sheet/timepoint.py` & `usdm-0.28.0/src/usdm_excel/study_soa_sheet/timepoint.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from usdm_excel.base_sheet import BaseSheet
 from usdm_excel.study_soa_sheet.soa_column_rows import SoAColumnRows
+from usdm_excel.study_soa_sheet.timepoint_type import TimepointType
+from usdm_excel.study_soa_sheet.window_type import WindowType
 from usdm_excel.id_manager import id_manager
 from usdm_excel.cross_ref import cross_references
 from usdm_excel.cdisc_ct import CDISCCT
 from usdm_model.timing import Timing
 from usdm_model.scheduled_instance import ScheduledActivityInstance, ScheduledDecisionInstance
-import pandas as pd
 
 class Timepoint():
   
   def __init__(self, parent, activity_names, col_index, type="", value="", cycle=None, additional=False):
     self.parent = parent
     self.col_index = col_index
     if col_index == None:
@@ -19,102 +20,92 @@
     self.encounter_xref = ""
     self.has_activities = not additional
     self.has_encounter = False
     if not additional:
       self.encounter_xref, encounter_is_null = self.parent.read_cell_empty_legacy(SoAColumnRows.VISIT_LABEL_ROW, col_index)
       if not self.encounter_xref == "":
         self.has_encounter = True
+      self.epoch = self.parent.read_cell_with_previous(SoAColumnRows.EPOCH_ROW, col_index, SoAColumnRows.FIRST_VISIT_COL)
+      epoch_ref = cross_references.get(self.epoch)
     self.activities = []
     self.activity_map = {}
-    self.timing_type = type
-    self.timing_value = value
+    self.__timepoint_type = None
     self.reference = None
+    #self.timing_type = type
+    #self.timing_value = value
+    self.__window = None
     self.cycle = cycle
-    #print("ENC:", self.encounter_xref, self.has_encounter)
     if not additional:
       self._process_timepoint()
       self._add_activities(activity_names)
     self.usdm_timepoint = self._as_usdm()
     if self.has_encounter:
       encounter = cross_references.get(self.encounter_xref)
-      self.usdm_timepoint.scheduledInstanceEncounterId = encounter.encounterId
+      self.usdm_timepoint.scheduledActivityInstanceEncounterId = encounter.encounterId
+    if epoch_ref is not None:
+      self.usdm_timepoint.epochId = epoch_ref.studyEpochId
 
   def key(self):
     return self._position_key
   
-  def add_encounter(self, encounter):
-    self.usdm_timepoint.scheduledInstanceEncounterId = encounter.usdm_encounter.encounterId
-
   def add_activity(self, activity):
     self.usdm_timepoint.activityIds.append(activity.usdm_activity.activityId)
 
   def _process_timepoint(self):
-    rel_ref = 0
-    timing_info = self.parent.read_cell(SoAColumnRows.TIMING_ROW, self.col_index)
-    if not timing_info == "":
-      timing_parts = timing_info.split(":")
-      if timing_parts[0].upper()[0] == "A":
-        self.timing_type = "anchor"
-        rel_ref = 0
-      if timing_parts[0].upper()[0] == "P":
-        self.timing_type = "previous"
-        rel_ref = self.get_relative_ref(timing_parts[0]) * -1
-      elif timing_parts[0].upper()[0] == "N":
-        self.timing_type = "next"
-        rel_ref = self.get_relative_ref(timing_parts[0])
-      elif timing_parts[0].upper()[0] == "C":
-        self.timing_type = "cycle start"
-        rel_ref = self.get_relative_ref(timing_parts[0])
-      if len(timing_parts) == 2:
-        self.timing_value = timing_parts[1].strip()
-    self.reference = self.col_index - SoAColumnRows.FIRST_VISIT_COL + rel_ref
+    self.__timepoint_type = TimepointType(self.parent, SoAColumnRows.TIMING_ROW, self.col_index)
+    self.reference = self.col_index - SoAColumnRows.FIRST_VISIT_COL + self.__timepoint_type.relative_ref
+    self.__window = WindowType(self.parent, SoAColumnRows.VISIT_WINDOW_ROW, self.col_index)
 
   def _as_usdm(self):
     instance = None
-    if self.timing_type in ["anchor", "next", "previous", "cycle start"]:
+    if self.__timepoint_type.timing_type in ["anchor", "next", "previous", "cycle start"]:
       timing = self._to_timing()
       instance = ScheduledActivityInstance(
         scheduledInstanceId=id_manager.build_id(ScheduledActivityInstance),
         scheduledInstanceType='ACTIVITY',
-        scheduleSequenceNumber=0,
-        scheduleTimelineExitId="",
-        scheduledInstanceEncounterId="",
+        scheduleTimelineExitId=None,
+        scheduledInstanceEncounterId=None,
         scheduledInstanceTimings=[timing],
-        scheduledInstanceTimelineId="",
+        scheduledInstanceTimelineId=None,
+        defaultConditionId=None,
+        epochId=None,
         activityIds=[]
       )
       timing.relativeFromScheduledInstanceId = instance.scheduledInstanceId
-    elif self.timing_type == "condition":
+    elif self.__timepoint_type.timing_type == "condition":
       instance = ScheduledDecisionInstance(
         scheduledInstanceId=id_manager.build_id(ScheduledActivityInstance),
         scheduledInstanceType='DECISION',
-        scheduleSequenceNumber=0,
-        scheduleTimelineExitId="",
-        scheduledInstanceEncounterId="",
+        scheduleTimelineExitId=None,
+        scheduledInstanceEncounterId=None,
         scheduledInstanceTimings=[],
-        scheduledInstanceTimelineId="",
+        scheduledInstanceTimelineId=None,
+        defaultConditionId=None,
         conditionAssignments=[]
       )
     else:
-      print("TYPE:", self.timing_type)
+      self.parent.general_warning(f"Unrecognized ScheduledInstance type: '{self.__timepoint_type.timing_type}'")
     return instance
 
   def _to_timing(self):
     type_code = {
       "ANCHOR": CDISCCT().code('C99901x3', 'Fixed Reference'),
-      "NEXT": CDISCCT().code('C99901x1', 'After'),
-      "PREVIOUS": CDISCCT().code('C99901x2', 'Before'),
+      "PREVIOUS": CDISCCT().code('C99901x1', 'After'),
+      "NEXT": CDISCCT().code('C99901x2', 'Before'),
       "CYCLE START": CDISCCT().code('C99901x3', 'Fixed Reference'),
     }
     return Timing(
       timingId=id_manager.build_id(Timing),
-      timingType=type_code[self.timing_type.upper()],
-      timingValue=self.timing_value,
+      timingType=type_code[self.__timepoint_type.timing_type.upper()],
+      timingValue=self.__timepoint_type.value,
+      timingDescription=self.__timepoint_type.description,
       timingRelativeToFrom=CDISCCT().code('C99900x1', 'Start to Start'),
-      timingWindow='',
+      timingWindow=self.__window.description,
+      timingWindowLower=self.__window.lower,
+      timingWindowUpper=self.__window.upper,
       relativeFromScheduledInstanceId='',
       relativeToScheduledInstanceId=''
     )
 
   def get_relative_ref(self, part):
     if len(part) > 1:
       return int(part[1:])
```

### Comparing `usdm-0.27.0/src/usdm_excel/study_soa_sheet/timepoints.py` & `usdm-0.28.0/src/usdm_excel/study_soa_sheet/timepoints.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_model/__init__.py` & `usdm-0.28.0/src/usdm_model/__init__.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_model/activity.py` & `usdm-0.28.0/src/usdm_model/activity.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import List, Union
 from .api_base_model import ApiBaseModel
 from .procedure import Procedure
 
 class Activity(ApiBaseModel):
   activityId: str
   activityName: str
-  activityDescription: str
+  activityDescription: Union[str, None] = None
   previousActivityId: Union[str, None] = None
   nextActivityId: Union[str, None] = None
   definedProcedures: List[Procedure] = []
   activityIsConditional: bool
-  activityIsConditionalReason: str
+  activityIsConditionalReason: Union[str, None] = None
   biomedicalConceptIds: List[str] = []
   bcCategoryIds: List[str] = []
   bcSurrogateIds: List[str] = []
-  activityTimelineId: Union[str, None] = None
+  activityTimelineId: Union[str, None] = None
```

### Comparing `usdm-0.27.0/src/usdm_model/api_base_model.py` & `usdm-0.28.0/src/usdm_model/api_base_model.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_model/encounter.py` & `usdm-0.28.0/src/usdm_model/encounter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import List, Union
-
 from .api_base_model import ApiBaseModel
 from .code import Code
 from .transition_rule import TransitionRule
 
 
 class Encounter(ApiBaseModel):
   encounterId: str
   encounterName: str
-  encounterDescription: str
+  encounterDescription: Union[str, None] = None
   previousEncounterId: Union[str, None] = None
   nextEncounterId: Union[str, None] = None
   encounterType: Union[Code, None] = None
   encounterEnvironmentalSetting: Union[Code, None] = None
   encounterContactModes: List[Code] = []
   transitionStartRule: Union[TransitionRule, None] = None
   transitionEndRule: Union[TransitionRule, None] = None
```

### Comparing `usdm-0.27.0/src/usdm_model/estimand.py` & `usdm-0.28.0/src/usdm_model/estimand.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/src/usdm_model/scheduled_instance.py` & `usdm-0.28.0/src/usdm_model/scheduled_instance.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from enum import Enum
 from typing import List, Dict, Union, Literal
-
 from .api_base_model import ApiBaseModel
 from .timing import Timing
 
 class ScheduledInstance(ApiBaseModel):
     scheduledInstanceId: str
     scheduledInstanceType: Literal['ACTIVITY', 'DECISION']
-    scheduleSequenceNumber: int
     scheduleTimelineExitId: Union[str, None] = None
-    scheduledInstanceEncounterId: Union[str, None] = None
     scheduledInstanceTimings: List[Timing] = []
     scheduledInstanceTimelineId: Union[str, None] = None
+    defaultConditionId: Union[str, None] = None
+    epochId: Union[str, None] = None
 
 class ScheduledActivityInstance(ScheduledInstance):
     activityIds: List[str] = []
+    scheduledActivityInstanceEncounterId: Union[str, None] = None
 
 class ScheduledDecisionInstance(ScheduledInstance):
     conditionAssignments: List[List] = []
```

### Comparing `usdm-0.27.0/src/usdm_model/study.py` & `usdm-0.28.0/src/usdm_model/study.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,7 @@
   studyPhase: Union[AliasCode, None] = None
   businessTherapeuticAreas: List[Code] = []
   studyIdentifiers: List[StudyIdentifier] = []
   studyProtocolVersions: List[StudyProtocolVersion] = []
   studyDesigns: List[StudyDesign] = []
   studyRationale: str
   studyAcronym: str
-
```

### Comparing `usdm-0.27.0/src/usdm_model/study_design.py` & `usdm-0.28.0/src/usdm_model/study_design.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,35 +6,41 @@
 from .biomedical_concept_category import BiomedicalConceptCategory
 from .biomedical_concept_surrogate import BiomedicalConceptSurrogate
 from .code import Code
 from .encounter import Encounter
 from .study_cell import StudyCell
 from .indication import Indication
 from .investigational_intervention import InvestigationalIntervention
+from .study_arm import StudyArm
+from .study_epoch import StudyEpoch
+from .study_element import StudyElement
 from .study_design_population import StudyDesignPopulation
 from .objective import Objective
 from .schedule_timeline import ScheduleTimeline
 from .estimand import Estimand
 import pandas as pd
 
 class StudyDesign(ApiBaseModel):
   studyDesignId: str
   studyDesignName: str
-  studyDesignDescription: str
+  studyDesignDescription: Union[str, None] = None
   trialIntentTypes: List[Code] = []
   trialType: List[Code] = []
   interventionModel: Code
-  studyCells: List[StudyCell] = []
+  studyCells: List[StudyCell]
   studyIndications: List[Indication] = []
   studyInvestigationalInterventions: List[InvestigationalIntervention] = []
   studyPopulations: List[StudyDesignPopulation] = []
   studyObjectives: List[Objective] = []
   studyScheduleTimelines: List[ScheduleTimeline] = []
   therapeuticAreas: List[Code] = []
   studyEstimands: List[Estimand] = []
   encounters: List[Encounter] = []
   activities: List[Activity] = []
   studyDesignRationale: str
-  studyDesignBlindingScheme: AliasCode = None
+  studyDesignBlindingScheme: Union[AliasCode, None] = None
   biomedicalConcepts: List[BiomedicalConcept] = []
   bcCategories: List[BiomedicalConceptCategory] = []
   bcSurrogates: List[BiomedicalConceptSurrogate] = []
+  studyArms: List[StudyArm]
+  studyEpochs: List[StudyEpoch]
+  studyElements: List[StudyElement] = []
```

### Comparing `usdm-0.27.0/tests/test_base_sheet.py` & `usdm-0.28.0/tests/test_base_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/tests/test_cdisc_biomedical_concept.py` & `usdm-0.28.0/tests/test_cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/tests/test_configuration_sheet.py` & `usdm-0.28.0/tests/test_configuration_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/tests/test_error.py` & `usdm-0.28.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/tests/test_errors.py` & `usdm-0.28.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/tests/test_iso_3166.py` & `usdm-0.28.0/tests/test_iso_3166.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/tests/test_option_manager.py` & `usdm-0.28.0/tests/test_option_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/tests/test_study_design_activity_sheet.py` & `usdm-0.28.0/tests/test_study_design_activity_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/tests/test_study_design_arm_sheet.py` & `usdm-0.28.0/tests/test_study_design_arm_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/tests/test_study_design_epoch_sheet.py` & `usdm-0.28.0/tests/test_study_design_epoch_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.27.0/tests/test_study_identifiers_sheet.py` & `usdm-0.28.0/tests/test_study_identifiers_sheet.py`

 * *Files identical despite different names*

