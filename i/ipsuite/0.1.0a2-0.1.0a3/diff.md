# Comparing `tmp/ipsuite-0.1.0a2.tar.gz` & `tmp/ipsuite-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipsuite-0.1.0a2.tar", max compression
+gzip compressed data, was "ipsuite-0.1.0a3.tar", max compression
```

## Comparing `ipsuite-0.1.0a2.tar` & `ipsuite-0.1.0a3.tar`

### file list

```diff
@@ -1,72 +1,78 @@
--rw-r--r--   0        0        0    14196 2023-03-20 16:34:18.597957 ipsuite-0.1.0a2/LICENSE
--rw-r--r--   0        0        0      867 2023-04-05 16:53:50.509938 ipsuite-0.1.0a2/README.md
--rw-r--r--   0        0        0      831 2023-04-09 19:55:33.180932 ipsuite-0.1.0a2/ipsuite/__init__.py
--rw-r--r--   0        0        0      986 2023-04-09 19:55:33.180932 ipsuite-0.1.0a2/ipsuite/analysis/__init__.py
--rw-r--r--   0        0        0     3809 2023-04-03 18:16:54.429558 ipsuite-0.1.0a2/ipsuite/analysis/bin_property.py
--rw-r--r--   0        0        0     3545 2023-03-10 11:03:12.800439 ipsuite-0.1.0a2/ipsuite/analysis/ensemble.py
--rw-r--r--   0        0        0      591 2023-04-09 19:55:33.180932 ipsuite-0.1.0a2/ipsuite/analysis/model/__init__.py
--rw-r--r--   0        0        0    13749 2023-04-09 20:31:23.917265 ipsuite-0.1.0a2/ipsuite/analysis/model/dynamics.py
--rw-r--r--   0        0        0     2334 2023-04-09 19:46:26.426933 ipsuite-0.1.0a2/ipsuite/analysis/model/dynamics_checks.py
--rw-r--r--   0        0        0     1888 2023-04-09 19:55:33.180932 ipsuite-0.1.0a2/ipsuite/analysis/model/math.py
--rw-r--r--   0        0        0     2535 2023-04-09 19:55:33.180932 ipsuite-0.1.0a2/ipsuite/analysis/model/plots.py
--rw-r--r--   0        0        0    11562 2023-04-09 20:31:23.917265 ipsuite-0.1.0a2/ipsuite/analysis/model/predict.py
--rw-r--r--   0        0        0     4900 2023-03-17 08:06:55.975052 ipsuite-0.1.0a2/ipsuite/analysis/sensitivity.py
--rw-r--r--   0        0        0      388 2023-04-08 17:35:11.105019 ipsuite-0.1.0a2/ipsuite/base/__init__.py
--rw-r--r--   0        0        0     6308 2023-04-05 16:53:50.519938 ipsuite-0.1.0a2/ipsuite/base/base.py
--rw-r--r--   0        0        0      971 2023-03-10 10:05:15.098799 ipsuite-0.1.0a2/ipsuite/base/protocol.py
--rw-r--r--   0        0        0      185 2023-04-03 18:16:54.439558 ipsuite-0.1.0a2/ipsuite/bootstrap/__init__.py
--rw-r--r--   0        0        0     4531 2023-04-03 18:16:54.439558 ipsuite-0.1.0a2/ipsuite/bootstrap/random_displacements.py
--rw-r--r--   0        0        0      430 2023-04-03 18:16:54.439558 ipsuite-0.1.0a2/ipsuite/calculators/__init__.py
--rw-r--r--   0        0        0      945 2023-04-10 20:57:04.627214 ipsuite-0.1.0a2/ipsuite/calculators/ase_geoopt.py
--rw-r--r--   0        0        0     6118 2023-04-09 20:31:23.927265 ipsuite-0.1.0a2/ipsuite/calculators/ase_md.py
--rw-r--r--   0        0        0     6518 2023-04-10 20:42:13.716982 ipsuite-0.1.0a2/ipsuite/calculators/cp2k.py
--rw-r--r--   0        0        0      738 2023-04-03 18:16:54.449558 ipsuite-0.1.0a2/ipsuite/calculators/lj.py
--rw-r--r--   0        0        0      942 2023-04-09 19:54:07.201876 ipsuite-0.1.0a2/ipsuite/calculators/xtb.py
--rw-r--r--   0        0        0     2328 2023-03-17 08:00:52.668953 ipsuite-0.1.0a2/ipsuite/configuration_comparison/MMKernel.py
--rw-r--r--   0        0        0     2267 2023-03-08 18:22:08.931925 ipsuite-0.1.0a2/ipsuite/configuration_comparison/REMatch.py
--rw-r--r--   0        0        0      136 2023-04-09 19:55:33.180932 ipsuite-0.1.0a2/ipsuite/configuration_comparison/__init__.py
--rw-r--r--   0        0        0      164 2023-04-09 19:55:33.180932 ipsuite-0.1.0a2/ipsuite/configuration_comparison/__init__.pyi
--rw-r--r--   0        0        0    11723 2023-03-17 08:00:52.668953 ipsuite-0.1.0a2/ipsuite/configuration_comparison/base.py
--rw-r--r--   0        0        0      161 2023-04-09 19:55:33.190932 ipsuite-0.1.0a2/ipsuite/configuration_generation/__init__.py
--rw-r--r--   0        0        0      177 2023-04-09 19:55:33.190932 ipsuite-0.1.0a2/ipsuite/configuration_generation/__init__.pyi
--rw-r--r--   0        0        0     1610 2023-04-10 20:11:13.807324 ipsuite-0.1.0a2/ipsuite/configuration_generation/packmol.py
--rw-r--r--   0        0        0     1110 2023-04-09 19:55:33.190932 ipsuite-0.1.0a2/ipsuite/configuration_generation/smiles_to_atoms.py
--rw-r--r--   0        0        0      859 2023-04-05 10:26:28.603373 ipsuite-0.1.0a2/ipsuite/configuration_selection/__init__.py
--rw-r--r--   0        0        0     4171 2023-04-05 08:34:02.197584 ipsuite-0.1.0a2/ipsuite/configuration_selection/base.py
--rw-r--r--   0        0        0      621 2023-04-05 08:34:02.207584 ipsuite-0.1.0a2/ipsuite/configuration_selection/index.py
--rw-r--r--   0        0        0     5161 2023-04-05 08:34:02.207584 ipsuite-0.1.0a2/ipsuite/configuration_selection/kernel.py
--rw-r--r--   0        0        0      609 2023-03-17 08:00:52.678953 ipsuite-0.1.0a2/ipsuite/configuration_selection/random.py
--rw-r--r--   0        0        0      603 2023-04-05 10:26:28.603373 ipsuite-0.1.0a2/ipsuite/configuration_selection/split.py
--rw-r--r--   0        0        0      942 2023-03-17 08:00:52.678953 ipsuite-0.1.0a2/ipsuite/configuration_selection/uniform_arange.py
--rw-r--r--   0        0        0     1443 2023-03-17 08:00:52.678953 ipsuite-0.1.0a2/ipsuite/configuration_selection/uniform_energetic.py
--rw-r--r--   0        0        0      602 2023-03-17 08:00:52.678953 ipsuite-0.1.0a2/ipsuite/configuration_selection/uniform_temporal.py
--rw-r--r--   0        0        0      186 2023-04-03 18:16:54.459557 ipsuite-0.1.0a2/ipsuite/data_loading/__init__.py
--rw-r--r--   0        0        0     2614 2023-03-16 20:32:58.182623 ipsuite-0.1.0a2/ipsuite/data_loading/add_data_ase.py
--rw-r--r--   0        0        0      517 2023-04-03 18:16:54.459557 ipsuite-0.1.0a2/ipsuite/data_loading/add_data_h5md.py
--rw-r--r--   0        0        0      103 2023-03-21 18:17:21.212138 ipsuite-0.1.0a2/ipsuite/fields/__init__.py
--rw-r--r--   0        0        0     1711 2023-04-03 18:16:54.459557 ipsuite-0.1.0a2/ipsuite/fields/atoms.py
--rw-r--r--   0        0        0       88 2023-03-22 18:15:23.427142 ipsuite-0.1.0a2/ipsuite/geometry/__init__.py
--rw-r--r--   0        0        0      924 2023-03-22 18:15:23.447142 ipsuite-0.1.0a2/ipsuite/geometry/barycenter_coarse_grain.py
--rw-r--r--   0        0        0      918 2023-03-22 18:15:23.447142 ipsuite-0.1.0a2/ipsuite/geometry/graphs.py
--rw-r--r--   0        0        0      956 2023-03-22 18:15:23.447142 ipsuite-0.1.0a2/ipsuite/geometry/mapping.py
--rw-r--r--   0        0        0     2141 2023-04-03 18:16:54.469557 ipsuite-0.1.0a2/ipsuite/geometry/unwrap.py
--rw-r--r--   0        0        0       97 2023-04-09 19:55:33.190932 ipsuite-0.1.0a2/ipsuite/models/__init__.py
--rw-r--r--   0        0        0      230 2023-04-09 19:55:33.190932 ipsuite-0.1.0a2/ipsuite/models/__init__.pyi
--rw-r--r--   0        0        0     3701 2023-03-10 11:03:12.780439 ipsuite-0.1.0a2/ipsuite/models/base.py
--rw-r--r--   0        0        0     2711 2023-03-17 08:06:55.995052 ipsuite-0.1.0a2/ipsuite/models/ensemble.py
--rw-r--r--   0        0        0    11709 2023-04-08 11:22:40.331464 ipsuite-0.1.0a2/ipsuite/models/gap.py
--rw-r--r--   0        0        0     5833 2023-04-10 20:57:04.637214 ipsuite-0.1.0a2/ipsuite/models/mace_model.py
--rw-r--r--   0        0        0     7315 2023-03-17 08:06:56.005052 ipsuite-0.1.0a2/ipsuite/models/nequip.py
--rw-r--r--   0        0        0      188 2023-04-03 20:55:43.075074 ipsuite-0.1.0a2/ipsuite/project/__init__.py
--rw-r--r--   0        0        0       96 2023-04-10 20:57:04.637214 ipsuite-0.1.0a2/ipsuite/static_data/__init__.py
--rw-r--r--   0        0        0     1608 2023-02-27 14:20:21.714354 ipsuite-0.1.0a2/ipsuite/static_data/gap.jinja2
--rw-r--r--   0        0        0      775 2023-04-10 20:57:04.637214 ipsuite-0.1.0a2/ipsuite/static_data/y_log.json
--rw-r--r--   0        0        0      155 2023-04-05 16:53:50.539938 ipsuite-0.1.0a2/ipsuite/utils/__init__.py
--rw-r--r--   0        0        0     1278 2023-04-09 20:31:23.927265 ipsuite-0.1.0a2/ipsuite/utils/ase_sim.py
--rw-r--r--   0        0        0     6223 2023-04-05 14:50:53.740280 ipsuite-0.1.0a2/ipsuite/utils/combine.py
--rw-r--r--   0        0        0     1447 2023-03-17 08:06:56.005052 ipsuite-0.1.0a2/ipsuite/utils/helpers.py
--rw-r--r--   0        0        0      572 2023-03-09 17:30:00.842723 ipsuite-0.1.0a2/ipsuite/utils/logs.py
--rw-r--r--   0        0        0      691 2023-04-05 16:53:50.539938 ipsuite-0.1.0a2/ipsuite/utils/md.py
--rw-r--r--   0        0        0     2437 2023-04-09 19:46:26.426933 ipsuite-0.1.0a2/ipsuite/utils/metrics.py
--rw-r--r--   0        0        0     2680 2023-04-10 21:04:24.092392 ipsuite-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     2475 1970-01-01 00:00:00.000000 ipsuite-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0    14197 2023-05-30 11:28:15.453762 ipsuite-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0      867 2023-05-30 11:28:15.473762 ipsuite-0.1.0a3/README.md
+-rw-r--r--   0        0        0      882 2023-05-30 12:26:18.215627 ipsuite-0.1.0a3/ipsuite/__init__.py
+-rw-r--r--   0        0        0     1169 2023-06-12 15:35:29.125912 ipsuite-0.1.0a3/ipsuite/analysis/__init__.py
+-rw-r--r--   0        0        0     3811 2023-05-30 11:28:15.493762 ipsuite-0.1.0a3/ipsuite/analysis/bin_property.py
+-rw-r--r--   0        0        0     6108 2023-05-30 11:28:15.513761 ipsuite-0.1.0a3/ipsuite/analysis/bond_stretch.py
+-rw-r--r--   0        0        0     3613 2023-05-30 11:28:48.163402 ipsuite-0.1.0a3/ipsuite/analysis/ensemble.py
+-rw-r--r--   0        0        0      685 2023-06-12 15:35:29.165912 ipsuite-0.1.0a3/ipsuite/analysis/model/__init__.py
+-rw-r--r--   0        0        0    14627 2023-06-12 15:35:29.185911 ipsuite-0.1.0a3/ipsuite/analysis/model/dynamics.py
+-rw-r--r--   0        0        0     6359 2023-06-12 14:17:19.486548 ipsuite-0.1.0a3/ipsuite/analysis/model/dynamics_checks.py
+-rw-r--r--   0        0        0     1888 2023-04-09 19:55:33.180932 ipsuite-0.1.0a3/ipsuite/analysis/model/math.py
+-rw-r--r--   0        0        0     2535 2023-04-09 19:55:33.180932 ipsuite-0.1.0a3/ipsuite/analysis/model/plots.py
+-rw-r--r--   0        0        0    14203 2023-05-30 11:28:15.553761 ipsuite-0.1.0a3/ipsuite/analysis/model/predict.py
+-rw-r--r--   0        0        0     4926 2023-05-30 12:26:18.215627 ipsuite-0.1.0a3/ipsuite/analysis/sensitivity.py
+-rw-r--r--   0        0        0      416 2023-05-30 12:26:18.215627 ipsuite-0.1.0a3/ipsuite/base/__init__.py
+-rw-r--r--   0        0        0     7070 2023-06-12 14:29:17.148738 ipsuite-0.1.0a3/ipsuite/base/base.py
+-rw-r--r--   0        0        0      971 2023-03-10 10:05:15.098799 ipsuite-0.1.0a3/ipsuite/base/protocol.py
+-rw-r--r--   0        0        0      185 2023-04-14 13:21:38.223441 ipsuite-0.1.0a3/ipsuite/bootstrap/__init__.py
+-rw-r--r--   0        0        0     4533 2023-05-30 11:28:15.563761 ipsuite-0.1.0a3/ipsuite/bootstrap/random_displacements.py
+-rw-r--r--   0        0        0       97 2023-05-30 11:28:15.573761 ipsuite-0.1.0a3/ipsuite/calculators/__init__.py
+-rw-r--r--   0        0        0      608 2023-06-02 12:33:22.945869 ipsuite-0.1.0a3/ipsuite/calculators/__init__.pyi
+-rw-r--r--   0        0        0     3156 2023-06-12 14:29:17.148738 ipsuite-0.1.0a3/ipsuite/calculators/apax_jax_md.py
+-rw-r--r--   0        0        0     1406 2023-06-12 14:29:17.148738 ipsuite-0.1.0a3/ipsuite/calculators/ase_geoopt.py
+-rw-r--r--   0        0        0     9613 2023-06-02 12:33:22.945869 ipsuite-0.1.0a3/ipsuite/calculators/ase_md.py
+-rw-r--r--   0        0        0     1343 2023-06-02 12:33:22.945869 ipsuite-0.1.0a3/ipsuite/calculators/ase_standard.py
+-rw-r--r--   0        0        0     8021 2023-05-30 11:28:15.633760 ipsuite-0.1.0a3/ipsuite/calculators/cp2k.py
+-rw-r--r--   0        0        0     1059 2023-05-30 11:28:15.673760 ipsuite-0.1.0a3/ipsuite/calculators/xtb.py
+-rw-r--r--   0        0        0     2328 2023-03-17 08:00:52.668953 ipsuite-0.1.0a3/ipsuite/configuration_comparison/MMKernel.py
+-rw-r--r--   0        0        0     2267 2023-03-08 18:22:08.931925 ipsuite-0.1.0a3/ipsuite/configuration_comparison/REMatch.py
+-rw-r--r--   0        0        0      136 2023-04-11 15:30:14.938963 ipsuite-0.1.0a3/ipsuite/configuration_comparison/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-11 15:30:14.938963 ipsuite-0.1.0a3/ipsuite/configuration_comparison/__init__.pyi
+-rw-r--r--   0        0        0    11581 2023-06-12 14:17:19.556547 ipsuite-0.1.0a3/ipsuite/configuration_comparison/base.py
+-rw-r--r--   0        0        0      161 2023-04-11 15:30:14.938963 ipsuite-0.1.0a3/ipsuite/configuration_generation/__init__.py
+-rw-r--r--   0        0        0      177 2023-04-11 15:30:14.938963 ipsuite-0.1.0a3/ipsuite/configuration_generation/__init__.pyi
+-rw-r--r--   0        0        0     3616 2023-06-01 08:44:58.894032 ipsuite-0.1.0a3/ipsuite/configuration_generation/packmol.py
+-rw-r--r--   0        0        0     1281 2023-05-30 12:26:18.225627 ipsuite-0.1.0a3/ipsuite/configuration_generation/smiles_to_atoms.py
+-rw-r--r--   0        0        0      958 2023-05-30 11:28:15.683760 ipsuite-0.1.0a3/ipsuite/configuration_selection/__init__.py
+-rw-r--r--   0        0        0     5111 2023-05-30 11:28:15.693759 ipsuite-0.1.0a3/ipsuite/configuration_selection/base.py
+-rw-r--r--   0        0        0      621 2023-04-05 08:34:02.207584 ipsuite-0.1.0a3/ipsuite/configuration_selection/index.py
+-rw-r--r--   0        0        0     5209 2023-05-30 11:28:15.693759 ipsuite-0.1.0a3/ipsuite/configuration_selection/kernel.py
+-rw-r--r--   0        0        0      609 2023-03-17 08:00:52.678953 ipsuite-0.1.0a3/ipsuite/configuration_selection/random.py
+-rw-r--r--   0        0        0      603 2023-04-05 10:26:28.603373 ipsuite-0.1.0a3/ipsuite/configuration_selection/split.py
+-rw-r--r--   0        0        0     4108 2023-06-01 12:24:56.989159 ipsuite-0.1.0a3/ipsuite/configuration_selection/threshold.py
+-rw-r--r--   0        0        0      945 2023-05-30 11:28:15.723759 ipsuite-0.1.0a3/ipsuite/configuration_selection/uniform_arange.py
+-rw-r--r--   0        0        0     1443 2023-03-17 08:00:52.678953 ipsuite-0.1.0a3/ipsuite/configuration_selection/uniform_energetic.py
+-rw-r--r--   0        0        0      602 2023-03-17 08:00:52.678953 ipsuite-0.1.0a3/ipsuite/configuration_selection/uniform_temporal.py
+-rw-r--r--   0        0        0      186 2023-04-03 18:16:54.459557 ipsuite-0.1.0a3/ipsuite/data_loading/__init__.py
+-rw-r--r--   0        0        0     2620 2023-05-30 12:26:18.225627 ipsuite-0.1.0a3/ipsuite/data_loading/add_data_ase.py
+-rw-r--r--   0        0        0      543 2023-05-30 12:26:18.225627 ipsuite-0.1.0a3/ipsuite/data_loading/add_data_h5md.py
+-rw-r--r--   0        0        0      103 2023-03-21 18:17:21.212138 ipsuite-0.1.0a3/ipsuite/fields/__init__.py
+-rw-r--r--   0        0        0     1711 2023-04-03 18:16:54.459557 ipsuite-0.1.0a3/ipsuite/fields/atoms.py
+-rw-r--r--   0        0        0       88 2023-03-22 18:15:23.427142 ipsuite-0.1.0a3/ipsuite/geometry/__init__.py
+-rw-r--r--   0        0        0      924 2023-03-22 18:15:23.447142 ipsuite-0.1.0a3/ipsuite/geometry/barycenter_coarse_grain.py
+-rw-r--r--   0        0        0     1236 2023-05-30 11:28:15.733759 ipsuite-0.1.0a3/ipsuite/geometry/graphs.py
+-rw-r--r--   0        0        0      956 2023-03-22 18:15:23.447142 ipsuite-0.1.0a3/ipsuite/geometry/mapping.py
+-rw-r--r--   0        0        0     2142 2023-05-30 11:28:15.743759 ipsuite-0.1.0a3/ipsuite/geometry/unwrap.py
+-rw-r--r--   0        0        0       97 2023-04-11 15:30:14.938963 ipsuite-0.1.0a3/ipsuite/models/__init__.py
+-rw-r--r--   0        0        0      235 2023-05-30 11:28:15.753759 ipsuite-0.1.0a3/ipsuite/models/__init__.pyi
+-rw-r--r--   0        0        0     4368 2023-06-12 08:03:57.512767 ipsuite-0.1.0a3/ipsuite/models/apax.py
+-rw-r--r--   0        0        0     2606 2023-05-30 11:28:15.773759 ipsuite-0.1.0a3/ipsuite/models/base.py
+-rw-r--r--   0        0        0     2684 2023-05-30 12:26:18.225627 ipsuite-0.1.0a3/ipsuite/models/ensemble.py
+-rw-r--r--   0        0        0    10462 2023-06-12 14:17:19.616546 ipsuite-0.1.0a3/ipsuite/models/gap.py
+-rw-r--r--   0        0        0     4446 2023-06-12 14:17:19.636546 ipsuite-0.1.0a3/ipsuite/models/mace_model.py
+-rw-r--r--   0        0        0     6596 2023-05-30 11:28:15.823758 ipsuite-0.1.0a3/ipsuite/models/nequip.py
+-rw-r--r--   0        0        0     4234 2023-06-12 15:35:29.255910 ipsuite-0.1.0a3/ipsuite/nodes.py
+-rw-r--r--   0        0        0      188 2023-04-03 20:55:43.075074 ipsuite-0.1.0a3/ipsuite/project/__init__.py
+-rw-r--r--   0        0        0       96 2023-04-11 15:30:14.948963 ipsuite-0.1.0a3/ipsuite/static_data/__init__.py
+-rw-r--r--   0        0        0     1609 2023-05-30 11:28:15.843758 ipsuite-0.1.0a3/ipsuite/static_data/gap.jinja2
+-rw-r--r--   0        0        0     2046 2023-06-12 08:03:57.512767 ipsuite-0.1.0a3/ipsuite/static_data/y_log.json
+-rw-r--r--   0        0        0      155 2023-04-05 16:53:50.539938 ipsuite-0.1.0a3/ipsuite/utils/__init__.py
+-rw-r--r--   0        0        0     1337 2023-04-13 20:08:01.697728 ipsuite-0.1.0a3/ipsuite/utils/ase_sim.py
+-rw-r--r--   0        0        0     6250 2023-05-30 11:28:15.903757 ipsuite-0.1.0a3/ipsuite/utils/combine.py
+-rw-r--r--   0        0        0     1717 2023-05-30 11:28:15.923757 ipsuite-0.1.0a3/ipsuite/utils/helpers.py
+-rw-r--r--   0        0        0      572 2023-03-09 17:30:00.842723 ipsuite-0.1.0a3/ipsuite/utils/logs.py
+-rw-r--r--   0        0        0      691 2023-04-05 16:53:50.539938 ipsuite-0.1.0a3/ipsuite/utils/md.py
+-rw-r--r--   0        0        0     2437 2023-04-09 19:46:26.426933 ipsuite-0.1.0a3/ipsuite/utils/metrics.py
+-rw-r--r--   0        0        0     2817 2023-06-12 15:37:23.474680 ipsuite-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     2475 1970-01-01 00:00:00.000000 ipsuite-0.1.0a3/PKG-INFO
```

### Comparing `ipsuite-0.1.0a2/LICENSE` & `ipsuite-0.1.0a3/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -270,8 +270,8 @@
   is not sufficient to license the Source Code under Secondary Licenses.
 
   If it is not possible or desirable to put the notice in a particular
   file, then You may include the notice in a location (such as a LICENSE
   file in a relevant directory) where a recipient would be likely to
   look for such a notice.
 
