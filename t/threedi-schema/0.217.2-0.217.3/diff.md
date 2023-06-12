# Comparing `tmp/threedi-schema-0.217.2.tar.gz` & `tmp/threedi-schema-0.217.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-schema-0.217.2.tar", last modified: Wed May 24 13:38:22 2023, max compression
+gzip compressed data, was "threedi-schema-0.217.3.tar", last modified: Mon Jun 12 13:31:06 2023, max compression
```

## Comparing `threedi-schema-0.217.2.tar` & `threedi-schema-0.217.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:22.258545 threedi-schema-0.217.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-24 13:38:22.258545 threedi-schema-0.217.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-24 13:38:22.258545 threedi-schema-0.217.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:22.254545 threedi-schema-0.217.2/threedi_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:22.254545 threedi-schema-0.217.2/threedi_schema/application/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/application/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/application/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/application/threedi_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/beta_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:22.254545 threedi-schema-0.217.2/threedi_schema/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/domain/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/domain/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/domain/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:22.254545 threedi-schema-0.217.2/threedi_schema/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/infrastructure/spatial_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/infrastructure/spatialite_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/infrastructure/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:22.254545 threedi-schema-0.217.2/threedi_schema/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:22.258545 threedi-schema-0.217.2/threedi_schema/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)    46413 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0200_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0202_remove_unused_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0203_remove_unused_cols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0205_settings_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0206_control_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0208_tables_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0209_remove_surface_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0210_global_raster_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0211_breach_and_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0216_vegetation_drag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:22.258545 threedi-schema-0.217.2/threedi_schema/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:22.258545 threedi-schema-0.217.2/threedi_schema/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/tests/test_gpkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/tests/test_migration_213.py
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-24 13:38:12.000000 threedi-schema-0.217.2/threedi_schema/tests/test_spatalite_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:22.254545 threedi-schema-0.217.2/threedi_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-24 13:38:22.000000 threedi-schema-0.217.2/threedi_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-24 13:38:22.000000 threedi-schema-0.217.2/threedi_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:38:22.000000 threedi-schema-0.217.2/threedi_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 13:38:22.000000 threedi-schema-0.217.2/threedi_schema.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:38:22.000000 threedi-schema-0.217.2/threedi_schema.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 13:38:22.000000 threedi-schema-0.217.2/threedi_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 13:38:22.000000 threedi-schema-0.217.2/threedi_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.096562 threedi-schema-0.217.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-12 13:31:06.096562 threedi-schema-0.217.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-12 13:31:06.096562 threedi-schema-0.217.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.084562 threedi-schema-0.217.3/threedi_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.088562 threedi-schema-0.217.3/threedi_schema/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/application/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/application/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/application/threedi_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/beta_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.088562 threedi-schema-0.217.3/threedi_schema/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/domain/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/domain/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.092562 threedi-schema-0.217.3/threedi_schema/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/infrastructure/spatial_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/infrastructure/spatialite_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/infrastructure/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.092562 threedi-schema-0.217.3/threedi_schema/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.096562 threedi-schema-0.217.3/threedi_schema/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)    46413 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0200_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0202_remove_unused_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0203_remove_unused_cols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0205_settings_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0206_control_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0208_tables_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0209_remove_surface_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0210_global_raster_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0211_breach_and_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0216_vegetation_drag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.096562 threedi-schema-0.217.3/threedi_schema/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.096562 threedi-schema-0.217.3/threedi_schema/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/test_gpkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/test_migration_213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-12 13:30:51.000000 threedi-schema-0.217.3/threedi_schema/tests/test_spatalite_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:31:06.088562 threedi-schema-0.217.3/threedi_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-12 13:31:06.000000 threedi-schema-0.217.3/threedi_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-12 13:31:06.000000 threedi-schema-0.217.3/threedi_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:31:06.000000 threedi-schema-0.217.3/threedi_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 13:31:06.000000 threedi-schema-0.217.3/threedi_schema.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:31:05.000000 threedi-schema-0.217.3/threedi_schema.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-12 13:31:06.000000 threedi-schema-0.217.3/threedi_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 13:31:06.000000 threedi-schema-0.217.3/threedi_schema.egg-info/top_level.txt
```

### Comparing `threedi-schema-0.217.2/CHANGES.rst` & `threedi-schema-0.217.3/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog of threedi-schema
 ===================================================
 
