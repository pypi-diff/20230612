# Comparing `tmp/dbt_semantic_interfaces-0.1.0.dev4.tar.gz` & `tmp/dbt_semantic_interfaces-0.1.0.dev5.tar.gz`

## Comparing `dbt_semantic_interfaces-0.1.0.dev4.tar` & `dbt_semantic_interfaces-0.1.0.dev5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/CHANGELOG.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/__init__.py
--rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/dataclass_serialization.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/enum_extension.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/errors.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/py.typed
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/references.py
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/__init__.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/base.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/metadata.py
--rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/metric.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/semantic_manifest.py
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/semantic_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/__init__.py
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/dimension.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/entity.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/measure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/filters/__init__.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/filters/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/__init__.py
--rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/dir_to_model.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/explicit_schema.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/objects.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/schema_validator.py
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/schemas.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/yaml_loader.py
--rw-r--r--   0        0        0    14950 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/__init__.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/dimension.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/entity.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/measure.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/metadata.py
--rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/metric.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/protocol_hint.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/semantic_manifest.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/semantic_model.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/__init__.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/agg_time_dimension.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/boolean_measure.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/convert_count.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/convert_median.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/names.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/proxy_measure.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/rule_set.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/transform_rule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/aggregation_type.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/dimension_type.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/entity_type.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/metric_type.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/time_granularity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/__init__.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/agg_time_dimension.py
--rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/common_entities.py
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/dimension_const.py
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/element_const.py
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/entities.py
--rw-r--r--   0        0        0    28504 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/measures.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/metrics.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/non_empty.py
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/reserved_keywords.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
--rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/semantic_models.py
--rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/unique_valid_name.py
--rw-r--r--   0        0        0    14682 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/validator_helpers.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/LICENSE
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/README.md
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/pyproject.toml
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/CHANGELOG.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/__init__.py
+-rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/dataclass_serialization.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/enum_extension.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/errors.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/pretty_print.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/py.typed
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/references.py
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/__init__.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/base.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/metadata.py
+-rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/metric.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/semantic_manifest.py
+-rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/semantic_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/__init__.py
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/dimension.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/entity.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/measure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/filters/__init__.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/filters/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/__init__.py
+-rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/dir_to_model.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/explicit_schema.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/objects.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/schema_validator.py
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/schemas.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/yaml_loader.py
+-rw-r--r--   0        0        0    14950 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/dimension.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/entity.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/measure.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/metadata.py
+-rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/metric.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/protocol_hint.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/semantic_manifest.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/semantic_model.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/__init__.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/agg_time_dimension.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/boolean_measure.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/convert_count.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/convert_median.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/names.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/proxy_measure.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/rule_set.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/transform_rule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/aggregation_type.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/dimension_type.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/entity_type.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/metric_type.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/time_granularity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/__init__.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/agg_time_dimension.py
+-rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/common_entities.py
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/dimension_const.py
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/element_const.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/entities.py
+-rw-r--r--   0        0        0    28504 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/measures.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/metrics.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/non_empty.py
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/reserved_keywords.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
+-rw-r--r--   0        0        0    11010 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/semantic_models.py
+-rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/unique_valid_name.py
+-rw-r--r--   0        0        0    15207 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/validator_helpers.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/LICENSE
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/README.md
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev5/PKG-INFO
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/Makefile` & `dbt_semantic_interfaces-0.1.0.dev5/Makefile`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/dataclass_serialization.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/dataclass_serialization.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/enum_extension.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/enum_extension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/errors.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/errors.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/pretty_print.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/pretty_print.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/references.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/references.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/test_utils.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/base.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/base.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/metric.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/semantic_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 
 class PydanticSemanticModelDefaults(HashableBaseModel, ProtocolHint[SemanticModelDefaults]):  # noqa: D
     @override
     def _implements_protocol(self) -> SemanticModelDefaults:  # noqa: D
         return self
 
-    agg_time_dimension: str
+    agg_time_dimension: Optional[str]
 
 
 class PydanticSemanticModel(HashableBaseModel, ModelWithMetadataParsing, ProtocolHint[SemanticModel]):
     """Describes a semantic model."""
 
     @override
     def _implements_protocol(self) -> SemanticModel:
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/entity.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/measure.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/elements/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/filters/where_filter.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/implementations/filters/where_filter.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/dir_to_model.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/dir_to_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/explicit_schema.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/explicit_schema.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/objects.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/objects.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/schema_validator.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/schemas.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/yaml_loader.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/entity.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/measure.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/metadata.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/metric.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/protocol_hint.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/protocol_hint.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/protocols/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/add_input_metric_measures.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/add_input_metric_measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/boolean_measure.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/boolean_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/convert_count.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/convert_count.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/convert_median.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/convert_median.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/names.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/names.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/proxy_measure.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/proxy_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/pydantic_rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/pydantic_rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/transform_rule.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/transformations/transform_rule.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/time_granularity.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/type_enums/time_granularity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/agg_time_dimension.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from typing import Generic, List, Sequence
 
 from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
 from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
-from dbt_semantic_interfaces.references import (
-    SemanticModelElementReference,
-    TimeDimensionReference,
-)
-from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
+from dbt_semantic_interfaces.references import SemanticModelElementReference
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     SemanticManifestValidationRule,
     SemanticModelElementContext,
     SemanticModelElementType,
+    SemanticModelValidationHelpers,
     ValidationError,
     ValidationIssue,
     validate_safely,
 )
 
 
 class AggregationTimeDimensionRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
@@ -27,38 +24,29 @@
         issues: List[ValidationIssue] = []
         for semantic_model in semantic_manifest.semantic_models:
             issues.extend(AggregationTimeDimensionRule._validate_semantic_model(semantic_model))
 
         return issues
 
     @staticmethod
-    def _time_dimension_in_model(
-        time_dimension_reference: TimeDimensionReference, semantic_model: SemanticModel
-    ) -> bool:
-        for dimension in semantic_model.dimensions:
-            if dimension.type == DimensionType.TIME and dimension.name == time_dimension_reference.element_name:
-                return True
-        return False
-
-    @staticmethod
     @validate_safely(whats_being_done="checking aggregation time dimension for a semantic model")
     def _validate_semantic_model(semantic_model: SemanticModel) -> List[ValidationIssue]:
         issues: List[ValidationIssue] = []
 
         for measure in semantic_model.measures:
             measure_context = SemanticModelElementContext(
                 file_context=FileContext.from_metadata(metadata=semantic_model.metadata),
                 semantic_model_element=SemanticModelElementReference(
                     semantic_model_name=semantic_model.name, element_name=measure.name
                 ),
                 element_type=SemanticModelElementType.MEASURE,
             )
             agg_time_dimension_reference = measure.checked_agg_time_dimension
-            if not AggregationTimeDimensionRule._time_dimension_in_model(
-                time_dimension_reference=agg_time_dimension_reference, semantic_model=semantic_model
+            if not SemanticModelValidationHelpers.time_dimension_in_model(
+                time_dimension_name=agg_time_dimension_reference.element_name, semantic_model=semantic_model
             ):
                 issues.append(
                     ValidationError(
                         context=measure_context,
                         message=f"In semantic model '{semantic_model.name}', measure '{measure.name}' has the "
                         f"aggregation time dimension set to '{agg_time_dimension_reference.element_name}', "
                         f"which is not a valid time dimension in the semantic model",
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/common_entities.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/common_entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/dimension_const.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/dimension_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/element_const.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/element_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/entities.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/measures.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/metrics.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/non_empty.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/non_empty.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/reserved_keywords.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/semantic_manifest_validator.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/semantic_manifest_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from dbt_semantic_interfaces.validations.metrics import (
     CumulativeMetricRule,
     DerivedMetricRule,
 )
 from dbt_semantic_interfaces.validations.non_empty import NonEmptyRule
 from dbt_semantic_interfaces.validations.reserved_keywords import ReservedKeywordsRule
 from dbt_semantic_interfaces.validations.semantic_models import (
+    SemanticModelDefaultsRule,
     SemanticModelTimeDimensionWarningsRule,
     SemanticModelValidityWindowRule,
 )
 from dbt_semantic_interfaces.validations.unique_valid_name import UniqueAndValidNameRule
 from dbt_semantic_interfaces.validations.validator_helpers import (
     SemanticManifestValidationException,
     SemanticManifestValidationResults,
@@ -74,14 +75,15 @@
         MetricMeasuresRule[SemanticManifestT](),
         CumulativeMetricRule[SemanticManifestT](),
         NonEmptyRule[SemanticManifestT](),
         UniqueAndValidNameRule[SemanticManifestT](),
         AggregationTimeDimensionRule[SemanticManifestT](),
         ReservedKeywordsRule[SemanticManifestT](),
         MeasuresNonAdditiveDimensionRule[SemanticManifestT](),
+        SemanticModelDefaultsRule[SemanticManifestT](),
     )
 
     def __init__(
         self, rules: Sequence[SemanticManifestValidationRule[SemanticManifestT]] = DEFAULT_RULES, max_workers: int = 1
     ) -> None:
         """Constructor.
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/semantic_models.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/semantic_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
 from dbt_semantic_interfaces.references import SemanticModelReference
 from dbt_semantic_interfaces.type_enums.entity_type import EntityType
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     SemanticManifestValidationRule,
     SemanticModelContext,
+    SemanticModelValidationHelpers,
     ValidationError,
     ValidationIssue,
     validate_safely,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -174,7 +175,47 @@
                     f"Measure names: {measure_names}. Validity param dimension names: "
                     f"{validity_param_dimension_names}."
                 ),
             )
             issues.append(error)
 
         return issues
+
+
+class SemanticModelDefaultsRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
+    """Checks defaults in semantic models."""
+
+    @staticmethod
+    @validate_safely(whats_being_done="running model validation ensuring the defaults are valid")
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
+        issues: List[ValidationIssue] = []
+
+        for semantic_model in semantic_manifest.semantic_models:
+            issues.extend(SemanticModelDefaultsRule._validate_default_agg_time_dimension(semantic_model=semantic_model))
+        return issues
+
+    @staticmethod
+    @validate_safely(whats_being_done="checking validity of the semantic model's default agg_time_dimension")
+    def _validate_default_agg_time_dimension(semantic_model: SemanticModel) -> List[ValidationIssue]:
+        issues: List[ValidationIssue] = []
+
+        if semantic_model.defaults is None:
+            return []
+
+        default_agg_time_dimension = semantic_model.defaults.agg_time_dimension
+        assert default_agg_time_dimension is not None, "should not be None"
+
+        if not SemanticModelValidationHelpers.time_dimension_in_model(
+            time_dimension_name=default_agg_time_dimension, semantic_model=semantic_model
+        ):
+            issues.append(
+                ValidationError(
+                    context=SemanticModelContext(
+                        file_context=FileContext.from_metadata(metadata=semantic_model.metadata),
+                        semantic_model=SemanticModelReference(semantic_model_name=semantic_model.name),
+                    ),
+                    message=f"Default aggregation time dimension was specified as '{default_agg_time_dimension}' which "
+                    f"doesn't exist as a time dimension in semantic model named '{semantic_model.name}'.",
+                )
+            )
+
+        return issues
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/unique_valid_name.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/unique_valid_name.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/validator_helpers.py` & `dbt_semantic_interfaces-0.1.0.dev5/dbt_semantic_interfaces/validations/validator_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 import click
 from pydantic import BaseModel, Extra
 
 from dbt_semantic_interfaces.implementations.base import FrozenBaseModel
 from dbt_semantic_interfaces.protocols.metadata import Metadata
 from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
+from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
 from dbt_semantic_interfaces.references import (
     MetricModelReference,
     SemanticModelElementReference,
     SemanticModelReference,
 )
 from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
 
@@ -399,7 +400,18 @@
 
 class SemanticManifestValidationException(Exception):
     """Exception raised when validation of a model fails."""
 
     def __init__(self, issues: Tuple[ValidationIssue, ...]) -> None:  # noqa: D
         issues_str = "\n".join([x.as_readable_str(verbose=True) for x in issues])
         super().__init__(f"Error validating model. Issues:\n{issues_str}")
+
+
+class SemanticModelValidationHelpers:
+    """Class containing all the helpers related to semantic model validations."""
+
+    @classmethod
+    def time_dimension_in_model(cls, time_dimension_name: str, semantic_model: SemanticModel) -> bool:  # noqa: D
+        for dimension in semantic_model.dimensions:
+            if dimension.type == DimensionType.TIME and dimension.name == time_dimension_name:
+                return True
+        return False
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/.gitignore` & `dbt_semantic_interfaces-0.1.0.dev5/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/LICENSE` & `dbt_semantic_interfaces-0.1.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/README.md` & `dbt_semantic_interfaces-0.1.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/pyproject.toml` & `dbt_semantic_interfaces-0.1.0.dev5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbt-semantic-interfaces"
-version = "0.1.0.dev4"
+version = "0.1.0.dev5"
 description = 'The shared semantic layer definitions that dbt-core and MetricFlow use'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev4/PKG-INFO` & `dbt_semantic_interfaces-0.1.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-semantic-interfaces
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs <info@dbtlabs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev4
+Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev5
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs
 dbtlabs.com> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