-  You may add additional accurate notices of copyright ownership.
+  You may add additional accurate notices of copyright ownership.
```

### Comparing `ipsuite-0.1.0a2/README.md` & `ipsuite-0.1.0a3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 [![ZnTrack](https://img.shields.io/badge/Powered%20by-ZnTrack-%23007CB0)](https://zntrack.readthedocs.io/en/latest/)
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 
 # IPS - The Inter Atomic Potential Suite
 
 IPS provides you with tools to generate Machine Learned Interatomic Potentials.
 
-Install the package to get started or check out an interactive notebook [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/IPSuite/HEAD) 
+Install the package to get started or check out an interactive notebook
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/IPSuite/HEAD)
+
 ```python
 pip install ipsuite
 ```
 
 Examples can be found at:
+
 - https://dagshub.com/PythonFZ/IPS-Examples/src/intro/main.ipynb
 - https://dagshub.com/PythonFZ/IPS-Examples/src/graph/main.ipynb
-- https://dagshub.com/PythonFZ/IPS-Examples/src/modifiy_graph/main.ipynb
+- https://dagshub.com/PythonFZ/IPS-Examples/src/modify_graph/main.ipynb
```

### Comparing `ipsuite-0.1.0a2/ipsuite/__init__.py` & `ipsuite-0.1.0a3/ipsuite/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     configuration_comparison,
     configuration_generation,
     configuration_selection,
     data_loading,
     fields,
     geometry,
     models,
+    nodes,
     utils,
 )
 from ipsuite.data_loading.add_data_ase import AddData
 from ipsuite.project import Project
 from ipsuite.utils import combine
 from ipsuite.utils.logs import setup_logging
 
@@ -32,11 +33,14 @@
     "models",
     "analysis",
     "fields",
     "calculators",
     "geometry",
     "combine",
     "data_loading",
+    "nodes",
 ]
 
 __version__ = importlib.metadata.version(__name__)
 setup_logging(__name__)
+
+utils.helpers.setup_ase()
```

### Comparing `ipsuite-0.1.0a2/ipsuite/analysis/__init__.py` & `ipsuite-0.1.0a3/ipsuite/analysis/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 from ipsuite.analysis.bin_property import (
     DipoleHistogram,
     EnergyHistogram,
     ForcesHistogram,
 )
+from ipsuite.analysis.bond_stretch import BondStretchAnalyses
 from ipsuite.analysis.ensemble import ModelEnsembleAnalysis
 from ipsuite.analysis.model import (
     BoxHeatUp,
     BoxScale,
     ConnectivityCheck,
     EnergySpikeCheck,
     ForceAngles,
     ForceDecomposition,
     MDStability,
     NaNCheck,
     Prediction,
     PredictionMetrics,
-    RattleAtoms,
+    RattleAnalysis,
+    TemperatureCheck,
+    ThresholdCheck,
 )
 from ipsuite.analysis.sensitivity import (
     AnalyseGlobalForceSensitivity,
     AnalyseSingleForceSensitivity,
     MoveSingleParticle,
 )
 
 __all__ = [
     "EnergyHistogram",
     "ForcesHistogram",
     "DipoleHistogram",
     "ModelEnsembleAnalysis",
     "PredictionMetrics",
     "ForceAngles",
-    "RattleAtoms",
+    "RattleAnalysis",
     "Prediction",
     "BoxScale",
     "BoxHeatUp",
     "NaNCheck",
+    "TemperatureCheck",
     "ConnectivityCheck",
     "EnergySpikeCheck",
     "MDStability",
     "MoveSingleParticle",
     "AnalyseGlobalForceSensitivity",
     "AnalyseSingleForceSensitivity",
     "ForceDecomposition",
+    "ThresholdCheck",
+    "BondStretchAnalyses",
 ]
```

### Comparing `ipsuite-0.1.0a2/ipsuite/analysis/bin_property.py` & `ipsuite-0.1.0a3/ipsuite/analysis/bin_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """Creates a Matplotlib figure based on precomputed bin edges and counts.
 
     Parameters
     ----------
     bin_edges: np.array
         Edges of the histogram bins.
     counts: np.array
-        Number of occurences in each bin.
+        Number of occurrences in each bin.
     datalabel: str
         Labels for the figure legend.
     xlabel: str
         X-axis label.
     ylabel: str
         Y-axis label.
     figsize: tuple
@@ -61,15 +61,15 @@
     """
 
     bins: int = zntrack.zn.params(None)
     plots_dir: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "plots")
     labels_df: pd.DataFrame = zntrack.zn.plots()
     datalabel: str = None
     xlabel: str = None
-    ylabel: str = "Occurences"
+    ylabel: str = "Occurrences"
     logy_scale: bool = True
 
     def _post_init_(self):
         """Load metrics - if available."""
         self.data = get_deps_if_node(self.data, "atoms")
 
     def get_labels(self):