+0.217.3 (2023-06-12)
+--------------------
+
+- Added groundwater 1D2D columns to the views.
+
+
 0.217.2 (2023-05-24)
 --------------------
 
 - Remove vegetation and groundwater settings from beta features, since they are going to be released.
 
 
 0.217.1 (2023-05-17)
```

### Comparing `threedi-schema-0.217.2/LICENSE` & `threedi-schema-0.217.3/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/PKG-INFO` & `threedi-schema-0.217.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.217.2
+Version: 0.217.3
 Summary: The schema of 3Di schematization files
 Home-page: https://github.com/nens/threedi-schema
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
@@ -81,14 +81,20 @@
 
   $ pip install threedi-schema
 
 
 Changelog of threedi-schema
 ===================================================
 
+0.217.3 (2023-06-12)
+--------------------
+
+- Added groundwater 1D2D columns to the views.
+
+
 0.217.2 (2023-05-24)
 --------------------
 
 - Remove vegetation and groundwater settings from beta features, since they are going to be released.
 
 
 0.217.1 (2023-05-17)
```

### Comparing `threedi-schema-0.217.2/README.rst` & `threedi-schema-0.217.3/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/setup.py` & `threedi-schema-0.217.3/setup.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/application/schema.py` & `threedi-schema-0.217.3/threedi_schema/application/schema.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/application/threedi_database.py` & `threedi-schema-0.217.3/threedi_schema/application/threedi_database.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/beta_features.py` & `threedi-schema-0.217.3/threedi_schema/beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/domain/constants.py` & `threedi-schema-0.217.3/threedi_schema/domain/constants.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/domain/custom_types.py` & `threedi-schema-0.217.3/threedi_schema/domain/custom_types.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/domain/indexes.py` & `threedi-schema-0.217.3/threedi_schema/domain/indexes.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/domain/models.py` & `threedi-schema-0.217.3/threedi_schema/domain/models.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/domain/views.py` & `threedi-schema-0.217.3/threedi_schema/domain/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,29 +32,29 @@
         "definition": "SELECT cul.rowid AS rowid, cul.id AS cul_id, cul.display_name AS cul_display_name, cul.code AS cul_code, cul.calculation_type AS cul_calculation_type, cul.friction_value AS cul_friction_value, cul.friction_type AS cul_friction_type, cul.dist_calc_points AS cul_dist_calc_points, cul.zoom_category AS cul_zoom_category, cul.cross_section_definition_id AS cul_cross_section_definition_id, cul.discharge_coefficient_positive AS cul_discharge_coefficient_positive, cul.discharge_coefficient_negative AS cul_discharge_coefficient_negative, cul.invert_level_start_point AS cul_invert_level_start_point, cul.invert_level_end_point AS cul_invert_level_end_point, cul.the_geom AS the_geom, cul.connection_node_start_id AS cul_connection_node_start_id, cul.connection_node_end_id AS cul_connection_node_end_id, def.id AS def_id, def.shape AS def_shape, def.width AS def_width, def.height AS def_height, def.code AS def_code FROM v2_culvert AS cul , v2_cross_section_definition AS def WHERE cul.cross_section_definition_id = def.id",
         "view_geometry": "the_geom",
         "view_rowid": "rowid",
         "f_table_name": "v2_culvert",
         "f_geometry_column": "the_geom",
     },
     "v2_manhole_view": {
-        "definition": "SELECT manh.rowid AS rowid, manh.id AS manh_id, manh.display_name AS manh_display_name, manh.code AS manh_code, manh.connection_node_id AS manh_connection_node_id, manh.shape AS manh_shape, manh.width AS manh_width, manh.length AS manh_length, manh.manhole_indicator AS manh_manhole_indicator, manh.calculation_type AS manh_calculation_type, manh.bottom_level AS manh_bottom_level, manh.surface_level AS manh_surface_level, manh.drain_level AS manh_drain_level, manh.sediment_level AS manh_sediment_level, manh.zoom_category AS manh_zoom_category, node.id AS node_id, node.storage_area AS node_storage_area, node.initial_waterlevel AS node_initial_waterlevel, node.code AS node_code, node.the_geom AS the_geom, node.the_geom_linestring AS node_the_geom_linestring FROM v2_manhole AS manh , v2_connection_nodes AS node WHERE manh.connection_node_id = node.id",
+        "definition": "SELECT manh.rowid AS rowid, manh.id AS manh_id, manh.display_name AS manh_display_name, manh.code AS manh_code, manh.connection_node_id AS manh_connection_node_id, manh.shape AS manh_shape, manh.width AS manh_width, manh.length AS manh_length, manh.manhole_indicator AS manh_manhole_indicator, manh.calculation_type AS manh_calculation_type, manh.bottom_level AS manh_bottom_level, manh.surface_level AS manh_surface_level, manh.drain_level AS manh_drain_level, manh.sediment_level AS manh_sediment_level, manh.zoom_category AS manh_zoom_category, manh.exchange_thickness AS manh_exchange_thickness, manh.hydraulic_conductivity_in AS manh_hydraulic_conductivity_in, manh.hydraulic_conductivity_out AS manh_hydraulic_conductivity_out, node.id AS node_id, node.storage_area AS node_storage_area, node.initial_waterlevel AS node_initial_waterlevel, node.code AS node_code, node.the_geom AS the_geom, node.the_geom_linestring AS node_the_geom_linestring FROM v2_manhole AS manh , v2_connection_nodes AS node WHERE manh.connection_node_id = node.id",
         "view_geometry": "the_geom",
         "view_rowid": "rowid",
         "f_table_name": "v2_connection_nodes",
         "f_geometry_column": "the_geom",
     },
     "v2_orifice_view": {
         "definition": "SELECT orf.rowid AS rowid, orf.id AS orf_id, orf.display_name AS orf_display_name, orf.code AS orf_code, orf.crest_level AS orf_crest_level, orf.sewerage AS orf_sewerage, orf.cross_section_definition_id AS orf_cross_section_definition_id, orf.friction_value AS orf_friction_value, orf.friction_type AS orf_friction_type, orf.discharge_coefficient_positive AS orf_discharge_coefficient_positive, orf.discharge_coefficient_negative AS orf_discharge_coefficient_negative, orf.zoom_category AS orf_zoom_category, orf.crest_type AS orf_crest_type, orf.connection_node_start_id AS orf_connection_node_start_id, orf.connection_node_end_id AS orf_connection_node_end_id, def.id AS def_id, def.shape AS def_shape, def.width AS def_width, def.height AS def_height, def.code AS def_code, MakeLine( start_node.the_geom, end_node.the_geom) AS the_geom FROM v2_orifice AS orf, v2_cross_section_definition AS def, v2_connection_nodes AS start_node, v2_connection_nodes AS end_node where orf.connection_node_start_id = start_node.id AND orf.connection_node_end_id = end_node.id AND orf.cross_section_definition_id = def.id",
         "view_geometry": "the_geom",
         "view_rowid": "rowid",
         "f_table_name": "v2_connection_nodes",
         "f_geometry_column": "the_geom_linestring",
     },
     "v2_pipe_view": {
-        "definition": "SELECT pipe.rowid AS rowid, pipe.id AS pipe_id, pipe.display_name AS pipe_display_name, pipe.code AS pipe_code, pipe.profile_num AS pipe_profile_num, pipe.sewerage_type AS pipe_sewerage_type, pipe.calculation_type AS pipe_calculation_type, pipe.invert_level_start_point AS pipe_invert_level_start_point, pipe.invert_level_end_point AS pipe_invert_level_end_point, pipe.cross_section_definition_id AS pipe_cross_section_definition_id, pipe.friction_value AS pipe_friction_value, pipe.friction_type AS pipe_friction_type, pipe.dist_calc_points AS pipe_dist_calc_points, pipe.material AS pipe_material, pipe.original_length AS pipe_original_length, pipe.zoom_category AS pipe_zoom_category, pipe.connection_node_start_id AS pipe_connection_node_start_id, pipe.connection_node_end_id AS pipe_connection_node_end_id, def.id AS def_id, def.shape AS def_shape, def.width AS def_width, def.height AS def_height, def.code AS def_code, MakeLine( start_node.the_geom, end_node.the_geom) AS the_geom FROM v2_pipe AS pipe , v2_cross_section_definition AS def , v2_connection_nodes AS start_node , v2_connection_nodes AS end_node WHERE pipe.connection_node_start_id = start_node.id AND pipe.connection_node_end_id = end_node.id AND pipe.cross_section_definition_id = def.id",
+        "definition": "SELECT pipe.rowid AS rowid, pipe.id AS pipe_id, pipe.display_name AS pipe_display_name, pipe.code AS pipe_code, pipe.profile_num AS pipe_profile_num, pipe.sewerage_type AS pipe_sewerage_type, pipe.calculation_type AS pipe_calculation_type, pipe.invert_level_start_point AS pipe_invert_level_start_point, pipe.invert_level_end_point AS pipe_invert_level_end_point, pipe.cross_section_definition_id AS pipe_cross_section_definition_id, pipe.friction_value AS pipe_friction_value, pipe.friction_type AS pipe_friction_type, pipe.dist_calc_points AS pipe_dist_calc_points, pipe.material AS pipe_material, pipe.original_length AS pipe_original_length, pipe.zoom_category AS pipe_zoom_category, pipe.connection_node_start_id AS pipe_connection_node_start_id, pipe.connection_node_end_id AS pipe_connection_node_end_id, pipe.exchange_thickness AS pipe_exchange_thickness, pipe.hydraulic_conductivity_in AS pipe_hydraulic_conductivity_in, pipe.hydraulic_conductivity_out AS pipe_hydraulic_conductivity_out, def.id AS def_id, def.shape AS def_shape, def.width AS def_width, def.height AS def_height, def.code AS def_code, MakeLine( start_node.the_geom, end_node.the_geom) AS the_geom FROM v2_pipe AS pipe , v2_cross_section_definition AS def , v2_connection_nodes AS start_node , v2_connection_nodes AS end_node WHERE pipe.connection_node_start_id = start_node.id AND pipe.connection_node_end_id = end_node.id AND pipe.cross_section_definition_id = def.id",
         "view_geometry": "the_geom",
         "view_rowid": "rowid",
         "f_table_name": "v2_connection_nodes",
         "f_geometry_column": "the_geom_linestring",
     },
     "v2_pumpstation_point_view": {
         "definition": "SELECT a.rowid AS rowid, a.id AS pump_id, a.display_name, a.code, a.classification, a.sewerage, a.start_level, a.lower_stop_level, a.upper_stop_level, a.capacity, a.zoom_category, a.connection_node_start_id, a.connection_node_end_id, a.type, b.id AS connection_node_id, b.storage_area, b.the_geom FROM v2_pumpstation a JOIN v2_connection_nodes b ON a.connection_node_start_id = b.id",
```

### Comparing `threedi-schema-0.217.2/threedi_schema/infrastructure/spatial_index.py` & `threedi-schema-0.217.3/threedi_schema/infrastructure/spatial_index.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/infrastructure/spatialite_versions.py` & `threedi-schema-0.217.3/threedi_schema/infrastructure/spatialite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/infrastructure/views.py` & `threedi-schema-0.217.3/threedi_schema/infrastructure/views.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/env.py` & `threedi-schema-0.217.3/threedi_schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0200_initial.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0200_initial.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0202_remove_unused_tables.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0202_remove_unused_tables.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0203_remove_unused_cols.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0203_remove_unused_cols.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0205_settings_defaults.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0205_settings_defaults.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0206_control_structures.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0206_control_structures.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0207_fix_schema_constraints.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0207_fix_schema_constraints.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0208_tables_settings.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0208_tables_settings.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0209_remove_surface_type.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0209_remove_surface_type.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0210_global_raster_values.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0210_global_raster_values.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0211_breach_and_exchange.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0211_breach_and_exchange.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0215_groundwater_1d2d.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0215_groundwater_1d2d.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0216_vegetation_drag.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0216_vegetation_drag.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py` & `threedi-schema-0.217.3/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/scripts.py` & `threedi-schema-0.217.3/threedi_schema/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/tests/conftest.py` & `threedi-schema-0.217.3/threedi_schema/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/tests/test_migration_213.py` & `threedi-schema-0.217.3/threedi_schema/tests/test_migration_213.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/tests/test_schema.py` & `threedi-schema-0.217.3/threedi_schema/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema/tests/test_spatalite_versions.py` & `threedi-schema-0.217.3/threedi_schema/tests/test_spatalite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.217.2/threedi_schema.egg-info/PKG-INFO` & `threedi-schema-0.217.3/threedi_schema.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.217.2
+Version: 0.217.3
 Summary: The schema of 3Di schematization files
 Home-page: https://github.com/nens/threedi-schema
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
@@ -81,14 +81,20 @@
 
   $ pip install threedi-schema
 
 
 Changelog of threedi-schema
 ===================================================
 
+0.217.3 (2023-06-12)
+--------------------
+
+- Added groundwater 1D2D columns to the views.
+
+
 0.217.2 (2023-05-24)
 --------------------
 
 - Remove vegetation and groundwater settings from beta features, since they are going to be released.
 
 
 0.217.1 (2023-05-17)
```

### Comparing `threedi-schema-0.217.2/threedi_schema.egg-info/SOURCES.txt` & `threedi-schema-0.217.3/threedi_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