```

### Comparing `ipsuite-0.1.0a2/ipsuite/analysis/ensemble.py` & `ipsuite-0.1.0a3/ipsuite/analysis/ensemble.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,103 @@
 import typing
 
 import ase.calculators.singlepoint
 import matplotlib.pyplot as plt
 import numpy as np
 import zntrack
 
-from ipsuite import utils
+from ipsuite import base, utils
 
 
 def plot_with_uncertainty(value, ylabel: str, xlabel: str, **kwargs) -> dict:
     """Parameters
     ----------
     value: data of shape (n, m) where n is the number of ensembles.
 
     Returns
     -------
 
     """
-    data = {
-        "mean": np.mean(value, axis=0),
-        "std": np.std(value, axis=0),
-        "max": np.max(value, axis=0),
-        "min": np.min(value, axis=0),
-    }
+    if isinstance(value, dict):
+        data = value
+    else:
+        data = {
+            "mean": np.mean(value, axis=0),
+            "std": np.std(value, axis=0),
+            "max": np.max(value, axis=0),
+            "min": np.min(value, axis=0),
+        }
 
     fig, ax = plt.subplots(**kwargs)
     ax.fill_between(
         np.arange(len(data["mean"])),
         data["mean"] + data["std"],
         data["mean"] - data["std"],
         facecolor="lightblue",
     )
-    ax.plot(data["max"], linestyle="--", color="darkcyan")
-    ax.plot(data["min"], linestyle="--", color="darkcyan")
+    if "max" in data:
+        ax.plot(data["max"], linestyle="--", color="darkcyan")
+    if "min" in data:
+        ax.plot(data["min"], linestyle="--", color="darkcyan")
     ax.plot(data["mean"], color="black")
     ax.set_ylabel(ylabel)
     ax.set_xlabel(xlabel)
 
-    return fig, data
+    return fig, ax, data
 
 
-class ModelEnsembleAnalysis(zntrack.Node):
+class ModelEnsembleAnalysis(base.AnalyseAtoms):
     """Attributes
     ----------
         models: list of models to ensemble
         data: list of ASE Atoms objects to evaluate against.
     """
 
     models: list = zntrack.zn.deps()
-    atoms: list = zntrack.zn.deps()
 
     normal_plot_path = zntrack.dvc.outs(zntrack.nwd / "normal_plot.png")
     sorted_plot_path = zntrack.dvc.outs(zntrack.nwd / "sorted_plot.png")
     histogram = zntrack.dvc.outs(zntrack.nwd / "histogram.png")
 
     prediction_list = zntrack.zn.outs()
     predictions: typing.List[ase.Atoms] = zntrack.zn.outs()
 
     bins: int = zntrack.zn.params(100)
 
     def _post_init_(self):
-        self.atoms = utils.helpers.get_deps_if_node(self.atoms, "atoms")
+        self.data = utils.helpers.get_deps_if_node(self.data, "atoms")
 
     def run(self):
         # TODO axis labels
         # TODO save indices
         # TODo rewrite this Node based on MLModel and then add a Analysis Node
-        self.prediction_list = [model.predict(self.atoms[:]) for model in self.models]
+        self.prediction_list = [model.predict(self.data[:]) for model in self.models]
 
         self.predictions = []
-        for idx, atom in enumerate(self.atoms):
+        for idx, atom in enumerate(self.data):
             atom.calc = ase.calculators.singlepoint.SinglePointCalculator(
                 atoms=atom,
-                energy=np.mean([p.energy[idx] for p in self.prediction_list]),
-                forces=np.mean([p.forces[idx] for p in self.prediction_list], axis=0),
+                energy=np.mean(
+                    [p[idx].get_potential_energy() for p in self.prediction_list]
+                ),
+                forces=np.mean(
+                    [p[idx].get_forces() for p in self.prediction_list], axis=0
+                ),
             )
             self.predictions.append(atom)
 
         figures = self.get_plots()
         figures[0][0].savefig(self.normal_plot_path)
         figures[1][0].savefig(self.sorted_plot_path)
         figures[2].savefig(self.histogram)
 
-    def calc(self):
-        # Ensemble could inherit from MLModel
-        raise NotImplementedError
-
     def get_plots(self):
-        energy = np.stack([p.energy for p in self.prediction_list])
+        energy = np.stack(
+            [np.stack(x.get_potential_energy() for x in p) for p in self.prediction_list]
+        )
 
         figures = []
         # Plot the energy
         figures.append(
             plot_with_uncertainty(
                 energy, figsize=(10, 5), xlabel="data point", ylabel="Energy / a.u."
             )
@@ -107,11 +113,7 @@
 
         # Plot the histogram
         fig, ax = plt.subplots(figsize=(10, 5))
         ax.hist(np.std(energy, axis=0), bins=self.bins)
         ax.set_xlabel("Energy standard deviation histogram")
         figures.append(fig)
         return figures
-
-    def predict(self, data):
-        # TODO create prediction object with uncertainties
-        pass
```

### Comparing `ipsuite-0.1.0a2/ipsuite/analysis/model/dynamics.py` & `ipsuite-0.1.0a3/ipsuite/analysis/model/dynamics.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from ipsuite.analysis.bin_property import get_histogram_figure
 from ipsuite.utils.ase_sim import freeze_copy_atoms
 from ipsuite.utils.md import get_energy_terms
 
 log = logging.getLogger(__name__)
 
 
-class RattleAtoms(base.ProcessSingleAtom):
+class RattleAnalysis(base.ProcessSingleAtom):
     """Move particles with a given stdev from a starting configuration and predict.
 
     Attributes
     ----------
     model: The MLModel node that implements the 'predict' method
     atoms: list[Atoms] to predict properties for
     logspace: bool, default=True
@@ -41,14 +41,15 @@
     factor: float, default = 0.001
         The 'np.linspace(0.0, stop, num) * factor'
     atom_id: int, default = 0
         The atom to pick from self.atoms as a starting point
     """
 
     model: models.MLModel = zntrack.zn.deps()
+    model_outs = zntrack.dvc.outs(zntrack.nwd / "model/")
 
     logspace: bool = zntrack.zn.params(True)
     stop: float = zntrack.zn.params(3.0)
     factor: float = zntrack.zn.params(0.001)
     num: int = zntrack.zn.params(100)
 
     seed: int = zntrack.zn.params(1234)
@@ -59,26 +60,29 @@
         # y_label="predicted energy",
     )
 
     def post_init(self):
         self.data = utils.helpers.get_deps_if_node(self.data, "atoms")
 
     def run(self):
+        self.model_outs.mkdir(parents=True, exist_ok=True)
+        (self.model_outs / "outs.txt").write_text("Lorem Ipsum")
+
         if self.logspace:
             stdev_space = (
                 np.logspace(start=0.0, stop=self.stop, num=self.num) * self.factor
             )
         else:
             stdev_space = (
                 np.linspace(start=0.0, stop=self.stop, num=self.num) * self.factor
             )
 
         atoms = self.get_data()
         reference = atoms.copy()
-        atoms.calc = self.model.calc
+        atoms.calc = self.model.get_calculator(directory=self.model_outs)
 
         energies = []
 
         self.atoms = []
 
         for stdev in tqdm.tqdm(stdev_space, ncols=70):
             atoms.positions = reference.positions
@@ -101,14 +105,15 @@
     stop: float, default = 1.0
         The stop value for the generated space of stdev points
     num: int, default = 100
         The size of the generated space of stdev points
     """
 
     model: models.MLModel = zntrack.zn.deps()
+    model_outs = zntrack.dvc.outs(zntrack.nwd / "model")
     mapping: base.Mapping = zntrack.zn.nodes(None)
 
     stop: float = zntrack.zn.params(2.0)
     num: int = zntrack.zn.params(100)
     start: float = zntrack.zn.params(1)
 
     plot = zntrack.dvc.outs(zntrack.nwd / "energy.png")
@@ -120,19 +125,21 @@
         # y_label="predicted energy",
     )
 
     def _post_init_(self):
         self.data = utils.helpers.get_deps_if_node(self.data, "atoms")
 
     def run(self):
+        self.model_outs.mkdir(parents=True, exist_ok=True)
+        (self.model_outs / "outs.txt").write_text("Lorem Ipsum")
         scale_space = np.linspace(start=self.start, stop=self.stop, num=self.num)
 
         original_atoms = self.get_data()
         cell = original_atoms.copy().cell
-        original_atoms.calc = self.model.calc
+        original_atoms.calc = self.model.get_calculator(directory=self.model_outs)
 
         energies = []
         self.atoms = []
         if self.mapping is None:
             scaling_atoms = original_atoms
         else:
             scaling_atoms, molecules = self.mapping.forward_mapping(original_atoms)
@@ -141,15 +148,15 @@
             scaling_atoms.set_cell(cell=cell * scale, scale_atoms=True)
 
             if self.mapping is None:
                 eval_atoms = scaling_atoms
             else:
                 eval_atoms = self.mapping.backward_mapping(scaling_atoms, molecules)
                 # New atoms object, does not have the calculator.
-                eval_atoms.calc = self.model.calc
+                eval_atoms.calc = original_atoms.calc
 
             energies.append(eval_atoms.get_potential_energy())
             self.atoms.append(freeze_copy_atoms(eval_atoms))
 
         self.energies = pd.DataFrame({"y": energies, "x": scale_space})
 
         fig, ax = plt.subplots()
@@ -183,14 +190,15 @@
     repeat = zntrack.zn.params((1, 1, 1))
 
     max_temperature: float = zntrack.zn.params(None)
 
     flux_data = zntrack.zn.plots()
 
     model = zntrack.zn.deps()
+    model_outs = zntrack.dvc.outs(zntrack.nwd / "model")
 
     plots = zntrack.dvc.outs(zntrack.nwd / "temperature.png")
 
     def get_atoms(self) -> ase.Atoms:
         atoms: ase.Atoms = self.get_data()
         return atoms.repeat(self.repeat)
 
@@ -205,18 +213,20 @@
         )
         ax.set_ylim(self.start_temperature, self.stop_temperature)
         ax.set_xlabel(r"Target temperature $t_\mathrm{target}$ / K")
         ax.set_ylabel(r"Measured temperature $t_\mathrm{exp}$ / K")
         fig.savefig(self.plots)
 
     def run(self):
+        self.model_outs.mkdir(parents=True, exist_ok=True)
+        (self.model_outs / "outs.txt").write_text("Lorem Ipsum")
         if self.max_temperature is None:
             self.max_temperature = self.stop_temperature * 1.5
         atoms = self.get_atoms()
-        atoms.set_calculator(self.model.calc)
+        atoms.calc = self.model.get_calculator(directory=self.model_outs)
         # Initialize velocities
         MaxwellBoltzmannDistribution(atoms, temperature_K=self.start_temperature)
         # initialize thermostat
         thermostat = Langevin(
             atoms,
             timestep=self.time_step * units.fs,
             temperature_K=self.start_temperature,
@@ -336,14 +346,15 @@
     distribution.
     save_last_n: how many configurations before the instability should be saved
     bins: number of bins in the histogram
     seed: seed for the MaxwellBoltzmann distribution
     """
 
     model = zntrack.zn.deps()
+    model_outs = zntrack.dvc.outs(zntrack.nwd / "model_outs")
     max_steps: int = zntrack.zn.params()
     checks: list[zntrack.Node] = zntrack.zn.nodes()
     time_step: float = zntrack.zn.params(0.5)
     initial_temperature: float = zntrack.zn.params(300)
     save_last_n: int = zntrack.zn.params(1)
     bins: int = zntrack.zn.params(None)
     seed: int = zntrack.zn.params(0)
@@ -365,21 +376,23 @@
         self.plots_dir.mkdir()
 
         label_hist = get_histogram_figure(
             bin_edges,
             counts,
             datalabel="NVE",
             xlabel="Number of stable time steps",
-            ylabel="Occurences",
+            ylabel="Occurrences",
         )
         label_hist.savefig(self.plots_dir / "hist.png")
 
     def run(self) -> None:
+        self.model_outs.mkdir(parents=True, exist_ok=True)
+        (self.model_outs / "outs.txt").write_text("Lorem Ipsum")
         data_lst = self.get_data()
-        calculator = self.model.calc
+        calculator = self.model.get_calculator(directory=self.model_outs)
         rng = default_rng(self.seed)
 
         stable_steps = []
 
         db = znh5md.io.DataWriter(self.traj_file)
         db.initialize_database_groups()
         unstable_atoms = []
```

### Comparing `ipsuite-0.1.0a2/ipsuite/analysis/model/math.py` & `ipsuite-0.1.0a3/ipsuite/analysis/model/math.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/analysis/model/plots.py` & `ipsuite-0.1.0a3/ipsuite/analysis/model/plots.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/analysis/model/predict.py` & `ipsuite-0.1.0a3/ipsuite/analysis/model/predict.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     predictions: list[Atoms] the atoms that have the predicted properties from model
     """
 
     model: models.MLModel = zntrack.zn.deps()
 
     def run(self):
         self.atoms = []
-        calc = self.model.calc
+        calc = self.model.get_calculator()
         for configuration in tqdm.tqdm(self.get_data(), ncols=70):
             configuration: ase.Atoms
             # Run calculation
             atoms = configuration.copy()
             atoms.calc = calc
             atoms.get_potential_energy()
 
@@ -43,15 +43,15 @@
 class PredictionMetrics(base.AnalyseProcessAtoms):
     """Analyse the Models Prediction.
 
     This Node computes
     - MAE
     - RMSE
     - L4 Error
-    - Maxium Error
+    - Maximum Error
     """
 
     energy_df_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "energy_df.csv")
     forces_df_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "forces_df.csv")
     stress_df_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "stress_df.csv")
 
     energy: dict = zntrack.zn.metrics()
@@ -226,24 +226,34 @@
 
 class ForceDecomposition(base.AnalyseProcessAtoms):
     """Node for decomposing forces in a system of molecular units into
     translational, rotational and vibrational components.
 
     The implementation follows the method described in
     https://doi.org/10.26434/chemrxiv-2022-l4tb9
+
+
+    Attributes
+    ----------
+    wasserstein_distance: float
+        Compute the wasserstein distance between the distributions of the
+        prediced and true forces for each trans, rot, vib component.
     """
 
     trans_forces: dict = zntrack.zn.metrics()
     rot_forces: dict = zntrack.zn.metrics()
     vib_forces: dict = zntrack.zn.metrics()
+    wasserstein_distance = zntrack.zn.metrics()
 
     rot_force_plt = zntrack.dvc.outs(zntrack.nwd / "rot_force.png")
     trans_force_plt = zntrack.dvc.outs(zntrack.nwd / "trans_force.png")
     vib_force_plt = zntrack.dvc.outs(zntrack.nwd / "vib_force.png")
 
+    histogram_plt = zntrack.dvc.outs(zntrack.nwd / "histogram.png")
+
     def get_plots(self):
         fig = get_figure(
             np.linalg.norm(self.true_forces["trans"], axis=-1),
             np.linalg.norm(self.pred_forces["trans"], axis=-1),
             datalabel="",
             xlabel=r"$ab~initio$ forces / eV$ \cdot \AA^{-1}$",
             ylabel=r"predicted forces / eV$ \cdot \AA^{-1}$",
@@ -279,40 +289,97 @@
             np.array(self.true_forces["rot"]), np.array(self.pred_forces["rot"])
         )
 
         self.vib_forces = utils.metrics.get_full_metrics(
             np.array(self.true_forces["vib"]), np.array(self.pred_forces["vib"])
         )
 
+    def get_histogram(self):
+        import matplotlib.pyplot as plt
+        from scipy.stats import wasserstein_distance
+
+        def get_rel_scalar_prod(main, relative) -> np.ndarray:
+            x = np.einsum("ij,ij->i", main, relative)
+            x /= np.linalg.norm(main, axis=-1)
+            return x
+
+        fig, axes = plt.subplots(4, 3, figsize=(4 * 5, 3 * 3))
+        fig.suptitle(
+            (
+                r"A fraction $\dfrac{\vec{a} \cdot"
+                r" \vec{b}}{\left|\left|\vec{a}\right|\right|_{2}} $ of $\vec{b}$ that"
+                r" contributes to $\vec{a}$"
+            ),
+            fontsize=16,
+        )
+
+        self.wasserstein_distance = {}
+
+        for label, ax_ in zip(self.true_forces.keys(), axes):
+            self.wasserstein_distance[label] = {}
+            for part, ax in zip(["vib", "rot", "trans"], ax_):
+                data = get_rel_scalar_prod(
+                    self.true_forces[label], self.true_forces[part]
+                )
+                true_bins = ax.hist(
+                    data, bins=50, density=True, label=f"true {label} {part}"
+                )
+
+                data = get_rel_scalar_prod(
+                    self.pred_forces[label], self.pred_forces[part]
+                )
+                pred_bins = ax.hist(
+                    data,
+                    bins=true_bins[1],
+                    density=True,
+                    alpha=0.5,
+                    label=f"pred {label} {part}",
+                )
+                ax.legend()
+                self.wasserstein_distance[label][part] = wasserstein_distance(
+                    true_bins[0], pred_bins[0]
+                )
+
+        fig.savefig(self.histogram_plt, bbox_inches="tight")
+
     def run(self):
         true_atoms, pred_atoms = self.get_data()
         mapping = BarycenterMapping(data=None)
+        # TODO make the force_decomposition return full forces
+        # TODO check if you sum the forces they yield the full forces
+        # TODO make mapping a 'zn.nodes' with Mapping(species="BF4")
+        #  maybe allow smiles and enumeration 0, 1, ...
 
-        self.true_forces = {"trans": [], "rot": [], "vib": []}
-        self.pred_forces = {"trans": [], "rot": [], "vib": []}
+        self.true_forces = {"all": [], "trans": [], "rot": [], "vib": []}
+        self.pred_forces = {"all": [], "trans": [], "rot": [], "vib": []}
 
         for atom in tqdm.tqdm(true_atoms):
             atom_trans_forces, atom_rot_forces, atom_vib_forces = force_decomposition(
                 atom, mapping
             )
+            self.true_forces["all"].append(atom.get_forces())
             self.true_forces["trans"].append(atom_trans_forces)
             self.true_forces["rot"].append(atom_rot_forces)
             self.true_forces["vib"].append(atom_vib_forces)
 
+        self.true_forces["all"] = np.concatenate(self.true_forces["all"])
         self.true_forces["trans"] = np.concatenate(self.true_forces["trans"])
         self.true_forces["rot"] = np.concatenate(self.true_forces["rot"])
         self.true_forces["vib"] = np.concatenate(self.true_forces["vib"])
 
         for atom in tqdm.tqdm(pred_atoms):
             atom_trans_forces, atom_rot_forces, atom_vib_forces = force_decomposition(
                 atom, mapping
             )
+            self.pred_forces["all"].append(atom.get_forces())
             self.pred_forces["trans"].append(atom_trans_forces)
             self.pred_forces["rot"].append(atom_rot_forces)
             self.pred_forces["vib"].append(atom_vib_forces)
 
+        self.pred_forces["all"] = np.concatenate(self.pred_forces["all"])
         self.pred_forces["trans"] = np.concatenate(self.pred_forces["trans"])
         self.pred_forces["rot"] = np.concatenate(self.pred_forces["rot"])
         self.pred_forces["vib"] = np.concatenate(self.pred_forces["vib"])
 
         self.get_metrics()
         self.get_plots()
+        self.get_histogram()
```

### Comparing `ipsuite-0.1.0a2/ipsuite/analysis/sensitivity.py` & `ipsuite-0.1.0a3/ipsuite/analysis/sensitivity.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import ase.geometry
 import ase.io
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy
 import zntrack
 
+from ipsuite import base
+
 
 def nonuniform_imshow(ax, x, y, z, aspect=1, cmap=plt.cm.rainbow):
     """Plot a non-uniformly sampled 2D array.
 
     References
     ----------
     adapted from https://stackoverflow.com/a/53780594/10504481
@@ -29,15 +31,15 @@
         cmap=cmap,
         extent=[x.min(), x.max(), y.max(), y.min()],
     )
     # ax.scatter(x, y, marker="x", s=2.5)
     ax.set_aspect(aspect)
 
 
-class MoveSingleParticle(zntrack.Node):
+class MoveSingleParticle(base.IPSNode):
     """Move a single particle in a given direction."""
 
     atoms_list = zntrack.zn.deps()
     atoms_list_id = zntrack.zn.params(0)  # the atoms object in the atoms list
     atom_id = zntrack.zn.params(0)  # the atom id to move
     scale = zntrack.zn.params(0.5)  # the standard deviation of the normal distribution
     seed = zntrack.zn.params(1234)
@@ -58,15 +60,15 @@
             self.atoms.append(atoms)
             ase.io.write(self.atoms_path / f"atoms_{idx}.xyz", atoms)
 
     def get_atom_filenames(self):
         return [str(self.atoms_path / f"atoms_{idx}.xyz") for idx in range(self.samples)]
 
 
-class AnalyseGlobalForceSensitivity(zntrack.Node):
+class AnalyseGlobalForceSensitivity(base.IPSNode):
     atoms_list = zntrack.zn.deps()
     plots = zntrack.dvc.outs(zntrack.nwd / "plots")
 
     def run(self):
         # assume all atoms have only a single particle changed
         r_ij, d_ij = ase.geometry.get_distances(self.atoms_list[-1].positions)
 
@@ -97,15 +99,15 @@
 class IsConstraintMD(typing.Protocol):
     """Protocol for objects that have a results attribute."""
 
     selected_atom_id: int
     radius: float
 
 
-class AnalyseSingleForceSensitivity(zntrack.Node):
+class AnalyseSingleForceSensitivity(base.IPSNode):
     """Attributes
     ----------
     sim_list : list[]
     """
 
     sim_list: typing.List[IsConstraintMD] = zntrack.zn.deps()
     atoms_list = zntrack.zn.deps()
```

### Comparing `ipsuite-0.1.0a2/ipsuite/base/base.py` & `ipsuite-0.1.0a3/ipsuite/base/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 import abc
 import collections.abc
+import pathlib
 import typing
 
 import ase
 import tqdm
 import znflow
 import zntrack
 
 from ipsuite import fields
 
 # TODO raise error if both data and data_file are given
 
 
-class ProcessAtoms(zntrack.Node):
+class IPSNode(zntrack.Node):
+    _module_ = "ipsuite.nodes"
+
+
+class ProcessAtoms(IPSNode):
     """Protocol for objects that process atoms.
 
     Attributes
     ----------
     data: list[ase.Atoms]
         The atoms data to process. This must be an input to the Node
     data_file: str | None
         The path to the file containing the atoms data. This is an
         alternative to 'data' and can be used to load the data from
         a file. If both are given, 'data' is used. Set 'data' to None
         if you want to use 'data_file'.
     atoms: list[ase.Atoms]
         The processed atoms data. This is an output of the Node.
-        It musn't be a 'field.Atoms' but can also be e.g. a 'property'.
+        It does not have to be 'field.Atoms' but can also be e.g. a 'property'.
     """
 
     data: list[ase.Atoms] = zntrack.zn.deps()
     data_file: str = zntrack.dvc.deps(None)
     atoms: list[ase.Atoms] = fields.Atoms()
 
     def _post_init_(self):
@@ -43,20 +48,25 @@
             self.data = self.get_data()
 
     def get_data(self) -> list[ase.Atoms]:
         """Get the atoms data to process."""
         if self.data is not None:
             return self.data
         elif self.data_file is not None:
-            return list(ase.io.iread(self.data_file))
+            try:
+                with self.state.fs.open(pathlib.Path(self.data_file).as_posix()) as f:
+                    return list(ase.io.iread(f))
+            except FileNotFoundError:
+                # File can not be opened with DVCFileSystem, try normal open
+                return list(ase.io.iread(self.data_file))
         else:
             raise ValueError("No data given.")
 
 
-class ProcessSingleAtom(zntrack.Node):
+class ProcessSingleAtom(IPSNode):
     """Protocol for objects that process a single atom.
 
     Attributes
     ----------
     data: ase.Atoms | list[ase.Atoms]
         The atoms data to process. This must be an input to the Node.
         It can either a single atoms object or a list of atoms objects
@@ -67,16 +77,16 @@
     data_file: str | None
         The path to the file containing the atoms data. This is an
         alternative to 'data' and can be used to load the data from
         a file. If both are given, 'data' is used. Set 'data' to None
         if you want to use 'data_file'.
     atoms: list[ase.Atoms]
         The processed atoms data. This is an output of the Node.
-        It musn't be a 'field.Atoms' but can also be e.g. a 'property'.
-        Altough we only process a single atoms object, we return a list.
+        It does not have to be 'field.Atoms' but can also be e.g. a 'property'.
+        Although, we only process a single atoms object, we return a list.
         This could e.g. be the case when we want to create a trajectory
         starting from a single atoms object.
     """
 
     data: typing.Union[ase.Atoms, typing.List[ase.Atoms]] = zntrack.zn.deps()
     data_file: str = zntrack.dvc.deps(None)
     data_id: typing.Optional[int] = zntrack.zn.params(0)
@@ -93,33 +103,38 @@
         """
         if self.data is not None:
             if isinstance(self.data, (list, collections.abc.Sequence)):
                 atoms = self.data[self.data_id].copy()
             else:
                 atoms = self.data.copy()
         elif self.data_file is not None:
-            atoms = list(ase.io.iread(self.data_file))[self.data_id]
+            try:
+                with self.state.fs.open(pathlib.Path(self.data_file).as_posix()) as f:
+                    atoms = list(ase.io.iread(f))[self.data_id]
+            except FileNotFoundError:
+                # File can not be opened with DVCFileSystem, try normal open
+                atoms = list(ase.io.iread(self.data_file))[self.data_id]
         else:
             raise ValueError("No data given.")
         return atoms
 
 
-class AnalyseAtoms(zntrack.Node):
+class AnalyseAtoms(IPSNode):
     """Protocol for objects that analyse atoms.
 
     Attributes
     ----------
     data: list[ase.Atoms]
         The atoms data to analyse. This must be an input to the Node
     """
 
     data: list[ase.Atoms] = zntrack.zn.deps()
 
 
-class AnalyseProcessAtoms(zntrack.Node):
+class AnalyseProcessAtoms(IPSNode):
     """Analyse the output of a ProcessAtoms Node."""
 
     data: ProcessAtoms = zntrack.zn.deps()
 
     def get_data(self) -> typing.Tuple[list[ase.Atoms], list[ase.Atoms]]:
         self.data.update_data()  # otherwise, data might not be available
         return self.data.data, self.data.atoms
@@ -165,25 +180,30 @@
 
     def backward_mapping(
         self, cg_atoms: ase.Atoms, molecules: list[ase.Atoms]
     ) -> list[ase.Atoms]:
         raise NotImplementedError
 
 
-class CheckBase(zntrack.Node):
+class CheckBase(IPSNode):
     """Base class for check nodes.
     These are callbacks that can be used to preemptively terminate
     a molecular dynamics simulation if a vertain condition is met.
     """
 
     def initialize(self, atoms: ase.Atoms) -> None:
         """Stores some reference property to compare the current property
         against and see whether the simulation should be stopped.
         Derived classes do not need to override this if they consider
-        absolute values and not comparissons.
+        absolute values and not comparisons.
         """
         pass
 
     @abc.abstractmethod
     def check(self, atoms: ase.Atoms) -> bool:
-        """method to check whether a simulation should be stopped."""
+        """Method to check whether a simulation should be stopped."""
+        ...
+
+    @abc.abstractmethod
+    def get_metric(self) -> dict:
+        """Returns the metric that is tracked for stopping."""
         ...
```

### Comparing `ipsuite-0.1.0a2/ipsuite/base/protocol.py` & `ipsuite-0.1.0a3/ipsuite/base/protocol.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/bootstrap/random_displacements.py` & `ipsuite-0.1.0a3/ipsuite/bootstrap/random_displacements.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     Derived classes need to implement a `bootstrap_config` method.
 
     Attributes
     ----------
     n_configurations: int
         Number of displaced configurations.
     maximum: float
-        Bounds for uniform distribution from which displacments are drawn.
+        Bounds for uniform distribution from which displacements are drawn.
     include_original: bool
-        Whether or not to include the orignal configuration in `self.atoms`.
+        Whether or not to include the original configuration in `self.atoms`.
     seed: int
         Random seed.
     """
 
     n_configurations: int = zntrack.zn.params()
     maximum: float = zntrack.zn.params()
     include_original: bool = zntrack.zn.params(True)
```

### Comparing `ipsuite-0.1.0a2/ipsuite/calculators/ase_md.py` & `ipsuite-0.1.0a3/ipsuite/analysis/model/dynamics_checks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,190 +1,197 @@
-import logging
-import pathlib
-import typing
+import collections
 
 import ase
-import ase.constraints
-import ase.geometry
 import numpy as np
-import pandas as pd
-import znh5md
 import zntrack
-from ase import units
-from ase.md.langevin import Langevin
-from ase.md.velocitydistribution import MaxwellBoltzmannDistribution
-from tqdm import trange
+from ase.neighborlist import build_neighbor_list
 
 from ipsuite import base
-from ipsuite.utils.ase_sim import freeze_copy_atoms, get_energy
+from ipsuite.utils.ase_sim import get_energy
 
-log = logging.getLogger(__name__)
 
+class NaNCheck(base.CheckBase):
+    """Check Node to see whether positions, energies or forces become NaN
+    during a simulation.
+    """
+
+    def check(self, atoms: ase.Atoms) -> bool:
+        positions = atoms.positions
+        epot = atoms.get_potential_energy()
+        forces = atoms.get_forces()
+
+        positions_is_none = np.any(positions is None)
+        epot_is_none = epot is None
+        forces_is_none = np.any(forces is None)
+
+        return any([positions_is_none, epot_is_none, forces_is_none])
+
+
+class ConnectivityCheck(base.CheckBase):
+    """Check to see whether the covalent connectivity of the system
+    changes during a simulation.
+    The connectivity is based on ASE's natural cutoffs.
+
+    """
+
+    def _post_init_(self) -> None:
+        self.nl = None
+        self.first_cm = None
+
+    def initialize(self, atoms):
+        self.nl = build_neighbor_list(atoms, self_interaction=False)
+        self.first_cm = self.nl.get_connectivity_matrix(sparse=False)
+        self.is_initialized = True
+
+    def check(self, atoms: ase.Atoms) -> bool:
+        self.nl.update(atoms)
+        cm = self.nl.get_connectivity_matrix(sparse=False)
 
-class ASEMD(base.ProcessSingleAtom):
-    """Class to run a MD simulation with ASE.
+        connectivity_change = np.sum(np.abs(self.first_cm - cm))
+
+        return connectivity_change > 0
+
+
+class EnergySpikeCheck(base.CheckBase):
+    """Check to see whether the potential energy of the system has fallen
+    below a minimum or above a maximum threshold.
+
+    Attributes
+    ----------
+    min_factor: Simulation stops if `E(current) > E(initial) * min_factor`
+    max_factor: Simulation stops if `E(current) < E(initial) * max_factor`
+    """
+
+    min_factor: float = zntrack.zn.params(0.5)
+    max_factor: float = zntrack.zn.params(2.0)
+
+    def _post_init_(self) -> None:
+        self.max_energy = None
+        self.min_energy = None
+
+    def initialize(self, atoms: ase.Atoms) -> None:
+        epot = atoms.get_potential_energy()
+        self.max_energy = epot * self.max_factor
+        self.min_energy = epot * self.min_factor
+
+    def check(self, atoms: ase.Atoms) -> bool:
+        epot = atoms.get_potential_energy()
+        # energy is negative, hence sign convention
+        return epot < self.max_energy or epot > self.min_energy
+
+
+class TemperatureCheck(base.CheckBase):
+    """Calculate and check teperature during a MD simulation
 
     Attributes
     ----------
-    atoms_lst: list
-        list of atoms objects to start simulation from
-    start_id: int
-        starting id to pick from list of atoms
-    model: MLModel
-        Model to use for simulation
-    temperature: float
-        temperature in K to simulate at
-    time_step: float
-        time step of simulation
-    friction: float
-        friction of the Langevin simulator
-    steps: int
-        number of steps to simulate
-    sampling_rate: int
-        number of sample runs
     max_temperature: float
         maximum temperature, when reaching it simulation will be stopped
-    flux_data:
-        saved temperature and total energy
-    repeat: float
-        number of repeats
-    traj_file: Path
-        path where to save the trajectory
-    dump_rate: int, default=1000
-        Keep a cache of the last 'dump_rate' atoms and
-        write them to the trajectory file every 'dump_rate' steps.
     """
 
-    model = zntrack.zn.deps()
-    temperature = zntrack.zn.params()
-    time_step = zntrack.zn.params()
-    friction = zntrack.zn.params()
-    steps = zntrack.zn.params()
-    sampling_rate = zntrack.zn.params()
-    dump_rate = zntrack.zn.params(1000)
-    max_temperature = zntrack.zn.params(10000.0)
-    flux_data = zntrack.zn.plots()  # temperature / energy
-    repeat = zntrack.zn.params((1, 1, 1))
-    steps_before_explosion: int = zntrack.zn.metrics()
-
-    traj_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "trajectory.h5")
-
-    def get_constraint(self):
-        return []
-
-    def get_atoms(self) -> ase.Atoms:
-        atoms: ase.Atoms = self.get_data()
-        return atoms.repeat(self.repeat)
-
-    @property
-    def atoms(self) -> typing.List[ase.Atoms]:
-        return znh5md.ASEH5MD(self.traj_file).get_atoms_list()
-
-    def run(self):
-        """Run the simulation."""
-        atoms = self.get_atoms()
-        atoms.calc = self.model.calc
-        # Initialize velocities
-        MaxwellBoltzmannDistribution(atoms, temperature_K=self.temperature)
-        # initialize thermostat
-        thermostat = Langevin(
-            atoms,
-            timestep=self.time_step * units.fs,
-            temperature_K=self.temperature,
-            friction=self.friction,
-        )
-        # Run simulation
-
-        energy = []
-        temperature, total_energy = get_energy(atoms)
-        total_fs = int(self.steps * self.time_step * self.sampling_rate)
-
-        atoms.set_constraint(self.get_constraint())
-
-        def get_desc():
-            """TQDM description."""
-            return (
-                f"Temp: {temperature:.3f} K \t Energy {total_energy:.3f} eV - (TQDM"
-                " in fs)"
+    max_temperature: float = zntrack.zn.params(10000.0)
+
+    def check(self, atoms):
+        self.temperature, _ = get_energy(atoms)
+        unstable = self.temperature > self.max_temperature
+
+        if unstable:
+            self.status = (
+                f"Temperature Check failed: last {self.temperature} >"
+                f" {self.max_temperature}"
             )
+        else:
+            self.status = f"Temperature Check {self.temperature} < {self.max_temperature}"
 
-        atoms_cache = []
+        return unstable
 
-        db = znh5md.io.DataWriter(self.traj_file)
-        db.initialize_database_groups()
+    def get_metric(self):
+        return {"temperature": self.temperature}
+
+    def __str__(self):
+        return self.status
+
+    def get_desc(self) -> str:
+        return str(self)
 
-        with trange(
-            total_fs,
-            desc=get_desc(),
-            leave=True,
-            ncols=120,
-        ) as pbar:
-            for idx in range(self.steps):
-                thermostat.run(self.sampling_rate)
-                temperature, total_energy = get_energy(atoms)
-                energy.append([temperature, total_energy])
-                atoms_cache.append(freeze_copy_atoms(atoms))
-                if len(atoms_cache) == self.dump_rate:
-                    db.add(
-                        znh5md.io.AtomsReader(
-                            atoms_cache,
-                            frames_per_chunk=self.dump_rate,
-                            step=1,
-                            time=self.sampling_rate,
-                        )
-                    )
-                    atoms_cache = []
-                if idx % (1 / self.time_step) == 0:
-                    pbar.set_description(get_desc())
-                    pbar.update(self.sampling_rate)
-                if temperature > self.max_temperature:
-                    log.critical(
-                        "Temperature of the simulation exceeded"
-                        f" {self.max_temperature} K. Simulation was stopped."
-                    )
-                    break
-        # save the last configurations
-        db.add(
-            znh5md.io.AtomsReader(
-                atoms_cache,
-                frames_per_chunk=self.dump_rate,
-                step=1,
-                time=self.sampling_rate,
-            )
-        )
-        self.flux_data = pd.DataFrame(energy, columns=["temperature", "energy"])
-        self.flux_data.index.name = "step"
-        if temperature > self.max_temperature:
-            self.steps_before_explosion = len(energy)
-        else:
-            self.steps_before_explosion = -1
 
+class ThresholdCheck(base.CheckBase):
+    """Calculate and check a given threshold and std during a MD simulation
 
-class FixedSphereASEMD(ASEMD):
-    """Attributes
+    Compute the standard deviation of the selected property.
+    If the property is off by more than a selected amount from the
+    mean, the simulation will be stopped.
+    Furthermore, the simulation will be stopped if the property
+    exceeds a threshold value.
+
+    Attributes
     ----------
-    atom_id: int
-        The id to use as the center of the sphere to fix.
-        If None, the closed atom to the center will be picked.
-    radius: float
+    value: str
+        name of the property to check
+    max_std: float, optional
+        Maximum number of standard deviations away from the mean to stop the simulation.
+        Roughly the value corresponds to the following percentiles:
+            {1: 68%, 2: 95%, 3: 99.7%}
+    window_size: int, optional
+        Number of steps to average over
+    max_value: float, optional
+        Maximum value of the property to check before the simulation is stopped
+    minimum_window_size: int, optional
+        Minimum number of steps to average over before checking the standard deviation.
+        Also minimum number of steps to run, before the simulation can be stopped.
+    larger_only: bool, optional
+        Only check the standard deviation of points that are larger than the mean.
+        E.g. useful for uncertainties, where a lower uncertainty is not a problem.
     """
 
-    atom_id = zntrack.zn.params(None)
-    selected_atom_id = zntrack.zn.outs()
-    radius = zntrack.zn.params()
-
-    def get_constraint(self):
-        atoms = self.get_atoms()
-        r_ij, d_ij = ase.geometry.get_distances(atoms.get_positions())
-        if self.atom_id is not None:
-            self.selected_atom_id = self.atom_id
-        else:
-            _, dist = ase.geometry.get_distances(
-                atoms.get_positions(), np.diag(atoms.get_cell() / 2)
+    value: str = zntrack.zn.params()
+    max_std: float = zntrack.zn.params(None)
+    window_size: int = zntrack.zn.params(500)
+    max_value: float = zntrack.zn.params(None)
+    minimum_window_size: int = zntrack.zn.params(50)
+    larger_only: bool = zntrack.zn.params(False)
+
+    def _post_init_(self):
+        if self.max_std is None and self.max_value is None:
+            raise ValueError("Either max_std or max_value must be set")
+
+    def _post_load_(self) -> None:
+        self.values = collections.deque(maxlen=self.window_size)
+        self.status = self.__class__.__name__
+
+    def get_value(self, atoms):
+        """Get the value of the property to check.
+
+        Extracted into method so it can be subclassed.
+        """
+        return atoms.calc.results[self.value]
+
+    def check(self, atoms) -> bool:
+        value = self.get_value(atoms)
+        self.values.append(value)
+        mean = np.mean(self.values)
+        std = np.std(self.values)
+
+        distance = value - mean
+        if self.larger_only:
+            distance = np.abs(distance)
+
+        if len(self.values) < self.minimum_window_size:
+            return False
+
+        if self.max_value is not None and value > self.max_value:
+            return True
+
+        if self.max_std is not None and distance > self.max_std * std:
+            self.status = (
+                f"StandardDeviationCheck for '{self.value}' triggered by"
+                f" '{self.values[-1]:.3f}' for '{np.mean(self.values):.3f} +-"
+                f" {np.std(self.values):.3f}' and max value '{self.max_value}'"
             )
-            self.selected_atom_id = np.argmin(dist)
+            return True
+        return False
 
-        if isinstance(self.selected_atom_id, np.generic):
-            self.selected_atom_id = self.selected_atom_id.item()
+    def __str__(self) -> str:
+        return self.status
 
-        indices = np.nonzero(d_ij[self.selected_atom_id] < self.radius)[0]
-        return ase.constraints.FixAtoms(indices=indices)
+    def get_desc(self) -> str:
+        return str(self)
```

### Comparing `ipsuite-0.1.0a2/ipsuite/calculators/cp2k.py` & `ipsuite-0.1.0a3/ipsuite/calculators/cp2k.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 import contextlib
 import functools
 import pathlib
 import shutil
 import subprocess
 from unittest.mock import patch
 
+import ase.calculators.cp2k
 import ase.io
 import cp2k_output_tools
 import pandas as pd
 import tqdm
 import yaml
+import znh5md
 import zntrack
 from ase.calculators.singlepoint import SinglePointCalculator
 from cp2k_input_tools.generator import CP2KInputGenerator
 
 from ipsuite import base
 
 
@@ -131,62 +133,110 @@
             atoms=atoms, energy=data["energies"]["total force_eval"], forces=forces
         )
 
         return atoms
 
 
 class CP2KSinglePoint(base.ProcessAtoms):
-    """Node for running CP2K Single point calculations."""
+    """Node for running CP2K Single point calculations.
+
+    Parameters
+    ----------
+    cp2k_shell : str
+        The cmd to run cp2k.
+    cp2k_params : str
+        The path to the cp2k yaml input file. cp2k-input-tools is used to
+        generate the input file from the yaml file.
+    cp2k_files : str
+        Additional dependencies for the cp2k calculation.
+    wfn_restart_file : str, optional
+        The path to the wfn restart file.
+    wfn_restart_node : str, optional
+        A cp2k Node that has a wfn restart file.
+    """
 
     cp2k_shell: str = zntrack.meta.Text("cp2k_shell.ssmp")
     cp2k_params = zntrack.dvc.params("cp2k.yaml")
-    cp2k_files = zntrack.dvc.deps()
+    cp2k_files = zntrack.dvc.deps(None)
 
-    wfn_restart: str = zntrack.dvc.deps(None)
-    output_file = zntrack.dvc.outs(zntrack.nwd / "atoms.extxyz")
+    wfn_restart_file: str = zntrack.dvc.deps(None)
+    wfn_restart_node = zntrack.zn.deps(None)
+    output_file = zntrack.dvc.outs(zntrack.nwd / "atoms.h5")
     cp2k_directory = zntrack.dvc.outs(zntrack.nwd / "cp2k")
 
     def run(self):
         """ZnTrack run method."""
-        self.atoms = self.get_data()
 
-        self.cp2k_directory.mkdir(exist_ok=True)
+        db = znh5md.io.DataWriter(self.output_file)
+        db.initialize_database_groups()
+
+        calc = self.get_calculator()
+
+        for atoms in tqdm.tqdm(self.get_data()):
+            atoms.calc = calc
+            atoms.get_potential_energy()
+            db.add(znh5md.io.AtomsReader([atoms]))
+
+        for file in self.cp2k_directory.glob("cp2k-RESTART.wfn.*"):
+            # we don't need all restart files
+            file.unlink()
+
+    @property
+    def atoms(self):
+        """Return the atoms object."""
+        return znh5md.ASEH5MD(self.output_file).get_atoms_list()
+
+    def get_input_script(self):
+        """Return the input script.
+
+        We use cached_property, because this will also copy the restart file
+        to the cp2k directory.
+        """
+        if not self.cp2k_directory.exists():
+            self.cp2k_directory.mkdir(exist_ok=True)
+
+            if self.wfn_restart_file is not None:
+                shutil.copy(
+                    self.wfn_restart_file, self.cp2k_directory / "cp2k-RESTART.wfn"
+                )
+            if self.wfn_restart_node is not None:
+                shutil.copy(
+                    self.wfn_restart_node.cp2k_directory / "cp2k-RESTART.wfn",
+                    self.cp2k_directory / "cp2k-RESTART.wfn",
+                )
+
         with pathlib.Path(self.cp2k_params).open("r") as file:
             cp2k_input_dict = yaml.safe_load(file)
 
         _update_paths(cp2k_input_dict)
 
-        cp2k_input_script = "\n".join(CP2KInputGenerator().line_iter(cp2k_input_dict))
+        return "\n".join(CP2KInputGenerator().line_iter(cp2k_input_dict))
 
-        if self.wfn_restart is not None:
-            shutil.copy(self.wfn_restart, self.cp2k_directory / "cp2k-RESTART.wfn")
+    def get_calculator(self, directory: str = None):
+        if directory is None:
+            directory = self.cp2k_directory
+        else:
+            restart_wfn = self.cp2k_directory / "cp2k-RESTART.wfn"
+            if restart_wfn.exists():
+                shutil.copy(restart_wfn, directory / "cp2k-RESTART.wfn")
 
-        with patch(
+        patch(
             "ase.calculators.cp2k.Popen",
-            wraps=functools.partial(subprocess.Popen, cwd=self.cp2k_directory),
-        ):
-            calculator = ase.calculators.cp2k.CP2K(
-                command=self.cp2k_shell,
-                inp=cp2k_input_script,
-                basis_set=None,
-                basis_set_file=None,
-                max_scf=None,
-                cutoff=None,
-                force_eval_method=None,
-                potential_file=None,
-                poisson_solver=None,
-                pseudo_potential=None,
-                stress_tensor=True,
-                xc=None,
-                print_level=None,
-                label="cp2k",
-            )
-
-            for atom in tqdm.tqdm(self.atoms):
-                atom.calc = calculator
-                atom.get_potential_energy()
-                ase.io.write(self.output_file.as_posix(), atom, append=True)
-                # TODO use ZnH5MD
+            wraps=functools.partial(subprocess.Popen, cwd=directory),
+        ).start()
 
-        for file in self.cp2k_directory.glob("cp2k-RESTART.wfn*"):
-            # we don't need the restart files
-            file.unlink()
+        return ase.calculators.cp2k.CP2K(
+            command=self.cp2k_shell,
+            inp=self.get_input_script(),
+            basis_set=None,
+            basis_set_file=None,
+            max_scf=None,
+            cutoff=None,
+            force_eval_method=None,
+            potential_file=None,
+            poisson_solver=None,
+            pseudo_potential=None,
+            stress_tensor=True,
+            xc=None,
+            print_level=None,
+            label="cp2k",
+        )
```

### Comparing `ipsuite-0.1.0a2/ipsuite/configuration_comparison/MMKernel.py` & `ipsuite-0.1.0a3/ipsuite/configuration_comparison/MMKernel.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/configuration_comparison/REMatch.py` & `ipsuite-0.1.0a3/ipsuite/configuration_comparison/REMatch.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/configuration_comparison/base.py` & `ipsuite-0.1.0a3/ipsuite/configuration_comparison/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,39 +37,33 @@
 
 @dataclass
 class SOAPParameter:
     """Dataclass to store SOAP parameter used for representation.
 
     Attributes
     ----------
-    atomic_keys: typing.List[int]
-        atomic numbers of the species
     r_cut: float
         cutoff radius of the soap descriptor in Angstrom
     n_max: int
         number of radial basis functions
     l_max: int
         maximum degree of spherical harmonics
-    periodic: bool
-        set to true to respect periodicity of the atomic system
     n_jobs: int
         number of parallel jobs to instantiate
     sigma: float
         The standard deviation of the gaussians used to expand the atomic density.
     rbf: str
         The radial basis functions to use
     weighting: dict
         Contains the options which control the weighting of the atomic density.
     """
 
-    atomic_keys: typing.List[int] = None
     r_cut: float = 9.0
     n_max: int = 7
     l_max: int = 7
-    periodic: bool = True
     n_jobs: int = -1
     sigma: float = 1.0
     rbf: str = "gto"
     weighting: dict = None
 
 
 class SOAPParameterConverter(znjson.ConverterBase):
@@ -115,15 +109,15 @@
     """Write data to HDF5 dataset."""
     with trange((len(data) - 1), desc=desc, leave=True, disable=disable_tqdm) as pbar:
         for max_index, atoms in enumerate(data):
             file[name][max_index] = soap.create(atoms, n_jobs=n_jobs)
             pbar.update(1)
 
 
-class ConfigurationComparison(zntrack.Node):
+class ConfigurationComparison(base.IPSNode):
     """Base of comparison methods to compare atomic configurations.
 
     Attributes
     ----------
         hash used to use this Node as zn.Nodes()
     reference: typing.Union[utils.helpers.UNION_ATOMS_OR_ATOMS_LST,
      utils.types.SupportsAtoms]
@@ -202,17 +196,18 @@
 
     def save_representation(self):
         """Save the SOAP descriptor representation as hdf5 file to save RAM.
 
         It will create SOAP descriptor for each configurations
          and save them ordered in a hdf5 file.
         """
+        species = [int(x) for x in set(self.analyte[0].get_atomic_numbers())]
         _soap = SOAP(
-            species=self.soap.atomic_keys,
-            periodic=self.soap.periodic,
+            species=species,
+            periodic=False,  # any(self.analyte[0].pbc),
             rcut=self.soap.r_cut,
             nmax=self.soap.n_max,
             lmax=self.soap.l_max,
             sigma=self.soap.sigma,
             rbf=self.soap.rbf,
             weighting=self.soap.weighting,
         )
```

### Comparing `ipsuite-0.1.0a2/ipsuite/configuration_generation/smiles_to_atoms.py` & `ipsuite-0.1.0a3/ipsuite/configuration_generation/smiles_to_atoms.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 import ase
 import zntrack
 from ase.visualize import view
 from rdkit import Chem
 from rdkit.Chem import AllChem, Draw
 
-from ipsuite import fields
+from ipsuite import base, fields
 
 
-class SmilesToAtoms(zntrack.Node):
+class SmilesToAtoms(base.IPSNode):
     atoms = fields.Atoms()
 
     smiles: str = zntrack.zn.params()
+    cell: float = zntrack.zn.params(None)
     seed: int = zntrack.zn.params(1234)
     optimizer: str = zntrack.zn.params("UFF")
     image: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "molecule.png")
 
     def run(self):
         mol = Chem.MolFromSmiles(self.smiles)
         Draw.MolToFile(mol, self.image)
@@ -30,11 +31,14 @@
             AllChem.MMFFOptimizeMolecule(mol)
 
         atoms = ase.Atoms(
             positions=mol.GetConformer().GetPositions(),
             numbers=[atom.GetAtomicNum() for atom in mol.GetAtoms()],
         )
         atoms.positions -= atoms.get_center_of_mass()
+        if self.cell is not None:
+            atoms.set_cell([self.cell, self.cell, self.cell])
+            atoms.center()
         self.atoms = [atoms]
 
     def view(self) -> view:
         return view(self.atoms[0], viewer="x3d")
```

### Comparing `ipsuite-0.1.0a2/ipsuite/configuration_selection/__init__.py` & `ipsuite-0.1.0a3/ipsuite/configuration_selection/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Configuration Selection Nodes."""
 from ipsuite.configuration_selection.base import ConfigurationSelection
 from ipsuite.configuration_selection.index import IndexSelection
 from ipsuite.configuration_selection.kernel import KernelSelection
 from ipsuite.configuration_selection.random import RandomSelection
 from ipsuite.configuration_selection.split import SplitSelection
+from ipsuite.configuration_selection.threshold import ThresholdSelection
 from ipsuite.configuration_selection.uniform_arange import UniformArangeSelection
 from ipsuite.configuration_selection.uniform_energetic import UniformEnergeticSelection
 from ipsuite.configuration_selection.uniform_temporal import UniformTemporalSelection
 
 __all__ = [
     "ConfigurationSelection",
     "RandomSelection",
     "UniformEnergeticSelection",
     "UniformTemporalSelection",
     "UniformArangeSelection",
     "KernelSelection",
     "IndexSelection",
+    "ThresholdSelection",
     "SplitSelection",
 ]
```

### Comparing `ipsuite-0.1.0a2/ipsuite/configuration_selection/base.py` & `ipsuite-0.1.0a3/ipsuite/configuration_selection/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Base Node for ConfigurationSelection."""
 import logging
 import typing
+import uuid
 
 import ase
 import znflow
 import zntrack
 
 from ipsuite import base
 from ipsuite.utils import combine
@@ -16,23 +17,25 @@
     """Base Node for ConfigurationSelection.
 
     Attributes
     ----------
     data: list[Atoms]|list[list[Atoms]]|utils.types.SupportsAtoms
         the data to select from
     exclude_configurations: dict[str, list]|utils.types.SupportsSelectedConfigurations
-        Atoms to exclude from the selection
+        Atoms to exclude from the
+    exclude: list[zntrack.Node]|zntrack.Node|None
+        Exclude the selected configurations from these nodes.
 
     """
 
+    _hash = zntrack.zn.outs()
     exclude_configurations: typing.Union[
         typing.Dict[str, typing.List[int]], base.protocol.HasSelectedConfigurations
-    ] = zntrack.zn.deps(
-        None
-    )  # TODO allow list of dicts that can be combined
+    ] = zntrack.zn.deps(None)
+    exclude: typing.Union[zntrack.Node, typing.List[zntrack.Node]] = zntrack.zn.deps(None)
     selected_configurations: typing.Dict[str, typing.List[int]] = zntrack.zn.outs()
 
     _name_ = "ConfigurationSelection"
 
     def _post_init_(self):
         if self.data is not None and not isinstance(self.data, dict):
             try:
@@ -40,14 +43,30 @@
                     self.data, attribute="atoms", return_dict_attr="name"
                 )
             except TypeError:
                 self.data = znflow.combine(self.data, attribute="atoms")
 
     def run(self):
         """ZnTrack Node Run method."""
+        self._hash = str(uuid.uuid4())
+        if self.exclude is not None:
+            if self.exclude_configurations is None:
+                self.exclude_configurations = {}
+            if not isinstance(self.exclude, list):
+                self.exclude = [self.exclude]
+            for exclude in self.exclude:
+                for key in exclude.selected_configurations:
+                    if key in self.exclude_configurations:
+                        self.exclude_configurations[key].extend(
+                            exclude.selected_configurations[key]
+                        )
+                    else:
+                        self.exclude_configurations[key] = (
+                            exclude.selected_configurations[key]
+                        )
 
         exclude = combine.ExcludeIds(self.get_data(), self.exclude_configurations)
         data = exclude.get_clean_data(flatten=True)
 
         log.debug(f"Selecting from {len(data)} configurations.")
 
         selected_configurations = self.select_atoms(data)
```

### Comparing `ipsuite-0.1.0a2/ipsuite/configuration_selection/index.py` & `ipsuite-0.1.0a3/ipsuite/configuration_selection/index.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/configuration_selection/kernel.py` & `ipsuite-0.1.0a3/ipsuite/configuration_selection/kernel.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             raise ValueError(
                 f"Unable to select {self.n_configurations}. Could only select"
                 f" {len(selected_ids)}"
             )
 
         return selected_ids
 
-    def plot_kernel(self, fps: int = 2, remove: bool = True):
+    def plot_kernel(self, duration: int = 1000, remove: bool = True):
         """Generate an animation of the Kernel change while extending the reference.
 
         Raises
         ------
         ImportError: the imageio package is not shipped with mlsuite by default but is
                         required for generating the animation.
         """
@@ -131,14 +131,16 @@
         for idx, results in enumerate(self.kernel_results):
             plt.plot(results)
             plt.title(f"Iteration {idx}")
             plt.ylabel("Kernel value")
             plt.savefig(img_dir / f"{str(idx).zfill(4)}.png")
             plt.close()
 
-        with imageio.get_writer("kernel_selection.gif", mode="I", fps=fps) as writer:
+        with imageio.get_writer(
+            "kernel_selection.gif", mode="I", duration=duration, loop=0
+        ) as writer:
             for filename in sorted(img_dir.glob("*.png")):
                 image = imageio.v2.imread(filename)
                 writer.append_data(image)
 
         if remove:
             shutil.rmtree(img_dir)
```

### Comparing `ipsuite-0.1.0a2/ipsuite/configuration_selection/random.py` & `ipsuite-0.1.0a3/ipsuite/configuration_selection/random.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/configuration_selection/split.py` & `ipsuite-0.1.0a3/ipsuite/configuration_selection/split.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/configuration_selection/uniform_arange.py` & `ipsuite-0.1.0a3/ipsuite/configuration_selection/uniform_arange.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Selecting atoms with a given step inbetween."""
+"""Selecting atoms with a given step between them."""
 import typing
 
 import ase
 import numpy as np
 import zntrack
 
 from ipsuite.configuration_selection import ConfigurationSelection
```

### Comparing `ipsuite-0.1.0a2/ipsuite/configuration_selection/uniform_energetic.py` & `ipsuite-0.1.0a3/ipsuite/configuration_selection/uniform_energetic.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/configuration_selection/uniform_temporal.py` & `ipsuite-0.1.0a3/ipsuite/configuration_selection/uniform_temporal.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/data_loading/add_data_ase.py` & `ipsuite-0.1.0a3/ipsuite/data_loading/add_data_ase.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pathlib
 import typing
 
 import ase.io
 import tqdm
 import zntrack
 
-from ipsuite import fields
+from ipsuite import base, fields
 
 log = logging.getLogger(__name__)
 
 
 def load_data(
     file: typing.Union[str, pathlib.Path],
     lines_to_read: int = None,
@@ -36,15 +36,15 @@
     ):
         if lines_to_read is not None and config >= lines_to_read:
             break
         atoms.append(atom)
     return atoms
 
 
-class AddData(zntrack.Node):
+class AddData(base.IPSNode):
     """Add data using ASE.
 
     Attributes
     ----------
     use_dvc: bool
         Don't use the filename as a parameter but rather use dvc add <file>
         to track the file with DVC.
```

### Comparing `ipsuite-0.1.0a2/ipsuite/data_loading/add_data_h5md.py` & `ipsuite-0.1.0a3/ipsuite/data_loading/add_data_h5md.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Load Data directly from a H5MD trajectory file."""
 import uuid
 
 import znh5md
 import zntrack
 
+from ipsuite import base
 
-class AddDataH5MD(zntrack.Node):
+
+class AddDataH5MD(base.IPSNode):
     """Load Data directly from a H5MD trajectory file."""
 
     file = zntrack.dvc.deps()
     _hash = zntrack.zn.outs()
     _atoms = None
 
     def run(self):
```

### Comparing `ipsuite-0.1.0a2/ipsuite/fields/atoms.py` & `ipsuite-0.1.0a3/ipsuite/fields/atoms.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/geometry/barycenter_coarse_grain.py` & `ipsuite-0.1.0a3/ipsuite/geometry/barycenter_coarse_grain.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/geometry/graphs.py` & `ipsuite-0.1.0a3/ipsuite/geometry/graphs.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,12 +19,25 @@
     """Identifies molecules in a structure based on the connected subgraphs."""
     G = atoms_to_graph(atoms)
     components = nx.connected_components(G)
     c_list = [np.array(list(c)) for c in components]
     return c_list
 
 
+def split_molecule(a0, a1, atoms):
+    G = atoms_to_graph(atoms)
+
+    try:
+        G.remove_edge(a0, a1)
+    except ValueError:
+        print(f"Atom {a0} and {a1} are not bonded. Pick bonded atoms.")
+
+    components = nx.connected_components(G)
+    c_list = [np.array(list(c)) for c in components]
+    return c_list
+
+
 def edges_from_atoms(atoms: ase.Atoms) -> np.ndarray:
     """Returns the graph edges of a molecular graph."""
     G = atoms_to_graph(atoms)
     edges = np.array(G.edges)
     return edges
```

### Comparing `ipsuite-0.1.0a2/ipsuite/geometry/mapping.py` & `ipsuite-0.1.0a3/ipsuite/geometry/mapping.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/geometry/unwrap.py` & `ipsuite-0.1.0a3/ipsuite/geometry/unwrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     filtered_edges = edges[mask]
 
     for next_idx in next_idxs:
         unwrap(atoms, filtered_edges, next_idx)
 
 
 def unwrap_system(atoms: ase.Atoms, components: list[np.ndarray]) -> list[ase.Atom]:
-    """Molecules in a system which extend across periodic bounaries are mapped such that
+    """Molecules in a system which extend across periodic boundaries are mapped such that
     they are connected but dangle out of the cell.
     Mapping to the side where the fragment of molecule is closest
     to the cell center is preferred.
     Can be reversed by joining the returned molecules
     and calling the `atoms.wrap()` method.
     """
     molecules = []
```

### Comparing `ipsuite-0.1.0a2/ipsuite/models/base.py` & `ipsuite-0.1.0a3/ipsuite/models/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,61 @@
 """Base class for all MLModel Implementations."""
-import contextlib
-import dataclasses
 import pathlib
 import typing
 
 import ase.calculators.calculator
 import ase.io
-import numpy as np
-import znjson
+import tqdm
 import zntrack
 
 from ipsuite import base
-
-
-@dataclasses.dataclass
-class Prediction:
-    """Dataclass to store prediction values of the model.
-
-    Attributes
-    ----------
-    energy: np.ndarray
-        energy prediction with shape (b,)
-    forces: np.ndarray
-        force prediction with shape (b, atoms, 3)
-    virials: np.ndarray
-        virials prediction with shape (b, 6)
-    n_atoms: int
-        number of atoms
-    """
-
-    energy: np.ndarray = None
-    forces: np.ndarray = None
-    stresses: np.ndarray = None
-    n_atoms: int = None
-
-    def update_n_atoms(self):
-        """Update the number of atoms if they are not provided.
-
-        n_atoms has a higher priority than the shape of the forces
-        """
-        if self.n_atoms is None:
-            with contextlib.suppress(AttributeError):
-                self.n_atoms = self.forces.shape[1]
-
-    @property
-    def asdict(self) -> dict:
-        """Convert dataclass to dict."""
-        return dataclasses.asdict(self)
-
-
-class PredictionConverter(znjson.ConverterBase):
-    """Converter for Prediction dataclass."""
-
-    instance = Prediction
-    representation = "ipsuite.models.Prediction"
-
-    def encode(self, value: Prediction):
-        return value.asdict
-
-    def decode(self, value: str):
-        return Prediction(**value)
-
-
-znjson.config.register(PredictionConverter)
+from ipsuite.utils.ase_sim import freeze_copy_atoms
 
 
 class MLModel(base.AnalyseAtoms):
     """Parent class for all MLModel Implementations."""
 
     _name_ = "MLModel"
 
     use_energy: bool = zntrack.zn.params(True)
     use_forces: bool = zntrack.zn.params(True)
     use_stresses: bool = zntrack.zn.params(False)
 
-    @property
-    def calc(self) -> ase.calculators.calculator.Calculator:
-        """Property to return a model specific ase calculator object.
+    def get_calculator(self, **kwargs) -> ase.calculators.calculator.Calculator:
+        """Get a model specific ase calculator object.
 
         Returns
         -------
         calc:
             ase calculator object
         """
         raise NotImplementedError
 
-    def predict(self, atoms: typing.List[ase.Atoms]) -> Prediction:
+    def predict(self, atoms_list: typing.List[ase.Atoms]) -> typing.List[ase.Atoms]:
         """Predict energy, forces and stresses.
 
         based on what was used to train for given atoms objects.
 
         Parameters
         ----------
-        atoms: typing.List[ase.Atoms]
+        atoms_list: typing.List[ase.Atoms]
             list of atoms objects to predict on
 
         Returns
         -------
-        Prediction: Prediction
-            dataclass which contains the predicted energy, forces and stresses
+        Prediction: typing.List[ase.Atoms]
+            Atoms with updated calculators
         """
-        raise NotImplementedError
+        calc = self.get_calculator()
+        results = []
+        for atoms in tqdm.tqdm(atoms_list, ncols=120):
+            atoms.calc = calc
+            atoms.get_potential_energy()
+            results.append(freeze_copy_atoms(atoms))
+        return results
 
     @property
     def lammps_pair_style(self) -> str:
         """Get the lammps pair_style command attribute.
 
         See https://docs.lammps.org/pair_style.html
         Returns
```

### Comparing `ipsuite-0.1.0a2/ipsuite/models/ensemble.py` & `ipsuite-0.1.0a3/ipsuite/models/ensemble.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 import ase
 import numpy as np
 import zntrack
 from ase.calculators.calculator import Calculator, all_changes
 from tqdm import tqdm
 
-from ipsuite.models.base import MLModel, Prediction
+from ipsuite import base
+from ipsuite.models.base import MLModel
+from ipsuite.utils.ase_sim import freeze_copy_atoms
 
 
 class EnsembleCalculator(Calculator):
     implemented_properties = ["energy", "forces"]
 
     def __init__(self, calculators: typing.List[Calculator], **kwargs):
         Calculator.__init__(self, **kwargs)
@@ -32,58 +34,57 @@
         for calc in self.calculators:
             _atoms = atoms.copy()
             _atoms.calc = calc
             results.append(_atoms)
 
         self.results["energy"] = np.mean([x.get_potential_energy() for x in results])
         self.results["forces"] = np.mean([x.get_forces() for x in results], axis=0)
+        self.results["energy_uncertainty"] = np.std(
+            [x.get_potential_energy() for x in results]
+        )
+        self.results["forces_uncertainty"] = np.std(
+            [x.get_forces() for x in results], axis=0
+        )
 
 
-class EnsembleModel(zntrack.Node):
+class EnsembleModel(base.IPSNode):
     models: typing.List[MLModel] = zntrack.zn.deps()
 
     uuid = zntrack.zn.outs()  # to connect this Node to other Nodes it requires an output.
 
     def run(self) -> None:
         self.uuid = str(uuid4())
 
-    @property
-    def calc(self) -> ase.calculators.calculator.Calculator:
+    def get_calculator(self, **kwargs) -> ase.calculators.calculator.Calculator:
         """Property to return a model specific ase calculator object.
 
         Returns
         -------
         calc:
             ase calculator object
         """
-        return EnsembleCalculator(calculators=[x.calc for x in self.models])
+        return EnsembleCalculator(
+            calculators=[x.get_calculator(**kwargs) for x in self.models]
+        )
 
-    def predict(self, atoms: typing.List[ase.Atoms]) -> Prediction:
+    def predict(self, atoms_list: typing.List[ase.Atoms]) -> typing.List[ase.Atoms]:
         """Predict energy, forces and stresses.
 
         based on what was used to train for given atoms objects.
 
         Parameters
         ----------
-        atoms: typing.List[ase.Atoms]
+        atoms_list: typing.List[ase.Atoms]
             list of atoms objects to predict on
 
         Returns
         -------
-        Prediction: Prediction
-            dataclass which contains the predicted energy, forces and stresses
+        typing.List[ase.Atoms]
+            Atoms with updated calculators
         """
-        potential = self.calc
-        validation_energy = []
-        validation_forces = []
-        for configuration in tqdm(atoms, ncols=70):
-            configuration.calc = potential
-            if all(x.use_energy for x in self.models):
-                validation_energy.append(configuration.get_potential_energy())
-            if all(x.use_forces for x in self.models):
-                validation_forces.append(configuration.get_forces())
-
-        return Prediction(
-            energy=np.array(validation_energy),
-            forces=np.array(validation_forces),
-            n_atoms=len(atoms[0]),
-        )
+        calc = self.get_calculator()
+        result = []
+        for atoms in tqdm(atoms_list, ncols=120):
+            atoms.calc = calc
+            atoms.get_potential_energy()
+            result.append(freeze_copy_atoms(atoms))
+        return result
```

### Comparing `ipsuite-0.1.0a2/ipsuite/models/gap.py` & `ipsuite-0.1.0a3/ipsuite/models/gap.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,26 @@
 import dataclasses
 import importlib.resources as pkg_resources
 import logging
 import subprocess as sp
 import typing
 from collections import OrderedDict
 from pathlib import Path
-from typing import List
 
 import ase
 import ase.io
-import numpy as np
 import quippy.potential
 import xmltodict
 import znflow
 import zntrack
-from ase import Atoms
 from jinja2 import Template
-from tqdm import tqdm
 from znjson import ConverterBase, config
 
 from ipsuite import static_data, utils
-from ipsuite.models import MLModel, Prediction
+from ipsuite.models import MLModel
 
 log = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass()
 class SOAP:
     """Dataclass to store SOAP parameters used by gap model.
@@ -196,24 +192,25 @@
         boolean parameter to set train on virials on or off
     model_outputs: Path
         Path to save model files
     train_data: List[ase.Atoms]
         atoms object to train the model on
     """
 
-    SOAP
+    # SOAP
     soap: typing.Union[dict, SOAP] = zntrack.zn.params(SOAP())
     # DistanceNb
     distance_nb: typing.Union[dict, DistanceNb] = zntrack.zn.params(DistanceNb())
     # GAP
     gap: typing.Union[dict, GapParameter] = zntrack.zn.params(GapParameter())
     # #
     model_directory: Path = zntrack.dvc.outs(zntrack.nwd / "model")
     train_data_file: Path = zntrack.dvc.outs(zntrack.nwd / "train_atoms.extxyz")
     gap_input_script: Path = zntrack.dvc.outs(zntrack.nwd / "gap.input")
+    _train_idx_file: Path = zntrack.dvc.outs(zntrack.nwd / "train_atoms.extxyz.idx")
 
     #
     OPENBLAS_NUM_THREADS = zntrack.meta.Environment(None)
 
     #
     def _post_init_(self):
         if not self.state.loaded:
@@ -234,15 +231,15 @@
 
     def run(self):
         """Create output directory and train the model."""
         self.model_directory.mkdir(exist_ok=True, parents=True)
         self.train_model()
 
     @property
-    def gap_input(self) -> (str, str):
+    def gap_input(self) -> typing.Tuple[str, str]:
         """Return the gap input string and the rendered template.
 
         Returns
         -------
         tuple:
             contains gap input string and rendered template
         """
@@ -283,54 +280,15 @@
 
         if not Path(self.gap_input[2]).exists():
             raise RuntimeError(
                 "gp_fit could not fit the given data. Check the GAP log files for more"
                 " information"
             )
 
-    #
-    def predict(self, atoms: List[Atoms]) -> Prediction:
-        """Predict energy, forces and stresses.
-
-        based on what was used to train on with trained GAP potential.
-
-        Parameters
-        ----------
-        atoms: List[Atoms]
-            contains atoms objects to validate
-
-        Returns
-        -------
-        Prediction
-            dataclass contains predicted energy, force and stresses
-        """
-        potential = self.calc
-        validation_energy = []
-        validation_forces = []
-        validation_stresses = []
-        for configuration in tqdm(atoms, ncols=70):
-            configuration.calc = potential
-            if self.use_energy:
-                validation_energy.append(configuration.get_potential_energy())
-            if self.use_forces:
-                validation_forces.append(configuration.get_forces())
-            if self.use_stresses:
-                validation_stresses.append(configuration.get_stress())
-
-        return Prediction(
-            energy=np.array(validation_energy),
-            forces=np.array(validation_forces),
-            # quippy potential output needs minus sign here
-            stresses=np.array(validation_stresses),
-            n_atoms=len(atoms[0]),
-        )
-
-    #
-    @property
-    def calc(self):
+    def get_calculator(self, **kwargs):
         """Get the calculator object.
 
         Returns
         -------
         Calculator object to use e.g. for ase.
         """
         with znflow.disable_graph():
```

### Comparing `ipsuite-0.1.0a2/ipsuite/models/mace_model.py` & `ipsuite-0.1.0a3/ipsuite/models/mace_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """MACE model module."""
 
-import functools
 import json
 import logging
 import pathlib
 import subprocess
-import typing
 
-import ase
-import numpy as np
 import pandas as pd
 import torch
-import tqdm
+import yaml
 import zntrack
 from mace.calculators import MACECalculator
 
 from ipsuite import utils
-from ipsuite.models import MLModel, Prediction
+from ipsuite.models import MLModel
 from ipsuite.static_data import STATIC_PATH
 
 log = logging.getLogger(__name__)
 
 
 def execute(cmd, **kwargs):
     """Execute a command and yield the output line by line.
@@ -40,75 +36,79 @@
     """MACE model."""
 
     train_data_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "train-data.extxyz")
 
     test_data = zntrack.zn.deps()
     test_data_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "test-data.extxyz")
     model_dir: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "model")
+
+    config: str = zntrack.dvc.deps("mace.yaml")
+    config_kwargs: dict = zntrack.zn.params(None)
+    device: str = zntrack.meta.Text(None)
+
     training: pathlib.Path = zntrack.dvc.plots(
         zntrack.nwd / "training.csv",
         template=STATIC_PATH / "y_log.json",
         x="epoch",
         y=["loss", "rmse_e_per_atom", "rmse_f"],
     )
 
-    seed = zntrack.zn.params(42)
-
-    hidden_irreps: str = zntrack.zn.params("16x0e + 16x1o")
-    r_max: float = zntrack.zn.params(5.0)
-    batch_size: int = zntrack.zn.params(10)
-    max_num_epochs: int = zntrack.zn.params(1000)
-    device: str = zntrack.meta.Text("cuda" if torch.cuda.is_available() else "cpu")
-
-    swa: bool = zntrack.zn.params(True)
-    start_swa: int = zntrack.zn.params(1200)
-
-    ema: bool = zntrack.zn.params(True)
-    ema_decay: int = zntrack.zn.params(0.99)
-
-    amsgrad: bool = zntrack.zn.params(True)
-
-    num_radial_basis: int = zntrack.zn.params(8)
-    num_cutoff_basis: int = zntrack.zn.params(5)
-
-    num_interactions: int = zntrack.zn.params(2)
-
     def _post_init_(self):
         self.data = utils.helpers.get_deps_if_node(self.data, "atoms")
         self.test_data = utils.helpers.get_deps_if_node(self.test_data, "atoms")
 
+    def _post_load_(self) -> None:
+        if self.device is None:
+            self.device = "cuda" if torch.cuda.is_available() else "cpu"
+
+    @classmethod
+    def generate_config_file(self, file: str = "mace.yaml"):
+        example = {
+            "amsgrad": True,
+            "batch_size": 5,
+            "ema": True,
+            "ema_decay": 0.99,
+            "hidden_irreps": "128x0e + 128x1o",
+            "max_num_epochs": 1000,
+            "num_cutoff_basis": 5,
+            "num_interactions": 2,
+            "num_radial_basis": 8,
+            "r_max": 5.0,
+            "seed": 42,
+            "start_swa": 1200,
+            "swa": True,
+            "E0s": "average",
+        }
+        pathlib.Path(file).write_text(yaml.safe_dump(example))
+
     def run(self):
         """Train a MACE model."""
         self.model_dir.mkdir(parents=True, exist_ok=True)
         cmd = """curl -sSL https://raw.githubusercontent.com/ACEsuit/mace/main/scripts/run_train.py | python - """  # noqa E501
         cmd += '--name="MACE_model" '
         cmd += f'--train_file="{self.train_data_file.resolve().as_posix()}" '
         cmd += "--valid_fraction=0.05 "
         cmd += f'--test_file="{self.test_data_file.resolve().as_posix()}" '
-        # cmd += """--config_type_weights='{"Default":1.0}' """
-        cmd += """--E0s='average' """
-        cmd += """--model="MACE" """
-        cmd += f"""--seed={self.seed} """
-        cmd += f"""--hidden_irreps='{self.hidden_irreps}' """
-        cmd += f"--r_max={self.r_max} "
-        cmd += f"--batch_size={self.batch_size} "
-        cmd += f"--max_num_epochs={self.max_num_epochs} "
         cmd += f"--device={self.device} "
-        cmd += f"--num_radial_basis={self.num_radial_basis} "
-        cmd += f"--num_cutoff_basis={self.num_cutoff_basis} "
-        cmd += f"--num_interactions={self.num_interactions} "
-
-        if self.swa and self.start_swa < self.max_num_epochs:
-            cmd += f"--swa --start_swa={self.start_swa} "
-
-        if self.ema:
-            cmd += f"--ema --ema_decay={self.ema_decay} "
 
-        if self.amsgrad:
-            cmd += "--amsgrad "
+        config = yaml.safe_load(pathlib.Path(self.config).read_text())
+        if self.config_kwargs:
+            log.warning(
+                f"Overwriting '{self.config}' with values from 'params.yaml':"
+                f" {self.config_kwargs}"
+            )
+            config.update(self.config_kwargs)
+
+        for key, val in config.items():
+            if val is True:
+                cmd += f"--{key} "
+            elif val is False:
+                pass
+            else:
+                cmd += f'--{key}="{val}" '
 
         self.write_data_to_file(file=self.train_data_file, atoms_list=self.data)
         self.write_data_to_file(file=self.test_data_file, atoms_list=self.test_data)
 
         log.debug(f"Running: {cmd}")
 
         for path in execute(cmd, shell=True, cwd=self.model_dir):
@@ -121,49 +121,13 @@
                     for line in f.readlines():
                         value = json.loads(line)
                         if value["mode"] == "eval":
                             data.append(value)
 
                 pd.DataFrame(data).set_index("epoch").to_csv(self.training)
 
-    @functools.cached_property
-    def calc(self):
+    def get_calculator(self, device=None, **kwargs):
         """Return the ASE calculator."""
+        device = device or self.device
         return MACECalculator(
             model_path=self.model_dir / "MACE_model.model", device=self.device
         )
-
-    def predict(self, atoms: typing.List[ase.Atoms]) -> Prediction:
-        """Predict energy, forces and stresses.
-
-        based on what was used to train on with trained GAP potential.
-
-        Parameters
-        ----------
-        atoms: List[Atoms]
-            contains atoms objects to validate
-
-        Returns
-        -------
-        Prediction
-            dataclass contains predicted energy, force and stresses
-        """
-        potential = self.calc
-        validation_energy = []
-        validation_forces = []
-        validation_stresses = []
-        for configuration in tqdm.tqdm(atoms, ncols=70):
-            configuration.calc = potential
-            if self.use_energy:
-                validation_energy.append(configuration.get_potential_energy())
-            if self.use_forces:
-                validation_forces.append(configuration.get_forces())
-            if self.use_stresses:
-                validation_stresses.append(configuration.get_stress())
-
-        return Prediction(
-            energy=np.array(validation_energy),
-            forces=np.array(validation_forces),
-            # quippy potential output needs minus sign here
-            stresses=np.array(validation_stresses),
-            n_atoms=len(atoms[0]),
-        )
```

### Comparing `ipsuite-0.1.0a2/ipsuite/models/nequip.py` & `ipsuite-0.1.0a3/ipsuite/models/nequip.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,22 @@
 import pathlib
 import shutil
 import subprocess
 import typing
 
 import ase.io
 import ase.symbols
-import numpy as np
 import pandas as pd
 import torch
 import yaml
 import zntrack
 import zntrack.utils
-from tqdm import tqdm
 
 from ipsuite import utils
-from ipsuite.models import MLModel, Prediction
+from ipsuite.models import MLModel
 from ipsuite.utils.helpers import check_duplicate_keys
 
 log = logging.getLogger(__name__)
 
 
 def _write_xyz_input_files(
     file: typing.Union[str, pathlib.Path], data: typing.List[ase.Atoms]
@@ -163,41 +161,23 @@
 
         self._handle_parameter_file(n_train, n_val, chemical_symbols)
         self.train_model()
         self.move_metrics()
         self.get_metrics_from_plots()
         self.deploy_model()
 
-    @property
-    def calc(self):
+    def get_calculator(self, **kwargs):
         """Get a nequip ase calculator."""
         from nequip.ase.nequip_calculator import NequIPCalculator
 
         return NequIPCalculator.from_deployed_model(
             model_path=self.deployed_model.as_posix(),
             device=self.device,
         )
 
-    def predict(self, atoms: typing.List[ase.Atoms]) -> Prediction:
-        """Use the nequip model to run a prediction."""
-        validation_energy = []
-        validation_forces = []
-        for configuration in tqdm(atoms, ncols=70):
-            configuration.set_calculator(self.calc)
-            if self.use_energy:
-                validation_energy.append(configuration.get_potential_energy())
-            if self.use_forces:
-                validation_forces.append(configuration.get_forces())
-
-        return Prediction(
-            energy=np.array(validation_energy),
-            forces=np.array(validation_forces),
-            n_atoms=len(atoms[0]),
-        )
-
     @property
     def lammps_pair_style(self) -> str:
         """Get the lammps pair style for the nequip model."""
         with (self.model_directory / "config.yaml").open("r") as file:
             parameter = yaml.safe_load(file)
         if "allegro.model.Allegro" in parameter.get("model_builders", []):
             return "allegro"
```

### Comparing `ipsuite-0.1.0a2/ipsuite/static_data/gap.jinja2` & `ipsuite-0.1.0a3/ipsuite/static_data/gap.jinja2`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,8 @@
 {% if general_params.use_stresses %}
     stress_parameter_name=stress
     virial_parameter_name=DUMMY
 {% else %}
     virial_parameter_name=DUMMY
     stress_parameter_name=DUMMY
 {% endif %}
->> {{ general_params.gp_dump }}
+>> {{ general_params.gp_dump }}
```

### Comparing `ipsuite-0.1.0a2/ipsuite/utils/ase_sim.py` & `ipsuite-0.1.0a3/ipsuite/utils/ase_sim.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 def get_desc(temperature: float, total_energy: float):
     """TQDM description."""
     return f"Temp: {temperature:.3f} K \t Energy {total_energy:.3f} eV - (TQDM in fs)"
 
 
 @functools.singledispatch
 def freeze_copy_atoms(atoms) -> ase.Atoms:
+    # TODO can we add the name of the original calculator?
     result = atoms.copy()
     result.calc = SinglePointCalculator(result, **atoms.calc.results)
     return result
 
 
 @freeze_copy_atoms.register
 def _(atoms: list) -> list[ase.Atoms]:
```

### Comparing `ipsuite-0.1.0a2/ipsuite/utils/combine.py` & `ipsuite-0.1.0a3/ipsuite/utils/combine.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,24 +161,24 @@
     -------
         >>> data = {'a': [1, 2, 3], 'b': [4, 5, 6]}
         >>> get_ids_per_key(data, [0, 1, 3, 5])
         >>> # {'a': [0, 1], 'b': [0, 2]}
     """
     if not isinstance(data, dict):
         if silent_ignore:
-            return ids
+            return np.array(ids).tolist()
         else:
             raise TypeError(f"data must be a dictionary and not {type(data)}")
 
     ids_per_key = {}
     ids = np.array(ids).astype(int)
     ids = np.sort(ids)
     start = 0
 
     for key, val in data.items():
         condition = ids - start
         condition = np.logical_and(condition < len(val), condition >= 0)
 
-        ids_per_key[key] = (ids[condition] - start).tolist()
+        ids_per_key[key] = np.array(ids[condition] - start).tolist()
         start += len(val)
 
     return ids_per_key
```

### Comparing `ipsuite-0.1.0a2/ipsuite/utils/logs.py` & `ipsuite-0.1.0a3/ipsuite/utils/logs.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/utils/md.py` & `ipsuite-0.1.0a3/ipsuite/utils/md.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/ipsuite/utils/metrics.py` & `ipsuite-0.1.0a3/ipsuite/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.0a2/pyproject.toml` & `ipsuite-0.1.0a3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipsuite"
-version = "0.1.0a2"
+version = "0.1.0a3"
 description = "A suite of tools for machine learned interatomic potentials."
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 keywords = ["data-version-control", "machine-learning", "reproducibility", "interatomic potentials"]
 license = "License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)"
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -35,14 +35,15 @@
 #[tool.poetry.group.GAP.dependencies]
 quippy-ase = { version = "^0.9.12", optional = true }
 xmltodict = "^0.13.0"
 
 
 
 nequip = { version = "^0.5.6", optional = true }
+
 rdkit = "^2022.9.5"
 lazy-loader = "^0.2"
 znflow = "^0.1.11"
 
 [tool.poetry.group.allegro.dependencies]
 mir-allegro = { git = "https://github.com/mir-group/allegro.git" }
 
@@ -53,24 +54,29 @@
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.1.0"
 ruff = "^0.0.252"
 
 [tool.poetry.group.notebook.dependencies]
 jupyterlab = "^3.6.1"
+ipywidgets = "^8.0.6"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.1"
 coverage = "^7.2.1"
 
+
+[tool.poetry.group.dev.dependencies]
+imageio = "^2.28.1"
+
 [tool.poetry.extras]
 comparison = ["h5py", "tensorflow", "llvmlite", "numba", "dscribe"]
 gap = ["quippy-ase", "xmltodict"]
 nequip = ["nequip"]
-
+# apax = ["apax"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = 'black'
@@ -79,15 +85,15 @@
 [tool.black]
 line-length = 90
 preview = true
 
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
-select = ["A", "B", "C", "E", "F", "I", "C90", "S", "C4", "TID", "PTH"] #  "D",
+select = ["A", "B", "C", "E", "F", "I", "C90", "C4", "TID", "PTH"] #  "D", "S"
 # ignore = ["D203", "D213", "D104", "D102", "D100", ]
 ignore = [
     "B905", # not supported in older python versions
 ]
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
@@ -116,7 +122,10 @@
 per-file-ignores = { }
 
 # Same as Black.
 line-length = 90
 
 # Assume Python 3.10.
 target-version = "py310"
+
+[tool.codespell]
+skip = "poetry.lock"
```

### Comparing `ipsuite-0.1.0a2/PKG-INFO` & `ipsuite-0.1.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipsuite
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A suite of tools for machine learned interatomic potentials.
 License: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Keywords: data-version-control,machine-learning,reproducibility,interatomic potentials
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
@@ -38,17 +38,20 @@
 [![ZnTrack](https://img.shields.io/badge/Powered%20by-ZnTrack-%23007CB0)](https://zntrack.readthedocs.io/en/latest/)
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 
 # IPS - The Inter Atomic Potential Suite
 
 IPS provides you with tools to generate Machine Learned Interatomic Potentials.
 
-Install the package to get started or check out an interactive notebook [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/IPSuite/HEAD) 
+Install the package to get started or check out an interactive notebook
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/IPSuite/HEAD)
+
 ```python
 pip install ipsuite
 ```
 
 Examples can be found at:
+
 - https://dagshub.com/PythonFZ/IPS-Examples/src/intro/main.ipynb
 - https://dagshub.com/PythonFZ/IPS-Examples/src/graph/main.ipynb
-- https://dagshub.com/PythonFZ/IPS-Examples/src/modifiy_graph/main.ipynb
+- https://dagshub.com/PythonFZ/IPS-Examples/src/modify_graph/main.ipynb
```

