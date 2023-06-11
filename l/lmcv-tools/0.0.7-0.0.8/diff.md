# Comparing `tmp/lmcv_tools-0.0.7.tar.gz` & `tmp/lmcv_tools-0.0.8.tar.gz`

## Comparing `lmcv_tools-0.0.7.tar` & `lmcv_tools-0.0.8.tar`

### file list

```diff
@@ -1,105 +1,124 @@
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/docs/To Do.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/commands/__init__.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/commands/extract.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/commands/generate.py
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/commands/translate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/databases/__init__.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/databases/extraction_attributes.json
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/databases/help_messages.json
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/databases/translation_reference.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/interface/__init__.py
--rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/interface/core.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/interface/filer.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/interface/messenger.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/interface/searcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/models/__init__.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/models/custom_errors.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/models/extraction_components.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/models/generation_artifacts.py
--rw-r--r--   0        0        0    14092 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/models/graphical_interfaces.py
--rw-r--r--   0        0        0    16239 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/lmcv_tools/models/translation_components.py
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/test_extract.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/test_generate.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/test_translate.py
--rw-r--r--   0        0        0   113958 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic.pos
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_and.csv
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_df.csv
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_eq.csv
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_ge.csv
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_gt.csv
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_in_1.csv
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_in_2.csv
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_le.csv
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_ls.csv
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_or.csv
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_1.csv
--rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_2.csv
--rw-r--r--   0        0        0     9436 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_3.csv
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_ur_1.csv
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_ur_2.csv
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_node_id.csv
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_node_x.csv
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_node_y.csv
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_node_z.csv
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_step_factor.csv
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_step_id.csv
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_u.csv
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_v.csv
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_w.csv
--rw-r--r--   0        0        0    38699 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/SquarePlate.pos
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/SquarePlate_exp_buckling_factor.csv
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/SquarePlate_exp_buckling_id.csv
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/SquarePlate_exp_buckling_node_u.csv
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/SquarePlate_exp_buckling_node_v.csv
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/extract/SquarePlate_exp_buckling_node_w.csv
--rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/generate/virtual_laminas_exp_mori_tanaka.inp
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/generate/virtual_laminas_exp_shell.inp
--rw-r--r--   0        0        0    13613 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/generate/virtual_laminas_exp_smart_1.inp
--rw-r--r--   0        0        0    13592 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/generate/virtual_laminas_exp_smart_2.inp
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/generate/virtual_laminas_exp_solid.inp
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/generate/virtual_laminas_exp_voight.inp
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/Circle_T3_Q4_4x4.dat
--rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/Circle_T3_Q4_4x4_exp.svg
--rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/HeartPlate_BT2_2x2.dat
--rw-r--r--   0        0        0    12375 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/HeartPlate_BT2_2x2_exp.svg
--rw-r--r--   0        0        0    47634 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/HeartPlate_BT3_4x4.dat
--rw-r--r--   0        0        0    60976 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/HeartPlate_BT3_4x4_exp.svg
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/HeartPlate_Q8_2x2.dat
--rw-r--r--   0        0        0    10305 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/HeartPlate_Q8_2x2_exp.svg
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Circle_S3_S4R_4x4.inp
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Circle_S3_S4R_4x4_exp.dat
--rw-r--r--   0        0        0    45691 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/ComplexPart_C3D20R.inp
--rw-r--r--   0        0        0    52988 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/ComplexPart_C3D20R_exp.dat
--rw-r--r--   0        0        0    50506 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/ComplexPart_S8R.inp
--rw-r--r--   0        0        0    60178 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/ComplexPart_S8R_exp.dat
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D20_1x1x1.inp
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D20_1x1x1_exp.dat
--rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D20_2x2x2.inp
--rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D20_2x2x2_exp.dat
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D8_1x1x1.inp
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D8_1x1x1_exp.dat
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D8_2x2x2.inp
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D8_2x2x2_exp.dat
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S4_1x1.inp
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S4_1x1_exp.dat
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S4_2x2.inp
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S4_2x2_exp.dat
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S8R_1x1.inp
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S8R_1x1_exp.dat
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S8R_2x2.inp
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S8R_2x2_exp.dat
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_S3_1x1.inp
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_S3_1x1_exp.dat
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_S3_2x2.inp
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_S3_2x2_exp.dat
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_1x1.inp
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_1x1_exp.dat
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_2x2.inp
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_2x2_exp.dat
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/.gitignore
--rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/LICENSE
--rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    10393 2020-02-02 00:00:00.000000 lmcv_tools-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/docs/To Do.md
+-rw-r--r--   0        0        0   576294 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/docs/notebooks/Optimization - Virtual Laminas Distribution.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/commands/__init__.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/commands/extract.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/commands/generate.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/commands/translate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/databases/__init__.py
+-rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/databases/extraction_attributes.json
+-rw-r--r--   0        0        0     4569 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/databases/help_messages.json
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/databases/translation_reference.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/interface/__init__.py
+-rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/interface/core.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/interface/filer.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/interface/messenger.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/interface/searcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/models/__init__.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/models/custom_errors.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/models/extraction_components.py
+-rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/models/generation_artifacts.py
+-rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/models/graphical_interfaces.py
+-rw-r--r--   0        0        0    19307 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/lmcv_tools/models/translation_components.py
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/test_extract.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/test_generate.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/test_translate.py
+-rw-r--r--   0        0        0   113958 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic.pos
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_and.csv
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_df.csv
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_eq.csv
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_ge.csv
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_gt.csv
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_in_1.csv
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_in_2.csv
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_le.csv
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_ls.csv
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_cond_or.csv
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_1.csv
+-rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_2.csv
+-rw-r--r--   0        0        0     9436 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_3.csv
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_ur_1.csv
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_ur_2.csv
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_node_id.csv
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_node_x.csv
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_node_y.csv
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_node_z.csv
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_step_factor.csv
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_step_id.csv
+-rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_u.csv
+-rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_v.csv
+-rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_w.csv
+-rw-r--r--   0        0        0    27669 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/HeartPlate.pos
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/HeartPlate_exp_vibration_factor.csv
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/HeartPlate_exp_vibration_id.csv
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/HeartPlate_exp_vibration_node_u.csv
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/HeartPlate_exp_vibration_node_v.csv
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/HeartPlate_exp_vibration_node_w.csv
+-rw-r--r--   0        0        0    44466 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/SquarePlate.pos
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/SquarePlate_exp_buckling_factor.csv
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/SquarePlate_exp_buckling_id.csv
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/SquarePlate_exp_buckling_node_u.csv
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/SquarePlate_exp_buckling_node_v.csv
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/extract/SquarePlate_exp_buckling_node_w.csv
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/generate/virtual_laminas_exp_hs_lb_1.inp
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/generate/virtual_laminas_exp_hs_lb_2.inp
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/generate/virtual_laminas_exp_hs_ub_1.inp
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/generate/virtual_laminas_exp_hs_ub_2.inp
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/generate/virtual_laminas_exp_mori_tanaka.inp
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/generate/virtual_laminas_exp_shell.inp
+-rw-r--r--   0        0        0    14317 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/generate/virtual_laminas_exp_smart_1.inp
+-rw-r--r--   0        0        0    14317 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/generate/virtual_laminas_exp_smart_2.inp
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/generate/virtual_laminas_exp_solid.inp
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/generate/virtual_laminas_exp_voigt.inp
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/Circle_T3_Q4_4x4.dat
+-rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/Circle_T3_Q4_4x4_exp.svg
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/Disform_BT2.dat
+-rw-r--r--   0        0        0     8911 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/Disform_BT2_exp.svg
+-rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/Disform_BT4.dat
+-rw-r--r--   0        0        0    15112 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/Disform_BT4_exp.svg
+-rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/HeartPlate_BT2_2x2.dat
+-rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/HeartPlate_BT2_2x2_exp.svg
+-rw-r--r--   0        0        0    47634 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/HeartPlate_BT3_4x4.dat
+-rw-r--r--   0        0        0    65204 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/HeartPlate_BT3_4x4_exp.svg
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/HeartPlate_Q8_2x2.dat
+-rw-r--r--   0        0        0    10305 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/HeartPlate_Q8_2x2_exp.svg
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Circle_S3_S4R_4x4.inp
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Circle_S3_S4R_4x4_exp.dat
+-rw-r--r--   0        0        0    45691 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/ComplexPart_C3D20R.inp
+-rw-r--r--   0        0        0    52988 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/ComplexPart_C3D20R_exp.dat
+-rw-r--r--   0        0        0    50506 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/ComplexPart_S8R.inp
+-rw-r--r--   0        0        0    60178 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/ComplexPart_S8R_exp.dat
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D10_12.inp
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D10_12_exp.dat
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D20_1x1x1.inp
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D20_1x1x1_exp.dat
+-rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D20_2x2x2.inp
+-rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D20_2x2x2_exp.dat
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D4_12.inp
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D4_12_exp.dat
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D8_1x1x1.inp
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D8_1x1x1_exp.dat
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D8_2x2x2.inp
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D8_2x2x2_exp.dat
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S4_1x1.inp
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S4_1x1_exp.dat
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S4_2x2.inp
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S4_2x2_exp.dat
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S8R_1x1.inp
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S8R_1x1_exp.dat
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S8R_2x2.inp
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S8R_2x2_exp.dat
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_S3_1x1.inp
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_S3_1x1_exp.dat
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_S3_2x2.inp
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_S3_2x2_exp.dat
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_1x1.inp
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_1x1_exp.dat
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_2x2.inp
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_2x2_exp.dat
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/.gitignore
+-rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/LICENSE
+-rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    11028 2020-02-02 00:00:00.000000 lmcv_tools-0.0.8/PKG-INFO
```

### Comparing `lmcv_tools-0.0.7/lmcv_tools/commands/extract.py` & `lmcv_tools-0.0.8/lmcv_tools/commands/extract.py`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/lmcv_tools/commands/generate.py` & `lmcv_tools-0.0.8/lmcv_tools/commands/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ..interface import filer
 from ..models.generation_artifacts import (
    VirtualLaminas,
    ElementConfiguration,
    MicromechanicalModel,
    Material
 )
-from ..models.graphical_interfaces import PromptGenerateVirtualLamina
+from ..models.graphical_interfaces import PromptGenerateVirtualLaminas
 from ..models.custom_errors import CommandError
 
 # Funções de Geração de Artefatos
 def generate_virtual_laminas(
    laminas_count: int,
    element_type: str,
    thickness: float,
@@ -52,15 +52,15 @@
 # Funções de Parâmetros de Artefatos
 def params_virtual_laminas(args: list[str]) -> dict:
    # Iniciando Parâmetros
    params = dict()
    
    # Exibindo Interface Gráfica para Preencher Parâmetros (Se não Houver Parâmetros)
    if len(args) == 0:
-      window = PromptGenerateVirtualLamina(params)
+      window = PromptGenerateVirtualLaminas(params)
       window.start()
 
       # Conferindo se Há um Caminho
       if params.get('path') is not None:
          if params['path'] != '':
             args = [params['path']]
          del params['path']
```

### Comparing `lmcv_tools-0.0.7/lmcv_tools/commands/translate.py` & `lmcv_tools-0.0.8/lmcv_tools/commands/translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
       x = node.x - x_min
       y = abs(node.y - y_max)
 
       # Ajustando Escala e Posição
       x = x * scale_coeff + 5
       y = y * scale_coeff + 5
 
-      svg_interpreter.model.add_node(ide, x, y, 0)
+      svg_interpreter.model.add_node(ide, x, y, 0, node.weight)
    svg_interpreter.model.element_groups = dat_interpreter.model.element_groups
 
    # Retornando Tradução
    return svg_interpreter.write()
 
 # Traduções Suportadas
 supported_translations = {
```

### Comparing `lmcv_tools-0.0.7/lmcv_tools/databases/extraction_attributes.json` & `lmcv_tools-0.0.8/lmcv_tools/databases/extraction_attributes.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7291666666666666%*

 * *Differences: {"'buckling.factor'": "{'format': {'keywords': "*

 * *                      "'%RESULT\\\\.CASE\\\\.STEP\\\\.BUCKLING\\\\.FACTOR\\n(?P<line>[^%]+)', "*

 * *                      "'line': "*

 * *                      "'^(?P<buckling_id>\\\\d+)\\\\s+(?P<value>[+-]?\\\\d+\\\\.\\\\d+e[+-]\\\\d+)'}}",*

 * * "'buckling.id'": "{'format': {'keywords': "*

 * *                  "'%RESULT\\\\.CASE\\\\.STEP\\\\.BUCKLING\\\\.FACTOR\\n(?P<line>[^%]+)', 'line': "*

 * *                  "'^(?P<value>\\\\d+)'}}",*

 * * "'buckling.node.u'": "{'format': {'keywo […]*

```diff
@@ -1,52 +1,52 @@
 {
     "buckling.factor": {
         "data_type": "float",
         "format": {
-            "keywords": "%RESULT\\.CASE\\.STEP\\.BUCKLING\\.MODES\n(?P<buckling_id>\\d+)\n\n%RESULT\\.CASE\\.STEP\\.BUCKLING\\.FACTOR\n(?P<line>[^%]+)",
-            "line": "(?P<value>[+-]?\\d+\\.\\d+e[+-]\\d+)"
+            "keywords": "%RESULT\\.CASE\\.STEP\\.BUCKLING\\.FACTOR\n(?P<line>[^%]+)",
+            "line": "^(?P<buckling_id>\\d+)\\s+(?P<value>[+-]?\\d+\\.\\d+e[+-]\\d+)"
         },
         "related_attributes": [
             "buckling.id"
         ]
     },
     "buckling.id": {
         "data_type": "int",
         "format": {
-            "keywords": "%RESULT\\.CASE\\.STEP\\.BUCKLING\\.MODES\n(?P<line>[^%]+)",
-            "line": "(?P<value>\\d+)"
+            "keywords": "%RESULT\\.CASE\\.STEP\\.BUCKLING\\.FACTOR\n(?P<line>[^%]+)",
+            "line": "^(?P<value>\\d+)"
         },
         "related_attributes": []
     },
     "buckling.node.u": {
         "data_type": "float",
         "format": {
-            "keywords": "%RESULT\\.CASE\\.STEP\\.BUCKLING\\.MODES\n(?P<buckling_id>\\d+)\n\n%RESULT\\.CASE\\.STEP\\.BUCKLING\\.FACTOR\n(?:.+)\n\n%RESULT\\.CASE\\.STEP\\.NODAL\\.EIGENVECTOR\n(?P<line>[^%]+)",
+            "keywords": "%RESULT\\.CASE\\.STEP\\.BUCKLING\\.FACTOR\n(?P<buckling_id>\\d+)\\s+(?:.+)\n\n%RESULT\\.CASE\\.STEP\\.NODAL\\.EIGENVECTOR\n(?P<line>[^%]+)",
             "line": "^(?P<node_id>\\d+)\\s+(?P<value>[+-]\\d+\\.\\d+e[+-]\\d+)"
         },
         "related_attributes": [
             "buckling.id",
             "node.id"
         ]
     },
     "buckling.node.v": {
         "data_type": "float",
         "format": {
-            "keywords": "%RESULT\\.CASE\\.STEP\\.BUCKLING\\.MODES\n(?P<buckling_id>\\d+)\n\n%RESULT\\.CASE\\.STEP\\.BUCKLING\\.FACTOR\n(?:.+)\n\n%RESULT\\.CASE\\.STEP\\.NODAL\\.EIGENVECTOR\n(?P<line>[^%]+)",
+            "keywords": "%RESULT\\.CASE\\.STEP\\.BUCKLING\\.FACTOR\n(?P<buckling_id>\\d+)\\s+(?:.+)\n\n%RESULT\\.CASE\\.STEP\\.NODAL\\.EIGENVECTOR\n(?P<line>[^%]+)",
             "line": "^(?P<node_id>\\d+)\\s+(?:[+-]\\d+\\.\\d+e[+-]\\d+)\\s+(?P<value>[+-]\\d+\\.\\d+e[+-]\\d+)"
         },
         "related_attributes": [
             "buckling.id",
             "node.id"
         ]
     },
     "buckling.node.w": {
         "data_type": "float",
         "format": {
-            "keywords": "%RESULT\\.CASE\\.STEP\\.BUCKLING\\.MODES\n(?P<buckling_id>\\d+)\n\n%RESULT\\.CASE\\.STEP\\.BUCKLING\\.FACTOR\n(?:.+)\n\n%RESULT\\.CASE\\.STEP\\.NODAL\\.EIGENVECTOR\n(?P<line>[^%]+)",
+            "keywords": "%RESULT\\.CASE\\.STEP\\.BUCKLING\\.FACTOR\n(?P<buckling_id>\\d+)\\s+(?:.+)\n\n%RESULT\\.CASE\\.STEP\\.NODAL\\.EIGENVECTOR\n(?P<line>[^%]+)",
             "line": "^(?P<node_id>\\d+)\\s+(?:[+-]\\d+\\.\\d+e[+-]\\d+)\\s+(?:[+-]\\d+\\.\\d+e[+-]\\d+)\\s+(?P<value>[+-]\\d+\\.\\d+e[+-]\\d+)"
         },
         "related_attributes": [
             "buckling.id",
             "node.id"
         ]
     },
@@ -134,9 +134,60 @@
             "keywords": "%RESULT\\.CASE\\.STEP\n(?P<step_id>\\d+)\n\n%RESULT\\.CASE\\.STEP\\.FACTOR\n(?:.+)\n\n%RESULT\\.CASE\\.STEP\\.NODAL\\.DISPLACEMENT\n(?P<line>[^%]+)",
             "line": "^(?P<node_id>\\d+)\\s+(?:[+-]\\d+\\.\\d+e[+-]\\d+)\\s+(?:[+-]\\d+\\.\\d+e[+-]\\d+)\\s+(?P<value>[+-]\\d+\\.\\d+e[+-]\\d+)"
         },
         "related_attributes": [
             "step.id",
             "node.id"
         ]
+    },
+    "vibration.factor": {
+        "data_type": "float",
+        "format": {
+            "keywords": "%RESULT\\.CASE\\.STEP\\.NATURAL\\.FREQUENCY\n(?P<line>[^%]+)",
+            "line": "^(?P<vibration_id>\\d+)\\s+(?P<value>[+-]?\\d+\\.\\d+e[+-]\\d+)"
+        },
+        "related_attributes": [
+            "vibration.id"
+        ]
+    },
+    "vibration.id": {
+        "data_type": "int",
+        "format": {
+            "keywords": "%RESULT\\.CASE\\.STEP\\.NATURAL\\.FREQUENCY\n(?P<line>[^%]+)",
+            "line": "^(?P<value>\\d+)"
+        },
+        "related_attributes": []
+    },
+    "vibration.node.u": {
+        "data_type": "float",
+        "format": {
+            "keywords": "%RESULT\\.CASE\\.STEP\\.NATURAL\\.FREQUENCY\n(?P<vibration_id>\\d+)\\s+(?:.+)\n\n%RESULT\\.CASE\\.STEP\\.NODAL\\.EIGENVECTOR\n(?P<line>[^%]+)",
+            "line": "^(?P<node_id>\\d+)\\s+(?P<value>[+-]\\d+\\.\\d+e[+-]\\d+)"
+        },
+        "related_attributes": [
+            "vibration.id",
+            "node.id"
+        ]
+    },
+    "vibration.node.v": {
+        "data_type": "float",
+        "format": {
+            "keywords": "%RESULT\\.CASE\\.STEP\\.NATURAL\\.FREQUENCY\n(?P<vibration_id>\\d+)\\s+(?:.+)\n\n%RESULT\\.CASE\\.STEP\\.NODAL\\.EIGENVECTOR\n(?P<line>[^%]+)",
+            "line": "^(?P<node_id>\\d+)\\s+(?:[+-]\\d+\\.\\d+e[+-]\\d+)\\s+(?P<value>[+-]\\d+\\.\\d+e[+-]\\d+)"
+        },
+        "related_attributes": [
+            "vibration.id",
+            "node.id"
+        ]
+    },
+    "vibration.node.w": {
+        "data_type": "float",
+        "format": {
+            "keywords": "%RESULT\\.CASE\\.STEP\\.NATURAL\\.FREQUENCY\n(?P<vibration_id>\\d+)\\s+(?:.+)\n\n%RESULT\\.CASE\\.STEP\\.NODAL\\.EIGENVECTOR\n(?P<line>[^%]+)",
+            "line": "^(?P<node_id>\\d+)\\s+(?:[+-]\\d+\\.\\d+e[+-]\\d+)\\s+(?:[+-]\\d+\\.\\d+e[+-]\\d+)\\s+(?P<value>[+-]\\d+\\.\\d+e[+-]\\d+)"
+        },
+        "related_attributes": [
+            "vibration.id",
+            "node.id"
+        ]
     }
 }
```

### Comparing `lmcv_tools-0.0.7/lmcv_tools/databases/help_messages.json` & `lmcv_tools-0.0.8/lmcv_tools/databases/help_messages.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981971153846153%*

 * *Differences: {"'extract'": "{'topics': {'Possible Arguments': {'[attributes]': 'Required argument. List of "*

 * *              'names (at least one) that represent a piece of data from a .pos file. Supported '*

 * *              'attributes: step.id, step.factor, node.id, node.x, node.y, node.z, step.node.u, '*

 * *              'step.node.v, step.node.w, buckling.id, buckling.factor, buckling.node.u, '*

 * *              'buckling.node.v, buckling.node.w, vibration.id, vibration.factor, vibration.node.u, '*

 * *              "vibration.node.v […]*

```diff
@@ -10,15 +10,15 @@
             }
         },
         "usage": "lmcv_tools [command] [args]"
     },
     "extract": {
         "topics": {
             "Possible Arguments": {
-                "[attributes]": "Required argument. List of names (at least one) that represent a piece of data from a .pos file. Supported attributes: step.id, step.factor, node.id, node.x, node.y, node.z, step.node.u, step.node.v, step.node.w, buckling.id, buckling.factor, buckling.node.u, buckling.node.v, buckling.node.w",
+                "[attributes]": "Required argument. List of names (at least one) that represent a piece of data from a .pos file. Supported attributes: step.id, step.factor, node.id, node.x, node.y, node.z, step.node.u, step.node.v, step.node.w, buckling.id, buckling.factor, buckling.node.u, buckling.node.v, buckling.node.w, vibration.id, vibration.factor, vibration.node.u, vibration.node.v, vibration.node.w",
                 "[condition]": "Optional argument. Series of attribute constraints, combining attribute names, operators and test values. Supported operators: and, or, =, >, <, >=, <=, !=, in. Remembering that the symbols '>' and '<' must be encapsulated by quotes. Otherwise, they will be interpreted by the shell as redirection operators. Example: [...] where step.id '>' 5 and step.factor '<' 1.0",
                 "[path/to/.csv]": "Optional argument. Relative path to .csv file. If it is not given, it will be the same as the .pos file",
                 "[path/to/.pos]": "Required argument. Relative path to .pos file"
             }
         },
         "usage": "extract [attributes] from [path/to/.pos] where [condition] to [path/to/.csv]"
     },
@@ -26,15 +26,15 @@
         "topics": {
             "Arguments for virtual_laminas": {
                 "[E1]": "Required float point argument. Elastic Modulus of Material 1",
                 "[E2]": "Required float point argument. Elastic Modulus of Material 2",
                 "[Element Type]": "Required string argument. Supported element types: Solid, Shell",
                 "[Laminas Count]": "Required integer argument",
                 "[Laminas Thickness]": "Required floatpoint argument",
-                "[Micromechanical Model]": "Required string argument. Supported micromechanical models: voight, mori_tanaka",
+                "[Micromechanical Model]": "Required string argument. Supported micromechanical models: voigt, mori_tanaka, hashin_shtrikman_lower_bound, hashin_shtrikman_upper_bound",
                 "[Number of Integration Points]": "Required integer argument",
                 "[Power Law Exponent]": "Required float point argument. Exponent of Power Law, a mathematical function that determines the volume fractions of the Functionally Graded Material represented by virtual laminas",
                 "[Smart Laminas]": "Required boolean argument. If True, the laminas will be generated by a new smart method",
                 "[nu1]": "Required float point argument. Poisson's Coefficient of Material 1",
                 "[nu2]": "Required float point argument. Poisson's Coefficient of Material 2",
                 "[pho1]": "Required float point argument. Density of Material 1",
                 "[pho2]": "Required float point argument. Density of Material 2"
```

### Comparing `lmcv_tools-0.0.7/lmcv_tools/databases/translation_reference.json` & `lmcv_tools-0.0.8/lmcv_tools/databases/translation_reference.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9560185185185185%*

 * *Differences: {"'dat'": "{'elements': {'TET4': OrderedDict([('geometry', 'Tetrahedron'), ('grade', 1), "*

 * *          "('n_nodes', 4)]), 'TET10': OrderedDict([('geometry', 'Tetrahedron'), ('grade', 2), "*

 * *          "('n_nodes', 10)])}}",*

 * * "'inp'": "{'elements': {'C3D4': OrderedDict([('geometry', 'Tetrahedron'), ('grade', 1), "*

 * *          "('n_nodes', 4)]), 'C3D10': OrderedDict([('geometry', 'Tetrahedron'), ('grade', 2), "*

 * *          "('n_nodes', 10)])}}",*

 * * "'inp_to_dat'": "{'nodes_reordering': {'Tetrahedron': OrderedDict([('1' […]*

```diff
@@ -29,34 +29,54 @@
                 "grade": 1,
                 "n_nodes": 3
             },
             "T6": {
                 "geometry": "Triangle",
                 "grade": 2,
                 "n_nodes": 6
+            },
+            "TET10": {
+                "geometry": "Tetrahedron",
+                "grade": 2,
+                "n_nodes": 10
+            },
+            "TET4": {
+                "geometry": "Tetrahedron",
+                "grade": 1,
+                "n_nodes": 4
             }
         },
         "theories": {
             "PLSTRAIN": "PlaneStrain",
             "PLSTRESS": "PlaneStress",
             "SHALLOWSHELL": "ShallowShell"
         }
     },
     "inp": {
         "elements": {
+            "C3D10": {
+                "geometry": "Tetrahedron",
+                "grade": 2,
+                "n_nodes": 10
+            },
             "C3D20": {
                 "geometry": "Hexahedron",
                 "grade": 2,
                 "n_nodes": 20
             },
             "C3D20R": {
                 "geometry": "Hexahedron",
                 "grade": 2,
                 "n_nodes": 20
             },
+            "C3D4": {
+                "geometry": "Tetrahedron",
+                "grade": 1,
+                "n_nodes": 4
+            },
             "C3D8": {
                 "geometry": "Hexahedron",
                 "grade": 1,
                 "n_nodes": 8
             },
             "C3D8R": {
                 "geometry": "Hexahedron",
@@ -151,14 +171,34 @@
                     8,
                     1,
                     5,
                     2,
                     6
                 ]
             },
+            "Tetrahedron": {
+                "1": [
+                    1,
+                    2,
+                    3,
+                    4
+                ],
+                "2": [
+                    1,
+                    5,
+                    2,
+                    10,
+                    3,
+                    7,
+                    8,
+                    9,
+                    6,
+                    4
+                ]
+            },
             "Triangle": {
                 "1": [
                     2,
                     3,
                     1
                 ],
                 "2": [
```

### Comparing `lmcv_tools-0.0.7/lmcv_tools/interface/core.py` & `lmcv_tools-0.0.8/lmcv_tools/interface/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from . import messenger, searcher
 from ..models.custom_errors import CommandError
 
 # Constantes Globais
-version = '0.0.7'
+version = '0.0.8'
 in_interactive_mode = False
 message_welcome = '''
 LMCV Tools is a command line tool that provides a series of useful functionali-
 ties for the day-to-day simulations of the "Laboratório de Mecânica Computacio-
 nal e Visualização" of the "Universidade Federal do Ceará" (UFC). 
 
 Since a command was not typed, interactive mode was started. Here, you can type
```

### Comparing `lmcv_tools-0.0.7/lmcv_tools/models/extraction_components.py` & `lmcv_tools-0.0.8/lmcv_tools/models/extraction_components.py`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/lmcv_tools/models/generation_artifacts.py` & `lmcv_tools-0.0.8/lmcv_tools/models/generation_artifacts.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,50 +22,73 @@
       self.K = self.E / (3 * (1 - 2 * self.nu))
 
       # Calculando Módulo de Cisalhamento
       self.G = self.E / (2 * (1 + self.nu))
 
 class MicromechanicalModel:
    # Funções de Homogeneização Privadas
-   def _voight(self, volume_fractions: list[float]):
+   def _voigt(self, volume_fractions: list[float]):
       E, nu, pho = 0, 0, 0
       for V, M in zip(volume_fractions, self.materials):
          E += V * M.E
          nu += V * M.nu
          pho += V * M.pho
       return E, nu, pho
+   
+   def _hashin_shtrikman(bound: str):
+      def function(self, volume_fractions: list[float]):
+         # Definindo Valores Especiais
+         V, M = volume_fractions, self.materials
+         V1, V2 = V[0], V[1]
+         K1, K2 = M[0].K, M[1].K
+         G1, G2 = M[0].G, M[1].G
+         pho_1, pho_2 = M[0].pho, M[1].pho
+
+         # Valores Iniciais do que é Matriz e do que são as Inclusões
+         Vm, Vi = V1, V2
+         Km, Ki = K1, K2
+         Gm, Gi = G1, G2
+         pho_m, pho_i = pho_1, pho_2
+
+         # Trocando Ordem com base no Bound Escolhido
+         if (
+            bound == 'upper' and M[0].E < M[1].E or
+            bound == 'lower' and M[0].E > M[1].E
+         ):
+            Vm, Vi = V2, V1
+            Km, Ki = K2, K1
+            Gm, Gi = G2, G1
+            pho_m, pho_i = pho_2, pho_1
+
+         # Calculando Valores Auxilizares
+         FK = (3 * Vm) / (3 * Km + 4 * Gm)
+         FG = 6 * Vm * (Km + 2 * Gm) / (5 * Gm * (3 * Km + 4 * Gm))
+
+         # Calculando Módulo Volumétrico
+         K = Km + Vi / ((1 / (Ki - Km)) + FK)
+
+         # Calculando Módulo de Cisalhamento
+         G = Gm + Vi / ((1 / (Gi - Gm)) + FG)
+
+         # Calculando Propriedades Efetivas
+         E = (9 * G * K) / (G + 3 * K)
+         nu = (3 * K - 2 * G) / (2 * (G + 3 * K))
 
-   def _mori_tanaka(self, volume_fractions: list[float]):
-      # Definindo Valores Especiais
-      V, M = volume_fractions, self.materials
-      V1, V2 = V[0], V[1]
-      K1, K2 = M[0].K, M[1].K
-      G1, G2 = M[0].G, M[1].G
-      FG = (G1 * (9 * K1 + 8 * G1)) / (6 * (K1 + 2 * G1))
-      FK = 4 * G1 / 3
-
-      # Calculando Módulo Volumétrico
-      K = K1 + V2 / ((1 / (K2 - K1)) + (V1 / (K1 + FK)))
-
-      # Calculando Módulo de Cisalhamento
-      G = G1 + V2 / ((1 / (G2 - G1)) + (V1 / (G1 + FG)))
-
-      # Calculando Propriedades Efetivas
-      E = (9 * K * G) / (3 * K + G)
-      nu = (3 * K - 2 * G) / (2 * (3 * K + G))
-
-      # Densidade Calculada pelo Modelo de Voight
-      pho = V1 * M[0].pho + V2 * M[1].pho
+         # Densidade Calculada pelo Modelo de voigt
+         pho = Vi * pho_i + Vm * pho_m
 
-      return E, nu, pho
+         return E, nu, pho
+      return function
 
    # Relação Modelo/Função de Homogeneização
    homogenize_functions = {
-      'voight': _voight,
-      'mori_tanaka': _mori_tanaka
+      'voigt': _voigt,
+      'mori_tanaka': _hashin_shtrikman('lower'),
+      'hashin_shtrikman_upper_bound': _hashin_shtrikman('upper'),
+      'hashin_shtrikman_lower_bound': _hashin_shtrikman('lower'),
    }
 
    def __init__(self, name: str, materials: list[Material]) -> None:
       self.name = name
       self.materials = materials
       try:
          self._homogenize = MicromechanicalModel.homogenize_functions[name]
@@ -105,15 +128,15 @@
    
    def volume_fraction(self, z: float):
       return (1 - z) ** self.power_law_exponent
    
    def z_coordinate(self, V: float):
       return 1 - V ** (1 / self.power_law_exponent)
 
-   def equally_thickness_laminas(self):
+   def same_thickness_laminas(self):
       step = 1 / self.laminas_count
       points = [step / 2 + i * step for i in range(self.laminas_count)]
       fractions = [self.volume_fraction(z) for z in points]
       if self.element_configuration.type == 'Solid':
          thickness = [self.thickness for _ in range(self.laminas_count)]
       else:
          thickness = [step * self.thickness for _ in range(self.laminas_count)]
@@ -197,41 +220,41 @@
       return fractions, thickness
 
    def generate(self):
       # Inicializando Dados
       inp_data = ''
 
       # Gerados Dados de Lâminas
-      laminas = self.smart_laminas() if self.smart else self.equally_thickness_laminas()
+      laminas = self.smart_laminas() if self.smart else self.same_thickness_laminas()
 
       # Escrevendo Materiais
       material_names = list()
       index = 1
       for V in laminas[0]:
          # Gerando e Armazando Nome de Material
          name =  f'FGM-L{index}'
          material_names.append(name)
 
          # Homogeneizando Propriedades
          E, nu, pho = self.micromechanical_model.homogenize([V, 1 - V])
 
          # Adicionando Dados
-         inp_data += f'*Material, name={name}\n    *Density\n    {pho:.3f},\n    *Elastic\n    {E:.3f}, {nu:.3f}\n'
+         inp_data += f'*Material, name={name}\n    *Density\n    {pho:.7E},\n    *Elastic\n    {E:.7E}, {nu:.3f}\n'
          
          index += 1
       
       # Preparando para Escrever Lâminas
       inp_data += '*Part, name=Virtual_Part\n*Node\n    1, 1.0, 1.0, 0.0\n    2, 0.0, 1.0, 0.0\n    3, 0.0, 0.0, 0.0\n    4, 1.0, 0.0, 0.0\n*Element, type=S4R\n    1, 1, 2, 3, 4\n*Elset, elset=Virtual\n    1'
       element_type = self.element_configuration.type
       int_points = self.element_configuration.number_integration_points
       rotation_angle = 0
 
       # Escrevendo Lâmina por Lâmina
       inp_data += f'\n*{element_type} Section, elset=Virtual, composite\n'
       index = 1
       for h, material in zip(laminas[1], material_names):
-         inp_data += f'    {h:.11E}, {int_points}, {material}, {rotation_angle}, Ply-{index}\n'
+         inp_data += f'    {h:.7E}, {int_points}, {material}, {rotation_angle}, Ply-{index}\n'
          index += 1
       inp_data += '*End Part'
 
       # Inseridos dados Inp no Atributo de Dados
       self.data = inp_data
```

### Comparing `lmcv_tools-0.0.7/lmcv_tools/models/graphical_interfaces.py` & `lmcv_tools-0.0.8/lmcv_tools/models/graphical_interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
    Spinbox,
    Combobox,
    Button,
    Checkbutton
 )
 from ..interface import messenger
 
-class PromptGenerateVirtualLamina:
+class PromptGenerateVirtualLaminas:
    def __init__(self, params: dict):
       # Dicionário de Parâmetros para Geração das Lâminas
       self.params = params
 
       # Definindo Janela Principal
       self.root = Tk()
       self.root.title('Generate Virtual Laminas')
@@ -169,31 +169,31 @@
          master = self.frame['grading_params'], 
          from_ = 0,
          to = 10,
          increment = 0.1,
          width = 6,
          font = self.default_font,
       )
-      self.entry['power_law_exponent'].grid(row = 1, column = 1, sticky = 'w')
+      self.entry['power_law_exponent'].grid(row = 2, column = 0, sticky = 'w')
 
       self.label['micromechanical_model'] = Label(
          master = self.frame['grading_params'], 
          text = 'Micromechanical Model:',
          padding = (0, 5, 10, 5),
       )
-      self.label['micromechanical_model'].grid(row = 2, column = 0, sticky = 'w')
+      self.label['micromechanical_model'].grid(row = 3, column = 0, sticky = 'w')
 
       self.entry['micromechanical_model'] = Combobox(
          master = self.frame['grading_params'],
          state = 'readonly',
-         values = ['voight', 'mori_tanaka'],
+         values = ['voigt', 'mori_tanaka', 'hashin_shtrikman_lower_bound', 'hashin_shtrikman_upper_bound'],
          font = self.default_font,
-         width = 12,
+         width = 25,
       )
-      self.entry['micromechanical_model'].grid(row = 2, column = 1, sticky = 'w')
+      self.entry['micromechanical_model'].grid(row = 4, column = 0, sticky = 'w')
 
    def layout_materials_params(self):
       self.frame['materials_params'] = Frame(
          master = self.root,
          padding = (10, 10),
       )
       self.frame['materials_params'].pack(fill = 'x')
```

### Comparing `lmcv_tools-0.0.7/lmcv_tools/models/translation_components.py` & `lmcv_tools-0.0.8/lmcv_tools/models/translation_components.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ..interface import searcher
 import re
+from math import factorial, floor
 
 class SimulationModel:
    def __init__(self):
       self.nodes = dict()
       self.element_groups = dict()
    
    def add_node(self, ide: int, x: float, y: float, z: float, weight: float = None):
@@ -307,14 +308,67 @@
       self.model = SimulationModel()
       self.node_radius = 1
       self.node_color = '#a95e5e'
       self.element_color = '#fcff5e'
       self.element_stroke_width = 1
       self.element_stroke_color = 'black'
    
+   def bezier_equiv_coord(self, c: float, c0: float, c2: float):
+      return 2 * c - 0.5 * (c0 + c2)
+
+   def calculate_colinearity(self, points: list[SimulationModel.Node]) -> float:
+      factor = 0
+      for i in range(0, len(points) - 2):
+         diag1 = points[i].x * points[i + 1].y + points[i + 1].x * points[i + 2].y + points[i + 2].x * points[i].y
+         diag2 = points[i].x * points[i + 2].y + points[i + 1].x * points[i].y + points[i + 2].x * points[i + 1].y
+         factor += abs(diag1 - diag2)
+      return abs(factor)
+   
+   def bernstein_polynomial(self, index: int, grade: int, region: float):
+      # Renomeando Parâmetros para Facilitar os Cálculos
+      i, p, t = index, grade, region
+      
+      # Verificando Validade dos Parâmetros
+      if i < 0 or i > p:
+         raise ValueError(f'Index {i} does not exist for Bernstein Polynomial with Grade {p}.')
+      
+      # Calculando Polinômio na Região Informada
+      return (factorial(p) / (factorial(i) * factorial(p - i))) * t ** i * (1 - t) ** (p - i)
+
+   def tesselate_bezier_curve(self, grade: int, points: list[SimulationModel.Node], n_regions: int):
+      # Variáveis Iniciais
+      tesselated_points = list()
+      p = grade
+      h = 1 / (n_regions - 1)
+
+      # Gerando Pontos da Curva
+      for nr in range(n_regions):
+         # Calculando Região do Espaço Paramétrico
+         t = nr * h
+         
+         # Calculando Ponto Cartesiano Correspondente
+         weight_sum, coord_x, coord_y = 0, 0, 0
+         for point, i in zip(points, range(0, p + 1)):
+            bp = self.bernstein_polynomial(i, p, t)
+            w = point.weight or 1
+            weight_sum += bp * w
+            coord_x += bp * point.x * w
+            coord_y += bp * point.y * w
+         coord_x /= weight_sum
+         coord_y /= weight_sum
+         tesselated_points.append([coord_x, coord_y])
+      
+      # Corrigindo Pontos Ímpares para Coordenada Equivalente na Representação de Curva de Bezier Quadrática
+      for i in range(1, len(tesselated_points), 2):
+         tesselated_points[i][0] = self.bezier_equiv_coord(tesselated_points[i][0], tesselated_points[i - 1][0], tesselated_points[i + 1][0])
+         tesselated_points[i][1] = self.bezier_equiv_coord(tesselated_points[i][1], tesselated_points[i - 1][1], tesselated_points[i + 1][1])
+      
+      # Retornando Pontos Tesselados (Excluindo o Primeiro)
+      return tesselated_points[1:]
+
    def write_nodes(self) -> str:
       # Inicializando Node Output
       output = f'\n   <g id="Nodes" fill="{self.node_color}">'
 
       # Escrevendo Cada Node
       for node in self.model.nodes.values():
          output += f'\n      <circle cx="{node.x:.8e}" cy="{node.y:.8e}" r="{self.node_radius}" />'
@@ -329,40 +383,53 @@
       nodes_total = int(3 + 3 * (p - 1) + ((p - 2) * (p - 1) / 2))
       indexes_corner = [1, nodes_total - p, nodes_total]
 
       # Index dos Nodes Intermediários
       ie1 = [int(1 + ((i + 1) * (i + 2) / 2)) for i in range(p - 1)]
       ie2 = [nodes_total - p + 1 + i for i in range(p - 1)]
       ie3 = [int((i + 2) * (i + 3) / 2) for i in range(p - 1)]
+      ie3.reverse()
       indexes_by_edge = [ie1, ie2, ie3]
 
       # Escrevendo Path de Cada Elemento
       for node_ides in group.elements.values():
          # Inicializando Path
          output += f'\n      <path d="'
 
          # Lado 1 - Ponto Incial
-         node = self.model.nodes[node_ides[indexes_corner[0] - 1]]
-         output += f'M {node.x:.8e} {node.y:.8e} '
+         node_corner_1 = self.model.nodes[node_ides[indexes_corner[0] - 1]]
+         output += f'M {node_corner_1.x:.8e} {node_corner_1.y:.8e} '
 
          # Construindo Curvas de Bezier para Cada Lado
          for indexes_edge, index_corner in zip(indexes_by_edge, indexes_corner[1:] + [indexes_corner[0]]):
-            # Calculando Coordenadas Médias dos Pontos Intermediários
-            x_m = 0
-            y_m = 0
-            for i in indexes_edge:
-               node = self.model.nodes[node_ides[i - 1]]
-               x_m += node.x
-               y_m += node.y
-            x_m /= (p - 1)
-            y_m /= (p - 1)
-
-            # Curva de Bezier Quadrática
-            node = self.model.nodes[node_ides[index_corner - 1]]
-            output += f'Q {x_m:.8e} {y_m:.8e}, {node.x:.8e} {node.y:.8e} '
+            # Obtendo Pontos do Lado
+            node_corner_2 = self.model.nodes[node_ides[index_corner - 1]]
+            points = [self.model.nodes[node_ides[i - 1]] for i in indexes_edge]
+            points.append(node_corner_2)
+            points.insert(0, node_corner_1)
+
+            # Calculando Fator de Colinearidade dos Pontos
+            c_factor = self.calculate_colinearity(points)
+
+            # Resumindo Path em Uma linha reta para um fator baixo
+            if c_factor < 0.1:
+               output += f'L {node_corner_2.x:.8e} {node_corner_2.y:.8e} '
+
+            # Tesselando Curva com Base no Fator
+            else:
+               # Definindo Discretização da Tesselação com Base no Fator de Colinearidade
+               n_regions = (2 * p - 1) + (2 * floor(c_factor / 50))
+
+               # Gerando Pontos de Tesselação
+               tp = self.tesselate_bezier_curve(p, points, n_regions)
+
+               for i in range(0, len(tp), 2):
+                  output += f'Q {tp[i][0]:.8e} {tp[i][1]:.8e}, {tp[i + 1][0]:.8e} {tp[i + 1][1]:.8e} '
+            
+            node_corner_1 = node_corner_2
 
          output += 'Z" />'
       
       return output
 
    def write_finite_elements(self, group: SimulationModel.ElementGroup):
       output = ''
@@ -376,29 +443,26 @@
             for ide in node_ides:
                node = self.model.nodes[ide]
                output += f'{node.x:.8e},{node.y:.8e} ' 
             output += '" />'
 
       # Tratamento para Elementos Lineares
       else:
-         # Função Para Encontrar Ponto de Bezier Equivalente
-         bezier_equiv_coord = lambda c, c0, c2: 2 * c - 0.5 * (c0 + c2)
-
          for node_ides in group.elements.values():
             # Escrevendo Ponto Inicial
             node = self.model.nodes[node_ides[0]]
             output += f'\n      <path d="M {node.x:.8e} {node.y:.8e} '
 
             # Escrevendo Lados como Curvas Quadráticas de Bezier
             for i in list(range(2, len(node_ides), 2)) + [0]:
                n2 = self.model.nodes[node_ides[i]]
                nc = self.model.nodes[node_ides[i - 1]]
                n0 = self.model.nodes[node_ides[i - 2]]
-               x1 = bezier_equiv_coord(nc.x, n0.x, n2.x)
-               y1 = bezier_equiv_coord(nc.y, n0.y, n2.y)
+               x1 = self.bezier_equiv_coord(nc.x, n0.x, n2.x)
+               y1 = self.bezier_equiv_coord(nc.y, n0.y, n2.y)
                output += f'Q {x1:.8e} {y1:.8e}, {n2.x:.8e} {n2.y:.8e} ' 
             output += 'Z" />'
       return output
 
    def write_elements(self) -> str:
       # Inicializando Node Output
       output = f'\n   <g id="Elements" fill="{self.element_color}" stroke="{self.element_stroke_color}" stroke-width="{self.element_stroke_width}">'
```

### Comparing `lmcv_tools-0.0.7/tests/test_extract.py` & `lmcv_tools-0.0.8/tests/test_extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,14 +108,44 @@
       self.default_test(*benchmark, attributes, condition)
    
    def test_buckling_node_w(self):
       benchmark = ('SquarePlate', 'buckling_node_w')
       attributes = ['buckling.node.w']
       condition = ''
       self.default_test(*benchmark, attributes, condition)
+   
+   def test_vibration_id(self):
+      benchmark = ('HeartPlate', 'vibration_id')
+      attributes = ['vibration.id']
+      condition = ''
+      self.default_test(*benchmark, attributes, condition)
+   
+   def test_vibration_factor(self):
+      benchmark = ('HeartPlate', 'vibration_factor')
+      attributes = ['vibration.factor']
+      condition = ''
+      self.default_test(*benchmark, attributes, condition)
+   
+   def test_vibration_node_u(self):
+      benchmark = ('HeartPlate', 'vibration_node_u')
+      attributes = ['vibration.node.u']
+      condition = ''
+      self.default_test(*benchmark, attributes, condition)
+   
+   def test_vibration_node_v(self):
+      benchmark = ('HeartPlate', 'vibration_node_v')
+      attributes = ['vibration.node.v']
+      condition = ''
+      self.default_test(*benchmark, attributes, condition)
+   
+   def test_vibration_node_w(self):
+      benchmark = ('HeartPlate', 'vibration_node_w')
+      attributes = ['vibration.node.w']
+      condition = ''
+      self.default_test(*benchmark, attributes, condition)
 
 class TestMultipleAttributes(DefaultTest):
    def test_multiple_1(self):
       benchmark = ('CirclePlate_Plastic', 'multiple_1')
       attributes = ['step.id', 'step.factor']
       condition = ''
       self.default_test(*benchmark, attributes, condition)
```

### Comparing `lmcv_tools-0.0.7/tests/test_generate.py` & `lmcv_tools-0.0.8/tests/test_generate.py`

 * *Files 25% similar despite different names*

```diff
@@ -27,44 +27,72 @@
       os.remove(artifact_path)
 
 class TestVirtualLaminas(DefaultTest):
    def test_shell_element(self):
       name = 'virtual_laminas'
       ext = 'inp'
       test_id = 'shell'
-      args = ['2', 'Shell', '0.5', '3', '1.0', 'voight', '380.0', '90.0', '0.30', '0.27', '1000', '2000', 'False']
+      args = ['2', 'Shell', '0.5', '3', '1.0', 'voigt', '90.0', '380.0', '0.27', '0.30', '2000', '1000', 'False']
       self.default_test(name, ext, test_id, args)
 
    def test_solid_element(self):
       name = 'virtual_laminas'
       ext = 'inp'
       test_id = 'solid'
-      args = ['2', 'Solid', '0.5', '3', '1.0', 'voight', '380.0', '90.0', '0.30', '0.27', '1000', '2000', 'False']
+      args = ['2', 'Solid', '0.5', '3', '1.0', 'voigt', '90.0', '380.0', '0.27', '0.30', '2000', '1000', 'False']
       self.default_test(name, ext, test_id, args)
 
-   def test_voight_model(self):
+   def test_voigt_model(self):
       name = 'virtual_laminas'
       ext = 'inp'
-      test_id = 'voight'
-      args = ['40', 'Solid', '0.25', '3', '1.0', 'voight', '380.0', '90.0', '0.30', '0.27', '1000', '2000', 'False']
+      test_id = 'voigt'
+      args = ['40', 'Solid', '0.25', '3', '1.0', 'voigt', '90.0', '380.0', '0.27', '0.30', '2000', '1000', 'False']
       self.default_test(name, ext, test_id, args)
    
    def test_mori_tanaka_model(self):
       name = 'virtual_laminas'
       ext = 'inp'
       test_id = 'mori_tanaka'
-      args = ['40', 'Solid', '0.25', '3', '1.0', 'mori_tanaka', '380.0', '90.0', '0.30', '0.27', '1000', '2000', 'False']
+      args = ['40', 'Solid', '0.25', '3', '1.0', 'mori_tanaka', '90.0', '380.0', '0.27', '0.30', '2000', '1000', 'False']
       self.default_test(name, ext, test_id, args)
    
+   def test_hashin_shtrikman_upper_bound_model_1(self):
+      name = 'virtual_laminas'
+      ext = 'inp'
+      test_id = 'hs_ub_1'
+      args = ['40', 'Solid', '0.25', '3', '1.0', 'hashin_shtrikman_upper_bound', '90.0', '380.0', '0.27', '0.30', '2000', '1000', 'False']
+      self.default_test(name, ext, test_id, args)
+   
+   def test_hashin_shtrikman_lower_bound_model_1(self):
+      name = 'virtual_laminas'
+      ext = 'inp'
+      test_id = 'hs_lb_1'
+      args = ['40', 'Solid', '0.25', '3', '1.0', 'hashin_shtrikman_lower_bound', '90.0', '380.0', '0.27', '0.30', '2000', '1000', 'False']
+      self.default_test(name, ext, test_id, args)
+   
+   def test_hashin_shtrikman_upper_bound_model_2(self):
+      name = 'virtual_laminas'
+      ext = 'inp'
+      test_id = 'hs_ub_2'
+      args = ['40', 'Solid', '0.25', '3', '1.0', 'hashin_shtrikman_upper_bound', '380.0', '90.0', '0.30', '0.27', '1000', '2000', 'False']
+      self.default_test(name, ext, test_id, args)
+   
+   def test_hashin_shtrikman_lower_bound_model_2(self):
+      name = 'virtual_laminas'
+      ext = 'inp'
+      test_id = 'hs_lb_2'
+      args = ['40', 'Solid', '0.25', '3', '1.0', 'hashin_shtrikman_lower_bound', '380.0', '90.0', '0.30', '0.27', '1000', '2000', 'False']
+      self.default_test(name, ext, test_id, args)
+
    def test_smart_laminas_1(self):
       name = 'virtual_laminas'
       ext = 'inp'
       test_id = 'smart_1'
-      args = ['100', 'Shell', '3.5', '3', '0.2', 'voight', '380.0', '90.0', '0.30', '0.27', '1000', '2000', 'True']
+      args = ['100', 'Shell', '3.5', '3', '0.2', 'voigt', '90.0', '380.0', '0.27', '0.30', '2000', '1000', 'True']
       self.default_test(name, ext, test_id, args)
    
    def test_smart_laminas_2(self):
       name = 'virtual_laminas'
       ext = 'inp'
       test_id = 'smart_2'
-      args = ['100', 'Shell', '3.5', '3', '5', 'voight', '380.0', '90.0', '0.30', '0.27', '1000', '2000', 'True']
+      args = ['100', 'Shell', '3.5', '3', '5', 'voigt', '90.0', '380.0', '0.27', '0.30', '2000', '1000', 'True']
       self.default_test(name, ext, test_id, args)
```

### Comparing `lmcv_tools-0.0.7/tests/test_translate.py` & `lmcv_tools-0.0.8/tests/test_translate.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,14 +55,20 @@
    
    def test_circle_S3_S4R_4x4(self):
       self.default_test('Circle_S3_S4R_4x4')
 
    def test_complex_part_S8R(self):
       self.default_test('ComplexPart_S8R')
 
+   def test_cube_C3D4_12(self):
+      self.default_test('Cube_C3D4_12')
+   
+   def test_cube_C3D10_12(self):
+      self.default_test('Cube_C3D10_12')
+
    def test_cube_C3D8_1x1x1(self):
       self.default_test('Cube_C3D8_1x1x1')
 
    def test_cube_C3D8_2x2x2(self):
       self.default_test('Cube_C3D8_2x2x2')
    
    def test_cube_C3D20_1x1x1(self):
@@ -85,8 +91,14 @@
    def test_heart_plate_Q8_2x2(self):
       self.default_test('HeartPlate_Q8_2x2')
 
    def test_heart_plate_BT2_2x2(self):
       self.default_test('HeartPlate_BT2_2x2')
 
    def test_heart_plate_BT3_4x4(self):
-      self.default_test('HeartPlate_BT3_4x4')
+      self.default_test('HeartPlate_BT3_4x4')
+
+   def test_disform_BT2(self):
+      self.default_test('Disform_BT2')
+   
+   def test_disform_BT4(self):
+      self.default_test('Disform_BT4')
```

### Comparing `lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic.pos` & `lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic.pos`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_2.csv` & `lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_2.csv`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_3.csv` & `lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_multiple_3.csv`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_u.csv` & `lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_u.csv`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_v.csv` & `lmcv_tools-0.0.8/tests/benchmark/extract/CirclePlate_Plastic_exp_step_node_v.csv`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/generate/virtual_laminas_exp_mori_tanaka.inp` & `lmcv_tools-0.0.8/tests/benchmark/generate/virtual_laminas_exp_hs_ub_1.inp`

 * *Files 9% similar despite different names*

```diff
@@ -1,252 +1,252 @@
 *Material, name=FGM-L1
     *Density
-    1012.500,
+    1.9875000E+03,
     *Elastic
-    374.177, 0.299
+    9.2251520E+01, 0.270
 *Material, name=FGM-L2
     *Density
-    1037.500,
+    1.9625000E+03,
     *Elastic
-    362.796, 0.298
+    9.6819753E+01, 0.270
 *Material, name=FGM-L3
     *Density
-    1062.500,
+    1.9375000E+03,
     *Elastic
-    351.754, 0.296
+    1.0147707E+02, 0.270
 *Material, name=FGM-L4
     *Density
-    1087.500,
+    1.9125000E+03,
     *Elastic
-    341.037, 0.295
+    1.0622617E+02, 0.270
 *Material, name=FGM-L5
     *Density
-    1112.500,
+    1.8875000E+03,
     *Elastic
-    330.629, 0.293
+    1.1106981E+02, 0.270
 *Material, name=FGM-L6
     *Density
-    1137.500,
+    1.8625000E+03,
     *Elastic
-    320.518, 0.292
+    1.1601089E+02, 0.270
 *Material, name=FGM-L7
     *Density
-    1162.500,
+    1.8375000E+03,
     *Elastic
-    310.691, 0.291
+    1.2105243E+02, 0.270
 *Material, name=FGM-L8
     *Density
-    1187.500,
+    1.8125000E+03,
     *Elastic
-    301.137, 0.289
+    1.2619754E+02, 0.270
 *Material, name=FGM-L9
     *Density
-    1212.500,
+    1.7875000E+03,
     *Elastic
-    291.844, 0.288
+    1.3144947E+02, 0.271
 *Material, name=FGM-L10
     *Density
-    1237.500,
+    1.7625000E+03,
     *Elastic
-    282.801, 0.287
+    1.3681162E+02, 0.271
 *Material, name=FGM-L11
     *Density
-    1262.500,
+    1.7375000E+03,
     *Elastic
-    274.000, 0.286
+    1.4228752E+02, 0.271
 *Material, name=FGM-L12
     *Density
-    1287.500,
+    1.7125000E+03,
     *Elastic
-    265.429, 0.285
+    1.4788084E+02, 0.272
 *Material, name=FGM-L13
     *Density
-    1312.500,
+    1.6875000E+03,
     *Elastic
-    257.081, 0.284
+    1.5359543E+02, 0.272
 *Material, name=FGM-L14
     *Density
-    1337.500,
+    1.6625000E+03,
     *Elastic
-    248.946, 0.283
+    1.5943528E+02, 0.273
 *Material, name=FGM-L15
     *Density
-    1362.500,
+    1.6375000E+03,
     *Elastic
-    241.017, 0.282
+    1.6540458E+02, 0.273
 *Material, name=FGM-L16
     *Density
-    1387.500,
+    1.6125000E+03,
     *Elastic
-    233.286, 0.281
+    1.7150770E+02, 0.274
 *Material, name=FGM-L17
     *Density
-    1412.500,
+    1.5875000E+03,
     *Elastic
-    225.745, 0.280
+    1.7774920E+02, 0.274
 *Material, name=FGM-L18
     *Density
-    1437.500,
+    1.5625000E+03,
     *Elastic
-    218.388, 0.279
+    1.8413385E+02, 0.275
 *Material, name=FGM-L19
     *Density
-    1462.500,
+    1.5375000E+03,
     *Elastic
-    211.208, 0.278
+    1.9066666E+02, 0.276
 *Material, name=FGM-L20
     *Density
-    1487.500,
+    1.5125000E+03,
     *Elastic
-    204.198, 0.277
+    1.9735285E+02, 0.277
 *Material, name=FGM-L21
     *Density
-    1512.500,
+    1.4875000E+03,
     *Elastic
-    197.353, 0.277
+    2.0419789E+02, 0.277
 *Material, name=FGM-L22
     *Density
-    1537.500,
+    1.4625000E+03,
     *Elastic
-    190.667, 0.276
+    2.1120753E+02, 0.278
 *Material, name=FGM-L23
     *Density
-    1562.500,
+    1.4375000E+03,
     *Elastic
-    184.134, 0.275
+    2.1838779E+02, 0.279
 *Material, name=FGM-L24
     *Density
-    1587.500,
+    1.4125000E+03,
     *Elastic
-    177.749, 0.274
+    2.2574497E+02, 0.280
 *Material, name=FGM-L25
     *Density
-    1612.500,
+    1.3875000E+03,
     *Elastic
-    171.508, 0.274
+    2.3328572E+02, 0.281
 *Material, name=FGM-L26
     *Density
-    1637.500,
+    1.3625000E+03,
     *Elastic
-    165.405, 0.273
+    2.4101699E+02, 0.282
 *Material, name=FGM-L27
     *Density
-    1662.500,
+    1.3375000E+03,
     *Elastic
-    159.435, 0.273
+    2.4894611E+02, 0.283
 *Material, name=FGM-L28
     *Density
-    1687.500,
+    1.3125000E+03,
     *Elastic
-    153.595, 0.272
+    2.5708077E+02, 0.284
 *Material, name=FGM-L29
     *Density
-    1712.500,
+    1.2875000E+03,
     *Elastic
-    147.881, 0.272
+    2.6542909E+02, 0.285
 *Material, name=FGM-L30
     *Density
-    1737.500,
+    1.2625000E+03,
     *Elastic
-    142.288, 0.271
+    2.7399959E+02, 0.286
 *Material, name=FGM-L31
     *Density
-    1762.500,
+    1.2375000E+03,
     *Elastic
-    136.812, 0.271
+    2.8280127E+02, 0.287
 *Material, name=FGM-L32
     *Density
-    1787.500,
+    1.2125000E+03,
     *Elastic
-    131.449, 0.271
+    2.9184363E+02, 0.288
 *Material, name=FGM-L33
     *Density
-    1812.500,
+    1.1875000E+03,
     *Elastic
-    126.198, 0.270
+    3.0113667E+02, 0.289
 *Material, name=FGM-L34
     *Density
-    1837.500,
+    1.1625000E+03,
     *Elastic
-    121.052, 0.270
+    3.1069097E+02, 0.291
 *Material, name=FGM-L35
     *Density
-    1862.500,
+    1.1375000E+03,
     *Elastic
-    116.011, 0.270
+    3.2051771E+02, 0.292
 *Material, name=FGM-L36
     *Density
-    1887.500,
+    1.1125000E+03,
     *Elastic
-    111.070, 0.270
+    3.3062872E+02, 0.293
 *Material, name=FGM-L37
     *Density
-    1912.500,
+    1.0875000E+03,
     *Elastic
-    106.226, 0.270
+    3.4103653E+02, 0.295
 *Material, name=FGM-L38
     *Density
-    1937.500,
+    1.0625000E+03,
     *Elastic
-    101.477, 0.270
+    3.5175438E+02, 0.296
 *Material, name=FGM-L39
     *Density
-    1962.500,
+    1.0375000E+03,
     *Elastic
-    96.820, 0.270
+    3.6279637E+02, 0.298
 *Material, name=FGM-L40
     *Density
-    1987.500,
+    1.0125000E+03,
     *Elastic
-    92.252, 0.270
+    3.7417741E+02, 0.299
 *Part, name=Virtual_Part
 *Node
     1, 1.0, 1.0, 0.0
     2, 0.0, 1.0, 0.0
     3, 0.0, 0.0, 0.0
     4, 1.0, 0.0, 0.0
 *Element, type=S4R
     1, 1, 2, 3, 4
 *Elset, elset=Virtual
     1
 *Solid Section, elset=Virtual, composite
-    2.50000000000E-01, 3, FGM-L1, 0, Ply-1
-    2.50000000000E-01, 3, FGM-L2, 0, Ply-2
-    2.50000000000E-01, 3, FGM-L3, 0, Ply-3
-    2.50000000000E-01, 3, FGM-L4, 0, Ply-4
-    2.50000000000E-01, 3, FGM-L5, 0, Ply-5
-    2.50000000000E-01, 3, FGM-L6, 0, Ply-6
-    2.50000000000E-01, 3, FGM-L7, 0, Ply-7
-    2.50000000000E-01, 3, FGM-L8, 0, Ply-8
-    2.50000000000E-01, 3, FGM-L9, 0, Ply-9
-    2.50000000000E-01, 3, FGM-L10, 0, Ply-10
-    2.50000000000E-01, 3, FGM-L11, 0, Ply-11
-    2.50000000000E-01, 3, FGM-L12, 0, Ply-12
-    2.50000000000E-01, 3, FGM-L13, 0, Ply-13
-    2.50000000000E-01, 3, FGM-L14, 0, Ply-14
-    2.50000000000E-01, 3, FGM-L15, 0, Ply-15
-    2.50000000000E-01, 3, FGM-L16, 0, Ply-16
-    2.50000000000E-01, 3, FGM-L17, 0, Ply-17
-    2.50000000000E-01, 3, FGM-L18, 0, Ply-18
-    2.50000000000E-01, 3, FGM-L19, 0, Ply-19
-    2.50000000000E-01, 3, FGM-L20, 0, Ply-20
-    2.50000000000E-01, 3, FGM-L21, 0, Ply-21
-    2.50000000000E-01, 3, FGM-L22, 0, Ply-22
-    2.50000000000E-01, 3, FGM-L23, 0, Ply-23
-    2.50000000000E-01, 3, FGM-L24, 0, Ply-24
-    2.50000000000E-01, 3, FGM-L25, 0, Ply-25
-    2.50000000000E-01, 3, FGM-L26, 0, Ply-26
-    2.50000000000E-01, 3, FGM-L27, 0, Ply-27
-    2.50000000000E-01, 3, FGM-L28, 0, Ply-28
-    2.50000000000E-01, 3, FGM-L29, 0, Ply-29
-    2.50000000000E-01, 3, FGM-L30, 0, Ply-30
-    2.50000000000E-01, 3, FGM-L31, 0, Ply-31
-    2.50000000000E-01, 3, FGM-L32, 0, Ply-32
-    2.50000000000E-01, 3, FGM-L33, 0, Ply-33
-    2.50000000000E-01, 3, FGM-L34, 0, Ply-34
-    2.50000000000E-01, 3, FGM-L35, 0, Ply-35
-    2.50000000000E-01, 3, FGM-L36, 0, Ply-36
-    2.50000000000E-01, 3, FGM-L37, 0, Ply-37
-    2.50000000000E-01, 3, FGM-L38, 0, Ply-38
-    2.50000000000E-01, 3, FGM-L39, 0, Ply-39
-    2.50000000000E-01, 3, FGM-L40, 0, Ply-40
+    2.5000000E-01, 3, FGM-L1, 0, Ply-1
+    2.5000000E-01, 3, FGM-L2, 0, Ply-2
+    2.5000000E-01, 3, FGM-L3, 0, Ply-3
+    2.5000000E-01, 3, FGM-L4, 0, Ply-4
+    2.5000000E-01, 3, FGM-L5, 0, Ply-5
+    2.5000000E-01, 3, FGM-L6, 0, Ply-6
+    2.5000000E-01, 3, FGM-L7, 0, Ply-7
+    2.5000000E-01, 3, FGM-L8, 0, Ply-8
+    2.5000000E-01, 3, FGM-L9, 0, Ply-9
+    2.5000000E-01, 3, FGM-L10, 0, Ply-10
+    2.5000000E-01, 3, FGM-L11, 0, Ply-11
+    2.5000000E-01, 3, FGM-L12, 0, Ply-12
+    2.5000000E-01, 3, FGM-L13, 0, Ply-13
+    2.5000000E-01, 3, FGM-L14, 0, Ply-14
+    2.5000000E-01, 3, FGM-L15, 0, Ply-15
+    2.5000000E-01, 3, FGM-L16, 0, Ply-16
+    2.5000000E-01, 3, FGM-L17, 0, Ply-17
+    2.5000000E-01, 3, FGM-L18, 0, Ply-18
+    2.5000000E-01, 3, FGM-L19, 0, Ply-19
+    2.5000000E-01, 3, FGM-L20, 0, Ply-20
+    2.5000000E-01, 3, FGM-L21, 0, Ply-21
+    2.5000000E-01, 3, FGM-L22, 0, Ply-22
+    2.5000000E-01, 3, FGM-L23, 0, Ply-23
+    2.5000000E-01, 3, FGM-L24, 0, Ply-24
+    2.5000000E-01, 3, FGM-L25, 0, Ply-25
+    2.5000000E-01, 3, FGM-L26, 0, Ply-26
+    2.5000000E-01, 3, FGM-L27, 0, Ply-27
+    2.5000000E-01, 3, FGM-L28, 0, Ply-28
+    2.5000000E-01, 3, FGM-L29, 0, Ply-29
+    2.5000000E-01, 3, FGM-L30, 0, Ply-30
+    2.5000000E-01, 3, FGM-L31, 0, Ply-31
+    2.5000000E-01, 3, FGM-L32, 0, Ply-32
+    2.5000000E-01, 3, FGM-L33, 0, Ply-33
+    2.5000000E-01, 3, FGM-L34, 0, Ply-34
+    2.5000000E-01, 3, FGM-L35, 0, Ply-35
+    2.5000000E-01, 3, FGM-L36, 0, Ply-36
+    2.5000000E-01, 3, FGM-L37, 0, Ply-37
+    2.5000000E-01, 3, FGM-L38, 0, Ply-38
+    2.5000000E-01, 3, FGM-L39, 0, Ply-39
+    2.5000000E-01, 3, FGM-L40, 0, Ply-40
 *End Part
```

### Comparing `lmcv_tools-0.0.7/tests/benchmark/generate/virtual_laminas_exp_smart_1.inp` & `lmcv_tools-0.0.8/tests/benchmark/generate/virtual_laminas_exp_smart_2.inp`

 * *Files 12% similar despite different names*

```diff
@@ -1,612 +1,612 @@
 *Material, name=FGM-L1
     *Density
-    1006.754,
+    1.9935354E+03,
     *Elastic
-    378.041, 0.300
+    9.1874724E+01, 0.270
 *Material, name=FGM-L2
     *Density
-    1020.841,
+    1.9806063E+03,
     *Elastic
-    373.956, 0.299
+    9.5624173E+01, 0.271
 *Material, name=FGM-L3
     *Density
-    1035.789,
+    1.9676772E+03,
     *Elastic
-    369.621, 0.299
+    9.9373622E+01, 0.271
 *Material, name=FGM-L4
     *Density
-    1051.726,
+    1.9547480E+03,
     *Elastic
-    365.000, 0.298
+    1.0312307E+02, 0.271
 *Material, name=FGM-L5
     *Density
-    1068.812,
+    1.9418189E+03,
     *Elastic
-    360.045, 0.298
+    1.0687252E+02, 0.272
 *Material, name=FGM-L6
     *Density
-    1087.253,
+    1.9288898E+03,
     *Elastic
-    354.697, 0.297
+    1.1062197E+02, 0.272
 *Material, name=FGM-L7
     *Density
-    1107.317,
+    1.9159606E+03,
     *Elastic
-    348.878, 0.297
+    1.1437142E+02, 0.273
 *Material, name=FGM-L8
     *Density
-    1129.366,
+    1.9030315E+03,
     *Elastic
-    342.484, 0.296
+    1.1812087E+02, 0.273
 *Material, name=FGM-L9
     *Density
-    1153.906,
+    1.8901024E+03,
     *Elastic
-    335.367, 0.295
+    1.2187031E+02, 0.273
 *Material, name=FGM-L10
     *Density
-    1181.675,
+    1.8771732E+03,
     *Elastic
-    327.314, 0.295
+    1.2561976E+02, 0.274
 *Material, name=FGM-L11
     *Density
-    1213.821,
+    1.8642441E+03,
     *Elastic
-    317.992, 0.294
+    1.2936921E+02, 0.274
 *Material, name=FGM-L12
     *Density
-    1252.292,
+    1.8513150E+03,
     *Elastic
-    306.835, 0.292
+    1.3311866E+02, 0.274
 *Material, name=FGM-L13
     *Density
-    1300.839,
+    1.8383858E+03,
     *Elastic
-    292.757, 0.291
+    1.3686811E+02, 0.275
 *Material, name=FGM-L14
     *Density
-    1335.103,
+    1.8254567E+03,
     *Elastic
-    282.820, 0.290
+    1.4061756E+02, 0.275
 *Material, name=FGM-L15
     *Density
-    1342.790,
+    1.8125276E+03,
     *Elastic
-    280.591, 0.290
+    1.4436701E+02, 0.276
 *Material, name=FGM-L16
     *Density
-    1350.476,
+    1.7995984E+03,
     *Elastic
-    278.362, 0.289
+    1.4811645E+02, 0.276
 *Material, name=FGM-L17
     *Density
-    1358.163,
+    1.7866693E+03,
     *Elastic
-    276.133, 0.289
+    1.5186590E+02, 0.276
 *Material, name=FGM-L18
     *Density
-    1365.850,
+    1.7737402E+03,
     *Elastic
-    273.904, 0.289
+    1.5561535E+02, 0.277
 *Material, name=FGM-L19
     *Density
-    1373.536,
+    1.7608110E+03,
     *Elastic
-    271.674, 0.289
+    1.5936480E+02, 0.277
 *Material, name=FGM-L20
     *Density
-    1381.223,
+    1.7478819E+03,
     *Elastic
-    269.445, 0.289
+    1.6311425E+02, 0.278
 *Material, name=FGM-L21
     *Density
-    1388.910,
+    1.7349528E+03,
     *Elastic
-    267.216, 0.288
+    1.6686370E+02, 0.278
 *Material, name=FGM-L22
     *Density
-    1396.596,
+    1.7220236E+03,
     *Elastic
-    264.987, 0.288
+    1.7061315E+02, 0.278
 *Material, name=FGM-L23
     *Density
-    1404.283,
+    1.7090945E+03,
     *Elastic
-    262.758, 0.288
+    1.7436260E+02, 0.279
 *Material, name=FGM-L24
     *Density
-    1411.970,
+    1.6961654E+03,
     *Elastic
-    260.529, 0.288
+    1.7811204E+02, 0.279
 *Material, name=FGM-L25
     *Density
-    1419.656,
+    1.6832362E+03,
     *Elastic
-    258.300, 0.287
+    1.8186149E+02, 0.280
 *Material, name=FGM-L26
     *Density
-    1427.343,
+    1.6703071E+03,
     *Elastic
-    256.071, 0.287
+    1.8561094E+02, 0.280
 *Material, name=FGM-L27
     *Density
-    1435.030,
+    1.6573780E+03,
     *Elastic
-    253.841, 0.287
+    1.8936039E+02, 0.280
 *Material, name=FGM-L28
     *Density
-    1442.716,
+    1.6444488E+03,
     *Elastic
-    251.612, 0.287
+    1.9310984E+02, 0.281
 *Material, name=FGM-L29
     *Density
-    1450.403,
+    1.6315197E+03,
     *Elastic
-    249.383, 0.286
+    1.9685929E+02, 0.281
 *Material, name=FGM-L30
     *Density
-    1458.090,
+    1.6185906E+03,
     *Elastic
-    247.154, 0.286
+    2.0060874E+02, 0.281
 *Material, name=FGM-L31
     *Density
-    1465.776,
+    1.6056614E+03,
     *Elastic
-    244.925, 0.286
+    2.0435819E+02, 0.282
 *Material, name=FGM-L32
     *Density
-    1473.463,
+    1.5927323E+03,
     *Elastic
-    242.696, 0.286
+    2.0810763E+02, 0.282
 *Material, name=FGM-L33
     *Density
-    1481.150,
+    1.5798032E+03,
     *Elastic
-    240.467, 0.286
+    2.1185708E+02, 0.283
 *Material, name=FGM-L34
     *Density
-    1488.836,
+    1.5668740E+03,
     *Elastic
-    238.237, 0.285
+    2.1560653E+02, 0.283
 *Material, name=FGM-L35
     *Density
-    1496.523,
+    1.5539449E+03,
     *Elastic
-    236.008, 0.285
+    2.1935598E+02, 0.283
 *Material, name=FGM-L36
     *Density
-    1504.210,
+    1.5410158E+03,
     *Elastic
-    233.779, 0.285
+    2.2310543E+02, 0.284
 *Material, name=FGM-L37
     *Density
-    1511.896,
+    1.5280866E+03,
     *Elastic
-    231.550, 0.285
+    2.2685488E+02, 0.284
 *Material, name=FGM-L38
     *Density
-    1519.583,
+    1.5151575E+03,
     *Elastic
-    229.321, 0.284
+    2.3060433E+02, 0.285
 *Material, name=FGM-L39
     *Density
-    1527.270,
+    1.5022284E+03,
     *Elastic
-    227.092, 0.284
+    2.3435377E+02, 0.285
 *Material, name=FGM-L40
     *Density
-    1534.956,
+    1.4892992E+03,
     *Elastic
-    224.863, 0.284
+    2.3810322E+02, 0.285
 *Material, name=FGM-L41
     *Density
-    1542.643,
+    1.4763701E+03,
     *Elastic
-    222.633, 0.284
+    2.4185267E+02, 0.286
 *Material, name=FGM-L42
     *Density
-    1550.330,
+    1.4634410E+03,
     *Elastic
-    220.404, 0.283
+    2.4560212E+02, 0.286
 *Material, name=FGM-L43
     *Density
-    1558.016,
+    1.4505118E+03,
     *Elastic
-    218.175, 0.283
+    2.4935157E+02, 0.286
 *Material, name=FGM-L44
     *Density
-    1565.703,
+    1.4375827E+03,
     *Elastic
-    215.946, 0.283
+    2.5310102E+02, 0.287
 *Material, name=FGM-L45
     *Density
-    1573.390,
+    1.4246536E+03,
     *Elastic
-    213.717, 0.283
+    2.5685047E+02, 0.287
 *Material, name=FGM-L46
     *Density
-    1581.076,
+    1.4117244E+03,
     *Elastic
-    211.488, 0.283
+    2.6059992E+02, 0.288
 *Material, name=FGM-L47
     *Density
-    1588.763,
+    1.3987953E+03,
     *Elastic
-    209.259, 0.282
+    2.6434936E+02, 0.288
 *Material, name=FGM-L48
     *Density
-    1596.450,
+    1.3858662E+03,
     *Elastic
-    207.030, 0.282
+    2.6809881E+02, 0.288
 *Material, name=FGM-L49
     *Density
-    1604.136,
+    1.3729370E+03,
     *Elastic
-    204.800, 0.282
+    2.7184826E+02, 0.289
 *Material, name=FGM-L50
     *Density
-    1611.823,
+    1.3600079E+03,
     *Elastic
-    202.571, 0.282
+    2.7559771E+02, 0.289
 *Material, name=FGM-L51
     *Density
-    1619.510,
+    1.3470788E+03,
     *Elastic
-    200.342, 0.281
+    2.7934716E+02, 0.290
 *Material, name=FGM-L52
     *Density
-    1627.196,
+    1.3341496E+03,
     *Elastic
-    198.113, 0.281
+    2.8309661E+02, 0.290
 *Material, name=FGM-L53
     *Density
-    1634.883,
+    1.3212205E+03,
     *Elastic
-    195.884, 0.281
+    2.8684606E+02, 0.290
 *Material, name=FGM-L54
     *Density
-    1642.570,
+    1.3082914E+03,
     *Elastic
-    193.655, 0.281
+    2.9059550E+02, 0.291
 *Material, name=FGM-L55
     *Density
-    1650.257,
+    1.2953622E+03,
     *Elastic
-    191.426, 0.280
+    2.9434495E+02, 0.291
 *Material, name=FGM-L56
     *Density
-    1657.943,
+    1.2824331E+03,
     *Elastic
-    189.196, 0.280
+    2.9809440E+02, 0.292
 *Material, name=FGM-L57
     *Density
-    1665.630,
+    1.2695040E+03,
     *Elastic
-    186.967, 0.280
+    3.0184385E+02, 0.292
 *Material, name=FGM-L58
     *Density
-    1673.317,
+    1.2565748E+03,
     *Elastic
-    184.738, 0.280
+    3.0559330E+02, 0.292
 *Material, name=FGM-L59
     *Density
-    1681.003,
+    1.2436457E+03,
     *Elastic
-    182.509, 0.280
+    3.0934275E+02, 0.293
 *Material, name=FGM-L60
     *Density
-    1688.690,
+    1.2307166E+03,
     *Elastic
-    180.280, 0.279
+    3.1309220E+02, 0.293
 *Material, name=FGM-L61
     *Density
-    1696.377,
+    1.2177874E+03,
     *Elastic
-    178.051, 0.279
+    3.1684165E+02, 0.293
 *Material, name=FGM-L62
     *Density
-    1704.063,
+    1.2048583E+03,
     *Elastic
-    175.822, 0.279
+    3.2059109E+02, 0.294
 *Material, name=FGM-L63
     *Density
-    1711.750,
+    1.1919292E+03,
     *Elastic
-    173.593, 0.279
+    3.2434054E+02, 0.294
 *Material, name=FGM-L64
     *Density
-    1719.437,
+    1.1790000E+03,
     *Elastic
-    171.363, 0.278
+    3.2808999E+02, 0.295
 *Material, name=FGM-L65
     *Density
-    1727.123,
+    1.1660709E+03,
     *Elastic
-    169.134, 0.278
+    3.3183944E+02, 0.295
 *Material, name=FGM-L66
     *Density
-    1734.810,
+    1.1531418E+03,
     *Elastic
-    166.905, 0.278
+    3.3558889E+02, 0.295
 *Material, name=FGM-L67
     *Density
-    1742.497,
+    1.1402126E+03,
     *Elastic
-    164.676, 0.278
+    3.3933834E+02, 0.296
 *Material, name=FGM-L68
     *Density
-    1750.183,
+    1.1239181E+03,
     *Elastic
-    162.447, 0.277
+    3.4406376E+02, 0.296
 *Material, name=FGM-L69
     *Density
-    1757.870,
+    1.1059914E+03,
     *Elastic
-    160.218, 0.277
+    3.4926250E+02, 0.297
 *Material, name=FGM-L70
     *Density
-    1765.557,
+    1.0902022E+03,
     *Elastic
-    157.989, 0.277
+    3.5384137E+02, 0.297
 *Material, name=FGM-L71
     *Density
-    1773.243,
+    1.0763533E+03,
     *Elastic
-    155.759, 0.277
+    3.5785754E+02, 0.298
 *Material, name=FGM-L72
     *Density
-    1780.930,
+    1.0642602E+03,
     *Elastic
-    153.530, 0.277
+    3.6136454E+02, 0.298
 *Material, name=FGM-L73
     *Density
-    1788.617,
+    1.0537503E+03,
     *Elastic
-    151.301, 0.276
+    3.6441240E+02, 0.298
 *Material, name=FGM-L74
     *Density
-    1796.303,
+    1.0446629E+03,
     *Elastic
-    149.072, 0.276
+    3.6704775E+02, 0.299
 *Material, name=FGM-L75
     *Density
-    1803.990,
+    1.0368484E+03,
     *Elastic
-    146.843, 0.276
+    3.6931396E+02, 0.299
 *Material, name=FGM-L76
     *Density
-    1811.677,
+    1.0301681E+03,
     *Elastic
-    144.614, 0.276
+    3.7125125E+02, 0.299
 *Material, name=FGM-L77
     *Density
-    1819.363,
+    1.0244939E+03,
     *Elastic
-    142.385, 0.275
+    3.7289678E+02, 0.299
 *Material, name=FGM-L78
     *Density
-    1827.050,
+    1.0197074E+03,
     *Elastic
-    140.156, 0.275
+    3.7428484E+02, 0.299
 *Material, name=FGM-L79
     *Density
-    1834.737,
+    1.0157004E+03,
     *Elastic
-    137.926, 0.275
+    3.7544689E+02, 0.300
 *Material, name=FGM-L80
     *Density
-    1842.423,
+    1.0123733E+03,
     *Elastic
-    135.697, 0.275
+    3.7641173E+02, 0.300
 *Material, name=FGM-L81
     *Density
-    1850.110,
+    1.0096359E+03,
     *Elastic
-    133.468, 0.274
+    3.7720560E+02, 0.300
 *Material, name=FGM-L82
     *Density
-    1857.797,
+    1.0074059E+03,
     *Elastic
-    131.239, 0.274
+    3.7785230E+02, 0.300
 *Material, name=FGM-L83
     *Density
-    1865.483,
+    1.0056093E+03,
     *Elastic
-    129.010, 0.274
+    3.7837331E+02, 0.300
 *Material, name=FGM-L84
     *Density
-    1873.170,
+    1.0041796E+03,
     *Elastic
-    126.781, 0.274
+    3.7878791E+02, 0.300
 *Material, name=FGM-L85
     *Density
-    1880.857,
+    1.0030576E+03,
     *Elastic
-    124.552, 0.274
+    3.7911330E+02, 0.300
 *Material, name=FGM-L86
     *Density
-    1888.543,
+    1.0021906E+03,
     *Elastic
-    122.322, 0.273
+    3.7936473E+02, 0.300
 *Material, name=FGM-L87
     *Density
-    1896.230,
+    1.0015325E+03,
     *Elastic
-    120.093, 0.273
+    3.7955559E+02, 0.300
 *Material, name=FGM-L88
     *Density
-    1903.917,
+    1.0010430E+03,
     *Elastic
-    117.864, 0.273
+    3.7969754E+02, 0.300
 *Material, name=FGM-L89
     *Density
-    1911.603,
+    1.0006874E+03,
     *Elastic
-    115.635, 0.273
+    3.7980066E+02, 0.300
 *Material, name=FGM-L90
     *Density
-    1919.290,
+    1.0004362E+03,
     *Elastic
-    113.406, 0.272
+    3.7987351E+02, 0.300
 *Material, name=FGM-L91
     *Density
-    1926.977,
+    1.0002644E+03,
     *Elastic
-    111.177, 0.272
+    3.7992331E+02, 0.300
 *Material, name=FGM-L92
     *Density
-    1934.663,
+    1.0001516E+03,
     *Elastic
-    108.948, 0.272
+    3.7995602E+02, 0.300
 *Material, name=FGM-L93
     *Density
-    1942.350,
+    1.0000811E+03,
     *Elastic
-    106.719, 0.272
+    3.7997648E+02, 0.300
 *Material, name=FGM-L94
     *Density
-    1950.037,
+    1.0000397E+03,
     *Elastic
-    104.489, 0.271
+    3.7998850E+02, 0.300
 *Material, name=FGM-L95
     *Density
-    1957.723,
+    1.0000172E+03,
     *Elastic
-    102.260, 0.271
+    3.7999501E+02, 0.300
 *Material, name=FGM-L96
     *Density
-    1965.410,
+    1.0000063E+03,
     *Elastic
-    100.031, 0.271
+    3.7999817E+02, 0.300
 *Material, name=FGM-L97
     *Density
-    1973.097,
+    1.0000018E+03,
     *Elastic
-    97.802, 0.271
+    3.7999948E+02, 0.300
 *Material, name=FGM-L98
     *Density
-    1980.783,
+    1.0000003E+03,
     *Elastic
-    95.573, 0.271
+    3.7999990E+02, 0.300
 *Material, name=FGM-L99
     *Density
-    1988.470,
+    1.0000000E+03,
     *Elastic
-    93.344, 0.270
+    3.7999999E+02, 0.300
 *Material, name=FGM-L100
     *Density
-    1996.157,
+    1.0000000E+03,
     *Elastic
-    91.115, 0.270
+    3.8000000E+02, 0.300
 *Part, name=Virtual_Part
 *Node
     1, 1.0, 1.0, 0.0
     2, 0.0, 1.0, 0.0
     3, 0.0, 0.0, 0.0
     4, 1.0, 0.0, 0.0
 *Element, type=S4R
     1, 1, 2, 3, 4
 *Elset, elset=Virtual
     1
 *Shell Section, elset=Virtual, composite
-    2.33221675886E-01, 3, FGM-L1, 0, Ply-1
-    2.33221675886E-01, 3, FGM-L2, 0, Ply-2
-    2.33221675886E-01, 3, FGM-L3, 0, Ply-3
-    2.33221675886E-01, 3, FGM-L4, 0, Ply-4
-    2.33221675886E-01, 3, FGM-L5, 0, Ply-5
-    2.33221675886E-01, 3, FGM-L6, 0, Ply-6
-    2.33221675886E-01, 3, FGM-L7, 0, Ply-7
-    2.33221675886E-01, 3, FGM-L8, 0, Ply-8
-    2.33221675886E-01, 3, FGM-L9, 0, Ply-9
-    2.33221675886E-01, 3, FGM-L10, 0, Ply-10
-    2.33221675886E-01, 3, FGM-L11, 0, Ply-11
-    2.33221675886E-01, 3, FGM-L12, 0, Ply-12
-    2.33221675886E-01, 3, FGM-L13, 0, Ply-13
-    2.62919459504E-02, 3, FGM-L14, 0, Ply-14
-    2.50970943095E-02, 3, FGM-L15, 0, Ply-15
-    2.39434389113E-02, 3, FGM-L16, 0, Ply-16
-    2.28300217691E-02, 3, FGM-L17, 0, Ply-17
-    2.17558961667E-02, 3, FGM-L18, 0, Ply-18
-    2.07201266584E-02, 3, FGM-L19, 0, Ply-19
-    1.97217890689E-02, 3, FGM-L20, 0, Ply-20
-    1.87599704931E-02, 3, FGM-L21, 0, Ply-21
-    1.78337692967E-02, 3, FGM-L22, 0, Ply-22
-    1.69422951157E-02, 3, FGM-L23, 0, Ply-23
-    1.60846688563E-02, 3, FGM-L24, 0, Ply-24
-    1.52600226954E-02, 3, FGM-L25, 0, Ply-25
-    1.44675000803E-02, 3, FGM-L26, 0, Ply-26
-    1.37062557287E-02, 3, FGM-L27, 0, Ply-27
-    1.29754556286E-02, 3, FGM-L28, 0, Ply-28
-    1.22742770386E-02, 3, FGM-L29, 0, Ply-29
-    1.16019084876E-02, 3, FGM-L30, 0, Ply-30
-    1.09575497752E-02, 3, FGM-L31, 0, Ply-31
-    1.03404119710E-02, 3, FGM-L32, 0, Ply-32
-    9.74971741546E-03, 3, FGM-L33, 0, Ply-33
-    9.18469971916E-03, 3, FGM-L34, 0, Ply-34
-    8.64460376325E-03, 3, FGM-L35, 0, Ply-35
-    8.12868569930E-03, 3, FGM-L36, 0, Ply-36
-    7.63621294930E-03, 3, FGM-L37, 0, Ply-37
-    7.16646420566E-03, 3, FGM-L38, 0, Ply-38
-    6.71872943124E-03, 3, FGM-L39, 0, Ply-39
-    6.29230985932E-03, 3, FGM-L40, 0, Ply-40
-    5.88651799362E-03, 3, FGM-L41, 0, Ply-41
-    5.50067760827E-03, 3, FGM-L42, 0, Ply-42
-    5.13412374785E-03, 3, FGM-L43, 0, Ply-43
-    4.78620272737E-03, 3, FGM-L44, 0, Ply-44
-    4.45627213227E-03, 3, FGM-L45, 0, Ply-45
-    4.14370081841E-03, 3, FGM-L46, 0, Ply-46
-    3.84786891209E-03, 3, FGM-L47, 0, Ply-47
-    3.56816781005E-03, 3, FGM-L48, 0, Ply-48
-    3.30400017943E-03, 3, FGM-L49, 0, Ply-49
-    3.05477995784E-03, 3, FGM-L50, 0, Ply-50
-    2.81993235329E-03, 3, FGM-L51, 0, Ply-51
-    2.59889384425E-03, 3, FGM-L52, 0, Ply-52
-    2.39111217959E-03, 3, FGM-L53, 0, Ply-53
-    2.19604637862E-03, 3, FGM-L54, 0, Ply-54
-    2.01316673111E-03, 3, FGM-L55, 0, Ply-55
-    1.84195479721E-03, 3, FGM-L56, 0, Ply-56
-    1.68190340755E-03, 3, FGM-L57, 0, Ply-57
-    1.53251666315E-03, 3, FGM-L58, 0, Ply-58
-    1.39330993549E-03, 3, FGM-L59, 0, Ply-59
-    1.26380986648E-03, 3, FGM-L60, 0, Ply-60
-    1.14355436843E-03, 3, FGM-L61, 0, Ply-61
-    1.03209262412E-03, 3, FGM-L62, 0, Ply-62
-    9.28985086742E-04, 3, FGM-L63, 0, Ply-63
-    8.33803479915E-04, 3, FGM-L64, 0, Ply-64
-    7.46130797695E-04, 3, FGM-L65, 0, Ply-65
-    6.65561304569E-04, 3, FGM-L66, 0, Ply-66
-    5.91700535457E-04, 3, FGM-L67, 0, Ply-67
-    5.24165295705E-04, 3, FGM-L68, 0, Ply-68
-    4.62583661092E-04, 3, FGM-L69, 0, Ply-69
-    4.06594977830E-04, 3, FGM-L70, 0, Ply-70
-    3.55849862559E-04, 3, FGM-L71, 0, Ply-71
-    3.10010202351E-04, 3, FGM-L72, 0, Ply-72
-    2.68749154709E-04, 3, FGM-L73, 0, Ply-73
-    2.31751147567E-04, 3, FGM-L74, 0, Ply-74
-    1.98711879290E-04, 3, FGM-L75, 0, Ply-75
-    1.69338318673E-04, 3, FGM-L76, 0, Ply-76
-    1.43348704944E-04, 3, FGM-L77, 0, Ply-77
-    1.20472547760E-04, 3, FGM-L78, 0, Ply-78
-    1.00450627209E-04, 3, FGM-L79, 0, Ply-79
-    8.30349938115E-05, 3, FGM-L80, 0, Ply-80
-    6.79889685176E-05, 3, FGM-L81, 0, Ply-81
-    5.50871427080E-05, 3, FGM-L82, 0, Ply-82
-    4.41153781959E-05, 3, FGM-L83, 0, Ply-83
-    3.48708072238E-05, 3, FGM-L84, 0, Ply-84
-    2.71618324662E-05, 3, FGM-L85, 0, Ply-85
-    2.08081270284E-05, 3, FGM-L86, 0, Ply-86
-    1.56406344461E-05, 3, FGM-L87, 0, Ply-87
-    1.15015686863E-05, 3, FGM-L88, 0, Ply-88
-    8.24441414721E-06, 3, FGM-L89, 0, Ply-89
-    5.73392565656E-06, 3, FGM-L90, 0, Ply-90
-    3.84612847587E-06, 3, FGM-L91, 0, Ply-91
-    2.46831829465E-06, 3, FGM-L92, 0, Ply-92
-    1.49906123387E-06, 3, FGM-L93, 0, Ply-93
-    8.48193847935E-07, 3, FGM-L94, 0, Ply-94
-    4.36823118843E-07, 3, FGM-L95, 0, Ply-95
-    1.97326461615E-07, 3, FGM-L96, 0, Ply-96
-    7.33517215856E-08, 3, FGM-L97, 0, Ply-97
-    1.98171744015E-08, 3, FGM-L98, 0, Ply-98
-    2.91152796317E-09, 3, FGM-L99, 0, Ply-99
-    9.39200939243E-11, 3, FGM-L100, 0, Ply-100
+    9.0975653E-03, 3, FGM-L1, 0, Ply-1
+    9.1934018E-03, 3, FGM-L2, 0, Ply-2
+    9.2915403E-03, 3, FGM-L3, 0, Ply-3
+    9.3920678E-03, 3, FGM-L4, 0, Ply-4
+    9.4950760E-03, 3, FGM-L5, 0, Ply-5
+    9.6006616E-03, 3, FGM-L6, 0, Ply-6
+    9.7089263E-03, 3, FGM-L7, 0, Ply-7
+    9.8199772E-03, 3, FGM-L8, 0, Ply-8
+    9.9339276E-03, 3, FGM-L9, 0, Ply-9
+    1.0050897E-02, 3, FGM-L10, 0, Ply-10
+    1.0171012E-02, 3, FGM-L11, 0, Ply-11
+    1.0294405E-02, 3, FGM-L12, 0, Ply-12
+    1.0421219E-02, 3, FGM-L13, 0, Ply-13
+    1.0551602E-02, 3, FGM-L14, 0, Ply-14
+    1.0685715E-02, 3, FGM-L15, 0, Ply-15
+    1.0823724E-02, 3, FGM-L16, 0, Ply-16
+    1.0965810E-02, 3, FGM-L17, 0, Ply-17
+    1.1112163E-02, 3, FGM-L18, 0, Ply-18
+    1.1262986E-02, 3, FGM-L19, 0, Ply-19
+    1.1418494E-02, 3, FGM-L20, 0, Ply-20
+    1.1578918E-02, 3, FGM-L21, 0, Ply-21
+    1.1744504E-02, 3, FGM-L22, 0, Ply-22
+    1.1915515E-02, 3, FGM-L23, 0, Ply-23
+    1.2092233E-02, 3, FGM-L24, 0, Ply-24
+    1.2274960E-02, 3, FGM-L25, 0, Ply-25
+    1.2464019E-02, 3, FGM-L26, 0, Ply-26
+    1.2659759E-02, 3, FGM-L27, 0, Ply-27
+    1.2862553E-02, 3, FGM-L28, 0, Ply-28
+    1.3072807E-02, 3, FGM-L29, 0, Ply-29
+    1.3290956E-02, 3, FGM-L30, 0, Ply-30
+    1.3517469E-02, 3, FGM-L31, 0, Ply-31
+    1.3752859E-02, 3, FGM-L32, 0, Ply-32
+    1.3997676E-02, 3, FGM-L33, 0, Ply-33
+    1.4252523E-02, 3, FGM-L34, 0, Ply-34
+    1.4518054E-02, 3, FGM-L35, 0, Ply-35
+    1.4794981E-02, 3, FGM-L36, 0, Ply-36
+    1.5084084E-02, 3, FGM-L37, 0, Ply-37
+    1.5386217E-02, 3, FGM-L38, 0, Ply-38
+    1.5702317E-02, 3, FGM-L39, 0, Ply-39
+    1.6033415E-02, 3, FGM-L40, 0, Ply-40
+    1.6380647E-02, 3, FGM-L41, 0, Ply-41
+    1.6745272E-02, 3, FGM-L42, 0, Ply-42
+    1.7128683E-02, 3, FGM-L43, 0, Ply-43
+    1.7532429E-02, 3, FGM-L44, 0, Ply-44
+    1.7958241E-02, 3, FGM-L45, 0, Ply-45
+    1.8408053E-02, 3, FGM-L46, 0, Ply-46
+    1.8884036E-02, 3, FGM-L47, 0, Ply-47
+    1.9388641E-02, 3, FGM-L48, 0, Ply-48
+    1.9924635E-02, 3, FGM-L49, 0, Ply-49
+    2.0495166E-02, 3, FGM-L50, 0, Ply-50
+    2.1103826E-02, 3, FGM-L51, 0, Ply-51
+    2.1754730E-02, 3, FGM-L52, 0, Ply-52
+    2.2452623E-02, 3, FGM-L53, 0, Ply-53
+    2.3203004E-02, 3, FGM-L54, 0, Ply-54
+    2.4012282E-02, 3, FGM-L55, 0, Ply-55
+    2.4887978E-02, 3, FGM-L56, 0, Ply-56
+    2.5838977E-02, 3, FGM-L57, 0, Ply-57
+    2.6875862E-02, 3, FGM-L58, 0, Ply-58
+    2.8011338E-02, 3, FGM-L59, 0, Ply-59
+    2.9260807E-02, 3, FGM-L60, 0, Ply-60
+    3.0643127E-02, 3, FGM-L61, 0, Ply-61
+    3.2181661E-02, 3, FGM-L62, 0, Ply-62
+    3.3905721E-02, 3, FGM-L63, 0, Ply-63
+    3.5852628E-02, 3, FGM-L64, 0, Ply-64
+    3.8070684E-02, 3, FGM-L65, 0, Ply-65
+    4.0623601E-02, 3, FGM-L66, 0, Ply-66
+    4.3597292E-02, 3, FGM-L67, 0, Ply-67
+    7.0927002E-02, 3, FGM-L68, 0, Ply-68
+    7.0927002E-02, 3, FGM-L69, 0, Ply-69
+    7.0927002E-02, 3, FGM-L70, 0, Ply-70
+    7.0927002E-02, 3, FGM-L71, 0, Ply-71
+    7.0927002E-02, 3, FGM-L72, 0, Ply-72
+    7.0927002E-02, 3, FGM-L73, 0, Ply-73
+    7.0927002E-02, 3, FGM-L74, 0, Ply-74
+    7.0927002E-02, 3, FGM-L75, 0, Ply-75
+    7.0927002E-02, 3, FGM-L76, 0, Ply-76
+    7.0927002E-02, 3, FGM-L77, 0, Ply-77
+    7.0927002E-02, 3, FGM-L78, 0, Ply-78
+    7.0927002E-02, 3, FGM-L79, 0, Ply-79
+    7.0927002E-02, 3, FGM-L80, 0, Ply-80
+    7.0927002E-02, 3, FGM-L81, 0, Ply-81
+    7.0927002E-02, 3, FGM-L82, 0, Ply-82
+    7.0927002E-02, 3, FGM-L83, 0, Ply-83
+    7.0927002E-02, 3, FGM-L84, 0, Ply-84
+    7.0927002E-02, 3, FGM-L85, 0, Ply-85
+    7.0927002E-02, 3, FGM-L86, 0, Ply-86
+    7.0927002E-02, 3, FGM-L87, 0, Ply-87
+    7.0927002E-02, 3, FGM-L88, 0, Ply-88
+    7.0927002E-02, 3, FGM-L89, 0, Ply-89
+    7.0927002E-02, 3, FGM-L90, 0, Ply-90
+    7.0927002E-02, 3, FGM-L91, 0, Ply-91
+    7.0927002E-02, 3, FGM-L92, 0, Ply-92
+    7.0927002E-02, 3, FGM-L93, 0, Ply-93
+    7.0927002E-02, 3, FGM-L94, 0, Ply-94
+    7.0927002E-02, 3, FGM-L95, 0, Ply-95
+    7.0927002E-02, 3, FGM-L96, 0, Ply-96
+    7.0927002E-02, 3, FGM-L97, 0, Ply-97
+    7.0927002E-02, 3, FGM-L98, 0, Ply-98
+    7.0927002E-02, 3, FGM-L99, 0, Ply-99
+    7.0927002E-02, 3, FGM-L100, 0, Ply-100
 *End Part
```

### Comparing `lmcv_tools-0.0.7/tests/benchmark/generate/virtual_laminas_exp_voight.inp` & `lmcv_tools-0.0.8/tests/benchmark/generate/virtual_laminas_exp_hs_ub_2.inp`

 * *Files 18% similar despite different names*

```diff
@@ -1,252 +1,252 @@
 *Material, name=FGM-L1
     *Density
-    1012.500,
+    1.0125000E+03,
     *Elastic
-    376.375, 0.300
+    3.7417741E+02, 0.299
 *Material, name=FGM-L2
     *Density
-    1037.500,
+    1.0375000E+03,
     *Elastic
-    369.125, 0.299
+    3.6279637E+02, 0.298
 *Material, name=FGM-L3
     *Density
-    1062.500,
+    1.0625000E+03,
     *Elastic
-    361.875, 0.298
+    3.5175438E+02, 0.296
 *Material, name=FGM-L4
     *Density
-    1087.500,
+    1.0875000E+03,
     *Elastic
-    354.625, 0.297
+    3.4103653E+02, 0.295
 *Material, name=FGM-L5
     *Density
-    1112.500,
+    1.1125000E+03,
     *Elastic
-    347.375, 0.297
+    3.3062872E+02, 0.293
 *Material, name=FGM-L6
     *Density
-    1137.500,
+    1.1375000E+03,
     *Elastic
-    340.125, 0.296
+    3.2051771E+02, 0.292
 *Material, name=FGM-L7
     *Density
-    1162.500,
+    1.1625000E+03,
     *Elastic
-    332.875, 0.295
+    3.1069097E+02, 0.291
 *Material, name=FGM-L8
     *Density
-    1187.500,
+    1.1875000E+03,
     *Elastic
-    325.625, 0.294
+    3.0113667E+02, 0.289
 *Material, name=FGM-L9
     *Density
-    1212.500,
+    1.2125000E+03,
     *Elastic
-    318.375, 0.294
+    2.9184363E+02, 0.288
 *Material, name=FGM-L10
     *Density
-    1237.500,
+    1.2375000E+03,
     *Elastic
-    311.125, 0.293
+    2.8280127E+02, 0.287
 *Material, name=FGM-L11
     *Density
-    1262.500,
+    1.2625000E+03,
     *Elastic
-    303.875, 0.292
+    2.7399959E+02, 0.286
 *Material, name=FGM-L12
     *Density
-    1287.500,
+    1.2875000E+03,
     *Elastic
-    296.625, 0.291
+    2.6542909E+02, 0.285
 *Material, name=FGM-L13
     *Density
-    1312.500,
+    1.3125000E+03,
     *Elastic
-    289.375, 0.291
+    2.5708077E+02, 0.284
 *Material, name=FGM-L14
     *Density
-    1337.500,
+    1.3375000E+03,
     *Elastic
-    282.125, 0.290
+    2.4894611E+02, 0.283
 *Material, name=FGM-L15
     *Density
-    1362.500,
+    1.3625000E+03,
     *Elastic
-    274.875, 0.289
+    2.4101699E+02, 0.282
 *Material, name=FGM-L16
     *Density
-    1387.500,
+    1.3875000E+03,
     *Elastic
-    267.625, 0.288
+    2.3328572E+02, 0.281
 *Material, name=FGM-L17
     *Density
-    1412.500,
+    1.4125000E+03,
     *Elastic
-    260.375, 0.288
+    2.2574497E+02, 0.280
 *Material, name=FGM-L18
     *Density
-    1437.500,
+    1.4375000E+03,
     *Elastic
-    253.125, 0.287
+    2.1838779E+02, 0.279
 *Material, name=FGM-L19
     *Density
-    1462.500,
+    1.4625000E+03,
     *Elastic
-    245.875, 0.286
+    2.1120753E+02, 0.278
 *Material, name=FGM-L20
     *Density
-    1487.500,
+    1.4875000E+03,
     *Elastic
-    238.625, 0.285
+    2.0419789E+02, 0.277
 *Material, name=FGM-L21
     *Density
-    1512.500,
+    1.5125000E+03,
     *Elastic
-    231.375, 0.285
+    1.9735285E+02, 0.277
 *Material, name=FGM-L22
     *Density
-    1537.500,
+    1.5375000E+03,
     *Elastic
-    224.125, 0.284
+    1.9066666E+02, 0.276
 *Material, name=FGM-L23
     *Density
-    1562.500,
+    1.5625000E+03,
     *Elastic
-    216.875, 0.283
+    1.8413385E+02, 0.275
 *Material, name=FGM-L24
     *Density
-    1587.500,
+    1.5875000E+03,
     *Elastic
-    209.625, 0.282
+    1.7774920E+02, 0.274
 *Material, name=FGM-L25
     *Density
-    1612.500,
+    1.6125000E+03,
     *Elastic
-    202.375, 0.282
+    1.7150770E+02, 0.274
 *Material, name=FGM-L26
     *Density
-    1637.500,
+    1.6375000E+03,
     *Elastic
-    195.125, 0.281
+    1.6540458E+02, 0.273
 *Material, name=FGM-L27
     *Density
-    1662.500,
+    1.6625000E+03,
     *Elastic
-    187.875, 0.280
+    1.5943528E+02, 0.273
 *Material, name=FGM-L28
     *Density
-    1687.500,
+    1.6875000E+03,
     *Elastic
-    180.625, 0.279
+    1.5359543E+02, 0.272
 *Material, name=FGM-L29
     *Density
-    1712.500,
+    1.7125000E+03,
     *Elastic
-    173.375, 0.279
+    1.4788084E+02, 0.272
 *Material, name=FGM-L30
     *Density
-    1737.500,
+    1.7375000E+03,
     *Elastic
-    166.125, 0.278
+    1.4228752E+02, 0.271
 *Material, name=FGM-L31
     *Density
-    1762.500,
+    1.7625000E+03,
     *Elastic
-    158.875, 0.277
+    1.3681162E+02, 0.271
 *Material, name=FGM-L32
     *Density
-    1787.500,
+    1.7875000E+03,
     *Elastic
-    151.625, 0.276
+    1.3144947E+02, 0.271
 *Material, name=FGM-L33
     *Density
-    1812.500,
+    1.8125000E+03,
     *Elastic
-    144.375, 0.276
+    1.2619754E+02, 0.270
 *Material, name=FGM-L34
     *Density
-    1837.500,
+    1.8375000E+03,
     *Elastic
-    137.125, 0.275
+    1.2105243E+02, 0.270
 *Material, name=FGM-L35
     *Density
-    1862.500,
+    1.8625000E+03,
     *Elastic
-    129.875, 0.274
+    1.1601089E+02, 0.270
 *Material, name=FGM-L36
     *Density
-    1887.500,
+    1.8875000E+03,
     *Elastic
-    122.625, 0.273
+    1.1106981E+02, 0.270
 *Material, name=FGM-L37
     *Density
-    1912.500,
+    1.9125000E+03,
     *Elastic
-    115.375, 0.273
+    1.0622617E+02, 0.270
 *Material, name=FGM-L38
     *Density
-    1937.500,
+    1.9375000E+03,
     *Elastic
-    108.125, 0.272
+    1.0147707E+02, 0.270
 *Material, name=FGM-L39
     *Density
-    1962.500,
+    1.9625000E+03,
     *Elastic
-    100.875, 0.271
+    9.6819753E+01, 0.270
 *Material, name=FGM-L40
     *Density
-    1987.500,
+    1.9875000E+03,
     *Elastic
-    93.625, 0.270
+    9.2251520E+01, 0.270
 *Part, name=Virtual_Part
 *Node
     1, 1.0, 1.0, 0.0
     2, 0.0, 1.0, 0.0
     3, 0.0, 0.0, 0.0
     4, 1.0, 0.0, 0.0
 *Element, type=S4R
     1, 1, 2, 3, 4
 *Elset, elset=Virtual
     1
 *Solid Section, elset=Virtual, composite
-    2.50000000000E-01, 3, FGM-L1, 0, Ply-1
-    2.50000000000E-01, 3, FGM-L2, 0, Ply-2
-    2.50000000000E-01, 3, FGM-L3, 0, Ply-3
-    2.50000000000E-01, 3, FGM-L4, 0, Ply-4
-    2.50000000000E-01, 3, FGM-L5, 0, Ply-5
-    2.50000000000E-01, 3, FGM-L6, 0, Ply-6
-    2.50000000000E-01, 3, FGM-L7, 0, Ply-7
-    2.50000000000E-01, 3, FGM-L8, 0, Ply-8
-    2.50000000000E-01, 3, FGM-L9, 0, Ply-9
-    2.50000000000E-01, 3, FGM-L10, 0, Ply-10
-    2.50000000000E-01, 3, FGM-L11, 0, Ply-11
-    2.50000000000E-01, 3, FGM-L12, 0, Ply-12
-    2.50000000000E-01, 3, FGM-L13, 0, Ply-13
-    2.50000000000E-01, 3, FGM-L14, 0, Ply-14
-    2.50000000000E-01, 3, FGM-L15, 0, Ply-15
-    2.50000000000E-01, 3, FGM-L16, 0, Ply-16
-    2.50000000000E-01, 3, FGM-L17, 0, Ply-17
-    2.50000000000E-01, 3, FGM-L18, 0, Ply-18
-    2.50000000000E-01, 3, FGM-L19, 0, Ply-19
-    2.50000000000E-01, 3, FGM-L20, 0, Ply-20
-    2.50000000000E-01, 3, FGM-L21, 0, Ply-21
-    2.50000000000E-01, 3, FGM-L22, 0, Ply-22
-    2.50000000000E-01, 3, FGM-L23, 0, Ply-23
-    2.50000000000E-01, 3, FGM-L24, 0, Ply-24
-    2.50000000000E-01, 3, FGM-L25, 0, Ply-25
-    2.50000000000E-01, 3, FGM-L26, 0, Ply-26
-    2.50000000000E-01, 3, FGM-L27, 0, Ply-27
-    2.50000000000E-01, 3, FGM-L28, 0, Ply-28
-    2.50000000000E-01, 3, FGM-L29, 0, Ply-29
-    2.50000000000E-01, 3, FGM-L30, 0, Ply-30
-    2.50000000000E-01, 3, FGM-L31, 0, Ply-31
-    2.50000000000E-01, 3, FGM-L32, 0, Ply-32
-    2.50000000000E-01, 3, FGM-L33, 0, Ply-33
-    2.50000000000E-01, 3, FGM-L34, 0, Ply-34
-    2.50000000000E-01, 3, FGM-L35, 0, Ply-35
-    2.50000000000E-01, 3, FGM-L36, 0, Ply-36
-    2.50000000000E-01, 3, FGM-L37, 0, Ply-37
-    2.50000000000E-01, 3, FGM-L38, 0, Ply-38
-    2.50000000000E-01, 3, FGM-L39, 0, Ply-39
-    2.50000000000E-01, 3, FGM-L40, 0, Ply-40
+    2.5000000E-01, 3, FGM-L1, 0, Ply-1
+    2.5000000E-01, 3, FGM-L2, 0, Ply-2
+    2.5000000E-01, 3, FGM-L3, 0, Ply-3
+    2.5000000E-01, 3, FGM-L4, 0, Ply-4
+    2.5000000E-01, 3, FGM-L5, 0, Ply-5
+    2.5000000E-01, 3, FGM-L6, 0, Ply-6
+    2.5000000E-01, 3, FGM-L7, 0, Ply-7
+    2.5000000E-01, 3, FGM-L8, 0, Ply-8
+    2.5000000E-01, 3, FGM-L9, 0, Ply-9
+    2.5000000E-01, 3, FGM-L10, 0, Ply-10
+    2.5000000E-01, 3, FGM-L11, 0, Ply-11
+    2.5000000E-01, 3, FGM-L12, 0, Ply-12
+    2.5000000E-01, 3, FGM-L13, 0, Ply-13
+    2.5000000E-01, 3, FGM-L14, 0, Ply-14
+    2.5000000E-01, 3, FGM-L15, 0, Ply-15
+    2.5000000E-01, 3, FGM-L16, 0, Ply-16
+    2.5000000E-01, 3, FGM-L17, 0, Ply-17
+    2.5000000E-01, 3, FGM-L18, 0, Ply-18
+    2.5000000E-01, 3, FGM-L19, 0, Ply-19
+    2.5000000E-01, 3, FGM-L20, 0, Ply-20
+    2.5000000E-01, 3, FGM-L21, 0, Ply-21
+    2.5000000E-01, 3, FGM-L22, 0, Ply-22
+    2.5000000E-01, 3, FGM-L23, 0, Ply-23
+    2.5000000E-01, 3, FGM-L24, 0, Ply-24
+    2.5000000E-01, 3, FGM-L25, 0, Ply-25
+    2.5000000E-01, 3, FGM-L26, 0, Ply-26
+    2.5000000E-01, 3, FGM-L27, 0, Ply-27
+    2.5000000E-01, 3, FGM-L28, 0, Ply-28
+    2.5000000E-01, 3, FGM-L29, 0, Ply-29
+    2.5000000E-01, 3, FGM-L30, 0, Ply-30
+    2.5000000E-01, 3, FGM-L31, 0, Ply-31
+    2.5000000E-01, 3, FGM-L32, 0, Ply-32
+    2.5000000E-01, 3, FGM-L33, 0, Ply-33
+    2.5000000E-01, 3, FGM-L34, 0, Ply-34
+    2.5000000E-01, 3, FGM-L35, 0, Ply-35
+    2.5000000E-01, 3, FGM-L36, 0, Ply-36
+    2.5000000E-01, 3, FGM-L37, 0, Ply-37
+    2.5000000E-01, 3, FGM-L38, 0, Ply-38
+    2.5000000E-01, 3, FGM-L39, 0, Ply-39
+    2.5000000E-01, 3, FGM-L40, 0, Ply-40
 *End Part
```

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/Circle_T3_Q4_4x4.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/Circle_T3_Q4_4x4.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/Circle_T3_Q4_4x4_exp.svg` & `lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/Circle_T3_Q4_4x4_exp.svg`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/HeartPlate_BT2_2x2.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/HeartPlate_BT2_2x2.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/HeartPlate_BT2_2x2_exp.svg` & `lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/HeartPlate_BT2_2x2_exp.svg`

 * *Files 10% similar despite different names*

```diff
@@ -7,768 +7,721 @@
 00000060: 6e74 7322 2066 696c 6c3d 2223 6663 6666  nts" fill="#fcff
 00000070: 3565 2220 7374 726f 6b65 3d22 626c 6163  5e" stroke="blac
 00000080: 6b22 2073 7472 6f6b 652d 7769 6474 683d  k" stroke-width=
 00000090: 2230 2e36 3133 3732 3132 3837 3634 3230  "0.6137212876420
 000000a0: 3830 3322 3e0d 0a20 2020 2020 203c 7061  803">..      <pa
 000000b0: 7468 2064 3d22 4d20 352e 3337 3237 3932  th d="M 5.372792
 000000c0: 3630 652b 3031 2037 2e31 3732 3739 3236  60e+01 7.1727926
-000000d0: 3065 2b30 3120 5120 342e 3834 3535 3834  0e+01 Q 4.845584
-000000e0: 3330 652b 3031 2037 2e37 3030 3030 3030  30e+01 7.7000000
-000000f0: 3065 2b30 312c 2034 2e31 3030 3030 3030  0e+01, 4.1000000
+000000d0: 3065 2b30 3120 5120 342e 3738 3837 3434  0e+01 Q 4.788744
+000000e0: 3734 652b 3031 2037 2e37 3130 3834 3137  74e+01 7.7108417
+000000f0: 3765 2b30 312c 2034 2e31 3030 3030 3030  7e+01, 4.1000000
 00000100: 3065 2b30 3120 372e 3730 3030 3030 3030  0e+01 7.70000000
-00000110: 652b 3031 2051 2034 2e35 3533 3430 3230  e+01 Q 4.5534020
-00000120: 3065 2b30 3120 382e 3631 3630 3037 3331  0e+01 8.61600731
+00000110: 652b 3031 2051 2034 2e35 3533 3332 3632  e+01 Q 4.5533262
+00000120: 3165 2b30 3120 382e 3631 3536 3530 3730  1e+01 8.61565070
 00000130: 652b 3031 2c20 352e 3030 3030 3030 3030  e+01, 5.00000000
 00000140: 652b 3031 2039 2e35 3030 3030 3030 3065  e+01 9.50000000e
-00000150: 2b30 3120 5120 352e 3232 3835 3832 3930  +01 Q 5.22858290
-00000160: 652b 3031 2038 2e33 3835 3338 3630 3065  e+01 8.38538600e
+00000150: 2b30 3120 5120 352e 3231 3439 3535 3431  +01 Q 5.21495541
+00000160: 652b 3031 2038 2e34 3736 3439 3130 3865  e+01 8.47649108e
 00000170: 2b30 312c 2035 2e33 3732 3739 3236 3065  +01, 5.37279260e
 00000180: 2b30 3120 372e 3137 3237 3932 3630 652b  +01 7.17279260e+
 00000190: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
 000001a0: 3c70 6174 6820 643d 224d 2035 2e33 3732  <path d="M 5.372
 000001b0: 3739 3236 3065 2b30 3120 372e 3137 3237  79260e+01 7.1727
-000001c0: 3932 3630 652b 3031 2051 2035 2e32 3238  9260e+01 Q 5.228
-000001d0: 3538 3239 3065 2b30 3120 382e 3338 3533  58290e+01 8.3853
-000001e0: 3836 3030 652b 3031 2c20 352e 3030 3030  8600e+01, 5.0000
+000001c0: 3932 3630 652b 3031 2051 2035 2e32 3134  9260e+01 Q 5.214
+000001d0: 3935 3534 3165 2b30 3120 382e 3437 3634  95541e+01 8.4764
+000001e0: 3931 3038 652b 3031 2c20 352e 3030 3030  9108e+01, 5.0000
 000001f0: 3030 3030 652b 3031 2039 2e35 3030 3030  0000e+01 9.50000
-00000200: 3030 3065 2b30 3120 5120 362e 3035 3338  000e+01 Q 6.0538
-00000210: 3130 3030 652b 3031 2038 2e33 3033 3232  1000e+01 8.30322
-00000220: 3836 3065 2b30 312c 2037 2e31 3039 3337  860e+01, 7.10937
+00000200: 3030 3065 2b30 3120 5120 362e 3031 3737  000e+01 Q 6.0177
+00000210: 3839 3939 652b 3031 2038 2e33 3434 3137  8999e+01 8.34417
+00000220: 3232 3865 2b30 312c 2037 2e31 3039 3337  228e+01, 7.10937
 00000230: 3233 3065 2b30 3120 372e 3130 3034 3137  230e+01 7.100417
-00000240: 3330 652b 3031 2051 2036 2e32 3633 3133  30e+01 Q 6.26313
-00000250: 3734 3065 2b30 3120 372e 3137 3238 3731  740e+01 7.172871
-00000260: 3830 652b 3031 2c20 352e 3337 3237 3932  80e+01, 5.372792
+00000240: 3330 652b 3031 2051 2036 2e33 3032 3338  30e+01 Q 6.30238
+00000250: 3932 3165 2b30 3120 372e 3137 3137 3733  921e+01 7.171773
+00000260: 3038 652b 3031 2c20 352e 3337 3237 3932  08e+01, 5.372792
 00000270: 3630 652b 3031 2037 2e31 3732 3739 3236  60e+01 7.1727926
 00000280: 3065 2b30 3120 5a22 202f 3e0d 0a20 2020  0e+01 Z" />..   
 00000290: 2020 203c 7061 7468 2064 3d22 4d20 352e     <path d="M 5.
 000002a0: 3930 3030 3030 3030 652b 3031 2035 2e39  90000000e+01 5.9
 000002b0: 3030 3030 3030 3065 2b30 3120 5120 352e  0000000e+01 Q 5.
-000002c0: 3930 3030 3030 3030 652b 3031 2036 2e36  90000000e+01 6.6
-000002d0: 3435 3538 3433 3065 2b30 312c 2035 2e33  4558430e+01, 5.3
+000002c0: 3931 3038 3431 3737 652b 3031 2036 2e35  91084177e+01 6.5
+000002d0: 3838 3734 3437 3465 2b30 312c 2035 2e33  8874474e+01, 5.3
 000002e0: 3732 3739 3236 3065 2b30 3120 372e 3137  7279260e+01 7.17
-000002f0: 3237 3932 3630 652b 3031 2051 2036 2e32  279260e+01 Q 6.2
-00000300: 3633 3133 3734 3065 2b30 3120 372e 3137  6313740e+01 7.17
-00000310: 3238 3731 3830 652b 3031 2c20 372e 3130  287180e+01, 7.10
+000002f0: 3237 3932 3630 652b 3031 2051 2036 2e33  279260e+01 Q 6.3
+00000300: 3032 3338 3932 3165 2b30 3120 372e 3137  0238921e+01 7.17
+00000310: 3137 3733 3038 652b 3031 2c20 372e 3130  177308e+01, 7.10
 00000320: 3933 3732 3330 652b 3031 2037 2e31 3030  937230e+01 7.100
-00000330: 3431 3733 3065 2b30 3120 5120 362e 3535  41730e+01 Q 6.55
-00000340: 3533 3033 3530 652b 3031 2036 2e35 3531  530350e+01 6.551
-00000350: 3332 3337 3065 2b30 312c 2035 2e39 3030  32370e+01, 5.900
+00000330: 3431 3733 3065 2b30 3120 5120 362e 3533  41730e+01 Q 6.53
+00000340: 3131 3732 3735 652b 3031 2036 2e35 3237  117275e+01 6.527
+00000350: 3332 3439 3965 2b30 312c 2035 2e39 3030  32499e+01, 5.900
 00000360: 3030 3030 3065 2b30 3120 352e 3930 3030  00000e+01 5.9000
 00000370: 3030 3030 652b 3031 205a 2220 2f3e 0d0a  0000e+01 Z" />..
 00000380: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
 00000390: 2037 2e37 3030 3030 3030 3065 2b30 3120   7.70000000e+01 
 000003a0: 342e 3130 3030 3030 3030 652b 3031 2051  4.10000000e+01 Q
-000003b0: 2037 2e37 3030 3030 3030 3065 2b30 3120   7.70000000e+01 
-000003c0: 342e 3834 3535 3834 3330 652b 3031 2c20  4.84558430e+01, 
+000003b0: 2037 2e37 3130 3834 3137 3765 2b30 3120   7.71084177e+01 
+000003c0: 342e 3738 3837 3434 3734 652b 3031 2c20  4.78874474e+01, 
 000003d0: 372e 3137 3237 3932 3630 652b 3031 2035  7.17279260e+01 5
 000003e0: 2e33 3732 3739 3236 3065 2b30 3120 5120  .37279260e+01 Q 
-000003f0: 382e 3338 3535 3632 3430 652b 3031 2035  8.38556240e+01 5
-00000400: 2e32 3238 3730 3434 3065 2b30 312c 2039  .22870440e+01, 9
+000003f0: 382e 3437 3636 3334 3433 652b 3031 2035  8.47663443e+01 5
+00000400: 2e32 3135 3132 3738 3765 2b30 312c 2039  .21512787e+01, 9
 00000410: 2e35 3030 3030 3030 3065 2b30 3120 352e  .50000000e+01 5.
 00000420: 3030 3030 3030 3030 652b 3031 2051 2038  00000000e+01 Q 8
-00000430: 2e36 3136 3134 3738 3065 2b30 3120 342e  .61614780e+01 4.
-00000440: 3535 3334 3638 3630 652b 3031 2c20 372e  55346860e+01, 7.
+00000430: 2e36 3135 3738 3535 3965 2b30 3120 342e  .61578559e+01 4.
+00000440: 3535 3333 3930 3830 652b 3031 2c20 372e  55339080e+01, 7.
 00000450: 3730 3030 3030 3030 652b 3031 2034 2e31  70000000e+01 4.1
 00000460: 3030 3030 3030 3065 2b30 3120 5a22 202f  0000000e+01 Z" /
 00000470: 3e0d 0a20 2020 2020 203c 7061 7468 2064  >..      <path d
 00000480: 3d22 4d20 392e 3530 3030 3030 3030 652b  ="M 9.50000000e+
 00000490: 3031 2035 2e30 3030 3030 3030 3065 2b30  01 5.00000000e+0
-000004a0: 3120 5120 382e 3338 3535 3632 3430 652b  1 Q 8.38556240e+
-000004b0: 3031 2035 2e32 3238 3730 3434 3065 2b30  01 5.22870440e+0
+000004a0: 3120 5120 382e 3437 3636 3334 3433 652b  1 Q 8.47663443e+
+000004b0: 3031 2035 2e32 3135 3132 3738 3765 2b30  01 5.21512787e+0
 000004c0: 312c 2037 2e31 3732 3739 3236 3065 2b30  1, 7.17279260e+0
 000004d0: 3120 352e 3337 3237 3932 3630 652b 3031  1 5.37279260e+01
-000004e0: 2051 2037 2e31 3736 3937 3133 3065 2b30   Q 7.17697130e+0
-000004f0: 3120 362e 3235 3833 3535 3730 652b 3031  1 6.25835570e+01
+000004e0: 2051 2037 2e31 3736 3038 3731 3965 2b30   Q 7.17608719e+0
+000004f0: 3120 362e 3239 3733 3933 3237 652b 3031  1 6.29739327e+01
 00000500: 2c20 372e 3130 3933 3732 3330 652b 3031  , 7.10937230e+01
 00000510: 2037 2e31 3030 3431 3733 3065 2b30 3120   7.10041730e+01 
-00000520: 5120 382e 3330 3735 3632 3130 652b 3031  Q 8.30756210e+01
-00000530: 2036 2e30 3439 3333 3235 3065 2b30 312c   6.04933250e+01,
+00000520: 5120 382e 3334 3833 3536 3132 652b 3031  Q 8.34835612e+01
+00000530: 2036 2e30 3133 3436 3435 3165 2b30 312c   6.01346451e+01,
 00000540: 2039 2e35 3030 3030 3030 3065 2b30 3120   9.50000000e+01 
 00000550: 352e 3030 3030 3030 3030 652b 3031 205a  5.00000000e+01 Z
 00000560: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
 00000570: 6820 643d 224d 2037 2e31 3039 3337 3233  h d="M 7.1093723
 00000580: 3065 2b30 3120 372e 3130 3034 3137 3330  0e+01 7.10041730
-00000590: 652b 3031 2051 2038 2e32 3930 3339 3535  e+01 Q 8.2903955
-000005a0: 3065 2b30 3120 382e 3238 3539 3734 3730  0e+01 8.28597470
-000005b0: 652b 3031 2c20 392e 3530 3030 3030 3030  e+01, 9.50000000
-000005c0: 652b 3031 2039 2e35 3030 3030 3030 3065  e+01 9.50000000e
-000005d0: 2b30 3120 5120 392e 3530 3030 3030 3030  +01 Q 9.50000000
-000005e0: 652b 3031 2037 2e32 3530 3030 3030 3065  e+01 7.25000000e
-000005f0: 2b30 312c 2039 2e35 3030 3030 3030 3065  +01, 9.50000000e
-00000600: 2b30 3120 352e 3030 3030 3030 3030 652b  +01 5.00000000e+
-00000610: 3031 2051 2038 2e33 3037 3536 3231 3065  01 Q 8.30756210e
-00000620: 2b30 3120 362e 3034 3933 3332 3530 652b  +01 6.04933250e+
-00000630: 3031 2c20 372e 3130 3933 3732 3330 652b  01, 7.10937230e+
-00000640: 3031 2037 2e31 3030 3431 3733 3065 2b30  01 7.10041730e+0
-00000650: 3120 5a22 202f 3e0d 0a20 2020 2020 203c  1 Z" />..      <
-00000660: 7061 7468 2064 3d22 4d20 372e 3534 3133  path d="M 7.5413
-00000670: 3632 3430 652b 3031 2032 2e34 3635 3931  6240e+01 2.46591
-00000680: 3539 3065 2b30 3120 5120 382e 3534 3738  590e+01 Q 8.5478
-00000690: 3136 3230 652b 3031 2033 2e37 3532 3834  1620e+01 3.75284
-000006a0: 3231 3065 2b30 312c 2039 2e35 3030 3030  210e+01, 9.50000
-000006b0: 3030 3065 2b30 3120 352e 3030 3030 3030  000e+01 5.000000
-000006c0: 3030 652b 3031 2051 2039 2e35 3030 3030  00e+01 Q 9.50000
-000006d0: 3030 3065 2b30 3120 322e 3735 3030 3030  000e+01 2.750000
-000006e0: 3030 652b 3031 2c20 392e 3530 3030 3030  00e+01, 9.500000
-000006f0: 3030 652b 3031 2035 2e30 3030 3030 3030  00e+01 5.0000000
-00000700: 3065 2b30 3020 5120 382e 3530 3439 3237  0e+00 Q 8.504927
-00000710: 3630 652b 3031 2031 2e34 3937 3039 3338  60e+01 1.4970938
-00000720: 3065 2b30 312c 2037 2e35 3431 3336 3234  0e+01, 7.5413624
-00000730: 3065 2b30 3120 322e 3436 3539 3135 3930  0e+01 2.46591590
-00000740: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
-00000750: 2020 3c70 6174 6820 643d 224d 2037 2e35    <path d="M 7.5
-00000760: 3431 3336 3234 3065 2b30 3120 322e 3436  4136240e+01 2.46
-00000770: 3539 3135 3930 652b 3031 2051 2037 2e37  591590e+01 Q 7.7
-00000780: 3631 3134 3630 3065 2b30 3120 332e 3235  6114600e+01 3.25
-00000790: 3639 3837 3130 652b 3031 2c20 372e 3730  698710e+01, 7.70
-000007a0: 3030 3030 3030 652b 3031 2034 2e31 3030  000000e+01 4.100
-000007b0: 3030 3030 3065 2b30 3120 5120 382e 3631  00000e+01 Q 8.61
-000007c0: 3631 3437 3830 652b 3031 2034 2e35 3533  614780e+01 4.553
-000007d0: 3436 3836 3065 2b30 312c 2039 2e35 3030  46860e+01, 9.500
-000007e0: 3030 3030 3065 2b30 3120 352e 3030 3030  00000e+01 5.0000
-000007f0: 3030 3030 652b 3031 2051 2038 2e35 3437  0000e+01 Q 8.547
-00000800: 3831 3632 3065 2b30 3120 332e 3735 3238  81620e+01 3.7528
-00000810: 3432 3130 652b 3031 2c20 372e 3534 3133  4210e+01, 7.5413
-00000820: 3632 3430 652b 3031 2032 2e34 3635 3931  6240e+01 2.46591
-00000830: 3539 3065 2b30 3120 5a22 202f 3e0d 0a20  590e+01 Z" />.. 
-00000840: 2020 2020 203c 7061 7468 2064 3d22 4d20       <path d="M 
-00000850: 372e 3137 3237 3932 3630 652b 3031 2035  7.17279260e+01 5
-00000860: 2e33 3732 3739 3236 3065 2b30 3120 5120  .37279260e+01 Q 
-00000870: 362e 3634 3535 3834 3330 652b 3031 2035  6.64558430e+01 5
-00000880: 2e39 3030 3030 3030 3065 2b30 312c 2035  .90000000e+01, 5
-00000890: 2e39 3030 3030 3030 3065 2b30 3120 352e  .90000000e+01 5.
-000008a0: 3930 3030 3030 3030 652b 3031 2051 2036  90000000e+01 Q 6
-000008b0: 2e35 3535 3330 3335 3065 2b30 3120 362e  .55530350e+01 6.
-000008c0: 3535 3133 3233 3730 652b 3031 2c20 372e  55132370e+01, 7.
-000008d0: 3130 3933 3732 3330 652b 3031 2037 2e31  10937230e+01 7.1
-000008e0: 3030 3431 3733 3065 2b30 3120 5120 372e  0041730e+01 Q 7.
-000008f0: 3137 3639 3731 3330 652b 3031 2036 2e32  17697130e+01 6.2
-00000900: 3538 3335 3537 3065 2b30 312c 2037 2e31  5835570e+01, 7.1
-00000910: 3732 3739 3236 3065 2b30 3120 352e 3337  7279260e+01 5.37
-00000920: 3237 3932 3630 652b 3031 205a 2220 2f3e  279260e+01 Z" />
-00000930: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
-00000940: 224d 2037 2e35 3431 3336 3234 3065 2b30  "M 7.54136240e+0
-00000950: 3120 322e 3436 3539 3135 3930 652b 3031  1 2.46591590e+01
-00000960: 2051 2037 2e33 3535 3839 3133 3065 2b30   Q 7.35589130e+0
-00000970: 3120 322e 3634 3736 3139 3630 652b 3031  1 2.64761960e+01
-00000980: 2c20 372e 3137 3237 3932 3630 652b 3031  , 7.17279260e+01
-00000990: 2032 2e38 3237 3230 3734 3065 2b30 3120   2.82720740e+01 
-000009a0: 5120 372e 3730 3030 3030 3030 652b 3031  Q 7.70000000e+01
-000009b0: 2033 2e33 3534 3431 3537 3065 2b30 312c   3.35441570e+01,
-000009c0: 2037 2e37 3030 3030 3030 3065 2b30 3120   7.70000000e+01 
-000009d0: 342e 3130 3030 3030 3030 652b 3031 2051  4.10000000e+01 Q
-000009e0: 2037 2e37 3631 3134 3630 3065 2b30 3120   7.76114600e+01 
-000009f0: 332e 3235 3639 3837 3130 652b 3031 2c20  3.25698710e+01, 
-00000a00: 372e 3534 3133 3632 3430 652b 3031 2032  7.54136240e+01 2
-00000a10: 2e34 3635 3931 3539 3065 2b30 3120 5a22  .46591590e+01 Z"
-00000a20: 202f 3e0d 0a20 2020 2020 203c 7061 7468   />..      <path
-00000a30: 2064 3d22 4d20 352e 3930 3030 3030 3030   d="M 5.90000000
-00000a40: 652b 3031 2032 2e33 3030 3030 3030 3065  e+01 2.30000000e
-00000a50: 2b30 3120 5120 362e 3634 3535 3834 3330  +01 Q 6.64558430
-00000a60: 652b 3031 2032 2e33 3030 3030 3030 3065  e+01 2.30000000e
-00000a70: 2b30 312c 2037 2e31 3732 3739 3236 3065  +01, 7.17279260e
-00000a80: 2b30 3120 322e 3832 3732 3037 3430 652b  +01 2.82720740e+
-00000a90: 3031 2051 2037 2e33 3535 3839 3133 3065  01 Q 7.35589130e
-00000aa0: 2b30 3120 322e 3634 3736 3139 3630 652b  +01 2.64761960e+
-00000ab0: 3031 2c20 372e 3534 3133 3632 3430 652b  01, 7.54136240e+
-00000ac0: 3031 2032 2e34 3635 3931 3539 3065 2b30  01 2.46591590e+0
-00000ad0: 3120 5120 362e 3734 3638 3838 3330 652b  1 Q 6.74688830e+
-00000ae0: 3031 2032 2e32 3430 3437 3331 3065 2b30  01 2.24047310e+0
-00000af0: 312c 2035 2e39 3030 3030 3030 3065 2b30  1, 5.90000000e+0
-00000b00: 3120 322e 3330 3030 3030 3030 652b 3031  1 2.30000000e+01
-00000b10: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
-00000b20: 6174 6820 643d 224d 2032 2e33 3030 3030  ath d="M 2.30000
-00000b30: 3030 3065 2b30 3120 342e 3130 3030 3030  000e+01 4.100000
-00000b40: 3030 652b 3031 2051 2032 2e33 3030 3030  00e+01 Q 2.30000
-00000b50: 3030 3065 2b30 3120 332e 3230 3030 3030  000e+01 3.200000
-00000b60: 3030 652b 3031 2c20 322e 3330 3030 3030  00e+01, 2.300000
-00000b70: 3030 652b 3031 2032 2e33 3030 3030 3030  00e+01 2.3000000
-00000b80: 3065 2b30 3120 5120 312e 3430 3031 3039  0e+01 Q 1.400109
-00000b90: 3830 652b 3031 2033 2e36 3439 3730 3231  80e+01 3.6497021
-00000ba0: 3065 2b30 312c 2035 2e30 3030 3030 3030  0e+01, 5.0000000
-00000bb0: 3065 2b30 3020 352e 3030 3030 3030 3030  0e+00 5.00000000
-00000bc0: 652b 3031 2051 2031 2e34 3030 3539 3232  e+01 Q 1.4005922
-00000bd0: 3065 2b30 3120 342e 3534 3931 3332 3430  0e+01 4.54913240
-00000be0: 652b 3031 2c20 322e 3330 3030 3030 3030  e+01, 2.30000000
-00000bf0: 652b 3031 2034 2e31 3030 3030 3030 3065  e+01 4.10000000e
-00000c00: 2b30 3120 5a22 202f 3e0d 0a20 2020 2020  +01 Z" />..     
-00000c10: 203c 7061 7468 2064 3d22 4d20 322e 3330   <path d="M 2.30
-00000c20: 3030 3030 3030 652b 3031 2035 2e39 3030  000000e+01 5.900
-00000c30: 3030 3030 3065 2b30 3120 5120 322e 3330  00000e+01 Q 2.30
-00000c40: 3030 3030 3030 652b 3031 2035 2e30 3030  000000e+01 5.000
-00000c50: 3030 3030 3065 2b30 312c 2032 2e33 3030  00000e+01, 2.300
-00000c60: 3030 3030 3065 2b30 3120 342e 3130 3030  00000e+01 4.1000
-00000c70: 3030 3030 652b 3031 2051 2031 2e34 3030  0000e+01 Q 1.400
-00000c80: 3539 3232 3065 2b30 3120 342e 3534 3931  59220e+01 4.5491
-00000c90: 3332 3430 652b 3031 2c20 352e 3030 3030  3240e+01, 5.0000
-00000ca0: 3030 3030 652b 3030 2035 2e30 3030 3030  0000e+00 5.00000
-00000cb0: 3030 3065 2b30 3120 5120 312e 3430 3636  000e+01 Q 1.4066
-00000cc0: 3134 3130 652b 3031 2035 2e34 3437 3531  1410e+01 5.44751
-00000cd0: 3936 3065 2b30 312c 2032 2e33 3030 3030  960e+01, 2.30000
-00000ce0: 3030 3065 2b30 3120 352e 3930 3030 3030  000e+01 5.900000
-00000cf0: 3030 652b 3031 205a 2220 2f3e 0d0a 2020  00e+01 Z" />..  
-00000d00: 2020 2020 3c70 6174 6820 643d 224d 2032      <path d="M 2
-00000d10: 2e34 3539 3535 3032 3065 2b30 3120 372e  .45955020e+01 7.
-00000d20: 3533 3439 3936 3730 652b 3031 2051 2031  53499670e+01 Q 1
-00000d30: 2e34 3539 3330 3436 3065 2b30 3120 362e  .45930460e+01 6.
-00000d40: 3234 3533 3631 3530 652b 3031 2c20 352e  24536150e+01, 5.
-00000d50: 3030 3030 3030 3030 652b 3030 2035 2e30  00000000e+00 5.0
-00000d60: 3030 3030 3030 3065 2b30 3120 5120 352e  0000000e+01 Q 5.
-00000d70: 3030 3030 3030 3030 652b 3030 2037 2e32  00000000e+00 7.2
-00000d80: 3530 3030 3030 3065 2b30 312c 2035 2e30  5000000e+01, 5.0
-00000d90: 3030 3030 3030 3065 2b30 3020 392e 3530  0000000e+00 9.50
-00000da0: 3030 3030 3030 652b 3031 2051 2031 2e34  000000e+01 Q 1.4
-00000db0: 3934 3038 3531 3065 2b30 3120 382e 3530  9408510e+01 8.50
-00000dc0: 3139 3239 3730 652b 3031 2c20 322e 3435  192970e+01, 2.45
-00000dd0: 3935 3530 3230 652b 3031 2037 2e35 3334  955020e+01 7.534
-00000de0: 3939 3637 3065 2b30 3120 5a22 202f 3e0d  99670e+01 Z" />.
-00000df0: 0a20 2020 2020 203c 7061 7468 2064 3d22  .      <path d="
-00000e00: 4d20 322e 3330 3030 3030 3030 652b 3031  M 2.30000000e+01
-00000e10: 2032 2e33 3030 3030 3030 3065 2b30 3120   2.30000000e+01 
-00000e20: 5120 312e 3339 3939 3736 3639 652b 3031  Q 1.39997669e+01
-00000e30: 2031 2e33 3939 3937 3636 3065 2b30 312c   1.39997660e+01,
-00000e40: 2035 2e30 3030 3030 3030 3065 2b30 3020   5.00000000e+00 
-00000e50: 352e 3030 3030 3030 3030 652b 3030 2051  5.00000000e+00 Q
-00000e60: 2035 2e30 3030 3030 3030 3065 2b30 3020   5.00000000e+00 
-00000e70: 322e 3735 3030 3030 3030 652b 3031 2c20  2.75000000e+01, 
-00000e80: 352e 3030 3030 3030 3030 652b 3030 2035  5.00000000e+00 5
-00000e90: 2e30 3030 3030 3030 3065 2b30 3120 5120  .00000000e+01 Q 
-00000ea0: 312e 3430 3031 3039 3830 652b 3031 2033  1.40010980e+01 3
-00000eb0: 2e36 3439 3730 3231 3065 2b30 312c 2032  .64970210e+01, 2
-00000ec0: 2e33 3030 3030 3030 3065 2b30 3120 322e  .30000000e+01 2.
-00000ed0: 3330 3030 3030 3030 652b 3031 205a 2220  30000000e+01 Z" 
-00000ee0: 2f3e 0d0a 2020 2020 2020 3c70 6174 6820  />..      <path 
-00000ef0: 643d 224d 2032 2e34 3539 3535 3032 3065  d="M 2.45955020e
-00000f00: 2b30 3120 372e 3533 3439 3936 3730 652b  +01 7.53499670e+
-00000f10: 3031 2051 2032 2e32 3338 3134 3636 3065  01 Q 2.23814660e
-00000f20: 2b30 3120 362e 3734 3335 3332 3230 652b  +01 6.74353220e+
-00000f30: 3031 2c20 322e 3330 3030 3030 3030 652b  01, 2.30000000e+
-00000f40: 3031 2035 2e39 3030 3030 3030 3065 2b30  01 5.90000000e+0
-00000f50: 3120 5120 312e 3430 3636 3134 3130 652b  1 Q 1.40661410e+
-00000f60: 3031 2035 2e34 3437 3531 3936 3065 2b30  01 5.44751960e+0
-00000f70: 312c 2035 2e30 3030 3030 3030 3065 2b30  1, 5.00000000e+0
-00000f80: 3020 352e 3030 3030 3030 3030 652b 3031  0 5.00000000e+01
-00000f90: 2051 2031 2e34 3539 3330 3436 3065 2b30   Q 1.45930460e+0
-00000fa0: 3120 362e 3234 3533 3631 3530 652b 3031  1 6.24536150e+01
-00000fb0: 2c20 322e 3435 3935 3530 3230 652b 3031  , 2.45955020e+01
-00000fc0: 2037 2e35 3334 3939 3637 3065 2b30 3120   7.53499670e+01 
-00000fd0: 5a22 202f 3e0d 0a20 2020 2020 203c 7061  Z" />..      <pa
-00000fe0: 7468 2064 3d22 4d20 322e 3330 3030 3030  th d="M 2.300000
-00000ff0: 3030 652b 3031 2032 2e33 3030 3030 3030  00e+01 2.3000000
-00001000: 3065 2b30 3120 5120 332e 3230 3030 3030  0e+01 Q 3.200000
-00001010: 3030 652b 3031 2032 2e33 3030 3030 3030  00e+01 2.3000000
-00001020: 3065 2b30 312c 2034 2e31 3030 3030 3030  0e+01, 4.1000000
-00001030: 3065 2b30 3120 322e 3330 3030 3030 3030  0e+01 2.30000000
-00001040: 652b 3031 2051 2034 2e35 3439 3134 3134  e+01 Q 4.5491414
-00001050: 3065 2b30 3120 312e 3430 3035 3935 3830  0e+01 1.40059580
-00001060: 652b 3031 2c20 352e 3030 3030 3030 3030  e+01, 5.00000000
-00001070: 652b 3031 2035 2e30 3030 3030 3030 3065  e+01 5.00000000e
-00001080: 2b30 3020 5120 332e 3634 3937 3035 3730  +00 Q 3.64970570
-00001090: 652b 3031 2031 2e34 3030 3131 3136 3065  e+01 1.40011160e
-000010a0: 2b30 312c 2032 2e33 3030 3030 3030 3065  +01, 2.30000000e
-000010b0: 2b30 3120 322e 3330 3030 3030 3030 652b  +01 2.30000000e+
-000010c0: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
-000010d0: 3c70 6174 6820 643d 224d 2034 2e31 3030  <path d="M 4.100
-000010e0: 3030 3030 3065 2b30 3120 322e 3330 3030  00000e+01 2.3000
-000010f0: 3030 3030 652b 3031 2051 2035 2e30 3030  0000e+01 Q 5.000
-00001100: 3030 3030 3065 2b30 3120 322e 3330 3030  00000e+01 2.3000
-00001110: 3030 3030 652b 3031 2c20 352e 3930 3030  0000e+01, 5.9000
-00001120: 3030 3030 652b 3031 2032 2e33 3030 3030  0000e+01 2.30000
-00001130: 3030 3065 2b30 3120 5120 352e 3434 3735  000e+01 Q 5.4475
-00001140: 3436 3630 652b 3031 2031 2e34 3036 3636  4660e+01 1.40666
-00001150: 3435 3065 2b30 312c 2035 2e30 3030 3030  450e+01, 5.00000
-00001160: 3030 3065 2b30 3120 352e 3030 3030 3030  000e+01 5.000000
-00001170: 3030 652b 3030 2051 2034 2e35 3439 3134  00e+00 Q 4.54914
-00001180: 3134 3065 2b30 3120 312e 3430 3035 3935  140e+01 1.400595
-00001190: 3830 652b 3031 2c20 342e 3130 3030 3030  80e+01, 4.100000
-000011a0: 3030 652b 3031 2032 2e33 3030 3030 3030  00e+01 2.3000000
-000011b0: 3065 2b30 3120 5a22 202f 3e0d 0a20 2020  0e+01 Z" />..   
-000011c0: 2020 203c 7061 7468 2064 3d22 4d20 392e     <path d="M 9.
-000011d0: 3530 3030 3030 3030 652b 3031 2035 2e30  50000000e+01 5.0
-000011e0: 3030 3030 3030 3065 2b30 3020 5120 372e  0000000e+00 Q 7.
-000011f0: 3235 3030 3030 3030 652b 3031 2035 2e30  25000000e+01 5.0
-00001200: 3030 3030 3030 3065 2b30 302c 2035 2e30  0000000e+00, 5.0
-00001210: 3030 3030 3030 3065 2b30 3120 352e 3030  0000000e+01 5.00
-00001220: 3030 3030 3030 652b 3030 2051 2036 2e32  000000e+00 Q 6.2
-00001230: 3438 3532 3134 3065 2b30 3120 312e 3436  4852140e+01 1.46
-00001240: 3138 3431 3730 652b 3031 2c20 372e 3534  184170e+01, 7.54
-00001250: 3133 3632 3430 652b 3031 2032 2e34 3635  136240e+01 2.465
-00001260: 3931 3539 3065 2b30 3120 5120 382e 3530  91590e+01 Q 8.50
-00001270: 3439 3237 3630 652b 3031 2031 2e34 3937  492760e+01 1.497
-00001280: 3039 3338 3065 2b30 312c 2039 2e35 3030  09380e+01, 9.500
-00001290: 3030 3030 3065 2b30 3120 352e 3030 3030  00000e+01 5.0000
-000012a0: 3030 3030 652b 3030 205a 2220 2f3e 0d0a  0000e+00 Z" />..
-000012b0: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
-000012c0: 2035 2e30 3030 3030 3030 3065 2b30 3020   5.00000000e+00 
-000012d0: 352e 3030 3030 3030 3030 652b 3030 2051  5.00000000e+00 Q
-000012e0: 2031 2e33 3939 3937 3636 3965 2b30 3120   1.39997669e+01 
-000012f0: 312e 3339 3939 3736 3630 652b 3031 2c20  1.39997660e+01, 
-00001300: 322e 3330 3030 3030 3030 652b 3031 2032  2.30000000e+01 2
-00001310: 2e33 3030 3030 3030 3065 2b30 3120 5120  .30000000e+01 Q 
-00001320: 332e 3634 3937 3035 3730 652b 3031 2031  3.64970570e+01 1
-00001330: 2e34 3030 3131 3136 3065 2b30 312c 2035  .40011160e+01, 5
-00001340: 2e30 3030 3030 3030 3065 2b30 3120 352e  .00000000e+01 5.
-00001350: 3030 3030 3030 3030 652b 3030 2051 2032  00000000e+00 Q 2
-00001360: 2e37 3530 3030 3030 3065 2b30 3120 352e  .75000000e+01 5.
-00001370: 3030 3030 3030 3030 652b 3030 2c20 352e  00000000e+00, 5.
-00001380: 3030 3030 3030 3030 652b 3030 2035 2e30  00000000e+00 5.0
-00001390: 3030 3030 3030 3065 2b30 3020 5a22 202f  0000000e+00 Z" /
-000013a0: 3e0d 0a20 2020 2020 203c 7061 7468 2064  >..      <path d
-000013b0: 3d22 4d20 352e 3930 3030 3030 3030 652b  ="M 5.90000000e+
-000013c0: 3031 2032 2e33 3030 3030 3030 3065 2b30  01 2.30000000e+0
-000013d0: 3120 5120 362e 3734 3638 3838 3330 652b  1 Q 6.74688830e+
-000013e0: 3031 2032 2e32 3430 3437 3331 3065 2b30  01 2.24047310e+0
-000013f0: 312c 2037 2e35 3431 3336 3234 3065 2b30  1, 7.54136240e+0
-00001400: 3120 322e 3436 3539 3135 3930 652b 3031  1 2.46591590e+01
-00001410: 2051 2036 2e32 3438 3532 3134 3065 2b30   Q 6.24852140e+0
-00001420: 3120 312e 3436 3138 3431 3730 652b 3031  1 1.46184170e+01
-00001430: 2c20 352e 3030 3030 3030 3030 652b 3031  , 5.00000000e+01
-00001440: 2035 2e30 3030 3030 3030 3065 2b30 3020   5.00000000e+00 
-00001450: 5120 352e 3434 3735 3436 3630 652b 3031  Q 5.44754660e+01
-00001460: 2031 2e34 3036 3636 3435 3065 2b30 312c   1.40666450e+01,
-00001470: 2035 2e39 3030 3030 3030 3065 2b30 3120   5.90000000e+01 
-00001480: 322e 3330 3030 3030 3030 652b 3031 205a  2.30000000e+01 Z
-00001490: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
-000014a0: 6820 643d 224d 2032 2e34 3539 3535 3032  h d="M 2.4595502
-000014b0: 3065 2b30 3120 372e 3533 3439 3936 3730  0e+01 7.53499670
-000014c0: 652b 3031 2051 2032 2e36 3434 3439 3834  e+01 Q 2.6444984
-000014d0: 3065 2b30 3120 372e 3335 3237 3637 3430  0e+01 7.35276740
-000014e0: 652b 3031 2c20 322e 3832 3732 3037 3430  e+01, 2.82720740
-000014f0: 652b 3031 2037 2e31 3732 3739 3236 3065  e+01 7.17279260e
-00001500: 2b30 3120 5120 322e 3330 3030 3030 3030  +01 Q 2.30000000
-00001510: 652b 3031 2036 2e36 3435 3538 3433 3065  e+01 6.64558430e
-00001520: 2b30 312c 2032 2e33 3030 3030 3030 3065  +01, 2.30000000e
-00001530: 2b30 3120 352e 3930 3030 3030 3030 652b  +01 5.90000000e+
-00001540: 3031 2051 2032 2e32 3338 3134 3636 3065  01 Q 2.23814660e
-00001550: 2b30 3120 362e 3734 3335 3332 3230 652b  +01 6.74353220e+
-00001560: 3031 2c20 322e 3435 3935 3530 3230 652b  01, 2.45955020e+
-00001570: 3031 2037 2e35 3334 3939 3637 3065 2b30  01 7.53499670e+0
-00001580: 3120 5a22 202f 3e0d 0a20 2020 2020 203c  1 Z" />..      <
-00001590: 7061 7468 2064 3d22 4d20 342e 3130 3030  path d="M 4.1000
-000015a0: 3030 3030 652b 3031 2037 2e37 3030 3030  0000e+01 7.70000
-000015b0: 3030 3065 2b30 3120 5120 332e 3335 3434  000e+01 Q 3.3544
-000015c0: 3135 3730 652b 3031 2037 2e37 3030 3030  1570e+01 7.70000
-000015d0: 3030 3065 2b30 312c 2032 2e38 3237 3230  000e+01, 2.82720
-000015e0: 3734 3065 2b30 3120 372e 3137 3237 3932  740e+01 7.172792
-000015f0: 3630 652b 3031 2051 2032 2e36 3434 3439  60e+01 Q 2.64449
-00001600: 3834 3065 2b30 3120 372e 3335 3237 3637  840e+01 7.352767
-00001610: 3430 652b 3031 2c20 322e 3435 3935 3530  40e+01, 2.459550
-00001620: 3230 652b 3031 2037 2e35 3334 3939 3637  20e+01 7.5349967
-00001630: 3065 2b30 3120 5120 332e 3235 3336 3230  0e+01 Q 3.253620
-00001640: 3230 652b 3031 2037 2e37 3538 3832 3133  20e+01 7.7588213
-00001650: 3065 2b30 312c 2034 2e31 3030 3030 3030  0e+01, 4.1000000
-00001660: 3065 2b30 3120 372e 3730 3030 3030 3030  0e+01 7.70000000
-00001670: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
-00001680: 2020 3c70 6174 6820 643d 224d 2039 2e35    <path d="M 9.5
-00001690: 3030 3030 3030 3065 2b30 3120 392e 3530  0000000e+01 9.50
-000016a0: 3030 3030 3030 652b 3031 2051 2038 2e32  000000e+01 Q 8.2
-000016b0: 3930 3339 3535 3065 2b30 3120 382e 3238  9039550e+01 8.28
-000016c0: 3539 3734 3730 652b 3031 2c20 372e 3130  597470e+01, 7.10
-000016d0: 3933 3732 3330 652b 3031 2037 2e31 3030  937230e+01 7.100
-000016e0: 3431 3733 3065 2b30 3120 5120 362e 3035  41730e+01 Q 6.05
-000016f0: 3338 3130 3030 652b 3031 2038 2e33 3033  381000e+01 8.303
-00001700: 3232 3836 3065 2b30 312c 2035 2e30 3030  22860e+01, 5.000
-00001710: 3030 3030 3065 2b30 3120 392e 3530 3030  00000e+01 9.5000
-00001720: 3030 3030 652b 3031 2051 2037 2e32 3530  0000e+01 Q 7.250
-00001730: 3030 3030 3065 2b30 3120 392e 3530 3030  00000e+01 9.5000
-00001740: 3030 3030 652b 3031 2c20 392e 3530 3030  0000e+01, 9.5000
-00001750: 3030 3030 652b 3031 2039 2e35 3030 3030  0000e+01 9.50000
-00001760: 3030 3065 2b30 3120 5a22 202f 3e0d 0a20  000e+01 Z" />.. 
-00001770: 2020 2020 203c 7061 7468 2064 3d22 4d20       <path d="M 
-00001780: 352e 3030 3030 3030 3030 652b 3030 2039  5.00000000e+00 9
-00001790: 2e35 3030 3030 3030 3065 2b30 3120 5120  .50000000e+01 Q 
-000017a0: 322e 3735 3030 3030 3030 652b 3031 2039  2.75000000e+01 9
-000017b0: 2e35 3030 3030 3030 3065 2b30 312c 2035  .50000000e+01, 5
-000017c0: 2e30 3030 3030 3030 3065 2b30 3120 392e  .00000000e+01 9.
-000017d0: 3530 3030 3030 3030 652b 3031 2051 2033  50000000e+01 Q 3
-000017e0: 2e37 3439 3637 3332 3065 2b30 3120 382e  .74967320e+01 8.
-000017f0: 3534 3532 3537 3530 652b 3031 2c20 322e  54525750e+01, 2.
-00001800: 3435 3935 3530 3230 652b 3031 2037 2e35  45955020e+01 7.5
-00001810: 3334 3939 3637 3065 2b30 3120 5120 312e  3499670e+01 Q 1.
-00001820: 3439 3430 3835 3130 652b 3031 2038 2e35  49408510e+01 8.5
-00001830: 3031 3932 3937 3065 2b30 312c 2035 2e30  0192970e+01, 5.0
-00001840: 3030 3030 3030 3065 2b30 3020 392e 3530  0000000e+00 9.50
-00001850: 3030 3030 3030 652b 3031 205a 2220 2f3e  000000e+01 Z" />
-00001860: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
-00001870: 224d 2034 2e31 3030 3030 3030 3065 2b30  "M 4.10000000e+0
-00001880: 3120 372e 3730 3030 3030 3030 652b 3031  1 7.70000000e+01
-00001890: 2051 2033 2e32 3533 3632 3032 3065 2b30   Q 3.25362020e+0
-000018a0: 3120 372e 3735 3838 3231 3330 652b 3031  1 7.75882130e+01
-000018b0: 2c20 322e 3435 3935 3530 3230 652b 3031  , 2.45955020e+01
-000018c0: 2037 2e35 3334 3939 3637 3065 2b30 3120   7.53499670e+01 
-000018d0: 5120 332e 3734 3936 3733 3230 652b 3031  Q 3.74967320e+01
-000018e0: 2038 2e35 3435 3235 3735 3065 2b30 312c   8.54525750e+01,
-000018f0: 2035 2e30 3030 3030 3030 3065 2b30 3120   5.00000000e+01 
-00001900: 392e 3530 3030 3030 3030 652b 3031 2051  9.50000000e+01 Q
-00001910: 2034 2e35 3533 3430 3230 3065 2b30 3120   4.55340200e+01 
-00001920: 382e 3631 3630 3037 3331 652b 3031 2c20  8.61600731e+01, 
-00001930: 342e 3130 3030 3030 3030 652b 3031 2037  4.10000000e+01 7
-00001940: 2e37 3030 3030 3030 3065 2b30 3120 5a22  .70000000e+01 Z"
-00001950: 202f 3e0d 0a20 2020 3c2f 673e 0d0a 2020   />..   </g>..  
-00001960: 203c 6720 6964 3d22 4e6f 6465 7322 2066   <g id="Nodes" f
-00001970: 696c 6c3d 2223 6139 3565 3565 223e 0d0a  ill="#a95e5e">..
-00001980: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00001990: 3d22 342e 3834 3535 3834 3330 652b 3031  ="4.84558430e+01
-000019a0: 2220 6379 3d22 372e 3730 3030 3030 3030  " cy="7.70000000
-000019b0: 652b 3031 2220 723d 2231 2e32 3237 3434  e+01" r="1.22744
-000019c0: 3235 3735 3238 3431 3630 3722 202f 3e0d  25752841607" />.
-000019d0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-000019e0: 783d 2235 2e33 3732 3739 3236 3065 2b30  x="5.37279260e+0
-000019f0: 3122 2063 793d 2237 2e31 3732 3739 3236  1" cy="7.1727926
-00001a00: 3065 2b30 3122 2072 3d22 312e 3232 3734  0e+01" r="1.2274
-00001a10: 3432 3537 3532 3834 3136 3037 2220 2f3e  425752841607" />
-00001a20: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00001a30: 6378 3d22 352e 3930 3030 3030 3030 652b  cx="5.90000000e+
-00001a40: 3031 2220 6379 3d22 362e 3634 3535 3834  01" cy="6.645584
-00001a50: 3330 652b 3031 2220 723d 2231 2e32 3237  30e+01" r="1.227
-00001a60: 3434 3235 3735 3238 3431 3630 3722 202f  4425752841607" /
-00001a70: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00001a80: 2063 783d 2239 2e35 3030 3030 3030 3065   cx="9.50000000e
-00001a90: 2b30 3122 2063 793d 2237 2e32 3530 3030  +01" cy="7.25000
-00001aa0: 3030 3065 2b30 3122 2072 3d22 312e 3232  000e+01" r="1.22
-00001ab0: 3734 3432 3537 3532 3834 3136 3037 2220  74425752841607" 
-00001ac0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00001ad0: 6520 6378 3d22 392e 3530 3030 3030 3030  e cx="9.50000000
-00001ae0: 652b 3031 2220 6379 3d22 352e 3030 3030  e+01" cy="5.0000
-00001af0: 3030 3030 652b 3031 2220 723d 2231 2e32  0000e+01" r="1.2
-00001b00: 3237 3434 3235 3735 3238 3431 3630 3722  274425752841607"
-00001b10: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00001b20: 6c65 2063 783d 2239 2e35 3030 3030 3030  le cx="9.5000000
-00001b30: 3065 2b30 3122 2063 793d 2232 2e37 3530  0e+01" cy="2.750
-00001b40: 3030 3030 3065 2b30 3122 2072 3d22 312e  00000e+01" r="1.
-00001b50: 3232 3734 3432 3537 3532 3834 3136 3037  2274425752841607
-00001b60: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00001b70: 636c 6520 6378 3d22 362e 3634 3535 3834  cle cx="6.645584
-00001b80: 3330 652b 3031 2220 6379 3d22 352e 3930  30e+01" cy="5.90
-00001b90: 3030 3030 3030 652b 3031 2220 723d 2231  000000e+01" r="1
-00001ba0: 2e32 3237 3434 3235 3735 3238 3431 3630  .227442575284160
-00001bb0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00001bc0: 7263 6c65 2063 783d 2237 2e31 3732 3739  rcle cx="7.17279
-00001bd0: 3236 3065 2b30 3122 2063 793d 2235 2e33  260e+01" cy="5.3
-00001be0: 3732 3739 3236 3065 2b30 3122 2072 3d22  7279260e+01" r="
-00001bf0: 312e 3232 3734 3432 3537 3532 3834 3136  1.22744257528416
-00001c00: 3037 2220 2f3e 0d0a 2020 2020 2020 3c63  07" />..      <c
-00001c10: 6972 636c 6520 6378 3d22 372e 3730 3030  ircle cx="7.7000
-00001c20: 3030 3030 652b 3031 2220 6379 3d22 342e  0000e+01" cy="4.
-00001c30: 3834 3535 3834 3330 652b 3031 2220 723d  84558430e+01" r=
-00001c40: 2231 2e32 3237 3434 3235 3735 3238 3431  "1.2274425752841
-00001c50: 3630 3722 202f 3e0d 0a20 2020 2020 203c  607" />..      <
-00001c60: 6369 7263 6c65 2063 783d 2237 2e37 3030  circle cx="7.700
-00001c70: 3030 3030 3065 2b30 3122 2063 793d 2233  00000e+01" cy="3
-00001c80: 2e33 3534 3431 3537 3065 2b30 3122 2072  .35441570e+01" r
-00001c90: 3d22 312e 3232 3734 3432 3537 3532 3834  ="1.227442575284
-00001ca0: 3136 3037 2220 2f3e 0d0a 2020 2020 2020  1607" />..      
-00001cb0: 3c63 6972 636c 6520 6378 3d22 372e 3137  <circle cx="7.17
-00001cc0: 3237 3932 3630 652b 3031 2220 6379 3d22  279260e+01" cy="
-00001cd0: 322e 3832 3732 3037 3430 652b 3031 2220  2.82720740e+01" 
-00001ce0: 723d 2231 2e32 3237 3434 3235 3735 3238  r="1.22744257528
-00001cf0: 3431 3630 3722 202f 3e0d 0a20 2020 2020  41607" />..     
-00001d00: 203c 6369 7263 6c65 2063 783d 2236 2e36   <circle cx="6.6
-00001d10: 3435 3538 3433 3065 2b30 3122 2063 793d  4558430e+01" cy=
-00001d20: 2232 2e33 3030 3030 3030 3065 2b30 3122  "2.30000000e+01"
-00001d30: 2072 3d22 312e 3232 3734 3432 3537 3532   r="1.2274425752
-00001d40: 3834 3136 3037 2220 2f3e 0d0a 2020 2020  841607" />..    
-00001d50: 2020 3c63 6972 636c 6520 6378 3d22 352e    <circle cx="5.
-00001d60: 3030 3030 3030 3030 652b 3030 2220 6379  00000000e+00" cy
-00001d70: 3d22 322e 3735 3030 3030 3030 652b 3031  ="2.75000000e+01
-00001d80: 2220 723d 2231 2e32 3237 3434 3235 3735  " r="1.227442575
-00001d90: 3238 3431 3630 3722 202f 3e0d 0a20 2020  2841607" />..   
-00001da0: 2020 203c 6369 7263 6c65 2063 783d 2235     <circle cx="5
-00001db0: 2e30 3030 3030 3030 3065 2b30 3022 2063  .00000000e+00" c
-00001dc0: 793d 2235 2e30 3030 3030 3030 3065 2b30  y="5.00000000e+0
-00001dd0: 3122 2072 3d22 312e 3232 3734 3432 3537  1" r="1.22744257
-00001de0: 3532 3834 3136 3037 2220 2f3e 0d0a 2020  52841607" />..  
-00001df0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00001e00: 352e 3030 3030 3030 3030 652b 3030 2220  5.00000000e+00" 
-00001e10: 6379 3d22 372e 3235 3030 3030 3030 652b  cy="7.25000000e+
-00001e20: 3031 2220 723d 2231 2e32 3237 3434 3235  01" r="1.2274425
-00001e30: 3735 3238 3431 3630 3722 202f 3e0d 0a20  752841607" />.. 
-00001e40: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00001e50: 2237 2e32 3530 3030 3030 3065 2b30 3122  "7.25000000e+01"
-00001e60: 2063 793d 2235 2e30 3030 3030 3030 3065   cy="5.00000000e
-00001e70: 2b30 3022 2072 3d22 312e 3232 3734 3432  +00" r="1.227442
-00001e80: 3537 3532 3834 3136 3037 2220 2f3e 0d0a  5752841607" />..
-00001e90: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00001ea0: 3d22 352e 3030 3030 3030 3030 652b 3031  ="5.00000000e+01
-00001eb0: 2220 6379 3d22 352e 3030 3030 3030 3030  " cy="5.00000000
-00001ec0: 652b 3030 2220 723d 2231 2e32 3237 3434  e+00" r="1.22744
-00001ed0: 3235 3735 3238 3431 3630 3722 202f 3e0d  25752841607" />.
-00001ee0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00001ef0: 783d 2232 2e37 3530 3030 3030 3065 2b30  x="2.75000000e+0
-00001f00: 3122 2063 793d 2235 2e30 3030 3030 3030  1" cy="5.0000000
-00001f10: 3065 2b30 3022 2072 3d22 312e 3232 3734  0e+00" r="1.2274
-00001f20: 3432 3537 3532 3834 3136 3037 2220 2f3e  425752841607" />
-00001f30: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00001f40: 6378 3d22 322e 3330 3030 3030 3030 652b  cx="2.30000000e+
-00001f50: 3031 2220 6379 3d22 362e 3634 3535 3834  01" cy="6.645584
-00001f60: 3330 652b 3031 2220 723d 2231 2e32 3237  30e+01" r="1.227
-00001f70: 3434 3235 3735 3238 3431 3630 3722 202f  4425752841607" /
-00001f80: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00001f90: 2063 783d 2232 2e38 3237 3230 3734 3065   cx="2.82720740e
-00001fa0: 2b30 3122 2063 793d 2237 2e31 3732 3739  +01" cy="7.17279
-00001fb0: 3236 3065 2b30 3122 2072 3d22 312e 3232  260e+01" r="1.22
-00001fc0: 3734 3432 3537 3532 3834 3136 3037 2220  74425752841607" 
-00001fd0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00001fe0: 6520 6378 3d22 332e 3335 3434 3135 3730  e cx="3.35441570
-00001ff0: 652b 3031 2220 6379 3d22 372e 3730 3030  e+01" cy="7.7000
-00002000: 3030 3030 652b 3031 2220 723d 2231 2e32  0000e+01" r="1.2
-00002010: 3237 3434 3235 3735 3238 3431 3630 3722  274425752841607"
-00002020: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00002030: 6c65 2063 783d 2235 2e30 3030 3030 3030  le cx="5.0000000
-00002040: 3065 2b30 3122 2063 793d 2232 2e33 3030  0e+01" cy="2.300
-00002050: 3030 3030 3065 2b30 3122 2072 3d22 312e  00000e+01" r="1.
-00002060: 3232 3734 3432 3537 3532 3834 3136 3037  2274425752841607
-00002070: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00002080: 636c 6520 6378 3d22 342e 3130 3030 3030  cle cx="4.100000
-00002090: 3030 652b 3031 2220 6379 3d22 322e 3330  00e+01" cy="2.30
-000020a0: 3030 3030 3030 652b 3031 2220 723d 2231  000000e+01" r="1
-000020b0: 2e32 3237 3434 3235 3735 3238 3431 3630  .227442575284160
-000020c0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-000020d0: 7263 6c65 2063 783d 2233 2e32 3030 3030  rcle cx="3.20000
-000020e0: 3030 3065 2b30 3122 2063 793d 2232 2e33  000e+01" cy="2.3
-000020f0: 3030 3030 3030 3065 2b30 3122 2072 3d22  0000000e+01" r="
-00002100: 312e 3232 3734 3432 3537 3532 3834 3136  1.22744257528416
-00002110: 3037 2220 2f3e 0d0a 2020 2020 2020 3c63  07" />..      <c
-00002120: 6972 636c 6520 6378 3d22 322e 3735 3030  ircle cx="2.7500
-00002130: 3030 3030 652b 3031 2220 6379 3d22 392e  0000e+01" cy="9.
-00002140: 3530 3030 3030 3030 652b 3031 2220 723d  50000000e+01" r=
-00002150: 2231 2e32 3237 3434 3235 3735 3238 3431  "1.2274425752841
-00002160: 3630 3722 202f 3e0d 0a20 2020 2020 203c  607" />..      <
-00002170: 6369 7263 6c65 2063 783d 2235 2e30 3030  circle cx="5.000
-00002180: 3030 3030 3065 2b30 3122 2063 793d 2239  00000e+01" cy="9
-00002190: 2e35 3030 3030 3030 3065 2b30 3122 2072  .50000000e+01" r
-000021a0: 3d22 312e 3232 3734 3432 3537 3532 3834  ="1.227442575284
-000021b0: 3136 3037 2220 2f3e 0d0a 2020 2020 2020  1607" />..      
-000021c0: 3c63 6972 636c 6520 6378 3d22 372e 3235  <circle cx="7.25
-000021d0: 3030 3030 3030 652b 3031 2220 6379 3d22  000000e+01" cy="
-000021e0: 392e 3530 3030 3030 3030 652b 3031 2220  9.50000000e+01" 
-000021f0: 723d 2231 2e32 3237 3434 3235 3735 3238  r="1.22744257528
-00002200: 3431 3630 3722 202f 3e0d 0a20 2020 2020  41607" />..     
-00002210: 203c 6369 7263 6c65 2063 783d 2232 2e33   <circle cx="2.3
-00002220: 3030 3030 3030 3065 2b30 3122 2063 793d  0000000e+01" cy=
-00002230: 2233 2e32 3030 3030 3030 3065 2b30 3122  "3.20000000e+01"
-00002240: 2072 3d22 312e 3232 3734 3432 3537 3532   r="1.2274425752
-00002250: 3834 3136 3037 2220 2f3e 0d0a 2020 2020  841607" />..    
-00002260: 2020 3c63 6972 636c 6520 6378 3d22 322e    <circle cx="2.
-00002270: 3330 3030 3030 3030 652b 3031 2220 6379  30000000e+01" cy
-00002280: 3d22 342e 3130 3030 3030 3030 652b 3031  ="4.10000000e+01
-00002290: 2220 723d 2231 2e32 3237 3434 3235 3735  " r="1.227442575
-000022a0: 3238 3431 3630 3722 202f 3e0d 0a20 2020  2841607" />..   
-000022b0: 2020 203c 6369 7263 6c65 2063 783d 2232     <circle cx="2
-000022c0: 2e33 3030 3030 3030 3065 2b30 3122 2063  .30000000e+01" c
-000022d0: 793d 2235 2e30 3030 3030 3030 3065 2b30  y="5.00000000e+0
-000022e0: 3122 2072 3d22 312e 3232 3734 3432 3537  1" r="1.22744257
-000022f0: 3532 3834 3136 3037 2220 2f3e 0d0a 2020  52841607" />..  
-00002300: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00002310: 392e 3530 3030 3030 3030 652b 3031 2220  9.50000000e+01" 
-00002320: 6379 3d22 392e 3530 3030 3030 3030 652b  cy="9.50000000e+
-00002330: 3031 2220 723d 2231 2e32 3237 3434 3235  01" r="1.2274425
-00002340: 3735 3238 3431 3630 3722 202f 3e0d 0a20  752841607" />.. 
-00002350: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00002360: 2239 2e35 3030 3030 3030 3065 2b30 3122  "9.50000000e+01"
-00002370: 2063 793d 2235 2e30 3030 3030 3030 3065   cy="5.00000000e
-00002380: 2b30 3022 2072 3d22 312e 3232 3734 3432  +00" r="1.227442
-00002390: 3537 3532 3834 3136 3037 2220 2f3e 0d0a  5752841607" />..
-000023a0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-000023b0: 3d22 352e 3030 3030 3030 3030 652b 3030  ="5.00000000e+00
-000023c0: 2220 6379 3d22 392e 3530 3030 3030 3030  " cy="9.50000000
-000023d0: 652b 3031 2220 723d 2231 2e32 3237 3434  e+01" r="1.22744
-000023e0: 3235 3735 3238 3431 3630 3722 202f 3e0d  25752841607" />.
-000023f0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00002400: 783d 2235 2e30 3030 3030 3030 3065 2b30  x="5.00000000e+0
-00002410: 3022 2063 793d 2235 2e30 3030 3030 3030  0" cy="5.0000000
-00002420: 3065 2b30 3022 2072 3d22 312e 3232 3734  0e+00" r="1.2274
-00002430: 3432 3537 3532 3834 3136 3037 2220 2f3e  425752841607" />
-00002440: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00002450: 6378 3d22 322e 3330 3030 3030 3030 652b  cx="2.30000000e+
-00002460: 3031 2220 6379 3d22 322e 3330 3030 3030  01" cy="2.300000
-00002470: 3030 652b 3031 2220 723d 2231 2e32 3237  00e+01" r="1.227
-00002480: 3434 3235 3735 3238 3431 3630 3722 202f  4425752841607" /
-00002490: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-000024a0: 2063 783d 2232 2e33 3030 3030 3030 3065   cx="2.30000000e
-000024b0: 2b30 3122 2063 793d 2235 2e39 3030 3030  +01" cy="5.90000
-000024c0: 3030 3065 2b30 3122 2072 3d22 312e 3232  000e+01" r="1.22
-000024d0: 3734 3432 3537 3532 3834 3136 3037 2220  74425752841607" 
-000024e0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-000024f0: 6520 6378 3d22 342e 3130 3030 3030 3030  e cx="4.10000000
-00002500: 652b 3031 2220 6379 3d22 372e 3730 3030  e+01" cy="7.7000
-00002510: 3030 3030 652b 3031 2220 723d 2231 2e32  0000e+01" r="1.2
-00002520: 3237 3434 3235 3735 3238 3431 3630 3722  274425752841607"
-00002530: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00002540: 6c65 2063 783d 2235 2e39 3030 3030 3030  le cx="5.9000000
-00002550: 3065 2b30 3122 2063 793d 2235 2e39 3030  0e+01" cy="5.900
-00002560: 3030 3030 3065 2b30 3122 2072 3d22 312e  00000e+01" r="1.
-00002570: 3232 3734 3432 3537 3532 3834 3136 3037  2274425752841607
-00002580: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00002590: 636c 6520 6378 3d22 372e 3730 3030 3030  cle cx="7.700000
-000025a0: 3030 652b 3031 2220 6379 3d22 342e 3130  00e+01" cy="4.10
-000025b0: 3030 3030 3030 652b 3031 2220 723d 2231  000000e+01" r="1
-000025c0: 2e32 3237 3434 3235 3735 3238 3431 3630  .227442575284160
-000025d0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-000025e0: 7263 6c65 2063 783d 2235 2e39 3030 3030  rcle cx="5.90000
-000025f0: 3030 3065 2b30 3122 2063 793d 2232 2e33  000e+01" cy="2.3
-00002600: 3030 3030 3030 3065 2b30 3122 2072 3d22  0000000e+01" r="
-00002610: 312e 3232 3734 3432 3537 3532 3834 3136  1.22744257528416
-00002620: 3037 2220 2f3e 0d0a 2020 2020 2020 3c63  07" />..      <c
-00002630: 6972 636c 6520 6378 3d22 372e 3130 3933  ircle cx="7.1093
-00002640: 3732 3330 652b 3031 2220 6379 3d22 372e  7230e+01" cy="7.
-00002650: 3130 3034 3137 3330 652b 3031 2220 723d  10041730e+01" r=
-00002660: 2231 2e32 3237 3434 3235 3735 3238 3431  "1.2274425752841
-00002670: 3630 3722 202f 3e0d 0a20 2020 2020 203c  607" />..      <
-00002680: 6369 7263 6c65 2063 783d 2237 2e35 3431  circle cx="7.541
-00002690: 3336 3234 3065 2b30 3122 2063 793d 2232  36240e+01" cy="2
-000026a0: 2e34 3635 3931 3539 3065 2b30 3122 2072  .46591590e+01" r
-000026b0: 3d22 312e 3232 3734 3432 3537 3532 3834  ="1.227442575284
-000026c0: 3136 3037 2220 2f3e 0d0a 2020 2020 2020  1607" />..      
-000026d0: 3c63 6972 636c 6520 6378 3d22 332e 3734  <circle cx="3.74
-000026e0: 3936 3733 3230 652b 3031 2220 6379 3d22  967320e+01" cy="
-000026f0: 382e 3534 3532 3537 3530 652b 3031 2220  8.54525750e+01" 
-00002700: 723d 2231 2e32 3237 3434 3235 3735 3238  r="1.22744257528
-00002710: 3431 3630 3722 202f 3e0d 0a20 2020 2020  41607" />..     
-00002720: 203c 6369 7263 6c65 2063 783d 2238 2e32   <circle cx="8.2
-00002730: 3930 3339 3535 3065 2b30 3122 2063 793d  9039550e+01" cy=
-00002740: 2238 2e32 3835 3937 3437 3065 2b30 3122  "8.28597470e+01"
-00002750: 2072 3d22 312e 3232 3734 3432 3537 3532   r="1.2274425752
-00002760: 3834 3136 3037 2220 2f3e 0d0a 2020 2020  841607" />..    
-00002770: 2020 3c63 6972 636c 6520 6378 3d22 312e    <circle cx="1.
-00002780: 3439 3430 3835 3130 652b 3031 2220 6379  49408510e+01" cy
-00002790: 3d22 382e 3530 3139 3239 3730 652b 3031  ="8.50192970e+01
-000027a0: 2220 723d 2231 2e32 3237 3434 3235 3735  " r="1.227442575
-000027b0: 3238 3431 3630 3722 202f 3e0d 0a20 2020  2841607" />..   
-000027c0: 2020 203c 6369 7263 6c65 2063 783d 2237     <circle cx="7
-000027d0: 2e33 3535 3839 3133 3065 2b30 3122 2063  .35589130e+01" c
-000027e0: 793d 2232 2e36 3437 3631 3936 3065 2b30  y="2.64761960e+0
-000027f0: 3122 2072 3d22 312e 3232 3734 3432 3537  1" r="1.22744257
-00002800: 3532 3834 3136 3037 2220 2f3e 0d0a 2020  52841607" />..  
-00002810: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00002820: 322e 3233 3831 3436 3630 652b 3031 2220  2.23814660e+01" 
-00002830: 6379 3d22 362e 3734 3335 3332 3230 652b  cy="6.74353220e+
-00002840: 3031 2220 723d 2231 2e32 3237 3434 3235  01" r="1.2274425
-00002850: 3735 3238 3431 3630 3722 202f 3e0d 0a20  752841607" />.. 
-00002860: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00002870: 2231 2e34 3036 3631 3431 3065 2b30 3122  "1.40661410e+01"
-00002880: 2063 793d 2235 2e34 3437 3531 3936 3065   cy="5.44751960e
-00002890: 2b30 3122 2072 3d22 312e 3232 3734 3432  +01" r="1.227442
-000028a0: 3537 3532 3834 3136 3037 2220 2f3e 0d0a  5752841607" />..
-000028b0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-000028c0: 3d22 362e 3035 3338 3130 3030 652b 3031  ="6.05381000e+01
-000028d0: 2220 6379 3d22 382e 3330 3332 3238 3630  " cy="8.30322860
-000028e0: 652b 3031 2220 723d 2231 2e32 3237 3434  e+01" r="1.22744
-000028f0: 3235 3735 3238 3431 3630 3722 202f 3e0d  25752841607" />.
-00002900: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00002910: 783d 2235 2e32 3238 3538 3239 3065 2b30  x="5.22858290e+0
-00002920: 3122 2063 793d 2238 2e33 3835 3338 3630  1" cy="8.3853860
-00002930: 3065 2b30 3122 2072 3d22 312e 3232 3734  0e+01" r="1.2274
-00002940: 3432 3537 3532 3834 3136 3037 2220 2f3e  425752841607" />
-00002950: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00002960: 6378 3d22 312e 3430 3035 3932 3230 652b  cx="1.40059220e+
-00002970: 3031 2220 6379 3d22 342e 3534 3931 3332  01" cy="4.549132
-00002980: 3430 652b 3031 2220 723d 2231 2e32 3237  40e+01" r="1.227
-00002990: 3434 3235 3735 3238 3431 3630 3722 202f  4425752841607" /
-000029a0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-000029b0: 2063 783d 2234 2e35 3439 3134 3134 3065   cx="4.54914140e
-000029c0: 2b30 3122 2063 793d 2231 2e34 3030 3539  +01" cy="1.40059
-000029d0: 3538 3065 2b30 3122 2072 3d22 312e 3232  580e+01" r="1.22
-000029e0: 3734 3432 3537 3532 3834 3136 3037 2220  74425752841607" 
-000029f0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00002a00: 6520 6378 3d22 322e 3435 3935 3530 3230  e cx="2.45955020
-00002a10: 652b 3031 2220 6379 3d22 372e 3533 3439  e+01" cy="7.5349
-00002a20: 3936 3730 652b 3031 2220 723d 2231 2e32  9670e+01" r="1.2
-00002a30: 3237 3434 3235 3735 3238 3431 3630 3722  274425752841607"
-00002a40: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00002a50: 6c65 2063 783d 2236 2e35 3535 3330 3335  le cx="6.5553035
-00002a60: 3065 2b30 3122 2063 793d 2236 2e35 3531  0e+01" cy="6.551
-00002a70: 3332 3337 3065 2b30 3122 2072 3d22 312e  32370e+01" r="1.
-00002a80: 3232 3734 3432 3537 3532 3834 3136 3037  2274425752841607
-00002a90: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00002aa0: 636c 6520 6378 3d22 382e 3631 3631 3437  cle cx="8.616147
-00002ab0: 3830 652b 3031 2220 6379 3d22 342e 3535  80e+01" cy="4.55
-00002ac0: 3334 3638 3630 652b 3031 2220 723d 2231  346860e+01" r="1
-00002ad0: 2e32 3237 3434 3235 3735 3238 3431 3630  .227442575284160
-00002ae0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00002af0: 7263 6c65 2063 783d 2231 2e33 3939 3937  rcle cx="1.39997
-00002b00: 3636 3965 2b30 3122 2063 793d 2231 2e33  669e+01" cy="1.3
-00002b10: 3939 3937 3636 3065 2b30 3122 2072 3d22  9997660e+01" r="
-00002b20: 312e 3232 3734 3432 3537 3532 3834 3136  1.22744257528416
-00002b30: 3037 2220 2f3e 0d0a 2020 2020 2020 3c63  07" />..      <c
-00002b40: 6972 636c 6520 6378 3d22 382e 3330 3735  ircle cx="8.3075
-00002b50: 3632 3130 652b 3031 2220 6379 3d22 362e  6210e+01" cy="6.
-00002b60: 3034 3933 3332 3530 652b 3031 2220 723d  04933250e+01" r=
-00002b70: 2231 2e32 3237 3434 3235 3735 3238 3431  "1.2274425752841
-00002b80: 3630 3722 202f 3e0d 0a20 2020 2020 203c  607" />..      <
-00002b90: 6369 7263 6c65 2063 783d 2236 2e37 3436  circle cx="6.746
-00002ba0: 3838 3833 3065 2b30 3122 2063 793d 2232  88830e+01" cy="2
-00002bb0: 2e32 3430 3437 3331 3065 2b30 3122 2072  .24047310e+01" r
-00002bc0: 3d22 312e 3232 3734 3432 3537 3532 3834  ="1.227442575284
-00002bd0: 3136 3037 2220 2f3e 0d0a 2020 2020 2020  1607" />..      
-00002be0: 3c63 6972 636c 6520 6378 3d22 312e 3435  <circle cx="1.45
-00002bf0: 3933 3034 3630 652b 3031 2220 6379 3d22  930460e+01" cy="
-00002c00: 362e 3234 3533 3631 3530 652b 3031 2220  6.24536150e+01" 
-00002c10: 723d 2231 2e32 3237 3434 3235 3735 3238  r="1.22744257528
-00002c20: 3431 3630 3722 202f 3e0d 0a20 2020 2020  41607" />..     
-00002c30: 203c 6369 7263 6c65 2063 783d 2238 2e33   <circle cx="8.3
-00002c40: 3835 3536 3234 3065 2b30 3122 2063 793d  8556240e+01" cy=
-00002c50: 2235 2e32 3238 3730 3434 3065 2b30 3122  "5.22870440e+01"
-00002c60: 2072 3d22 312e 3232 3734 3432 3537 3532   r="1.2274425752
-00002c70: 3834 3136 3037 2220 2f3e 0d0a 2020 2020  841607" />..    
-00002c80: 2020 3c63 6972 636c 6520 6378 3d22 312e    <circle cx="1.
-00002c90: 3430 3031 3039 3830 652b 3031 2220 6379  40010980e+01" cy
-00002ca0: 3d22 332e 3634 3937 3032 3130 652b 3031  ="3.64970210e+01
-00002cb0: 2220 723d 2231 2e32 3237 3434 3235 3735  " r="1.227442575
-00002cc0: 3238 3431 3630 3722 202f 3e0d 0a20 2020  2841607" />..   
-00002cd0: 2020 203c 6369 7263 6c65 2063 783d 2233     <circle cx="3
-00002ce0: 2e36 3439 3730 3537 3065 2b30 3122 2063  .64970570e+01" c
-00002cf0: 793d 2231 2e34 3030 3131 3136 3065 2b30  y="1.40011160e+0
-00002d00: 3122 2072 3d22 312e 3232 3734 3432 3537  1" r="1.22744257
-00002d10: 3532 3834 3136 3037 2220 2f3e 0d0a 2020  52841607" />..  
-00002d20: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00002d30: 362e 3234 3835 3231 3430 652b 3031 2220  6.24852140e+01" 
-00002d40: 6379 3d22 312e 3436 3138 3431 3730 652b  cy="1.46184170e+
-00002d50: 3031 2220 723d 2231 2e32 3237 3434 3235  01" r="1.2274425
-00002d60: 3735 3238 3431 3630 3722 202f 3e0d 0a20  752841607" />.. 
-00002d70: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00002d80: 2236 2e32 3633 3133 3734 3065 2b30 3122  "6.26313740e+01"
-00002d90: 2063 793d 2237 2e31 3732 3837 3138 3065   cy="7.17287180e
-00002da0: 2b30 3122 2072 3d22 312e 3232 3734 3432  +01" r="1.227442
-00002db0: 3537 3532 3834 3136 3037 2220 2f3e 0d0a  5752841607" />..
-00002dc0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00002dd0: 3d22 342e 3535 3334 3032 3030 652b 3031  ="4.55340200e+01
-00002de0: 2220 6379 3d22 382e 3631 3630 3037 3331  " cy="8.61600731
-00002df0: 652b 3031 2220 723d 2231 2e32 3237 3434  e+01" r="1.22744
-00002e00: 3235 3735 3238 3431 3630 3722 202f 3e0d  25752841607" />.
-00002e10: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00002e20: 783d 2237 2e37 3631 3134 3630 3065 2b30  x="7.76114600e+0
-00002e30: 3122 2063 793d 2233 2e32 3536 3938 3731  1" cy="3.2569871
-00002e40: 3065 2b30 3122 2072 3d22 312e 3232 3734  0e+01" r="1.2274
-00002e50: 3432 3537 3532 3834 3136 3037 2220 2f3e  425752841607" />
-00002e60: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00002e70: 6378 3d22 332e 3235 3336 3230 3230 652b  cx="3.25362020e+
-00002e80: 3031 2220 6379 3d22 372e 3735 3838 3231  01" cy="7.758821
-00002e90: 3330 652b 3031 2220 723d 2231 2e32 3237  30e+01" r="1.227
-00002ea0: 3434 3235 3735 3238 3431 3630 3722 202f  4425752841607" /
-00002eb0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00002ec0: 2063 783d 2235 2e34 3437 3534 3636 3065   cx="5.44754660e
-00002ed0: 2b30 3122 2063 793d 2231 2e34 3036 3636  +01" cy="1.40666
-00002ee0: 3435 3065 2b30 3122 2072 3d22 312e 3232  450e+01" r="1.22
-00002ef0: 3734 3432 3537 3532 3834 3136 3037 2220  74425752841607" 
-00002f00: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00002f10: 6520 6378 3d22 382e 3530 3439 3237 3630  e cx="8.50492760
-00002f20: 652b 3031 2220 6379 3d22 312e 3439 3730  e+01" cy="1.4970
-00002f30: 3933 3830 652b 3031 2220 723d 2231 2e32  9380e+01" r="1.2
-00002f40: 3237 3434 3235 3735 3238 3431 3630 3722  274425752841607"
-00002f50: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00002f60: 6c65 2063 783d 2237 2e31 3736 3937 3133  le cx="7.1769713
-00002f70: 3065 2b30 3122 2063 793d 2236 2e32 3538  0e+01" cy="6.258
-00002f80: 3335 3537 3065 2b30 3122 2072 3d22 312e  35570e+01" r="1.
-00002f90: 3232 3734 3432 3537 3532 3834 3136 3037  2274425752841607
-00002fa0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00002fb0: 636c 6520 6378 3d22 382e 3534 3738 3136  cle cx="8.547816
-00002fc0: 3230 652b 3031 2220 6379 3d22 332e 3735  20e+01" cy="3.75
-00002fd0: 3238 3432 3130 652b 3031 2220 723d 2231  284210e+01" r="1
-00002fe0: 2e32 3237 3434 3235 3735 3238 3431 3630  .227442575284160
-00002ff0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00003000: 7263 6c65 2063 783d 2232 2e36 3434 3439  rcle cx="2.64449
-00003010: 3834 3065 2b30 3122 2063 793d 2237 2e33  840e+01" cy="7.3
-00003020: 3532 3736 3734 3065 2b30 3122 2072 3d22  5276740e+01" r="
-00003030: 312e 3232 3734 3432 3537 3532 3834 3136  1.22744257528416
-00003040: 3037 2220 2f3e 0d0a 2020 203c 2f67 3e0d  07" />..   </g>.
-00003050: 0a3c 2f73 7667 3e                        .</svg>
+00000590: 652b 3031 204c 2039 2e35 3030 3030 3030  e+01 L 9.5000000
+000005a0: 3065 2b30 3120 392e 3530 3030 3030 3030  0e+01 9.50000000
+000005b0: 652b 3031 204c 2039 2e35 3030 3030 3030  e+01 L 9.5000000
+000005c0: 3065 2b30 3120 352e 3030 3030 3030 3030  0e+01 5.00000000
+000005d0: 652b 3031 2051 2038 2e33 3438 3335 3631  e+01 Q 8.3483561
+000005e0: 3265 2b30 3120 362e 3031 3334 3634 3531  2e+01 6.01346451
+000005f0: 652b 3031 2c20 372e 3130 3933 3732 3330  e+01, 7.10937230
+00000600: 652b 3031 2037 2e31 3030 3431 3733 3065  e+01 7.10041730e
+00000610: 2b30 3120 5a22 202f 3e0d 0a20 2020 2020  +01 Z" />..     
+00000620: 203c 7061 7468 2064 3d22 4d20 372e 3534   <path d="M 7.54
+00000630: 3133 3632 3430 652b 3031 2032 2e34 3635  136240e+01 2.465
+00000640: 3931 3539 3065 2b30 3120 5120 382e 3539  91590e+01 Q 8.59
+00000650: 3837 3631 3835 652b 3031 2033 2e38 3138  876185e+01 3.818
+00000660: 3638 3335 3165 2b30 312c 2039 2e35 3030  68351e+01, 9.500
+00000670: 3030 3030 3065 2b30 3120 352e 3030 3030  00000e+01 5.0000
+00000680: 3030 3030 652b 3031 204c 2039 2e35 3030  0000e+01 L 9.500
+00000690: 3030 3030 3065 2b30 3120 352e 3030 3030  00000e+01 5.0000
+000006a0: 3030 3030 652b 3030 2051 2038 2e35 3534  0000e+00 Q 8.554
+000006b0: 3432 3630 3465 2b30 3120 312e 3434 3733  42604e+01 1.4473
+000006c0: 3732 3237 652b 3031 2c20 372e 3534 3133  7227e+01, 7.5413
+000006d0: 3632 3430 652b 3031 2032 2e34 3635 3931  6240e+01 2.46591
+000006e0: 3539 3065 2b30 3120 5a22 202f 3e0d 0a20  590e+01 Z" />.. 
+000006f0: 2020 2020 203c 7061 7468 2064 3d22 4d20       <path d="M 
+00000700: 372e 3534 3133 3632 3430 652b 3031 2032  7.54136240e+01 2
+00000710: 2e34 3635 3931 3539 3065 2b30 3120 5120  .46591590e+01 Q 
+00000720: 372e 3735 3633 3031 3733 652b 3031 2033  7.75630173e+01 3
+00000730: 2e33 3034 3130 3138 3365 2b30 312c 2037  .30410183e+01, 7
+00000740: 2e37 3030 3030 3030 3065 2b30 3120 342e  .70000000e+01 4.
+00000750: 3130 3030 3030 3030 652b 3031 2051 2038  10000000e+01 Q 8
+00000760: 2e36 3135 3738 3535 3965 2b30 3120 342e  .61578559e+01 4.
+00000770: 3535 3333 3930 3830 652b 3031 2c20 392e  55339080e+01, 9.
+00000780: 3530 3030 3030 3030 652b 3031 2035 2e30  50000000e+01 5.0
+00000790: 3030 3030 3030 3065 2b30 3120 5120 382e  0000000e+01 Q 8.
+000007a0: 3539 3837 3631 3835 652b 3031 2033 2e38  59876185e+01 3.8
+000007b0: 3138 3638 3335 3165 2b30 312c 2037 2e35  1868351e+01, 7.5
+000007c0: 3431 3336 3234 3065 2b30 3120 322e 3436  4136240e+01 2.46
+000007d0: 3539 3135 3930 652b 3031 205a 2220 2f3e  591590e+01 Z" />
+000007e0: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
+000007f0: 224d 2037 2e31 3732 3739 3236 3065 2b30  "M 7.17279260e+0
+00000800: 3120 352e 3337 3237 3932 3630 652b 3031  1 5.37279260e+01
+00000810: 2051 2036 2e35 3838 3734 3437 3465 2b30   Q 6.58874474e+0
+00000820: 3120 352e 3931 3038 3431 3737 652b 3031  1 5.91084177e+01
+00000830: 2c20 352e 3930 3030 3030 3030 652b 3031  , 5.90000000e+01
+00000840: 2035 2e39 3030 3030 3030 3065 2b30 3120   5.90000000e+01 
+00000850: 5120 362e 3533 3131 3732 3735 652b 3031  Q 6.53117275e+01
+00000860: 2036 2e35 3237 3332 3439 3965 2b30 312c   6.52732499e+01,
+00000870: 2037 2e31 3039 3337 3233 3065 2b30 3120   7.10937230e+01 
+00000880: 372e 3130 3034 3137 3330 652b 3031 2051  7.10041730e+01 Q
+00000890: 2037 2e31 3736 3038 3731 3965 2b30 3120   7.17608719e+01 
+000008a0: 362e 3239 3733 3933 3237 652b 3031 2c20  6.29739327e+01, 
+000008b0: 372e 3137 3237 3932 3630 652b 3031 2035  7.17279260e+01 5
+000008c0: 2e33 3732 3739 3236 3065 2b30 3120 5a22  .37279260e+01 Z"
+000008d0: 202f 3e0d 0a20 2020 2020 203c 7061 7468   />..      <path
+000008e0: 2064 3d22 4d20 372e 3534 3133 3632 3430   d="M 7.54136240
+000008f0: 652b 3031 2032 2e34 3635 3931 3539 3065  e+01 2.46591590e
+00000900: 2b30 3120 4c20 372e 3137 3237 3932 3630  +01 L 7.17279260
+00000910: 652b 3031 2032 2e38 3237 3230 3734 3065  e+01 2.82720740e
+00000920: 2b30 3120 5120 372e 3731 3038 3431 3737  +01 Q 7.71084177
+00000930: 652b 3031 2033 2e34 3131 3235 3532 3665  e+01 3.41125526e
+00000940: 2b30 312c 2037 2e37 3030 3030 3030 3065  +01, 7.70000000e
+00000950: 2b30 3120 342e 3130 3030 3030 3030 652b  +01 4.10000000e+
+00000960: 3031 2051 2037 2e37 3536 3330 3137 3365  01 Q 7.75630173e
+00000970: 2b30 3120 332e 3330 3431 3031 3833 652b  +01 3.30410183e+
+00000980: 3031 2c20 372e 3534 3133 3632 3430 652b  01, 7.54136240e+
+00000990: 3031 2032 2e34 3635 3931 3539 3065 2b30  01 2.46591590e+0
+000009a0: 3120 5a22 202f 3e0d 0a20 2020 2020 203c  1 Z" />..      <
+000009b0: 7061 7468 2064 3d22 4d20 352e 3930 3030  path d="M 5.9000
+000009c0: 3030 3030 652b 3031 2032 2e33 3030 3030  0000e+01 2.30000
+000009d0: 3030 3065 2b30 3120 5120 362e 3538 3837  000e+01 Q 6.5887
+000009e0: 3434 3734 652b 3031 2032 2e32 3839 3135  4474e+01 2.28915
+000009f0: 3832 3365 2b30 312c 2037 2e31 3732 3739  823e+01, 7.17279
+00000a00: 3236 3065 2b30 3120 322e 3832 3732 3037  260e+01 2.827207
+00000a10: 3430 652b 3031 204c 2037 2e35 3431 3336  40e+01 L 7.54136
+00000a20: 3234 3065 2b30 3120 322e 3436 3539 3135  240e+01 2.465915
+00000a30: 3930 652b 3031 2051 2036 2e36 3939 3438  90e+01 Q 6.69948
+00000a40: 3932 3565 2b30 3120 322e 3234 3533 3831  925e+01 2.245381
+00000a50: 3432 652b 3031 2c20 352e 3930 3030 3030  42e+01, 5.900000
+00000a60: 3030 652b 3031 2032 2e33 3030 3030 3030  00e+01 2.3000000
+00000a70: 3065 2b30 3120 5a22 202f 3e0d 0a20 2020  0e+01 Z" />..   
+00000a80: 2020 203c 7061 7468 2064 3d22 4d20 322e     <path d="M 2.
+00000a90: 3330 3030 3030 3030 652b 3031 2034 2e31  30000000e+01 4.1
+00000aa0: 3030 3030 3030 3065 2b30 3120 4c20 322e  0000000e+01 L 2.
+00000ab0: 3330 3030 3030 3030 652b 3031 2032 2e33  30000000e+01 2.3
+00000ac0: 3030 3030 3030 3065 2b30 3120 4c20 352e  0000000e+01 L 5.
+00000ad0: 3030 3030 3030 3030 652b 3030 2035 2e30  00000000e+00 5.0
+00000ae0: 3030 3030 3030 3065 2b30 3120 5120 312e  0000000e+01 Q 1.
+00000af0: 3430 3035 3932 3032 652b 3031 2034 2e35  40059202e+01 4.5
+00000b00: 3439 3133 3236 3665 2b30 312c 2032 2e33  4913266e+01, 2.3
+00000b10: 3030 3030 3030 3065 2b30 3120 342e 3130  0000000e+01 4.10
+00000b20: 3030 3030 3030 652b 3031 205a 2220 2f3e  000000e+01 Z" />
+00000b30: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
+00000b40: 224d 2032 2e33 3030 3030 3030 3065 2b30  "M 2.30000000e+0
+00000b50: 3120 352e 3930 3030 3030 3030 652b 3031  1 5.90000000e+01
+00000b60: 204c 2032 2e33 3030 3030 3030 3065 2b30   L 2.30000000e+0
+00000b70: 3120 342e 3130 3030 3030 3030 652b 3031  1 4.10000000e+01
+00000b80: 2051 2031 2e34 3030 3539 3230 3265 2b30   Q 1.40059202e+0
+00000b90: 3120 342e 3534 3931 3332 3636 652b 3031  1 4.54913266e+01
+00000ba0: 2c20 352e 3030 3030 3030 3030 652b 3030  , 5.00000000e+00
+00000bb0: 2035 2e30 3030 3030 3030 3065 2b30 3120   5.00000000e+01 
+00000bc0: 5120 312e 3430 3636 3033 3636 652b 3031  Q 1.40660366e+01
+00000bd0: 2035 2e34 3437 3532 3335 3165 2b30 312c   5.44752351e+01,
+00000be0: 2032 2e33 3030 3030 3030 3065 2b30 3120   2.30000000e+01 
+00000bf0: 352e 3930 3030 3030 3030 652b 3031 205a  5.90000000e+01 Z
+00000c00: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+00000c10: 6820 643d 224d 2032 2e34 3539 3535 3032  h d="M 2.4595502
+00000c20: 3065 2b30 3120 372e 3533 3439 3936 3730  0e+01 7.53499670
+00000c30: 652b 3031 2051 2031 2e34 3038 3633 3932  e+01 Q 1.4086392
+00000c40: 3865 2b30 3120 362e 3137 3938 3735 3831  8e+01 6.17987581
+00000c50: 652b 3031 2c20 352e 3030 3030 3030 3030  e+01, 5.00000000
+00000c60: 652b 3030 2035 2e30 3030 3030 3030 3065  e+00 5.00000000e
+00000c70: 2b30 3120 4c20 352e 3030 3030 3030 3030  +01 L 5.00000000
+00000c80: 652b 3030 2039 2e35 3030 3030 3030 3065  e+00 9.50000000e
+00000c90: 2b30 3120 5120 312e 3434 3435 3336 3638  +01 Q 1.44453668
+00000ca0: 652b 3031 2038 2e35 3531 3538 3735 3565  e+01 8.55158755e
+00000cb0: 2b30 312c 2032 2e34 3539 3535 3032 3065  +01, 2.45955020e
+00000cc0: 2b30 3120 372e 3533 3439 3936 3730 652b  +01 7.53499670e+
+00000cd0: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
+00000ce0: 3c70 6174 6820 643d 224d 2032 2e33 3030  <path d="M 2.300
+00000cf0: 3030 3030 3065 2b30 3120 322e 3330 3030  00000e+01 2.3000
+00000d00: 3030 3030 652b 3031 204c 2035 2e30 3030  0000e+01 L 5.000
+00000d10: 3030 3030 3065 2b30 3020 352e 3030 3030  00000e+00 5.0000
+00000d20: 3030 3030 652b 3030 204c 2035 2e30 3030  0000e+00 L 5.000
+00000d30: 3030 3030 3065 2b30 3020 352e 3030 3030  00000e+00 5.0000
+00000d40: 3030 3030 652b 3031 204c 2032 2e33 3030  0000e+01 L 2.300
+00000d50: 3030 3030 3065 2b30 3120 322e 3330 3030  00000e+01 2.3000
+00000d60: 3030 3030 652b 3031 205a 2220 2f3e 0d0a  0000e+01 Z" />..
+00000d70: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
+00000d80: 2032 2e34 3539 3535 3032 3065 2b30 3120   2.45955020e+01 
+00000d90: 372e 3533 3439 3936 3730 652b 3031 2051  7.53499670e+01 Q
+00000da0: 2032 2e32 3433 3034 3334 3465 2b30 3120   2.24304344e+01 
+00000db0: 362e 3639 3633 3934 3636 652b 3031 2c20  6.69639466e+01, 
+00000dc0: 322e 3330 3030 3030 3030 652b 3031 2035  2.30000000e+01 5
+00000dd0: 2e39 3030 3030 3030 3065 2b30 3120 5120  .90000000e+01 Q 
+00000de0: 312e 3430 3636 3033 3636 652b 3031 2035  1.40660366e+01 5
+00000df0: 2e34 3437 3532 3335 3165 2b30 312c 2035  .44752351e+01, 5
+00000e00: 2e30 3030 3030 3030 3065 2b30 3020 352e  .00000000e+00 5.
+00000e10: 3030 3030 3030 3030 652b 3031 2051 2031  00000000e+01 Q 1
+00000e20: 2e34 3038 3633 3932 3865 2b30 3120 362e  .40863928e+01 6.
+00000e30: 3137 3938 3735 3831 652b 3031 2c20 322e  17987581e+01, 2.
+00000e40: 3435 3935 3530 3230 652b 3031 2037 2e35  45955020e+01 7.5
+00000e50: 3334 3939 3637 3065 2b30 3120 5a22 202f  3499670e+01 Z" /
+00000e60: 3e0d 0a20 2020 2020 203c 7061 7468 2064  >..      <path d
+00000e70: 3d22 4d20 322e 3330 3030 3030 3030 652b  ="M 2.30000000e+
+00000e80: 3031 2032 2e33 3030 3030 3030 3065 2b30  01 2.30000000e+0
+00000e90: 3120 4c20 342e 3130 3030 3030 3030 652b  1 L 4.10000000e+
+00000ea0: 3031 2032 2e33 3030 3030 3030 3065 2b30  01 2.30000000e+0
+00000eb0: 3120 5120 342e 3534 3931 3431 3635 652b  1 Q 4.54914165e+
+00000ec0: 3031 2031 2e34 3030 3539 3536 3365 2b30  01 1.40059563e+0
+00000ed0: 312c 2035 2e30 3030 3030 3030 3065 2b30  1, 5.00000000e+0
+00000ee0: 3120 352e 3030 3030 3030 3030 652b 3030  1 5.00000000e+00
+00000ef0: 204c 2032 2e33 3030 3030 3030 3065 2b30   L 2.30000000e+0
+00000f00: 3120 322e 3330 3030 3030 3030 652b 3031  1 2.30000000e+01
+00000f10: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00000f20: 6174 6820 643d 224d 2034 2e31 3030 3030  ath d="M 4.10000
+00000f30: 3030 3065 2b30 3120 322e 3330 3030 3030  000e+01 2.300000
+00000f40: 3030 652b 3031 204c 2035 2e39 3030 3030  00e+01 L 5.90000
+00000f50: 3030 3065 2b30 3120 322e 3330 3030 3030  000e+01 2.300000
+00000f60: 3030 652b 3031 2051 2035 2e34 3437 3535  00e+01 Q 5.44755
+00000f70: 3033 3365 2b30 3120 312e 3430 3636 3534  033e+01 1.406654
+00000f80: 3337 652b 3031 2c20 352e 3030 3030 3030  37e+01, 5.000000
+00000f90: 3030 652b 3031 2035 2e30 3030 3030 3030  00e+01 5.0000000
+00000fa0: 3065 2b30 3020 5120 342e 3534 3931 3431  0e+00 Q 4.549141
+00000fb0: 3635 652b 3031 2031 2e34 3030 3539 3536  65e+01 1.4005956
+00000fc0: 3365 2b30 312c 2034 2e31 3030 3030 3030  3e+01, 4.1000000
+00000fd0: 3065 2b30 3120 322e 3330 3030 3030 3030  0e+01 2.30000000
+00000fe0: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
+00000ff0: 2020 3c70 6174 6820 643d 224d 2039 2e35    <path d="M 9.5
+00001000: 3030 3030 3030 3065 2b30 3120 352e 3030  0000000e+01 5.00
+00001010: 3030 3030 3030 652b 3030 204c 2035 2e30  000000e+00 L 5.0
+00001020: 3030 3030 3030 3065 2b30 3120 352e 3030  0000000e+01 5.00
+00001030: 3030 3030 3030 652b 3030 2051 2036 2e31  000000e+00 Q 6.1
+00001040: 3832 3834 3637 3765 2b30 3120 312e 3431  8284677e+01 1.41
+00001050: 3039 3836 3130 652b 3031 2c20 372e 3534  098610e+01, 7.54
+00001060: 3133 3632 3430 652b 3031 2032 2e34 3635  136240e+01 2.465
+00001070: 3931 3539 3065 2b30 3120 5120 382e 3535  91590e+01 Q 8.55
+00001080: 3434 3236 3034 652b 3031 2031 2e34 3437  442604e+01 1.447
+00001090: 3337 3232 3765 2b30 312c 2039 2e35 3030  37227e+01, 9.500
+000010a0: 3030 3030 3065 2b30 3120 352e 3030 3030  00000e+01 5.0000
+000010b0: 3030 3030 652b 3030 205a 2220 2f3e 0d0a  0000e+00 Z" />..
+000010c0: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
+000010d0: 2035 2e30 3030 3030 3030 3065 2b30 3020   5.00000000e+00 
+000010e0: 352e 3030 3030 3030 3030 652b 3030 204c  5.00000000e+00 L
+000010f0: 2032 2e33 3030 3030 3030 3065 2b30 3120   2.30000000e+01 
+00001100: 322e 3330 3030 3030 3030 652b 3031 204c  2.30000000e+01 L
+00001110: 2035 2e30 3030 3030 3030 3065 2b30 3120   5.00000000e+01 
+00001120: 352e 3030 3030 3030 3030 652b 3030 204c  5.00000000e+00 L
+00001130: 2035 2e30 3030 3030 3030 3065 2b30 3020   5.00000000e+00 
+00001140: 352e 3030 3030 3030 3030 652b 3030 205a  5.00000000e+00 Z
+00001150: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+00001160: 6820 643d 224d 2035 2e39 3030 3030 3030  h d="M 5.9000000
+00001170: 3065 2b30 3120 322e 3330 3030 3030 3030  0e+01 2.30000000
+00001180: 652b 3031 2051 2036 2e36 3939 3438 3932  e+01 Q 6.6994892
+00001190: 3565 2b30 3120 322e 3234 3533 3831 3432  5e+01 2.24538142
+000011a0: 652b 3031 2c20 372e 3534 3133 3632 3430  e+01, 7.54136240
+000011b0: 652b 3031 2032 2e34 3635 3931 3539 3065  e+01 2.46591590e
+000011c0: 2b30 3120 5120 362e 3138 3238 3436 3737  +01 Q 6.18284677
+000011d0: 652b 3031 2031 2e34 3130 3938 3631 3065  e+01 1.41098610e
+000011e0: 2b30 312c 2035 2e30 3030 3030 3030 3065  +01, 5.00000000e
+000011f0: 2b30 3120 352e 3030 3030 3030 3030 652b  +01 5.00000000e+
+00001200: 3030 2051 2035 2e34 3437 3535 3033 3365  00 Q 5.44755033e
+00001210: 2b30 3120 312e 3430 3636 3534 3337 652b  +01 1.40665437e+
+00001220: 3031 2c20 352e 3930 3030 3030 3030 652b  01, 5.90000000e+
+00001230: 3031 2032 2e33 3030 3030 3030 3065 2b30  01 2.30000000e+0
+00001240: 3120 5a22 202f 3e0d 0a20 2020 2020 203c  1 Z" />..      <
+00001250: 7061 7468 2064 3d22 4d20 322e 3435 3935  path d="M 2.4595
+00001260: 3530 3230 652b 3031 2037 2e35 3334 3939  5020e+01 7.53499
+00001270: 3637 3065 2b30 3120 4c20 322e 3832 3732  670e+01 L 2.8272
+00001280: 3037 3430 652b 3031 2037 2e31 3732 3739  0740e+01 7.17279
+00001290: 3236 3065 2b30 3120 5120 322e 3238 3931  260e+01 Q 2.2891
+000012a0: 3538 3233 652b 3031 2036 2e35 3838 3734  5823e+01 6.58874
+000012b0: 3437 3465 2b30 312c 2032 2e33 3030 3030  474e+01, 2.30000
+000012c0: 3030 3065 2b30 3120 352e 3930 3030 3030  000e+01 5.900000
+000012d0: 3030 652b 3031 2051 2032 2e32 3433 3034  00e+01 Q 2.24304
+000012e0: 3334 3465 2b30 3120 362e 3639 3633 3934  344e+01 6.696394
+000012f0: 3636 652b 3031 2c20 322e 3435 3935 3530  66e+01, 2.459550
+00001300: 3230 652b 3031 2037 2e35 3334 3939 3637  20e+01 7.5349967
+00001310: 3065 2b30 3120 5a22 202f 3e0d 0a20 2020  0e+01 Z" />..   
+00001320: 2020 203c 7061 7468 2064 3d22 4d20 342e     <path d="M 4.
+00001330: 3130 3030 3030 3030 652b 3031 2037 2e37  10000000e+01 7.7
+00001340: 3030 3030 3030 3065 2b30 3120 5120 332e  0000000e+01 Q 3.
+00001350: 3431 3132 3535 3236 652b 3031 2037 2e37  41125526e+01 7.7
+00001360: 3130 3834 3137 3765 2b30 312c 2032 2e38  1084177e+01, 2.8
+00001370: 3237 3230 3734 3065 2b30 3120 372e 3137  2720740e+01 7.17
+00001380: 3237 3932 3630 652b 3031 204c 2032 2e34  279260e+01 L 2.4
+00001390: 3539 3535 3032 3065 2b30 3120 372e 3533  5955020e+01 7.53
+000013a0: 3439 3936 3730 652b 3031 2051 2033 2e33  499670e+01 Q 3.3
+000013b0: 3030 3938 3338 3165 2b30 3120 372e 3735  0098381e+01 7.75
+000013c0: 3339 3633 3636 652b 3031 2c20 342e 3130  396366e+01, 4.10
+000013d0: 3030 3030 3030 652b 3031 2037 2e37 3030  000000e+01 7.700
+000013e0: 3030 3030 3065 2b30 3120 5a22 202f 3e0d  00000e+01 Z" />.
+000013f0: 0a20 2020 2020 203c 7061 7468 2064 3d22  .      <path d="
+00001400: 4d20 392e 3530 3030 3030 3030 652b 3031  M 9.50000000e+01
+00001410: 2039 2e35 3030 3030 3030 3065 2b30 3120   9.50000000e+01 
+00001420: 4c20 372e 3130 3933 3732 3330 652b 3031  L 7.10937230e+01
+00001430: 2037 2e31 3030 3431 3733 3065 2b30 3120   7.10041730e+01 
+00001440: 5120 362e 3031 3737 3839 3939 652b 3031  Q 6.01778999e+01
+00001450: 2038 2e33 3434 3137 3232 3865 2b30 312c   8.34417228e+01,
+00001460: 2035 2e30 3030 3030 3030 3065 2b30 3120   5.00000000e+01 
+00001470: 392e 3530 3030 3030 3030 652b 3031 204c  9.50000000e+01 L
+00001480: 2039 2e35 3030 3030 3030 3065 2b30 3120   9.50000000e+01 
+00001490: 392e 3530 3030 3030 3030 652b 3031 205a  9.50000000e+01 Z
+000014a0: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+000014b0: 6820 643d 224d 2035 2e30 3030 3030 3030  h d="M 5.0000000
+000014c0: 3065 2b30 3020 392e 3530 3030 3030 3030  0e+00 9.50000000
+000014d0: 652b 3031 204c 2035 2e30 3030 3030 3030  e+01 L 5.0000000
+000014e0: 3065 2b30 3120 392e 3530 3030 3030 3030  0e+01 9.50000000
+000014f0: 652b 3031 2051 2033 2e38 3135 3638 3433  e+01 Q 3.8156843
+00001500: 3865 2b30 3120 382e 3539 3633 3730 3836  8e+01 8.59637086
+00001510: 652b 3031 2c20 322e 3435 3935 3530 3230  e+01, 2.45955020
+00001520: 652b 3031 2037 2e35 3334 3939 3637 3065  e+01 7.53499670e
+00001530: 2b30 3120 5120 312e 3434 3435 3336 3638  +01 Q 1.44453668
+00001540: 652b 3031 2038 2e35 3531 3538 3735 3565  e+01 8.55158755e
+00001550: 2b30 312c 2035 2e30 3030 3030 3030 3065  +01, 5.00000000e
+00001560: 2b30 3020 392e 3530 3030 3030 3030 652b  +00 9.50000000e+
+00001570: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
+00001580: 3c70 6174 6820 643d 224d 2034 2e31 3030  <path d="M 4.100
+00001590: 3030 3030 3065 2b30 3120 372e 3730 3030  00000e+01 7.7000
+000015a0: 3030 3030 652b 3031 2051 2033 2e33 3030  0000e+01 Q 3.300
+000015b0: 3938 3338 3165 2b30 3120 372e 3735 3339  98381e+01 7.7539
+000015c0: 3633 3636 652b 3031 2c20 322e 3435 3935  6366e+01, 2.4595
+000015d0: 3530 3230 652b 3031 2037 2e35 3334 3939  5020e+01 7.53499
+000015e0: 3637 3065 2b30 3120 5120 332e 3831 3536  670e+01 Q 3.8156
+000015f0: 3834 3338 652b 3031 2038 2e35 3936 3337  8438e+01 8.59637
+00001600: 3038 3665 2b30 312c 2035 2e30 3030 3030  086e+01, 5.00000
+00001610: 3030 3065 2b30 3120 392e 3530 3030 3030  000e+01 9.500000
+00001620: 3030 652b 3031 2051 2034 2e35 3533 3332  00e+01 Q 4.55332
+00001630: 3632 3165 2b30 3120 382e 3631 3536 3530  621e+01 8.615650
+00001640: 3730 652b 3031 2c20 342e 3130 3030 3030  70e+01, 4.100000
+00001650: 3030 652b 3031 2037 2e37 3030 3030 3030  00e+01 7.7000000
+00001660: 3065 2b30 3120 5a22 202f 3e0d 0a20 2020  0e+01 Z" />..   
+00001670: 3c2f 673e 0d0a 2020 203c 6720 6964 3d22  </g>..   <g id="
+00001680: 4e6f 6465 7322 2066 696c 6c3d 2223 6139  Nodes" fill="#a9
+00001690: 3565 3565 223e 0d0a 2020 2020 2020 3c63  5e5e">..      <c
+000016a0: 6972 636c 6520 6378 3d22 342e 3834 3535  ircle cx="4.8455
+000016b0: 3834 3330 652b 3031 2220 6379 3d22 372e  8430e+01" cy="7.
+000016c0: 3730 3030 3030 3030 652b 3031 2220 723d  70000000e+01" r=
+000016d0: 2231 2e32 3237 3434 3235 3735 3238 3431  "1.2274425752841
+000016e0: 3630 3722 202f 3e0d 0a20 2020 2020 203c  607" />..      <
+000016f0: 6369 7263 6c65 2063 783d 2235 2e33 3732  circle cx="5.372
+00001700: 3739 3236 3065 2b30 3122 2063 793d 2237  79260e+01" cy="7
+00001710: 2e31 3732 3739 3236 3065 2b30 3122 2072  .17279260e+01" r
+00001720: 3d22 312e 3232 3734 3432 3537 3532 3834  ="1.227442575284
+00001730: 3136 3037 2220 2f3e 0d0a 2020 2020 2020  1607" />..      
+00001740: 3c63 6972 636c 6520 6378 3d22 352e 3930  <circle cx="5.90
+00001750: 3030 3030 3030 652b 3031 2220 6379 3d22  000000e+01" cy="
+00001760: 362e 3634 3535 3834 3330 652b 3031 2220  6.64558430e+01" 
+00001770: 723d 2231 2e32 3237 3434 3235 3735 3238  r="1.22744257528
+00001780: 3431 3630 3722 202f 3e0d 0a20 2020 2020  41607" />..     
+00001790: 203c 6369 7263 6c65 2063 783d 2239 2e35   <circle cx="9.5
+000017a0: 3030 3030 3030 3065 2b30 3122 2063 793d  0000000e+01" cy=
+000017b0: 2237 2e32 3530 3030 3030 3065 2b30 3122  "7.25000000e+01"
+000017c0: 2072 3d22 312e 3232 3734 3432 3537 3532   r="1.2274425752
+000017d0: 3834 3136 3037 2220 2f3e 0d0a 2020 2020  841607" />..    
+000017e0: 2020 3c63 6972 636c 6520 6378 3d22 392e    <circle cx="9.
+000017f0: 3530 3030 3030 3030 652b 3031 2220 6379  50000000e+01" cy
+00001800: 3d22 352e 3030 3030 3030 3030 652b 3031  ="5.00000000e+01
+00001810: 2220 723d 2231 2e32 3237 3434 3235 3735  " r="1.227442575
+00001820: 3238 3431 3630 3722 202f 3e0d 0a20 2020  2841607" />..   
+00001830: 2020 203c 6369 7263 6c65 2063 783d 2239     <circle cx="9
+00001840: 2e35 3030 3030 3030 3065 2b30 3122 2063  .50000000e+01" c
+00001850: 793d 2232 2e37 3530 3030 3030 3065 2b30  y="2.75000000e+0
+00001860: 3122 2072 3d22 312e 3232 3734 3432 3537  1" r="1.22744257
+00001870: 3532 3834 3136 3037 2220 2f3e 0d0a 2020  52841607" />..  
+00001880: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+00001890: 362e 3634 3535 3834 3330 652b 3031 2220  6.64558430e+01" 
+000018a0: 6379 3d22 352e 3930 3030 3030 3030 652b  cy="5.90000000e+
+000018b0: 3031 2220 723d 2231 2e32 3237 3434 3235  01" r="1.2274425
+000018c0: 3735 3238 3431 3630 3722 202f 3e0d 0a20  752841607" />.. 
+000018d0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+000018e0: 2237 2e31 3732 3739 3236 3065 2b30 3122  "7.17279260e+01"
+000018f0: 2063 793d 2235 2e33 3732 3739 3236 3065   cy="5.37279260e
+00001900: 2b30 3122 2072 3d22 312e 3232 3734 3432  +01" r="1.227442
+00001910: 3537 3532 3834 3136 3037 2220 2f3e 0d0a  5752841607" />..
+00001920: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+00001930: 3d22 372e 3730 3030 3030 3030 652b 3031  ="7.70000000e+01
+00001940: 2220 6379 3d22 342e 3834 3535 3834 3330  " cy="4.84558430
+00001950: 652b 3031 2220 723d 2231 2e32 3237 3434  e+01" r="1.22744
+00001960: 3235 3735 3238 3431 3630 3722 202f 3e0d  25752841607" />.
+00001970: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+00001980: 783d 2237 2e37 3030 3030 3030 3065 2b30  x="7.70000000e+0
+00001990: 3122 2063 793d 2233 2e33 3534 3431 3537  1" cy="3.3544157
+000019a0: 3065 2b30 3122 2072 3d22 312e 3232 3734  0e+01" r="1.2274
+000019b0: 3432 3537 3532 3834 3136 3037 2220 2f3e  425752841607" />
+000019c0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+000019d0: 6378 3d22 372e 3137 3237 3932 3630 652b  cx="7.17279260e+
+000019e0: 3031 2220 6379 3d22 322e 3832 3732 3037  01" cy="2.827207
+000019f0: 3430 652b 3031 2220 723d 2231 2e32 3237  40e+01" r="1.227
+00001a00: 3434 3235 3735 3238 3431 3630 3722 202f  4425752841607" /
+00001a10: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+00001a20: 2063 783d 2236 2e36 3435 3538 3433 3065   cx="6.64558430e
+00001a30: 2b30 3122 2063 793d 2232 2e33 3030 3030  +01" cy="2.30000
+00001a40: 3030 3065 2b30 3122 2072 3d22 312e 3232  000e+01" r="1.22
+00001a50: 3734 3432 3537 3532 3834 3136 3037 2220  74425752841607" 
+00001a60: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+00001a70: 6520 6378 3d22 352e 3030 3030 3030 3030  e cx="5.00000000
+00001a80: 652b 3030 2220 6379 3d22 322e 3735 3030  e+00" cy="2.7500
+00001a90: 3030 3030 652b 3031 2220 723d 2231 2e32  0000e+01" r="1.2
+00001aa0: 3237 3434 3235 3735 3238 3431 3630 3722  274425752841607"
+00001ab0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+00001ac0: 6c65 2063 783d 2235 2e30 3030 3030 3030  le cx="5.0000000
+00001ad0: 3065 2b30 3022 2063 793d 2235 2e30 3030  0e+00" cy="5.000
+00001ae0: 3030 3030 3065 2b30 3122 2072 3d22 312e  00000e+01" r="1.
+00001af0: 3232 3734 3432 3537 3532 3834 3136 3037  2274425752841607
+00001b00: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+00001b10: 636c 6520 6378 3d22 352e 3030 3030 3030  cle cx="5.000000
+00001b20: 3030 652b 3030 2220 6379 3d22 372e 3235  00e+00" cy="7.25
+00001b30: 3030 3030 3030 652b 3031 2220 723d 2231  000000e+01" r="1
+00001b40: 2e32 3237 3434 3235 3735 3238 3431 3630  .227442575284160
+00001b50: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+00001b60: 7263 6c65 2063 783d 2237 2e32 3530 3030  rcle cx="7.25000
+00001b70: 3030 3065 2b30 3122 2063 793d 2235 2e30  000e+01" cy="5.0
+00001b80: 3030 3030 3030 3065 2b30 3022 2072 3d22  0000000e+00" r="
+00001b90: 312e 3232 3734 3432 3537 3532 3834 3136  1.22744257528416
+00001ba0: 3037 2220 2f3e 0d0a 2020 2020 2020 3c63  07" />..      <c
+00001bb0: 6972 636c 6520 6378 3d22 352e 3030 3030  ircle cx="5.0000
+00001bc0: 3030 3030 652b 3031 2220 6379 3d22 352e  0000e+01" cy="5.
+00001bd0: 3030 3030 3030 3030 652b 3030 2220 723d  00000000e+00" r=
+00001be0: 2231 2e32 3237 3434 3235 3735 3238 3431  "1.2274425752841
+00001bf0: 3630 3722 202f 3e0d 0a20 2020 2020 203c  607" />..      <
+00001c00: 6369 7263 6c65 2063 783d 2232 2e37 3530  circle cx="2.750
+00001c10: 3030 3030 3065 2b30 3122 2063 793d 2235  00000e+01" cy="5
+00001c20: 2e30 3030 3030 3030 3065 2b30 3022 2072  .00000000e+00" r
+00001c30: 3d22 312e 3232 3734 3432 3537 3532 3834  ="1.227442575284
+00001c40: 3136 3037 2220 2f3e 0d0a 2020 2020 2020  1607" />..      
+00001c50: 3c63 6972 636c 6520 6378 3d22 322e 3330  <circle cx="2.30
+00001c60: 3030 3030 3030 652b 3031 2220 6379 3d22  000000e+01" cy="
+00001c70: 362e 3634 3535 3834 3330 652b 3031 2220  6.64558430e+01" 
+00001c80: 723d 2231 2e32 3237 3434 3235 3735 3238  r="1.22744257528
+00001c90: 3431 3630 3722 202f 3e0d 0a20 2020 2020  41607" />..     
+00001ca0: 203c 6369 7263 6c65 2063 783d 2232 2e38   <circle cx="2.8
+00001cb0: 3237 3230 3734 3065 2b30 3122 2063 793d  2720740e+01" cy=
+00001cc0: 2237 2e31 3732 3739 3236 3065 2b30 3122  "7.17279260e+01"
+00001cd0: 2072 3d22 312e 3232 3734 3432 3537 3532   r="1.2274425752
+00001ce0: 3834 3136 3037 2220 2f3e 0d0a 2020 2020  841607" />..    
+00001cf0: 2020 3c63 6972 636c 6520 6378 3d22 332e    <circle cx="3.
+00001d00: 3335 3434 3135 3730 652b 3031 2220 6379  35441570e+01" cy
+00001d10: 3d22 372e 3730 3030 3030 3030 652b 3031  ="7.70000000e+01
+00001d20: 2220 723d 2231 2e32 3237 3434 3235 3735  " r="1.227442575
+00001d30: 3238 3431 3630 3722 202f 3e0d 0a20 2020  2841607" />..   
+00001d40: 2020 203c 6369 7263 6c65 2063 783d 2235     <circle cx="5
+00001d50: 2e30 3030 3030 3030 3065 2b30 3122 2063  .00000000e+01" c
+00001d60: 793d 2232 2e33 3030 3030 3030 3065 2b30  y="2.30000000e+0
+00001d70: 3122 2072 3d22 312e 3232 3734 3432 3537  1" r="1.22744257
+00001d80: 3532 3834 3136 3037 2220 2f3e 0d0a 2020  52841607" />..  
+00001d90: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+00001da0: 342e 3130 3030 3030 3030 652b 3031 2220  4.10000000e+01" 
+00001db0: 6379 3d22 322e 3330 3030 3030 3030 652b  cy="2.30000000e+
+00001dc0: 3031 2220 723d 2231 2e32 3237 3434 3235  01" r="1.2274425
+00001dd0: 3735 3238 3431 3630 3722 202f 3e0d 0a20  752841607" />.. 
+00001de0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00001df0: 2233 2e32 3030 3030 3030 3065 2b30 3122  "3.20000000e+01"
+00001e00: 2063 793d 2232 2e33 3030 3030 3030 3065   cy="2.30000000e
+00001e10: 2b30 3122 2072 3d22 312e 3232 3734 3432  +01" r="1.227442
+00001e20: 3537 3532 3834 3136 3037 2220 2f3e 0d0a  5752841607" />..
+00001e30: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+00001e40: 3d22 322e 3735 3030 3030 3030 652b 3031  ="2.75000000e+01
+00001e50: 2220 6379 3d22 392e 3530 3030 3030 3030  " cy="9.50000000
+00001e60: 652b 3031 2220 723d 2231 2e32 3237 3434  e+01" r="1.22744
+00001e70: 3235 3735 3238 3431 3630 3722 202f 3e0d  25752841607" />.
+00001e80: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+00001e90: 783d 2235 2e30 3030 3030 3030 3065 2b30  x="5.00000000e+0
+00001ea0: 3122 2063 793d 2239 2e35 3030 3030 3030  1" cy="9.5000000
+00001eb0: 3065 2b30 3122 2072 3d22 312e 3232 3734  0e+01" r="1.2274
+00001ec0: 3432 3537 3532 3834 3136 3037 2220 2f3e  425752841607" />
+00001ed0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+00001ee0: 6378 3d22 372e 3235 3030 3030 3030 652b  cx="7.25000000e+
+00001ef0: 3031 2220 6379 3d22 392e 3530 3030 3030  01" cy="9.500000
+00001f00: 3030 652b 3031 2220 723d 2231 2e32 3237  00e+01" r="1.227
+00001f10: 3434 3235 3735 3238 3431 3630 3722 202f  4425752841607" /
+00001f20: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+00001f30: 2063 783d 2232 2e33 3030 3030 3030 3065   cx="2.30000000e
+00001f40: 2b30 3122 2063 793d 2233 2e32 3030 3030  +01" cy="3.20000
+00001f50: 3030 3065 2b30 3122 2072 3d22 312e 3232  000e+01" r="1.22
+00001f60: 3734 3432 3537 3532 3834 3136 3037 2220  74425752841607" 
+00001f70: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+00001f80: 6520 6378 3d22 322e 3330 3030 3030 3030  e cx="2.30000000
+00001f90: 652b 3031 2220 6379 3d22 342e 3130 3030  e+01" cy="4.1000
+00001fa0: 3030 3030 652b 3031 2220 723d 2231 2e32  0000e+01" r="1.2
+00001fb0: 3237 3434 3235 3735 3238 3431 3630 3722  274425752841607"
+00001fc0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+00001fd0: 6c65 2063 783d 2232 2e33 3030 3030 3030  le cx="2.3000000
+00001fe0: 3065 2b30 3122 2063 793d 2235 2e30 3030  0e+01" cy="5.000
+00001ff0: 3030 3030 3065 2b30 3122 2072 3d22 312e  00000e+01" r="1.
+00002000: 3232 3734 3432 3537 3532 3834 3136 3037  2274425752841607
+00002010: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+00002020: 636c 6520 6378 3d22 392e 3530 3030 3030  cle cx="9.500000
+00002030: 3030 652b 3031 2220 6379 3d22 392e 3530  00e+01" cy="9.50
+00002040: 3030 3030 3030 652b 3031 2220 723d 2231  000000e+01" r="1
+00002050: 2e32 3237 3434 3235 3735 3238 3431 3630  .227442575284160
+00002060: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+00002070: 7263 6c65 2063 783d 2239 2e35 3030 3030  rcle cx="9.50000
+00002080: 3030 3065 2b30 3122 2063 793d 2235 2e30  000e+01" cy="5.0
+00002090: 3030 3030 3030 3065 2b30 3022 2072 3d22  0000000e+00" r="
+000020a0: 312e 3232 3734 3432 3537 3532 3834 3136  1.22744257528416
+000020b0: 3037 2220 2f3e 0d0a 2020 2020 2020 3c63  07" />..      <c
+000020c0: 6972 636c 6520 6378 3d22 352e 3030 3030  ircle cx="5.0000
+000020d0: 3030 3030 652b 3030 2220 6379 3d22 392e  0000e+00" cy="9.
+000020e0: 3530 3030 3030 3030 652b 3031 2220 723d  50000000e+01" r=
+000020f0: 2231 2e32 3237 3434 3235 3735 3238 3431  "1.2274425752841
+00002100: 3630 3722 202f 3e0d 0a20 2020 2020 203c  607" />..      <
+00002110: 6369 7263 6c65 2063 783d 2235 2e30 3030  circle cx="5.000
+00002120: 3030 3030 3065 2b30 3022 2063 793d 2235  00000e+00" cy="5
+00002130: 2e30 3030 3030 3030 3065 2b30 3022 2072  .00000000e+00" r
+00002140: 3d22 312e 3232 3734 3432 3537 3532 3834  ="1.227442575284
+00002150: 3136 3037 2220 2f3e 0d0a 2020 2020 2020  1607" />..      
+00002160: 3c63 6972 636c 6520 6378 3d22 322e 3330  <circle cx="2.30
+00002170: 3030 3030 3030 652b 3031 2220 6379 3d22  000000e+01" cy="
+00002180: 322e 3330 3030 3030 3030 652b 3031 2220  2.30000000e+01" 
+00002190: 723d 2231 2e32 3237 3434 3235 3735 3238  r="1.22744257528
+000021a0: 3431 3630 3722 202f 3e0d 0a20 2020 2020  41607" />..     
+000021b0: 203c 6369 7263 6c65 2063 783d 2232 2e33   <circle cx="2.3
+000021c0: 3030 3030 3030 3065 2b30 3122 2063 793d  0000000e+01" cy=
+000021d0: 2235 2e39 3030 3030 3030 3065 2b30 3122  "5.90000000e+01"
+000021e0: 2072 3d22 312e 3232 3734 3432 3537 3532   r="1.2274425752
+000021f0: 3834 3136 3037 2220 2f3e 0d0a 2020 2020  841607" />..    
+00002200: 2020 3c63 6972 636c 6520 6378 3d22 342e    <circle cx="4.
+00002210: 3130 3030 3030 3030 652b 3031 2220 6379  10000000e+01" cy
+00002220: 3d22 372e 3730 3030 3030 3030 652b 3031  ="7.70000000e+01
+00002230: 2220 723d 2231 2e32 3237 3434 3235 3735  " r="1.227442575
+00002240: 3238 3431 3630 3722 202f 3e0d 0a20 2020  2841607" />..   
+00002250: 2020 203c 6369 7263 6c65 2063 783d 2235     <circle cx="5
+00002260: 2e39 3030 3030 3030 3065 2b30 3122 2063  .90000000e+01" c
+00002270: 793d 2235 2e39 3030 3030 3030 3065 2b30  y="5.90000000e+0
+00002280: 3122 2072 3d22 312e 3232 3734 3432 3537  1" r="1.22744257
+00002290: 3532 3834 3136 3037 2220 2f3e 0d0a 2020  52841607" />..  
+000022a0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+000022b0: 372e 3730 3030 3030 3030 652b 3031 2220  7.70000000e+01" 
+000022c0: 6379 3d22 342e 3130 3030 3030 3030 652b  cy="4.10000000e+
+000022d0: 3031 2220 723d 2231 2e32 3237 3434 3235  01" r="1.2274425
+000022e0: 3735 3238 3431 3630 3722 202f 3e0d 0a20  752841607" />.. 
+000022f0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00002300: 2235 2e39 3030 3030 3030 3065 2b30 3122  "5.90000000e+01"
+00002310: 2063 793d 2232 2e33 3030 3030 3030 3065   cy="2.30000000e
+00002320: 2b30 3122 2072 3d22 312e 3232 3734 3432  +01" r="1.227442
+00002330: 3537 3532 3834 3136 3037 2220 2f3e 0d0a  5752841607" />..
+00002340: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+00002350: 3d22 372e 3130 3933 3732 3330 652b 3031  ="7.10937230e+01
+00002360: 2220 6379 3d22 372e 3130 3034 3137 3330  " cy="7.10041730
+00002370: 652b 3031 2220 723d 2231 2e32 3237 3434  e+01" r="1.22744
+00002380: 3235 3735 3238 3431 3630 3722 202f 3e0d  25752841607" />.
+00002390: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+000023a0: 783d 2237 2e35 3431 3336 3234 3065 2b30  x="7.54136240e+0
+000023b0: 3122 2063 793d 2232 2e34 3635 3931 3539  1" cy="2.4659159
+000023c0: 3065 2b30 3122 2072 3d22 312e 3232 3734  0e+01" r="1.2274
+000023d0: 3432 3537 3532 3834 3136 3037 2220 2f3e  425752841607" />
+000023e0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+000023f0: 6378 3d22 332e 3734 3936 3733 3230 652b  cx="3.74967320e+
+00002400: 3031 2220 6379 3d22 382e 3534 3532 3537  01" cy="8.545257
+00002410: 3530 652b 3031 2220 723d 2231 2e32 3237  50e+01" r="1.227
+00002420: 3434 3235 3735 3238 3431 3630 3722 202f  4425752841607" /
+00002430: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+00002440: 2063 783d 2238 2e32 3930 3339 3535 3065   cx="8.29039550e
+00002450: 2b30 3122 2063 793d 2238 2e32 3835 3937  +01" cy="8.28597
+00002460: 3437 3065 2b30 3122 2072 3d22 312e 3232  470e+01" r="1.22
+00002470: 3734 3432 3537 3532 3834 3136 3037 2220  74425752841607" 
+00002480: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+00002490: 6520 6378 3d22 312e 3439 3430 3835 3130  e cx="1.49408510
+000024a0: 652b 3031 2220 6379 3d22 382e 3530 3139  e+01" cy="8.5019
+000024b0: 3239 3730 652b 3031 2220 723d 2231 2e32  2970e+01" r="1.2
+000024c0: 3237 3434 3235 3735 3238 3431 3630 3722  274425752841607"
+000024d0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+000024e0: 6c65 2063 783d 2237 2e33 3535 3839 3133  le cx="7.3558913
+000024f0: 3065 2b30 3122 2063 793d 2232 2e36 3437  0e+01" cy="2.647
+00002500: 3631 3936 3065 2b30 3122 2072 3d22 312e  61960e+01" r="1.
+00002510: 3232 3734 3432 3537 3532 3834 3136 3037  2274425752841607
+00002520: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+00002530: 636c 6520 6378 3d22 322e 3233 3831 3436  cle cx="2.238146
+00002540: 3630 652b 3031 2220 6379 3d22 362e 3734  60e+01" cy="6.74
+00002550: 3335 3332 3230 652b 3031 2220 723d 2231  353220e+01" r="1
+00002560: 2e32 3237 3434 3235 3735 3238 3431 3630  .227442575284160
+00002570: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+00002580: 7263 6c65 2063 783d 2231 2e34 3036 3631  rcle cx="1.40661
+00002590: 3431 3065 2b30 3122 2063 793d 2235 2e34  410e+01" cy="5.4
+000025a0: 3437 3531 3936 3065 2b30 3122 2072 3d22  4751960e+01" r="
+000025b0: 312e 3232 3734 3432 3537 3532 3834 3136  1.22744257528416
+000025c0: 3037 2220 2f3e 0d0a 2020 2020 2020 3c63  07" />..      <c
+000025d0: 6972 636c 6520 6378 3d22 362e 3035 3338  ircle cx="6.0538
+000025e0: 3130 3030 652b 3031 2220 6379 3d22 382e  1000e+01" cy="8.
+000025f0: 3330 3332 3238 3630 652b 3031 2220 723d  30322860e+01" r=
+00002600: 2231 2e32 3237 3434 3235 3735 3238 3431  "1.2274425752841
+00002610: 3630 3722 202f 3e0d 0a20 2020 2020 203c  607" />..      <
+00002620: 6369 7263 6c65 2063 783d 2235 2e32 3238  circle cx="5.228
+00002630: 3538 3239 3065 2b30 3122 2063 793d 2238  58290e+01" cy="8
+00002640: 2e33 3835 3338 3630 3065 2b30 3122 2072  .38538600e+01" r
+00002650: 3d22 312e 3232 3734 3432 3537 3532 3834  ="1.227442575284
+00002660: 3136 3037 2220 2f3e 0d0a 2020 2020 2020  1607" />..      
+00002670: 3c63 6972 636c 6520 6378 3d22 312e 3430  <circle cx="1.40
+00002680: 3035 3932 3230 652b 3031 2220 6379 3d22  059220e+01" cy="
+00002690: 342e 3534 3931 3332 3430 652b 3031 2220  4.54913240e+01" 
+000026a0: 723d 2231 2e32 3237 3434 3235 3735 3238  r="1.22744257528
+000026b0: 3431 3630 3722 202f 3e0d 0a20 2020 2020  41607" />..     
+000026c0: 203c 6369 7263 6c65 2063 783d 2234 2e35   <circle cx="4.5
+000026d0: 3439 3134 3134 3065 2b30 3122 2063 793d  4914140e+01" cy=
+000026e0: 2231 2e34 3030 3539 3538 3065 2b30 3122  "1.40059580e+01"
+000026f0: 2072 3d22 312e 3232 3734 3432 3537 3532   r="1.2274425752
+00002700: 3834 3136 3037 2220 2f3e 0d0a 2020 2020  841607" />..    
+00002710: 2020 3c63 6972 636c 6520 6378 3d22 322e    <circle cx="2.
+00002720: 3435 3935 3530 3230 652b 3031 2220 6379  45955020e+01" cy
+00002730: 3d22 372e 3533 3439 3936 3730 652b 3031  ="7.53499670e+01
+00002740: 2220 723d 2231 2e32 3237 3434 3235 3735  " r="1.227442575
+00002750: 3238 3431 3630 3722 202f 3e0d 0a20 2020  2841607" />..   
+00002760: 2020 203c 6369 7263 6c65 2063 783d 2236     <circle cx="6
+00002770: 2e35 3535 3330 3335 3065 2b30 3122 2063  .55530350e+01" c
+00002780: 793d 2236 2e35 3531 3332 3337 3065 2b30  y="6.55132370e+0
+00002790: 3122 2072 3d22 312e 3232 3734 3432 3537  1" r="1.22744257
+000027a0: 3532 3834 3136 3037 2220 2f3e 0d0a 2020  52841607" />..  
+000027b0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+000027c0: 382e 3631 3631 3437 3830 652b 3031 2220  8.61614780e+01" 
+000027d0: 6379 3d22 342e 3535 3334 3638 3630 652b  cy="4.55346860e+
+000027e0: 3031 2220 723d 2231 2e32 3237 3434 3235  01" r="1.2274425
+000027f0: 3735 3238 3431 3630 3722 202f 3e0d 0a20  752841607" />.. 
+00002800: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00002810: 2231 2e33 3939 3937 3636 3965 2b30 3122  "1.39997669e+01"
+00002820: 2063 793d 2231 2e33 3939 3937 3636 3065   cy="1.39997660e
+00002830: 2b30 3122 2072 3d22 312e 3232 3734 3432  +01" r="1.227442
+00002840: 3537 3532 3834 3136 3037 2220 2f3e 0d0a  5752841607" />..
+00002850: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+00002860: 3d22 382e 3330 3735 3632 3130 652b 3031  ="8.30756210e+01
+00002870: 2220 6379 3d22 362e 3034 3933 3332 3530  " cy="6.04933250
+00002880: 652b 3031 2220 723d 2231 2e32 3237 3434  e+01" r="1.22744
+00002890: 3235 3735 3238 3431 3630 3722 202f 3e0d  25752841607" />.
+000028a0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+000028b0: 783d 2236 2e37 3436 3838 3833 3065 2b30  x="6.74688830e+0
+000028c0: 3122 2063 793d 2232 2e32 3430 3437 3331  1" cy="2.2404731
+000028d0: 3065 2b30 3122 2072 3d22 312e 3232 3734  0e+01" r="1.2274
+000028e0: 3432 3537 3532 3834 3136 3037 2220 2f3e  425752841607" />
+000028f0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+00002900: 6378 3d22 312e 3435 3933 3034 3630 652b  cx="1.45930460e+
+00002910: 3031 2220 6379 3d22 362e 3234 3533 3631  01" cy="6.245361
+00002920: 3530 652b 3031 2220 723d 2231 2e32 3237  50e+01" r="1.227
+00002930: 3434 3235 3735 3238 3431 3630 3722 202f  4425752841607" /
+00002940: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+00002950: 2063 783d 2238 2e33 3835 3536 3234 3065   cx="8.38556240e
+00002960: 2b30 3122 2063 793d 2235 2e32 3238 3730  +01" cy="5.22870
+00002970: 3434 3065 2b30 3122 2072 3d22 312e 3232  440e+01" r="1.22
+00002980: 3734 3432 3537 3532 3834 3136 3037 2220  74425752841607" 
+00002990: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+000029a0: 6520 6378 3d22 312e 3430 3031 3039 3830  e cx="1.40010980
+000029b0: 652b 3031 2220 6379 3d22 332e 3634 3937  e+01" cy="3.6497
+000029c0: 3032 3130 652b 3031 2220 723d 2231 2e32  0210e+01" r="1.2
+000029d0: 3237 3434 3235 3735 3238 3431 3630 3722  274425752841607"
+000029e0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+000029f0: 6c65 2063 783d 2233 2e36 3439 3730 3537  le cx="3.6497057
+00002a00: 3065 2b30 3122 2063 793d 2231 2e34 3030  0e+01" cy="1.400
+00002a10: 3131 3136 3065 2b30 3122 2072 3d22 312e  11160e+01" r="1.
+00002a20: 3232 3734 3432 3537 3532 3834 3136 3037  2274425752841607
+00002a30: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+00002a40: 636c 6520 6378 3d22 362e 3234 3835 3231  cle cx="6.248521
+00002a50: 3430 652b 3031 2220 6379 3d22 312e 3436  40e+01" cy="1.46
+00002a60: 3138 3431 3730 652b 3031 2220 723d 2231  184170e+01" r="1
+00002a70: 2e32 3237 3434 3235 3735 3238 3431 3630  .227442575284160
+00002a80: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+00002a90: 7263 6c65 2063 783d 2236 2e32 3633 3133  rcle cx="6.26313
+00002aa0: 3734 3065 2b30 3122 2063 793d 2237 2e31  740e+01" cy="7.1
+00002ab0: 3732 3837 3138 3065 2b30 3122 2072 3d22  7287180e+01" r="
+00002ac0: 312e 3232 3734 3432 3537 3532 3834 3136  1.22744257528416
+00002ad0: 3037 2220 2f3e 0d0a 2020 2020 2020 3c63  07" />..      <c
+00002ae0: 6972 636c 6520 6378 3d22 342e 3535 3334  ircle cx="4.5534
+00002af0: 3032 3030 652b 3031 2220 6379 3d22 382e  0200e+01" cy="8.
+00002b00: 3631 3630 3037 3331 652b 3031 2220 723d  61600731e+01" r=
+00002b10: 2231 2e32 3237 3434 3235 3735 3238 3431  "1.2274425752841
+00002b20: 3630 3722 202f 3e0d 0a20 2020 2020 203c  607" />..      <
+00002b30: 6369 7263 6c65 2063 783d 2237 2e37 3631  circle cx="7.761
+00002b40: 3134 3630 3065 2b30 3122 2063 793d 2233  14600e+01" cy="3
+00002b50: 2e32 3536 3938 3731 3065 2b30 3122 2072  .25698710e+01" r
+00002b60: 3d22 312e 3232 3734 3432 3537 3532 3834  ="1.227442575284
+00002b70: 3136 3037 2220 2f3e 0d0a 2020 2020 2020  1607" />..      
+00002b80: 3c63 6972 636c 6520 6378 3d22 332e 3235  <circle cx="3.25
+00002b90: 3336 3230 3230 652b 3031 2220 6379 3d22  362020e+01" cy="
+00002ba0: 372e 3735 3838 3231 3330 652b 3031 2220  7.75882130e+01" 
+00002bb0: 723d 2231 2e32 3237 3434 3235 3735 3238  r="1.22744257528
+00002bc0: 3431 3630 3722 202f 3e0d 0a20 2020 2020  41607" />..     
+00002bd0: 203c 6369 7263 6c65 2063 783d 2235 2e34   <circle cx="5.4
+00002be0: 3437 3534 3636 3065 2b30 3122 2063 793d  4754660e+01" cy=
+00002bf0: 2231 2e34 3036 3636 3435 3065 2b30 3122  "1.40666450e+01"
+00002c00: 2072 3d22 312e 3232 3734 3432 3537 3532   r="1.2274425752
+00002c10: 3834 3136 3037 2220 2f3e 0d0a 2020 2020  841607" />..    
+00002c20: 2020 3c63 6972 636c 6520 6378 3d22 382e    <circle cx="8.
+00002c30: 3530 3439 3237 3630 652b 3031 2220 6379  50492760e+01" cy
+00002c40: 3d22 312e 3439 3730 3933 3830 652b 3031  ="1.49709380e+01
+00002c50: 2220 723d 2231 2e32 3237 3434 3235 3735  " r="1.227442575
+00002c60: 3238 3431 3630 3722 202f 3e0d 0a20 2020  2841607" />..   
+00002c70: 2020 203c 6369 7263 6c65 2063 783d 2237     <circle cx="7
+00002c80: 2e31 3736 3937 3133 3065 2b30 3122 2063  .17697130e+01" c
+00002c90: 793d 2236 2e32 3538 3335 3537 3065 2b30  y="6.25835570e+0
+00002ca0: 3122 2072 3d22 312e 3232 3734 3432 3537  1" r="1.22744257
+00002cb0: 3532 3834 3136 3037 2220 2f3e 0d0a 2020  52841607" />..  
+00002cc0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+00002cd0: 382e 3534 3738 3136 3230 652b 3031 2220  8.54781620e+01" 
+00002ce0: 6379 3d22 332e 3735 3238 3432 3130 652b  cy="3.75284210e+
+00002cf0: 3031 2220 723d 2231 2e32 3237 3434 3235  01" r="1.2274425
+00002d00: 3735 3238 3431 3630 3722 202f 3e0d 0a20  752841607" />.. 
+00002d10: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00002d20: 2232 2e36 3434 3439 3834 3065 2b30 3122  "2.64449840e+01"
+00002d30: 2063 793d 2237 2e33 3532 3736 3734 3065   cy="7.35276740e
+00002d40: 2b30 3122 2072 3d22 312e 3232 3734 3432  +01" r="1.227442
+00002d50: 3537 3532 3834 3136 3037 2220 2f3e 0d0a  5752841607" />..
+00002d60: 2020 203c 2f67 3e0d 0a3c 2f73 7667 3e       </g>..</svg>
```

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/HeartPlate_BT3_4x4.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/HeartPlate_BT3_4x4.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/HeartPlate_BT3_4x4_exp.svg` & `lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/HeartPlate_BT3_4x4_exp.svg`

 * *Files 6% similar despite different names*

```diff
@@ -7,3805 +7,4070 @@
 00000060: 6e74 7322 2066 696c 6c3d 2223 6663 6666  nts" fill="#fcff
 00000070: 3565 2220 7374 726f 6b65 3d22 626c 6163  5e" stroke="blac
 00000080: 6b22 2073 7472 6f6b 652d 7769 6474 683d  k" stroke-width=
 00000090: 2230 2e32 3638 3430 3532 3332 3638 3930  "0.2684052326890
 000000a0: 3538 3836 223e 0d0a 2020 2020 2020 3c70  5886">..      <p
 000000b0: 6174 6820 643d 224d 2036 2e32 3231 3836  ath d="M 6.22186
 000000c0: 3433 3065 2b30 3120 312e 3537 3433 3035  430e+01 1.574305
-000000d0: 3730 652b 3031 2051 2036 2e37 3336 3535  70e+01 Q 6.73655
-000000e0: 3835 3565 2b30 3120 312e 3033 3735 3239  855e+01 1.037529
-000000f0: 3935 652b 3031 2c20 372e 3235 3030 3030  95e+01, 7.250000
-00000100: 3030 652b 3031 2035 2e30 3030 3030 3030  00e+01 5.0000000
-00000110: 3065 2b30 3020 5120 362e 3132 3530 3030  0e+00 Q 6.125000
-00000120: 3930 652b 3031 2035 2e30 3030 3030 3030  90e+01 5.0000000
-00000130: 3065 2b30 302c 2035 2e30 3030 3030 3138  0e+00, 5.0000018
-00000140: 3065 2b30 3120 352e 3030 3030 3030 3030  0e+01 5.00000000
-00000150: 652b 3030 2051 2035 2e36 3039 3835 3537  e+00 Q 5.6098557
-00000160: 3565 2b30 3120 312e 3034 3030 3438 3135  5e+01 1.04004815
-00000170: 652b 3031 2c20 362e 3232 3138 3634 3330  e+01, 6.22186430
-00000180: 652b 3031 2031 2e35 3734 3330 3537 3065  e+01 1.57430570e
-00000190: 2b30 3120 5a22 202f 3e0d 0a20 2020 2020  +01 Z" />..     
-000001a0: 203c 7061 7468 2064 3d22 4d20 392e 3530   <path d="M 9.50
-000001b0: 3030 3030 3030 652b 3031 2035 2e30 3030  000000e+01 5.000
-000001c0: 3030 3030 3065 2b30 3020 5120 382e 3337  00000e+00 Q 8.37
-000001d0: 3530 3030 3030 652b 3031 2035 2e30 3030  500000e+01 5.000
-000001e0: 3030 3030 3065 2b30 302c 2037 2e32 3530  00000e+00, 7.250
-000001f0: 3030 3030 3065 2b30 3120 352e 3030 3030  00000e+01 5.0000
-00000200: 3030 3030 652b 3030 2051 2037 2e37 3734  0000e+00 Q 7.774
-00000210: 3734 3233 3065 2b30 3120 312e 3130 3033  74230e+01 1.1003
-00000220: 3533 3535 652b 3031 2c20 382e 3239 3934  5355e+01, 8.2994
-00000230: 3834 3630 652b 3031 2031 2e37 3030 3730  8460e+01 1.70070
-00000240: 3731 3065 2b30 3120 5120 382e 3839 3937  710e+01 Q 8.8997
-00000250: 3432 3330 652b 3031 2031 2e31 3030 3335  4230e+01 1.10035
-00000260: 3335 3565 2b30 312c 2039 2e35 3030 3030  355e+01, 9.50000
-00000270: 3030 3065 2b30 3120 352e 3030 3030 3030  000e+01 5.000000
-00000280: 3030 652b 3030 205a 2220 2f3e 0d0a 2020  00e+00 Z" />..  
-00000290: 2020 2020 3c70 6174 6820 643d 224d 2038      <path d="M 8
-000002a0: 2e32 3939 3438 3436 3065 2b30 3120 312e  .29948460e+01 1.
-000002b0: 3730 3037 3037 3130 652b 3031 2051 2037  70070710e+01 Q 7
-000002c0: 2e37 3734 3734 3233 3065 2b30 3120 312e  .77474230e+01 1.
-000002d0: 3130 3033 3533 3535 652b 3031 2c20 372e  10035355e+01, 7.
-000002e0: 3235 3030 3030 3030 652b 3031 2035 2e30  25000000e+01 5.0
-000002f0: 3030 3030 3030 3065 2b30 3020 5120 372e  0000000e+00 Q 7.
-00000300: 3235 3332 3135 3235 652b 3031 2031 2e32  25321525e+01 1.2
-00000310: 3336 3137 3532 3565 2b30 312c 2037 2e32  3617525e+01, 7.2
-00000320: 3630 3131 3333 3065 2b30 3120 312e 3937  6011330e+01 1.97
-00000330: 3030 3534 3630 652b 3031 2051 2037 2e37  005460e+01 Q 7.7
-00000340: 3830 3339 3433 3065 2b30 3120 312e 3833  8039430e+01 1.83
-00000350: 3539 3938 3235 652b 3031 2c20 382e 3239  599825e+01, 8.29
-00000360: 3934 3834 3630 652b 3031 2031 2e37 3030  948460e+01 1.700
-00000370: 3730 3731 3065 2b30 3120 5a22 202f 3e0d  70710e+01 Z" />.
-00000380: 0a20 2020 2020 203c 7061 7468 2064 3d22  .      <path d="
-00000390: 4d20 372e 3235 3030 3030 3030 652b 3031  M 7.25000000e+01
-000003a0: 2035 2e30 3030 3030 3030 3065 2b30 3020   5.00000000e+00 
-000003b0: 5120 362e 3733 3635 3538 3535 652b 3031  Q 6.73655855e+01
-000003c0: 2031 2e30 3337 3532 3939 3565 2b30 312c   1.03752995e+01,
-000003d0: 2036 2e32 3231 3836 3433 3065 2b30 3120   6.22186430e+01 
-000003e0: 312e 3537 3433 3035 3730 652b 3031 2051  1.57430570e+01 Q
-000003f0: 2036 2e37 3431 3339 3536 3065 2b30 3120   6.74139560e+01 
-00000400: 312e 3736 3937 3132 3830 652b 3031 2c20  1.76971280e+01, 
-00000410: 372e 3236 3031 3133 3330 652b 3031 2031  7.26011330e+01 1
-00000420: 2e39 3730 3035 3436 3065 2b30 3120 5120  .97005460e+01 Q 
-00000430: 372e 3235 3332 3135 3235 652b 3031 2031  7.25321525e+01 1
-00000440: 2e32 3336 3137 3532 3565 2b30 312c 2037  .23617525e+01, 7
-00000450: 2e32 3530 3030 3030 3065 2b30 3120 352e  .25000000e+01 5.
-00000460: 3030 3030 3030 3030 652b 3030 205a 2220  00000000e+00 Z" 
-00000470: 2f3e 0d0a 2020 2020 2020 3c70 6174 6820  />..      <path 
-00000480: 643d 224d 2035 2e30 3030 3030 3138 3065  d="M 5.00000180e
-00000490: 2b30 3120 352e 3030 3030 3030 3030 652b  +01 5.00000000e+
-000004a0: 3030 2051 2033 2e38 3735 3030 3138 3065  00 Q 3.87500180e
-000004b0: 2b30 3120 352e 3030 3030 3030 3030 652b  +01 5.00000000e+
-000004c0: 3030 2c20 322e 3735 3030 3030 3930 652b  00, 2.75000090e+
-000004d0: 3031 2035 2e30 3030 3030 3030 3065 2b30  01 5.00000000e+0
-000004e0: 3020 5120 332e 3333 3035 3436 3830 652b  0 Q 3.33054680e+
-000004f0: 3031 2039 2e38 3332 3539 3035 3065 2b30  01 9.83259050e+0
-00000500: 302c 2033 2e39 3131 3039 3138 3065 2b30  0, 3.91109180e+0
-00000510: 3120 312e 3436 3635 3138 3130 652b 3031  1 1.46651810e+01
-00000520: 2051 2034 2e34 3535 3534 3638 3065 2b30   Q 4.45554680e+0
-00000530: 3120 392e 3833 3235 3930 3530 652b 3030  1 9.83259050e+00
-00000540: 2c20 352e 3030 3030 3031 3830 652b 3031  , 5.00000180e+01
-00000550: 2035 2e30 3030 3030 3030 3065 2b30 3020   5.00000000e+00 
-00000560: 5a22 202f 3e0d 0a20 2020 2020 203c 7061  Z" />..      <pa
-00000570: 7468 2064 3d22 4d20 352e 3030 3030 3031  th d="M 5.000001
-00000580: 3830 652b 3031 2035 2e30 3030 3030 3030  80e+01 5.0000000
-00000590: 3065 2b30 3020 5120 342e 3435 3535 3436  0e+00 Q 4.455546
-000005a0: 3830 652b 3031 2039 2e38 3332 3539 3035  80e+01 9.8325905
-000005b0: 3065 2b30 302c 2033 2e39 3131 3039 3138  0e+00, 3.9110918
-000005c0: 3065 2b30 3120 312e 3436 3635 3138 3130  0e+01 1.46651810
-000005d0: 652b 3031 2051 2034 2e32 3739 3733 3736  e+01 Q 4.2797376
-000005e0: 3565 2b30 3120 312e 3536 3431 3237 3135  5e+01 1.56412715
-000005f0: 652b 3031 2c20 342e 3634 3833 3833 3530  e+01, 4.64838350
-00000600: 652b 3031 2031 2e36 3631 3733 3731 3065  e+01 1.66173710e
-00000610: 2b30 3120 5120 342e 3832 3431 3932 3635  +01 Q 4.82419265
-00000620: 652b 3031 2031 2e30 3830 3836 3835 3565  e+01 1.08086855e
-00000630: 2b30 312c 2035 2e30 3030 3030 3138 3065  +01, 5.00000180e
-00000640: 2b30 3120 352e 3030 3030 3030 3030 652b  +01 5.00000000e+
-00000650: 3030 205a 2220 2f3e 0d0a 2020 2020 2020  00 Z" />..      
-00000660: 3c70 6174 6820 643d 224d 2035 2e30 3030  <path d="M 5.000
-00000670: 3030 3138 3065 2b30 3120 352e 3030 3030  00180e+01 5.0000
-00000680: 3030 3030 652b 3030 2051 2034 2e38 3234  0000e+00 Q 4.824
-00000690: 3139 3236 3565 2b30 3120 312e 3038 3038  19265e+01 1.0808
-000006a0: 3638 3535 652b 3031 2c20 342e 3634 3833  6855e+01, 4.6483
-000006b0: 3833 3530 652b 3031 2031 2e36 3631 3733  8350e+01 1.66173
-000006c0: 3731 3065 2b30 3120 5120 342e 3938 3439  710e+01 Q 4.9849
-000006d0: 3931 3630 652b 3031 2031 2e36 3833 3937  9160e+01 1.68397
-000006e0: 3631 3065 2b30 312c 2035 2e33 3231 3432  610e+01, 5.32142
-000006f0: 3333 3065 2b30 3120 312e 3730 3535 3737  330e+01 1.705577
-00000700: 3030 652b 3031 2051 2035 2e31 3630 3533  00e+01 Q 5.16053
-00000710: 3532 3565 2b30 3120 312e 3130 3237 3537  525e+01 1.102757
-00000720: 3435 652b 3031 2c20 352e 3030 3030 3031  45e+01, 5.000001
-00000730: 3830 652b 3031 2035 2e30 3030 3030 3030  80e+01 5.0000000
-00000740: 3065 2b30 3020 5a22 202f 3e0d 0a20 2020  0e+00 Z" />..   
-00000750: 2020 203c 7061 7468 2064 3d22 4d20 352e     <path d="M 5.
-00000760: 3030 3030 3031 3830 652b 3031 2035 2e30  00000180e+01 5.0
-00000770: 3030 3030 3030 3065 2b30 3020 5120 352e  0000000e+00 Q 5.
-00000780: 3136 3035 3335 3235 652b 3031 2031 2e31  16053525e+01 1.1
-00000790: 3032 3735 3734 3565 2b30 312c 2035 2e33  0275745e+01, 5.3
-000007a0: 3231 3432 3333 3065 2b30 3120 312e 3730  2142330e+01 1.70
-000007b0: 3535 3737 3030 652b 3031 2051 2035 2e37  557700e+01 Q 5.7
-000007c0: 3730 3632 3134 3065 2b30 3120 312e 3633  7062140e+01 1.63
-000007d0: 3938 3534 3035 652b 3031 2c20 362e 3232  985405e+01, 6.22
-000007e0: 3138 3634 3330 652b 3031 2031 2e35 3734  186430e+01 1.574
-000007f0: 3330 3537 3065 2b30 3120 5120 352e 3630  30570e+01 Q 5.60
-00000800: 3938 3535 3735 652b 3031 2031 2e30 3430  985575e+01 1.040
-00000810: 3034 3831 3565 2b30 312c 2035 2e30 3030  04815e+01, 5.000
-00000820: 3030 3138 3065 2b30 3120 352e 3030 3030  00180e+01 5.0000
-00000830: 3030 3030 652b 3030 205a 2220 2f3e 0d0a  0000e+00 Z" />..
-00000840: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
-00000850: 2032 2e37 3530 3030 3039 3065 2b30 3120   2.75000090e+01 
-00000860: 352e 3030 3030 3030 3030 652b 3030 2051  5.00000000e+00 Q
-00000870: 2031 2e36 3235 3030 3033 3165 2b30 3120   1.62500031e+01 
-00000880: 352e 3030 3030 3030 3030 652b 3030 2c20  5.00000000e+00, 
-00000890: 352e 3030 3030 3030 3030 652b 3030 2035  5.00000000e+00 5
-000008a0: 2e30 3030 3030 3030 3065 2b30 3020 5120  .00000000e+00 Q 
-000008b0: 312e 3339 3939 3939 3837 652b 3031 2031  1.39999987e+01 1
-000008c0: 2e34 3030 3030 3030 3065 2b30 312c 2032  .40000000e+01, 2
-000008d0: 2e33 3030 3030 3030 3065 2b30 3120 322e  .30000000e+01 2.
-000008e0: 3330 3030 3030 3030 652b 3031 2051 2032  30000000e+01 Q 2
-000008f0: 2e35 3235 3030 3034 3565 2b30 3120 312e  .52500045e+01 1.
-00000900: 3430 3030 3030 3030 652b 3031 2c20 322e  40000000e+01, 2.
-00000910: 3735 3030 3030 3930 652b 3031 2035 2e30  75000090e+01 5.0
-00000920: 3030 3030 3030 3065 2b30 3020 5a22 202f  0000000e+00 Z" /
-00000930: 3e0d 0a20 2020 2020 203c 7061 7468 2064  >..      <path d
-00000940: 3d22 4d20 322e 3330 3030 3030 3030 652b  ="M 2.30000000e+
-00000950: 3031 2032 2e33 3030 3030 3030 3065 2b30  01 2.30000000e+0
-00000960: 3120 5120 322e 3735 3030 3030 3030 652b  1 Q 2.75000000e+
-00000970: 3031 2032 2e33 3030 3030 3030 3065 2b30  01 2.30000000e+0
-00000980: 312c 2033 2e32 3030 3030 3030 3065 2b30  1, 3.20000000e+0
-00000990: 3120 322e 3330 3030 3030 3030 652b 3031  1 2.30000000e+01
-000009a0: 2051 2032 2e39 3735 3030 3039 3065 2b30   Q 2.97500090e+0
-000009b0: 3120 312e 3430 3030 3030 3030 652b 3031  1 1.40000000e+01
-000009c0: 2c20 322e 3735 3030 3030 3930 652b 3031  , 2.75000090e+01
-000009d0: 2035 2e30 3030 3030 3030 3065 2b30 3020   5.00000000e+00 
-000009e0: 5120 322e 3532 3530 3030 3435 652b 3031  Q 2.52500045e+01
-000009f0: 2031 2e34 3030 3030 3030 3065 2b30 312c   1.40000000e+01,
-00000a00: 2032 2e33 3030 3030 3030 3065 2b30 3120   2.30000000e+01 
-00000a10: 322e 3330 3030 3030 3030 652b 3031 205a  2.30000000e+01 Z
-00000a20: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
-00000a30: 6820 643d 224d 2033 2e32 3030 3030 3030  h d="M 3.2000000
-00000a40: 3065 2b30 3120 322e 3330 3030 3030 3030  0e+01 2.30000000
-00000a50: 652b 3031 2051 2033 2e35 3535 3534 3633  e+01 Q 3.5555463
-00000a60: 3565 2b30 3120 312e 3838 3332 3539 3035  5e+01 1.88325905
-00000a70: 652b 3031 2c20 332e 3931 3130 3931 3830  e+01, 3.91109180
-00000a80: 652b 3031 2031 2e34 3636 3531 3831 3065  e+01 1.46651810e
-00000a90: 2b30 3120 5120 332e 3333 3035 3436 3830  +01 Q 3.33054680
-00000aa0: 652b 3031 2039 2e38 3332 3539 3035 3065  e+01 9.83259050e
-00000ab0: 2b30 302c 2032 2e37 3530 3030 3039 3065  +00, 2.75000090e
-00000ac0: 2b30 3120 352e 3030 3030 3030 3030 652b  +01 5.00000000e+
-00000ad0: 3030 2051 2032 2e39 3735 3030 3039 3065  00 Q 2.97500090e
-00000ae0: 2b30 3120 312e 3430 3030 3030 3030 652b  +01 1.40000000e+
-00000af0: 3031 2c20 332e 3230 3030 3030 3030 652b  01, 3.20000000e+
-00000b00: 3031 2032 2e33 3030 3030 3030 3065 2b30  01 2.30000000e+0
-00000b10: 3120 5a22 202f 3e0d 0a20 2020 2020 203c  1 Z" />..      <
-00000b20: 7061 7468 2064 3d22 4d20 352e 3337 3237  path d="M 5.3727
-00000b30: 3931 3730 652b 3031 2037 2e31 3732 3739  9170e+01 7.17279
-00000b40: 3236 3065 2b30 3120 5120 352e 3130 3532  260e+01 Q 5.1052
-00000b50: 3436 3930 652b 3031 2037 2e34 3037 3230  4690e+01 7.40720
-00000b60: 3132 3065 2b30 312c 2034 2e37 3838 3833  120e+01, 4.78883
-00000b70: 3033 3065 2b30 3120 372e 3536 3239 3833  030e+01 7.562983
-00000b80: 3130 652b 3031 2051 2035 2e32 3536 3035  10e+01 Q 5.25605
-00000b90: 3232 3565 2b30 3120 372e 3836 3230 3830  225e+01 7.862080
-00000ba0: 3535 652b 3031 2c20 352e 3731 3037 3439  55e+01, 5.710749
-00000bb0: 3830 652b 3031 2038 2e31 3330 3638 3837  80e+01 8.1306887
-00000bc0: 3065 2b30 3120 5120 352e 3535 3136 3939  0e+01 Q 5.551699
-00000bd0: 3130 652b 3031 2037 2e36 3632 3834 3335  10e+01 7.6628435
-00000be0: 3065 2b30 312c 2035 2e33 3732 3739 3137  0e+01, 5.3727917
-00000bf0: 3065 2b30 3120 372e 3137 3237 3932 3630  0e+01 7.17279260
-00000c00: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
-00000c10: 2020 3c70 6174 6820 643d 224d 2034 2e37    <path d="M 4.7
-00000c20: 3838 3833 3033 3065 2b30 3120 372e 3536  8883030e+01 7.56
-00000c30: 3239 3833 3130 652b 3031 2051 2034 2e34  298310e+01 Q 4.4
-00000c40: 3438 3833 3539 3565 2b30 3120 372e 3637  4883595e+01 7.67
-00000c50: 3737 3734 3035 652b 3031 2c20 342e 3130  777405e+01, 4.10
-00000c60: 3030 3030 3030 652b 3031 2037 2e37 3030  000000e+01 7.700
-00000c70: 3030 3030 3065 2b30 3120 5120 342e 3337  00000e+01 Q 4.37
-00000c80: 3931 3935 3735 652b 3031 2037 2e39 3934  919575e+01 7.994
-00000c90: 3035 3136 3065 2b30 312c 2034 2e36 3539  05160e+01, 4.659
-00000ca0: 3831 3236 3065 2b30 3120 382e 3235 3330  81260e+01 8.2530
-00000cb0: 3434 3630 652b 3031 2051 2034 2e37 3239  4460e+01 Q 4.729
-00000cc0: 3730 3739 3565 2b30 3120 372e 3932 3030  70795e+01 7.9200
-00000cd0: 3938 3135 652b 3031 2c20 342e 3738 3838  9815e+01, 4.7888
-00000ce0: 3330 3330 652b 3031 2037 2e35 3632 3938  3030e+01 7.56298
-00000cf0: 3331 3065 2b30 3120 5a22 202f 3e0d 0a20  310e+01 Z" />.. 
-00000d00: 2020 2020 203c 7061 7468 2064 3d22 4d20       <path d="M 
-00000d10: 352e 3731 3037 3439 3830 652b 3031 2038  5.71074980e+01 8
-00000d20: 2e31 3330 3638 3837 3065 2b30 3120 5120  .13068870e+01 Q 
-00000d30: 352e 3235 3630 3532 3235 652b 3031 2037  5.25605225e+01 7
-00000d40: 2e38 3632 3038 3035 3565 2b30 312c 2034  .86208055e+01, 4
-00000d50: 2e37 3838 3833 3033 3065 2b30 3120 372e  .78883030e+01 7.
-00000d60: 3536 3239 3833 3130 652b 3031 2051 2034  56298310e+01 Q 4
-00000d70: 2e37 3239 3730 3739 3565 2b30 3120 372e  .72970795e+01 7.
-00000d80: 3932 3030 3938 3135 652b 3031 2c20 342e  92009815e+01, 4.
-00000d90: 3635 3938 3132 3630 652b 3031 2038 2e32  65981260e+01 8.2
-00000da0: 3533 3034 3436 3065 2b30 3120 5120 352e  5304460e+01 Q 5.
-00000db0: 3138 3634 3836 3330 652b 3031 2038 2e31  18648630e+01 8.1
-00000dc0: 3931 3937 3639 3065 2b30 312c 2035 2e37  9197690e+01, 5.7
-00000dd0: 3130 3734 3938 3065 2b30 3120 382e 3133  1074980e+01 8.13
-00000de0: 3036 3838 3730 652b 3031 205a 2220 2f3e  068870e+01 Z" />
-00000df0: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
-00000e00: 224d 2035 2e37 3632 3938 3331 3065 2b30  "M 5.76298310e+0
-00000e10: 3120 362e 3538 3838 3330 3330 652b 3031  1 6.58883030e+01
-00000e20: 2051 2035 2e36 3037 3230 3132 3065 2b30   Q 5.60720120e+0
-00000e30: 3120 362e 3930 3532 3436 3930 652b 3031  1 6.90524690e+01
-00000e40: 2c20 352e 3337 3237 3931 3730 652b 3031  , 5.37279170e+01
-00000e50: 2037 2e31 3732 3739 3236 3065 2b30 3120   7.17279260e+01 
-00000e60: 5120 352e 3733 3030 3237 3335 652b 3031  Q 5.73002735e+01
-00000e70: 2037 2e32 3138 3734 3838 3565 2b30 312c   7.21874885e+01,
-00000e80: 2036 2e30 3637 3837 3631 3065 2b30 3120   6.06787610e+01 
-00000e90: 372e 3234 3236 3636 3830 652b 3031 2051  7.24266680e+01 Q
-00000ea0: 2035 2e39 3330 3033 3537 3065 2b30 3120   5.93003570e+01 
-00000eb0: 362e 3932 3237 3133 3230 652b 3031 2c20  6.92271320e+01, 
-00000ec0: 352e 3736 3239 3833 3130 652b 3031 2036  5.76298310e+01 6
-00000ed0: 2e35 3838 3833 3033 3065 2b30 3120 5a22  .58883030e+01 Z"
-00000ee0: 202f 3e0d 0a20 2020 2020 203c 7061 7468   />..      <path
-00000ef0: 2064 3d22 4d20 352e 3337 3237 3931 3730   d="M 5.37279170
-00000f00: 652b 3031 2037 2e31 3732 3739 3236 3065  e+01 7.17279260e
-00000f10: 2b30 3120 5120 352e 3535 3136 3939 3130  +01 Q 5.55169910
-00000f20: 652b 3031 2037 2e36 3632 3834 3335 3065  e+01 7.66284350e
-00000f30: 2b30 312c 2035 2e37 3130 3734 3938 3065  +01, 5.71074980e
-00000f40: 2b30 3120 382e 3133 3036 3838 3730 652b  +01 8.13068870e+
-00000f50: 3031 2051 2035 2e38 3838 3737 3032 3565  01 Q 5.88877025e
-00000f60: 2b30 3120 372e 3638 3733 3836 3035 652b  +01 7.68738605e+
-00000f70: 3031 2c20 362e 3036 3738 3736 3130 652b  01, 6.06787610e+
-00000f80: 3031 2037 2e32 3432 3636 3638 3065 2b30  01 7.24266680e+0
-00000f90: 3120 5120 352e 3733 3030 3237 3335 652b  1 Q 5.73002735e+
-00000fa0: 3031 2037 2e32 3138 3734 3838 3565 2b30  01 7.21874885e+0
-00000fb0: 312c 2035 2e33 3732 3739 3137 3065 2b30  1, 5.37279170e+0
-00000fc0: 3120 372e 3137 3237 3932 3630 652b 3031  1 7.17279260e+01
-00000fd0: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
-00000fe0: 6174 6820 643d 224d 2035 2e39 3030 3030  ath d="M 5.90000
-00000ff0: 3030 3065 2b30 3120 352e 3930 3030 3030  000e+01 5.900000
-00001000: 3030 652b 3031 2051 2035 2e38 3737 3737  00e+01 Q 5.87777
-00001010: 3430 3565 2b30 3120 362e 3234 3838 3335  405e+01 6.248835
-00001020: 3935 652b 3031 2c20 352e 3736 3239 3833  95e+01, 5.762983
-00001030: 3130 652b 3031 2036 2e35 3838 3833 3033  10e+01 6.5888303
-00001040: 3065 2b30 3120 5120 362e 3139 3335 3436  0e+01 Q 6.193546
-00001050: 3730 652b 3031 2036 2e36 3035 3233 3539  70e+01 6.6052359
-00001060: 3565 2b30 312c 2036 2e36 3030 3938 3735  5e+01, 6.6009875
-00001070: 3065 2b30 3120 362e 3630 3338 3136 3230  0e+01 6.60381620
-00001080: 652b 3031 2051 2036 2e32 3635 3936 3131  e+01 Q 6.2659611
-00001090: 3565 2b30 3120 362e 3236 3733 3331 3430  5e+01 6.26733140
-000010a0: 652b 3031 2c20 352e 3930 3030 3030 3030  e+01, 5.90000000
-000010b0: 652b 3031 2035 2e39 3030 3030 3030 3065  e+01 5.90000000e
-000010c0: 2b30 3120 5a22 202f 3e0d 0a20 2020 2020  +01 Z" />..     
-000010d0: 203c 7061 7468 2064 3d22 4d20 352e 3736   <path d="M 5.76
-000010e0: 3239 3833 3130 652b 3031 2036 2e35 3838  298310e+01 6.588
-000010f0: 3833 3033 3065 2b30 3120 5120 352e 3933  83030e+01 Q 5.93
-00001100: 3030 3335 3730 652b 3031 2036 2e39 3232  003570e+01 6.922
-00001110: 3731 3332 3065 2b30 312c 2036 2e30 3637  71320e+01, 6.067
+000000d0: 3730 652b 3031 204c 2037 2e32 3530 3030  70e+01 L 7.25000
+000000e0: 3030 3065 2b30 3120 352e 3030 3030 3030  000e+01 5.000000
+000000f0: 3030 652b 3030 204c 2035 2e30 3030 3030  00e+00 L 5.00000
+00000100: 3138 3065 2b30 3120 352e 3030 3030 3030  180e+01 5.000000
+00000110: 3030 652b 3030 2051 2035 2e33 3034 3539  00e+00 Q 5.30459
+00000120: 3832 3965 2b30 3120 372e 3730 3037 3037  829e+01 7.700707
+00000130: 3233 652b 3030 2c20 352e 3630 3737 3033  23e+00, 5.607703
+00000140: 3338 652b 3031 2031 2e30 3337 3230 3031  38e+01 1.0372001
+00000150: 3265 2b30 3120 5120 352e 3931 3030 3832  2e+01 Q 5.910082
+00000160: 3534 652b 3031 2031 2e33 3033 3731 3531  54e+01 1.3037151
+00000170: 3165 2b30 312c 2036 2e32 3231 3836 3433  1e+01, 6.2218643
+00000180: 3065 2b30 3120 312e 3537 3433 3035 3730  0e+01 1.57430570
+00000190: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
+000001a0: 2020 3c70 6174 6820 643d 224d 2039 2e35    <path d="M 9.5
+000001b0: 3030 3030 3030 3065 2b30 3120 352e 3030  0000000e+01 5.00
+000001c0: 3030 3030 3030 652b 3030 204c 2037 2e32  000000e+00 L 7.2
+000001d0: 3530 3030 3030 3065 2b30 3120 352e 3030  5000000e+01 5.00
+000001e0: 3030 3030 3030 652b 3030 204c 2038 2e32  000000e+00 L 8.2
+000001f0: 3939 3438 3436 3065 2b30 3120 312e 3730  9948460e+01 1.70
+00000200: 3037 3037 3130 652b 3031 204c 2039 2e35  070710e+01 L 9.5
+00000210: 3030 3030 3030 3065 2b30 3120 352e 3030  0000000e+01 5.00
+00000220: 3030 3030 3030 652b 3030 205a 2220 2f3e  000000e+00 Z" />
+00000230: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
+00000240: 224d 2038 2e32 3939 3438 3436 3065 2b30  "M 8.29948460e+0
+00000250: 3120 312e 3730 3037 3037 3130 652b 3031  1 1.70070710e+01
+00000260: 204c 2037 2e32 3530 3030 3030 3065 2b30   L 7.25000000e+0
+00000270: 3120 352e 3030 3030 3030 3030 652b 3030  1 5.00000000e+00
+00000280: 2051 2037 2e32 3531 3339 3639 3665 2b30   Q 7.25139696e+0
+00000290: 3120 382e 3635 3433 3838 3336 652b 3030  1 8.65438836e+00
+000002a0: 2c20 372e 3235 3336 3235 3238 652b 3031  , 7.25362528e+01
+000002b0: 2031 2e32 3238 3838 3630 3365 2b30 3120   1.22888603e+01 
+000002c0: 5120 372e 3235 3538 3239 3539 652b 3031  Q 7.25582959e+01
+000002d0: 2031 2e35 3931 3732 3436 3165 2b30 312c   1.59172461e+01,
+000002e0: 2037 2e32 3630 3131 3333 3065 2b30 3120   7.26011330e+01 
+000002f0: 312e 3937 3030 3534 3630 652b 3031 204c  1.97005460e+01 L
+00000300: 2038 2e32 3939 3438 3436 3065 2b30 3120   8.29948460e+01 
+00000310: 312e 3730 3037 3037 3130 652b 3031 205a  1.70070710e+01 Z
+00000320: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+00000330: 6820 643d 224d 2037 2e32 3530 3030 3030  h d="M 7.2500000
+00000340: 3065 2b30 3120 352e 3030 3030 3030 3030  0e+01 5.00000000
+00000350: 652b 3030 204c 2036 2e32 3231 3836 3433  e+00 L 6.2218643
+00000360: 3065 2b30 3120 312e 3537 3433 3035 3730  0e+01 1.57430570
+00000370: 652b 3031 2051 2036 2e34 3737 3639 3133  e+01 Q 6.4776913
+00000380: 3965 2b30 3120 312e 3636 3933 3133 3939  9e+01 1.66931399
+00000390: 652b 3031 2c20 362e 3733 3739 3938 3533  e+01, 6.73799853
+000003a0: 652b 3031 2031 2e37 3639 3037 3037 3865  e+01 1.76907078e
+000003b0: 2b30 3120 5120 362e 3939 3933 3933 3134  +01 Q 6.99939314
+000003c0: 652b 3031 2031 2e38 3639 3236 3131 3165  e+01 1.86926111e
+000003d0: 2b30 312c 2037 2e32 3630 3131 3333 3065  +01, 7.26011330e
+000003e0: 2b30 3120 312e 3937 3030 3534 3630 652b  +01 1.97005460e+
+000003f0: 3031 2051 2037 2e32 3535 3832 3935 3965  01 Q 7.25582959e
+00000400: 2b30 3120 312e 3539 3137 3234 3631 652b  +01 1.59172461e+
+00000410: 3031 2c20 372e 3235 3336 3235 3238 652b  01, 7.25362528e+
+00000420: 3031 2031 2e32 3238 3838 3630 3365 2b30  01 1.22888603e+0
+00000430: 3120 5120 372e 3235 3133 3936 3936 652b  1 Q 7.25139696e+
+00000440: 3031 2038 2e36 3534 3338 3833 3665 2b30  01 8.65438836e+0
+00000450: 302c 2037 2e32 3530 3030 3030 3065 2b30  0, 7.25000000e+0
+00000460: 3120 352e 3030 3030 3030 3030 652b 3030  1 5.00000000e+00
+00000470: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00000480: 6174 6820 643d 224d 2035 2e30 3030 3030  ath d="M 5.00000
+00000490: 3138 3065 2b30 3120 352e 3030 3030 3030  180e+01 5.000000
+000004a0: 3030 652b 3030 204c 2032 2e37 3530 3030  00e+00 L 2.75000
+000004b0: 3039 3065 2b30 3120 352e 3030 3030 3030  090e+01 5.000000
+000004c0: 3030 652b 3030 204c 2033 2e39 3131 3039  00e+00 L 3.91109
+000004d0: 3138 3065 2b30 3120 312e 3436 3635 3138  180e+01 1.466518
+000004e0: 3130 652b 3031 204c 2035 2e30 3030 3030  10e+01 L 5.00000
+000004f0: 3138 3065 2b30 3120 352e 3030 3030 3030  180e+01 5.000000
+00000500: 3030 652b 3030 205a 2220 2f3e 0d0a 2020  00e+00 Z" />..  
+00000510: 2020 2020 3c70 6174 6820 643d 224d 2035      <path d="M 5
+00000520: 2e30 3030 3030 3138 3065 2b30 3120 352e  .00000180e+01 5.
+00000530: 3030 3030 3030 3030 652b 3030 204c 2033  00000000e+00 L 3
+00000540: 2e39 3131 3039 3138 3065 2b30 3120 312e  .91109180e+01 1.
+00000550: 3436 3635 3138 3130 652b 3031 204c 2034  46651810e+01 L 4
+00000560: 2e36 3438 3338 3335 3065 2b30 3120 312e  .64838350e+01 1.
+00000570: 3636 3137 3337 3130 652b 3031 204c 2035  66173710e+01 L 5
+00000580: 2e30 3030 3030 3138 3065 2b30 3120 352e  .00000180e+01 5.
+00000590: 3030 3030 3030 3030 652b 3030 205a 2220  00000000e+00 Z" 
+000005a0: 2f3e 0d0a 2020 2020 2020 3c70 6174 6820  />..      <path 
+000005b0: 643d 224d 2035 2e30 3030 3030 3138 3065  d="M 5.00000180e
+000005c0: 2b30 3120 352e 3030 3030 3030 3030 652b  +01 5.00000000e+
+000005d0: 3030 204c 2034 2e36 3438 3338 3335 3065  00 L 4.64838350e
+000005e0: 2b30 3120 312e 3636 3137 3337 3130 652b  +01 1.66173710e+
+000005f0: 3031 204c 2035 2e33 3231 3432 3333 3065  01 L 5.32142330e
+00000600: 2b30 3120 312e 3730 3535 3737 3030 652b  +01 1.70557700e+
+00000610: 3031 204c 2035 2e30 3030 3030 3138 3065  01 L 5.00000180e
+00000620: 2b30 3120 352e 3030 3030 3030 3030 652b  +01 5.00000000e+
+00000630: 3030 205a 2220 2f3e 0d0a 2020 2020 2020  00 Z" />..      
+00000640: 3c70 6174 6820 643d 224d 2035 2e30 3030  <path d="M 5.000
+00000650: 3030 3138 3065 2b30 3120 352e 3030 3030  00180e+01 5.0000
+00000660: 3030 3030 652b 3030 204c 2035 2e33 3231  0000e+00 L 5.321
+00000670: 3432 3333 3065 2b30 3120 312e 3730 3535  42330e+01 1.7055
+00000680: 3737 3030 652b 3031 2051 2035 2e35 3434  7700e+01 Q 5.544
+00000690: 3832 3039 3265 2b30 3120 312e 3637 3336  82092e+01 1.6736
+000006a0: 3436 3031 652b 3031 2c20 352e 3736 3931  4601e+01, 5.7691
+000006b0: 3235 3430 652b 3031 2031 2e36 3430 3133  2540e+01 1.64013
+000006c0: 3634 3865 2b30 3120 5120 352e 3939 3337  648e+01 Q 5.9937
+000006d0: 3635 3635 652b 3031 2031 2e36 3036 3536  6565e+01 1.60656
+000006e0: 3835 3565 2b30 312c 2036 2e32 3231 3836  855e+01, 6.22186
+000006f0: 3433 3065 2b30 3120 312e 3537 3433 3035  430e+01 1.574305
+00000700: 3730 652b 3031 2051 2035 2e39 3130 3038  70e+01 Q 5.91008
+00000710: 3235 3465 2b30 3120 312e 3330 3337 3135  254e+01 1.303715
+00000720: 3131 652b 3031 2c20 352e 3630 3737 3033  11e+01, 5.607703
+00000730: 3338 652b 3031 2031 2e30 3337 3230 3031  38e+01 1.0372001
+00000740: 3265 2b30 3120 5120 352e 3330 3435 3938  2e+01 Q 5.304598
+00000750: 3239 652b 3031 2037 2e37 3030 3730 3732  29e+01 7.7007072
+00000760: 3365 2b30 302c 2035 2e30 3030 3030 3138  3e+00, 5.0000018
+00000770: 3065 2b30 3120 352e 3030 3030 3030 3030  0e+01 5.00000000
+00000780: 652b 3030 205a 2220 2f3e 0d0a 2020 2020  e+00 Z" />..    
+00000790: 2020 3c70 6174 6820 643d 224d 2032 2e37    <path d="M 2.7
+000007a0: 3530 3030 3039 3065 2b30 3120 352e 3030  5000090e+01 5.00
+000007b0: 3030 3030 3030 652b 3030 204c 2035 2e30  000000e+00 L 5.0
+000007c0: 3030 3030 3030 3065 2b30 3020 352e 3030  0000000e+00 5.00
+000007d0: 3030 3030 3030 652b 3030 204c 2032 2e33  000000e+00 L 2.3
+000007e0: 3030 3030 3030 3065 2b30 3120 322e 3330  0000000e+01 2.30
+000007f0: 3030 3030 3030 652b 3031 204c 2032 2e37  000000e+01 L 2.7
+00000800: 3530 3030 3039 3065 2b30 3120 352e 3030  5000090e+01 5.00
+00000810: 3030 3030 3030 652b 3030 205a 2220 2f3e  000000e+00 Z" />
+00000820: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
+00000830: 224d 2032 2e33 3030 3030 3030 3065 2b30  "M 2.30000000e+0
+00000840: 3120 322e 3330 3030 3030 3030 652b 3031  1 2.30000000e+01
+00000850: 204c 2033 2e32 3030 3030 3030 3065 2b30   L 3.20000000e+0
+00000860: 3120 322e 3330 3030 3030 3030 652b 3031  1 2.30000000e+01
+00000870: 204c 2032 2e37 3530 3030 3039 3065 2b30   L 2.75000090e+0
+00000880: 3120 352e 3030 3030 3030 3030 652b 3030  1 5.00000000e+00
+00000890: 204c 2032 2e33 3030 3030 3030 3065 2b30   L 2.30000000e+0
+000008a0: 3120 322e 3330 3030 3030 3030 652b 3031  1 2.30000000e+01
+000008b0: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+000008c0: 6174 6820 643d 224d 2033 2e32 3030 3030  ath d="M 3.20000
+000008d0: 3030 3065 2b30 3120 322e 3330 3030 3030  000e+01 2.300000
+000008e0: 3030 652b 3031 204c 2033 2e39 3131 3039  00e+01 L 3.91109
+000008f0: 3138 3065 2b30 3120 312e 3436 3635 3138  180e+01 1.466518
+00000900: 3130 652b 3031 204c 2032 2e37 3530 3030  10e+01 L 2.75000
+00000910: 3039 3065 2b30 3120 352e 3030 3030 3030  090e+01 5.000000
+00000920: 3030 652b 3030 204c 2033 2e32 3030 3030  00e+00 L 3.20000
+00000930: 3030 3065 2b30 3120 322e 3330 3030 3030  000e+01 2.300000
+00000940: 3030 652b 3031 205a 2220 2f3e 0d0a 2020  00e+01 Z" />..  
+00000950: 2020 2020 3c70 6174 6820 643d 224d 2035      <path d="M 5
+00000960: 2e33 3732 3739 3137 3065 2b30 3120 372e  .37279170e+01 7.
+00000970: 3137 3237 3932 3630 652b 3031 2051 2035  17279260e+01 Q 5
+00000980: 2e32 3435 3439 3732 3565 2b30 3120 372e  .24549725e+01 7.
+00000990: 3239 3939 3032 3438 652b 3031 2c20 352e  29990248e+01, 5.
+000009a0: 3039 3731 3634 3439 652b 3031 2037 2e33  09716449e+01 7.3
+000009b0: 3938 3535 3334 3465 2b30 3120 5120 342e  9855344e+01 Q 4.
+000009c0: 3934 3837 3538 3339 652b 3031 2037 2e34  94875839e+01 7.4
+000009d0: 3936 3936 3034 3965 2b30 312c 2034 2e37  9696049e+01, 4.7
+000009e0: 3838 3833 3033 3065 2b30 3120 372e 3536  8883030e+01 7.56
+000009f0: 3239 3833 3130 652b 3031 2051 2035 2e30  298310e+01 Q 5.0
+00000a00: 3330 3231 3830 3665 2b30 3120 372e 3732  3021806e+01 7.72
+00000a10: 3735 3136 3331 652b 3031 2c20 352e 3235  751631e+01, 5.25
+00000a20: 3938 3238 3037 652b 3031 2037 2e38 3631  982807e+01 7.861
+00000a30: 3432 3339 3965 2b30 3120 5120 352e 3438  42399e+01 Q 5.48
+00000a40: 3837 3237 3332 652b 3031 2037 2e39 3935  872732e+01 7.995
+00000a50: 3134 3335 3265 2b30 312c 2035 2e37 3130  14352e+01, 5.710
+00000a60: 3734 3938 3065 2b30 3120 382e 3133 3036  74980e+01 8.1306
+00000a70: 3838 3730 652b 3031 2051 2035 2e36 3330  8870e+01 Q 5.630
+00000a80: 3530 3639 3565 2b30 3120 372e 3930 3134  50695e+01 7.9014
+00000a90: 3838 3339 652b 3031 2c20 352e 3535 3139  8839e+01, 5.5519
+00000aa0: 3233 3830 652b 3031 2037 2e36 3637 3839  2380e+01 7.66789
+00000ab0: 3533 3165 2b30 3120 5120 352e 3437 3430  531e+01 Q 5.4740
+00000ac0: 3237 3934 652b 3031 2037 2e34 3335 3538  2794e+01 7.43558
+00000ad0: 3535 3765 2b30 312c 2035 2e33 3732 3739  557e+01, 5.37279
+00000ae0: 3137 3065 2b30 3120 372e 3137 3237 3932  170e+01 7.172792
+00000af0: 3630 652b 3031 205a 2220 2f3e 0d0a 2020  60e+01 Z" />..  
+00000b00: 2020 2020 3c70 6174 6820 643d 224d 2034      <path d="M 4
+00000b10: 2e37 3838 3833 3033 3065 2b30 3120 372e  .78883030e+01 7.
+00000b20: 3536 3239 3833 3130 652b 3031 2051 2034  56298310e+01 Q 4
+00000b30: 2e36 3135 3633 3331 3165 2b30 3120 372e  .61563311e+01 7.
+00000b40: 3633 3431 3631 3635 652b 3031 2c20 342e  63416165e+01, 4.
+00000b50: 3434 3037 3636 3630 652b 3031 2037 2e36  44076660e+01 7.6
+00000b60: 3637 3434 3934 3365 2b30 3120 5120 342e  6744943e+01 Q 4.
+00000b70: 3236 3630 3833 3437 652b 3031 2037 2e37  26608347e+01 7.7
+00000b80: 3030 3531 3730 3765 2b30 312c 2034 2e31  0051707e+01, 4.1
+00000b90: 3030 3030 3030 3065 2b30 3120 372e 3730  0000000e+01 7.70
+00000ba0: 3030 3030 3030 652b 3031 2051 2034 2e32  000000e+01 Q 4.2
+00000bb0: 3330 3630 3132 3765 2b30 3120 372e 3835  3060127e+01 7.85
+00000bc0: 3137 3733 3238 652b 3031 2c20 342e 3337  177328e+01, 4.37
+00000bd0: 3830 3431 3931 652b 3031 2037 2e39 3838  804191e+01 7.988
+00000be0: 3133 3939 3565 2b30 3120 5120 342e 3532  13995e+01 Q 4.52
+00000bf0: 3331 3835 3935 652b 3031 2038 2e31 3231  318595e+01 8.121
+00000c00: 3830 3131 3365 2b30 312c 2034 2e36 3539  80113e+01, 4.659
+00000c10: 3831 3236 3065 2b30 3120 382e 3235 3330  81260e+01 8.2530
+00000c20: 3434 3630 652b 3031 2051 2034 2e36 3933  4460e+01 Q 4.693
+00000c30: 3231 3236 3065 2b30 3120 382e 3038 3839  21260e+01 8.0889
+00000c40: 3538 3033 652b 3031 2c20 342e 3732 3736  5803e+01, 4.7276
+00000c50: 3737 3339 652b 3031 2037 2e39 3230 3637  7739e+01 7.92067
+00000c60: 3034 3465 2b30 3120 5120 342e 3736 3231  044e+01 Q 4.7621
+00000c70: 3132 3238 652b 3031 2037 2e37 3533 3239  1228e+01 7.75329
+00000c80: 3330 3365 2b30 312c 2034 2e37 3838 3833  303e+01, 4.78883
+00000c90: 3033 3065 2b30 3120 372e 3536 3239 3833  030e+01 7.562983
+00000ca0: 3130 652b 3031 205a 2220 2f3e 0d0a 2020  10e+01 Z" />..  
+00000cb0: 2020 2020 3c70 6174 6820 643d 224d 2035      <path d="M 5
+00000cc0: 2e37 3130 3734 3938 3065 2b30 3120 382e  .71074980e+01 8.
+00000cd0: 3133 3036 3838 3730 652b 3031 2051 2035  13068870e+01 Q 5
+00000ce0: 2e34 3838 3732 3733 3265 2b30 3120 372e  .48872732e+01 7.
+00000cf0: 3939 3531 3433 3532 652b 3031 2c20 352e  99514352e+01, 5.
+00000d00: 3235 3938 3238 3037 652b 3031 2037 2e38  25982807e+01 7.8
+00000d10: 3631 3432 3339 3965 2b30 3120 5120 352e  6142399e+01 Q 5.
+00000d20: 3033 3032 3138 3036 652b 3031 2037 2e37  03021806e+01 7.7
+00000d30: 3237 3531 3633 3165 2b30 312c 2034 2e37  2751631e+01, 4.7
+00000d40: 3838 3833 3033 3065 2b30 3120 372e 3536  8883030e+01 7.56
+00000d50: 3239 3833 3130 652b 3031 2051 2034 2e37  298310e+01 Q 4.7
+00000d60: 3632 3131 3232 3865 2b30 3120 372e 3735  6211228e+01 7.75
+00000d70: 3332 3933 3033 652b 3031 2c20 342e 3732  329303e+01, 4.72
+00000d80: 3736 3737 3339 652b 3031 2037 2e39 3230  767739e+01 7.920
+00000d90: 3637 3034 3465 2b30 3120 5120 342e 3639  67044e+01 Q 4.69
+00000da0: 3332 3132 3630 652b 3031 2038 2e30 3838  321260e+01 8.088
+00000db0: 3935 3830 3365 2b30 312c 2034 2e36 3539  95803e+01, 4.659
+00000dc0: 3831 3236 3065 2b30 3120 382e 3235 3330  81260e+01 8.2530
+00000dd0: 3434 3630 652b 3031 2051 2034 2e39 3231  4460e+01 Q 4.921
+00000de0: 3036 3639 3665 2b30 3120 382e 3232 3233  06696e+01 8.2223
+00000df0: 3538 3833 652b 3031 2c20 352e 3138 3539  5883e+01, 5.1859
+00000e00: 3232 3435 652b 3031 2038 2e31 3931 3937  2245e+01 8.19197
+00000e10: 3930 3965 2b30 3120 5120 352e 3435 3037  909e+01 Q 5.4507
+00000e20: 3938 3436 652b 3031 2038 2e31 3631 3539  9846e+01 8.16159
+00000e30: 3635 3565 2b30 312c 2035 2e37 3130 3734  655e+01, 5.71074
+00000e40: 3938 3065 2b30 3120 382e 3133 3036 3838  980e+01 8.130688
+00000e50: 3730 652b 3031 205a 2220 2f3e 0d0a 2020  70e+01 Z" />..  
+00000e60: 2020 2020 3c70 6174 6820 643d 224d 2035      <path d="M 5
+00000e70: 2e37 3632 3938 3331 3065 2b30 3120 362e  .76298310e+01 6.
+00000e80: 3538 3838 3330 3330 652b 3031 2051 2035  58883030e+01 Q 5
+00000e90: 2e36 3936 3936 3035 3265 2b30 3120 362e  .69696052e+01 6.
+00000ea0: 3734 3837 3538 3336 652b 3031 2c20 352e  74875836e+01, 5.
+00000eb0: 3539 3835 3533 3332 652b 3031 2036 2e38  59855332e+01 6.8
+00000ec0: 3937 3136 3436 3065 2b30 3120 5120 352e  9716460e+01 Q 5.
+00000ed0: 3439 3939 3032 3233 652b 3031 2037 2e30  49990223e+01 7.0
+00000ee0: 3435 3439 3735 3065 2b30 312c 2035 2e33  4549750e+01, 5.3
+00000ef0: 3732 3739 3137 3065 2b30 3120 372e 3137  7279170e+01 7.17
+00000f00: 3237 3932 3630 652b 3031 2051 2035 2e35  279260e+01 Q 5.5
+00000f10: 3631 3337 3930 3165 2b30 3120 372e 3230  6137901e+01 7.20
+00000f20: 3335 3633 3830 652b 3031 2c20 352e 3733  356380e+01, 5.73
+00000f30: 3139 3538 3533 652b 3031 2037 2e32 3136  195853e+01 7.216
+00000f40: 3337 3534 3665 2b30 3120 5120 352e 3930  37546e+01 Q 5.90
+00000f50: 3237 3230 3538 652b 3031 2037 2e32 3239  272058e+01 7.229
+00000f60: 3339 3234 3265 2b30 312c 2036 2e30 3637  39242e+01, 6.067
+00000f70: 3837 3631 3065 2b30 3120 372e 3234 3236  87610e+01 7.2426
+00000f80: 3636 3830 652b 3031 2051 2035 2e39 3937  6680e+01 Q 5.997
+00000f90: 3836 3736 3165 2b30 3120 372e 3038 3636  86761e+01 7.0866
+00000fa0: 3331 3730 652b 3031 2c20 352e 3932 3733  3170e+01, 5.9273
+00000fb0: 3437 3930 652b 3031 2036 2e39 3233 3231  4790e+01 6.92321
+00000fc0: 3239 3165 2b30 3120 5120 352e 3835 3636  291e+01 Q 5.8566
+00000fd0: 3734 3934 652b 3031 2036 2e37 3539 3238  7494e+01 6.75928
+00000fe0: 3539 3865 2b30 312c 2035 2e37 3632 3938  598e+01, 5.76298
+00000ff0: 3331 3065 2b30 3120 362e 3538 3838 3330  310e+01 6.588830
+00001000: 3330 652b 3031 205a 2220 2f3e 0d0a 2020  30e+01 Z" />..  
+00001010: 2020 2020 3c70 6174 6820 643d 224d 2035      <path d="M 5
+00001020: 2e33 3732 3739 3137 3065 2b30 3120 372e  .37279170e+01 7.
+00001030: 3137 3237 3932 3630 652b 3031 2051 2035  17279260e+01 Q 5
+00001040: 2e34 3734 3032 3739 3465 2b30 3120 372e  .47402794e+01 7.
+00001050: 3433 3535 3835 3537 652b 3031 2c20 352e  43558557e+01, 5.
+00001060: 3535 3139 3233 3830 652b 3031 2037 2e36  55192380e+01 7.6
+00001070: 3637 3839 3533 3165 2b30 3120 5120 352e  6789531e+01 Q 5.
+00001080: 3633 3035 3036 3935 652b 3031 2037 2e39  63050695e+01 7.9
+00001090: 3031 3438 3833 3965 2b30 312c 2035 2e37  0148839e+01, 5.7
+000010a0: 3130 3734 3938 3065 2b30 3120 382e 3133  1074980e+01 8.13
+000010b0: 3036 3838 3730 652b 3031 2051 2035 2e37  068870e+01 Q 5.7
+000010c0: 3938 3934 3031 3765 2b30 3120 372e 3931  9894017e+01 7.91
+000010d0: 3232 3632 3338 652b 3031 2c20 352e 3838  226238e+01, 5.88
+000010e0: 3830 3032 3637 652b 3031 2037 2e36 3839  800267e+01 7.689
+000010f0: 3436 3637 3865 2b30 3120 5120 352e 3937  46678e+01 Q 5.97
+00001100: 3732 3138 3538 652b 3031 2037 2e34 3636  721858e+01 7.466
+00001110: 3237 3130 3465 2b30 312c 2036 2e30 3637  27104e+01, 6.067
 00001120: 3837 3631 3065 2b30 3120 372e 3234 3236  87610e+01 7.2426
-00001130: 3636 3830 652b 3031 2051 2036 2e33 3334  6680e+01 Q 6.334
-00001140: 3536 3539 3065 2b30 3120 362e 3932 3235  56590e+01 6.9225
-00001150: 3631 3535 652b 3031 2c20 362e 3630 3039  6155e+01, 6.6009
-00001160: 3837 3530 652b 3031 2036 2e36 3033 3831  8750e+01 6.60381
-00001170: 3632 3065 2b30 3120 5120 362e 3139 3335  620e+01 Q 6.1935
-00001180: 3436 3730 652b 3031 2036 2e36 3035 3233  4670e+01 6.60523
-00001190: 3539 3565 2b30 312c 2035 2e37 3632 3938  595e+01, 5.76298
-000011a0: 3331 3065 2b30 3120 362e 3538 3838 3330  310e+01 6.588830
-000011b0: 3330 652b 3031 205a 2220 2f3e 0d0a 2020  30e+01 Z" />..  
-000011c0: 2020 2020 3c70 6174 6820 643d 224d 2039      <path d="M 9
-000011d0: 2e35 3030 3030 3030 3065 2b30 3120 372e  .50000000e+01 7.
-000011e0: 3235 3030 3030 3030 652b 3031 2051 2039  25000000e+01 Q 9
-000011f0: 2e35 3030 3030 3030 3065 2b30 3120 362e  .50000000e+01 6.
-00001200: 3132 3530 3030 3930 652b 3031 2c20 392e  12500090e+01, 9.
-00001210: 3530 3030 3030 3030 652b 3031 2035 2e30  50000000e+01 5.0
-00001220: 3030 3030 3138 3065 2b30 3120 5120 382e  0000180e+01 Q 8.
-00001230: 3831 3630 3936 3735 652b 3031 2035 2e33  81609675e+01 5.3
-00001240: 3535 3735 3338 3065 2b30 312c 2038 2e31  5575380e+01, 8.1
-00001250: 3239 3738 3639 3065 2b30 3120 352e 3731  2978690e+01 5.71
-00001260: 3136 3634 3230 652b 3031 2051 2038 2e38  166420e+01 Q 8.8
-00001270: 3132 3430 3835 3565 2b30 3120 362e 3437  1240855e+01 6.47
-00001280: 3936 3837 3330 652b 3031 2c20 392e 3530  968730e+01, 9.50
-00001290: 3030 3030 3030 652b 3031 2037 2e32 3530  000000e+01 7.250
-000012a0: 3030 3030 3065 2b30 3120 5a22 202f 3e0d  00000e+01 Z" />.
-000012b0: 0a20 2020 2020 203c 7061 7468 2064 3d22  .      <path d="
-000012c0: 4d20 392e 3530 3030 3030 3030 652b 3031  M 9.50000000e+01
-000012d0: 2039 2e35 3030 3030 3030 3065 2b30 3120   9.50000000e+01 
-000012e0: 5120 392e 3530 3030 3030 3030 652b 3031  Q 9.50000000e+01
-000012f0: 2038 2e33 3734 3939 3938 3765 2b30 312c   8.37499987e+01,
-00001300: 2039 2e35 3030 3030 3030 3065 2b30 3120   9.50000000e+01 
-00001310: 372e 3235 3030 3030 3030 652b 3031 2051  7.25000000e+01 Q
-00001320: 2038 2e38 3436 3531 3633 3065 2b30 3120   8.84651630e+01 
-00001330: 372e 3732 3233 3739 3430 652b 3031 2c20  7.72237940e+01, 
-00001340: 382e 3139 3330 3333 3530 652b 3031 2038  8.19303350e+01 8
-00001350: 2e31 3934 3735 3838 3065 2b30 3120 5120  .19475880e+01 Q 
-00001360: 382e 3834 3635 3136 3330 652b 3031 2038  8.84651630e+01 8
-00001370: 2e38 3437 3337 3933 3165 2b30 312c 2039  .84737931e+01, 9
-00001380: 2e35 3030 3030 3030 3065 2b30 3120 392e  .50000000e+01 9.
-00001390: 3530 3030 3030 3030 652b 3031 205a 2220  50000000e+01 Z" 
-000013a0: 2f3e 0d0a 2020 2020 2020 3c70 6174 6820  />..      <path 
-000013b0: 643d 224d 2038 2e31 3933 3033 3335 3065  d="M 8.19303350e
-000013c0: 2b30 3120 382e 3139 3437 3538 3830 652b  +01 8.19475880e+
-000013d0: 3031 2051 2038 2e38 3436 3531 3633 3065  01 Q 8.84651630e
-000013e0: 2b30 3120 372e 3732 3233 3739 3430 652b  +01 7.72237940e+
-000013f0: 3031 2c20 392e 3530 3030 3030 3030 652b  01, 9.50000000e+
-00001400: 3031 2037 2e32 3530 3030 3030 3065 2b30  01 7.25000000e+0
-00001410: 3120 5120 382e 3632 3637 3338 3130 652b  1 Q 8.62673810e+
-00001420: 3031 2037 2e30 3836 3832 3436 3065 2b30  01 7.08682460e+0
-00001430: 312c 2037 2e37 3533 3437 3632 3065 2b30  1, 7.75347620e+0
-00001440: 3120 362e 3932 3336 3439 3230 652b 3031  1 6.92364920e+01
-00001450: 2051 2037 2e39 3733 3235 3438 3565 2b30   Q 7.97325485e+0
-00001460: 3120 372e 3535 3932 3034 3435 652b 3031  1 7.55920445e+01
-00001470: 2c20 382e 3139 3330 3333 3530 652b 3031  , 8.19303350e+01
-00001480: 2038 2e31 3934 3735 3838 3065 2b30 3120   8.19475880e+01 
-00001490: 5a22 202f 3e0d 0a20 2020 2020 203c 7061  Z" />..      <pa
-000014a0: 7468 2064 3d22 4d20 392e 3530 3030 3030  th d="M 9.500000
-000014b0: 3030 652b 3031 2037 2e32 3530 3030 3030  00e+01 7.2500000
-000014c0: 3065 2b30 3120 5120 382e 3831 3234 3038  0e+01 Q 8.812408
-000014d0: 3535 652b 3031 2036 2e34 3739 3638 3733  55e+01 6.4796873
-000014e0: 3065 2b30 312c 2038 2e31 3239 3738 3639  0e+01, 8.1297869
-000014f0: 3065 2b30 3120 352e 3731 3136 3634 3230  0e+01 5.71166420
-00001500: 652b 3031 2051 2037 2e39 3434 3036 3734  e+01 Q 7.9440674
-00001510: 3065 2b30 3120 362e 3331 3937 3134 3130  0e+01 6.31971410
-00001520: 652b 3031 2c20 372e 3735 3334 3736 3230  e+01, 7.75347620
-00001530: 652b 3031 2036 2e39 3233 3634 3932 3065  e+01 6.92364920e
-00001540: 2b30 3120 5120 382e 3632 3637 3338 3130  +01 Q 8.62673810
-00001550: 652b 3031 2037 2e30 3836 3832 3436 3065  e+01 7.08682460e
-00001560: 2b30 312c 2039 2e35 3030 3030 3030 3065  +01, 9.50000000e
-00001570: 2b30 3120 372e 3235 3030 3030 3030 652b  +01 7.25000000e+
-00001580: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
-00001590: 3c70 6174 6820 643d 224d 2039 2e35 3030  <path d="M 9.500
-000015a0: 3030 3030 3065 2b30 3120 352e 3030 3030  00000e+01 5.0000
-000015b0: 3031 3830 652b 3031 2051 2039 2e35 3030  0180e+01 Q 9.500
-000015c0: 3030 3030 3065 2b30 3120 332e 3837 3530  00000e+01 3.8750
-000015d0: 3031 3830 652b 3031 2c20 392e 3530 3030  0180e+01, 9.5000
-000015e0: 3030 3030 652b 3031 2032 2e37 3530 3030  0000e+01 2.75000
-000015f0: 3039 3065 2b30 3120 5120 382e 3935 3537  090e+01 Q 8.9557
-00001600: 3038 3830 652b 3031 2033 2e32 3538 3438  0880e+01 3.25848
-00001610: 3536 3065 2b30 312c 2038 2e34 3134 3730  560e+01, 8.41470
-00001620: 3938 3065 2b30 3120 332e 3736 3833 3136  980e+01 3.768316
-00001630: 3730 652b 3031 2051 2038 2e39 3537 3032  70e+01 Q 8.95702
-00001640: 3031 3065 2b30 3120 342e 3338 3538 3232  010e+01 4.385822
-00001650: 3930 652b 3031 2c20 392e 3530 3030 3030  90e+01, 9.500000
-00001660: 3030 652b 3031 2035 2e30 3030 3030 3138  00e+01 5.0000018
-00001670: 3065 2b30 3120 5a22 202f 3e0d 0a20 2020  0e+01 Z" />..   
-00001680: 2020 203c 7061 7468 2064 3d22 4d20 392e     <path d="M 9.
-00001690: 3530 3030 3030 3030 652b 3031 2035 2e30  50000000e+01 5.0
-000016a0: 3030 3030 3138 3065 2b30 3120 5120 382e  0000180e+01 Q 8.
-000016b0: 3935 3730 3230 3130 652b 3031 2034 2e33  95702010e+01 4.3
-000016c0: 3835 3832 3239 3065 2b30 312c 2038 2e34  8582290e+01, 8.4
-000016d0: 3134 3730 3938 3065 2b30 3120 332e 3736  1470980e+01 3.76
-000016e0: 3833 3136 3730 652b 3031 2051 2038 2e33  831670e+01 Q 8.3
-000016f0: 3334 3634 3632 3565 2b30 3120 342e 3231  3464625e+01 4.21
-00001700: 3430 3130 3635 652b 3031 2c20 382e 3235  401065e+01, 8.25
-00001710: 3239 3139 3530 652b 3031 2034 2e36 3539  291950e+01 4.659
-00001720: 3938 3534 3065 2b30 3120 5120 382e 3837  98540e+01 Q 8.87
-00001730: 3532 3739 3430 652b 3031 2034 2e38 3330  527940e+01 4.830
-00001740: 3334 3031 3065 2b30 312c 2039 2e35 3030  34010e+01, 9.500
-00001750: 3030 3030 3065 2b30 3120 352e 3030 3030  00000e+01 5.0000
-00001760: 3031 3830 652b 3031 205a 2220 2f3e 0d0a  0180e+01 Z" />..
-00001770: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
-00001780: 2038 2e31 3239 3738 3639 3065 2b30 3120   8.12978690e+01 
-00001790: 352e 3731 3136 3634 3230 652b 3031 2051  5.71166420e+01 Q
-000017a0: 2038 2e38 3136 3039 3637 3565 2b30 3120   8.81609675e+01 
-000017b0: 352e 3335 3537 3533 3830 652b 3031 2c20  5.35575380e+01, 
-000017c0: 392e 3530 3030 3030 3030 652b 3031 2035  9.50000000e+01 5
-000017d0: 2e30 3030 3030 3138 3065 2b30 3120 5120  .00000180e+01 Q 
-000017e0: 382e 3837 3532 3739 3430 652b 3031 2034  8.87527940e+01 4
-000017f0: 2e38 3330 3334 3031 3065 2b30 312c 2038  .83034010e+01, 8
-00001800: 2e32 3532 3931 3935 3065 2b30 3120 342e  .25291950e+01 4.
-00001810: 3635 3939 3835 3430 652b 3031 2051 2038  65998540e+01 Q 8
-00001820: 2e31 3931 3436 3334 3565 2b30 3120 352e  .19146345e+01 5.
-00001830: 3138 3730 3331 3730 652b 3031 2c20 382e  18703170e+01, 8.
-00001840: 3132 3937 3836 3930 652b 3031 2035 2e37  12978690e+01 5.7
-00001850: 3131 3636 3432 3065 2b30 3120 5a22 202f  1166420e+01 Z" /
-00001860: 3e0d 0a20 2020 2020 203c 7061 7468 2064  >..      <path d
-00001870: 3d22 4d20 392e 3530 3030 3030 3030 652b  ="M 9.50000000e+
-00001880: 3031 2032 2e37 3530 3030 3039 3065 2b30  01 2.75000090e+0
-00001890: 3120 5120 392e 3530 3030 3030 3030 652b  1 Q 9.50000000e+
-000018a0: 3031 2031 2e36 3235 3030 3034 3565 2b30  01 1.62500045e+0
-000018b0: 312c 2039 2e35 3030 3030 3030 3065 2b30  1, 9.50000000e+0
-000018c0: 3120 352e 3030 3030 3030 3030 652b 3030  1 5.00000000e+00
-000018d0: 2051 2038 2e38 3939 3734 3233 3065 2b30   Q 8.89974230e+0
-000018e0: 3120 312e 3130 3033 3533 3535 652b 3031  1 1.10035355e+01
-000018f0: 2c20 382e 3239 3934 3834 3630 652b 3031  , 8.29948460e+01
-00001900: 2031 2e37 3030 3730 3731 3065 2b30 3120   1.70070710e+01 
-00001910: 5120 382e 3839 3937 3432 3330 652b 3031  Q 8.89974230e+01
-00001920: 2032 2e32 3235 3335 3430 3065 2b30 312c   2.22535400e+01,
-00001930: 2039 2e35 3030 3030 3030 3065 2b30 3120   9.50000000e+01 
-00001940: 322e 3735 3030 3030 3930 652b 3031 205a  2.75000090e+01 Z
-00001950: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
-00001960: 6820 643d 224d 2039 2e35 3030 3030 3030  h d="M 9.5000000
-00001970: 3065 2b30 3120 322e 3735 3030 3030 3930  0e+01 2.75000090
-00001980: 652b 3031 2051 2038 2e38 3939 3734 3233  e+01 Q 8.8997423
-00001990: 3065 2b30 3120 322e 3232 3533 3534 3030  0e+01 2.22535400
-000019a0: 652b 3031 2c20 382e 3239 3934 3834 3630  e+01, 8.29948460
-000019b0: 652b 3031 2031 2e37 3030 3730 3731 3065  e+01 1.70070710e
-000019c0: 2b30 3120 5120 382e 3136 3330 3832 3835  +01 Q 8.16308285
-000019d0: 652b 3031 2032 2e32 3139 3039 3237 3065  e+01 2.21909270e
-000019e0: 2b30 312c 2038 2e30 3238 3034 3832 3065  +01, 8.02804820e
-000019f0: 2b30 3120 322e 3733 3837 3032 3330 652b  +01 2.73870230e+
-00001a00: 3031 2051 2038 2e37 3632 3939 3430 3565  01 Q 8.76299405e
-00001a10: 2b30 3120 322e 3734 3539 3534 3035 652b  +01 2.74595405e+
-00001a20: 3031 2c20 392e 3530 3030 3030 3030 652b  01, 9.50000000e+
-00001a30: 3031 2032 2e37 3530 3030 3039 3065 2b30  01 2.75000090e+0
-00001a40: 3120 5a22 202f 3e0d 0a20 2020 2020 203c  1 Z" />..      <
-00001a50: 7061 7468 2064 3d22 4d20 382e 3431 3437  path d="M 8.4147
-00001a60: 3039 3830 652b 3031 2033 2e37 3638 3331  0980e+01 3.76831
-00001a70: 3637 3065 2b30 3120 5120 382e 3935 3537  670e+01 Q 8.9557
-00001a80: 3038 3830 652b 3031 2033 2e32 3538 3438  0880e+01 3.25848
-00001a90: 3536 3065 2b30 312c 2039 2e35 3030 3030  560e+01, 9.50000
-00001aa0: 3030 3065 2b30 3120 322e 3735 3030 3030  000e+01 2.750000
-00001ab0: 3930 652b 3031 2051 2038 2e37 3632 3939  90e+01 Q 8.76299
-00001ac0: 3430 3565 2b30 3120 322e 3734 3539 3534  405e+01 2.745954
-00001ad0: 3035 652b 3031 2c20 382e 3032 3830 3438  05e+01, 8.028048
-00001ae0: 3230 652b 3031 2032 2e37 3338 3730 3233  20e+01 2.7387023
-00001af0: 3065 2b30 3120 5120 382e 3232 3236 3537  0e+01 Q 8.222657
-00001b00: 3435 652b 3031 2033 2e32 3533 3239 3933  45e+01 3.2532993
-00001b10: 3565 2b30 312c 2038 2e34 3134 3730 3938  5e+01, 8.4147098
-00001b20: 3065 2b30 3120 332e 3736 3833 3136 3730  0e+01 3.76831670
-00001b30: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
-00001b40: 2020 3c70 6174 6820 643d 224d 2032 2e38    <path d="M 2.8
-00001b50: 3237 3230 3734 3065 2b30 3120 372e 3137  2720740e+01 7.17
-00001b60: 3237 3931 3730 652b 3031 2051 2032 2e35  279170e+01 Q 2.5
-00001b70: 3932 3739 3838 3065 2b30 3120 362e 3930  9279880e+01 6.90
-00001b80: 3532 3436 3930 652b 3031 2c20 322e 3433  524690e+01, 2.43
-00001b90: 3730 3136 3930 652b 3031 2036 2e35 3838  701690e+01 6.588
-00001ba0: 3833 3033 3065 2b30 3120 5120 322e 3138  83030e+01 Q 2.18
-00001bb0: 3936 3030 3630 652b 3031 2036 2e39 3238  960060e+01 6.928
-00001bc0: 3830 3735 3565 2b30 312c 2031 2e39 3639  80755e+01, 1.969
-00001bd0: 3538 3132 3065 2b30 3120 372e 3235 3936  58120e+01 7.2596
-00001be0: 3335 3430 652b 3031 2051 2032 2e33 3837  3540e+01 Q 2.387
-00001bf0: 3334 3836 3065 2b30 3120 372e 3232 3731  34860e+01 7.2271
-00001c00: 3837 3235 652b 3031 2c20 322e 3832 3732  8725e+01, 2.8272
-00001c10: 3037 3430 652b 3031 2037 2e31 3732 3739  0740e+01 7.17279
-00001c20: 3137 3065 2b30 3120 5a22 202f 3e0d 0a20  170e+01 Z" />.. 
-00001c30: 2020 2020 203c 7061 7468 2064 3d22 4d20       <path d="M 
-00001c40: 322e 3433 3730 3136 3930 652b 3031 2036  2.43701690e+01 6
-00001c50: 2e35 3838 3833 3033 3065 2b30 3120 5120  .58883030e+01 Q 
-00001c60: 322e 3332 3232 3235 3935 652b 3031 2036  2.32222595e+01 6
-00001c70: 2e32 3438 3833 3539 3565 2b30 312c 2032  .24883595e+01, 2
-00001c80: 2e33 3030 3030 3030 3065 2b30 3120 352e  .30000000e+01 5.
-00001c90: 3930 3030 3030 3030 652b 3031 2051 2031  90000000e+01 Q 1
-00001ca0: 2e39 3236 3234 3731 3065 2b30 3120 362e  .92624710e+01 6.
-00001cb0: 3035 3935 3234 3535 652b 3031 2c20 312e  05952455e+01, 1.
-00001cc0: 3537 3431 3836 3930 652b 3031 2036 2e32  57418690e+01 6.2
-00001cd0: 3231 3734 3139 3065 2b30 3120 5120 312e  2174190e+01 Q 1.
-00001ce0: 3938 3932 3538 3335 652b 3031 2036 2e34  98925835e+01 6.4
-00001cf0: 3130 3538 3632 3065 2b30 312c 2032 2e34  1058620e+01, 2.4
-00001d00: 3337 3031 3639 3065 2b30 3120 362e 3538  3701690e+01 6.58
-00001d10: 3838 3330 3330 652b 3031 205a 2220 2f3e  883030e+01 Z" />
-00001d20: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
-00001d30: 224d 2031 2e39 3639 3538 3132 3065 2b30  "M 1.96958120e+0
-00001d40: 3120 372e 3235 3936 3335 3430 652b 3031  1 7.25963540e+01
-00001d50: 2051 2032 2e31 3839 3630 3036 3065 2b30   Q 2.18960060e+0
-00001d60: 3120 362e 3932 3838 3037 3535 652b 3031  1 6.92880755e+01
-00001d70: 2c20 322e 3433 3730 3136 3930 652b 3031  , 2.43701690e+01
-00001d80: 2036 2e35 3838 3833 3033 3065 2b30 3120   6.58883030e+01 
-00001d90: 5120 312e 3938 3932 3538 3335 652b 3031  Q 1.98925835e+01
-00001da0: 2036 2e34 3130 3538 3632 3065 2b30 312c   6.41058620e+01,
-00001db0: 2031 2e35 3734 3138 3639 3065 2b30 3120   1.57418690e+01 
-00001dc0: 362e 3232 3137 3431 3930 652b 3031 2051  6.22174190e+01 Q
-00001dd0: 2031 2e37 3639 3431 3736 3065 2b30 3120   1.76941760e+01 
-00001de0: 362e 3734 3130 3935 3435 652b 3031 2c20  6.74109545e+01, 
-00001df0: 312e 3936 3935 3831 3230 652b 3031 2037  1.96958120e+01 7
-00001e00: 2e32 3539 3633 3534 3065 2b30 3120 5a22  .25963540e+01 Z"
-00001e10: 202f 3e0d 0a20 2020 2020 203c 7061 7468   />..      <path
-00001e20: 2064 3d22 4d20 332e 3431 3131 3639 3730   d="M 3.41116970
-00001e30: 652b 3031 2037 2e35 3632 3938 3331 3065  e+01 7.56298310e
-00001e40: 2b30 3120 5120 332e 3039 3437 3533 3130  +01 Q 3.09475310
-00001e50: 652b 3031 2037 2e34 3037 3230 3132 3065  e+01 7.40720120e
-00001e60: 2b30 312c 2032 2e38 3237 3230 3734 3065  +01, 2.82720740e
-00001e70: 2b30 3120 372e 3137 3237 3931 3730 652b  +01 7.17279170e+
-00001e80: 3031 2051 2032 2e37 3731 3836 3332 3565  01 Q 2.77186325e
-00001e90: 2b30 3120 372e 3631 3132 3338 3835 652b  +01 7.61123885e+
-00001ea0: 3031 2c20 322e 3733 3832 3234 3430 652b  01, 2.73822440e+
-00001eb0: 3031 2038 2e30 3237 3537 3339 3065 2b30  01 8.02757390e+0
-00001ec0: 3120 5120 332e 3037 3032 3137 3735 652b  1 Q 3.07021775e+
-00001ed0: 3031 2037 2e38 3039 3330 3831 3565 2b30  01 7.80930815e+0
-00001ee0: 312c 2033 2e34 3131 3136 3937 3065 2b30  1, 3.41116970e+0
-00001ef0: 3120 372e 3536 3239 3833 3130 652b 3031  1 7.56298310e+01
-00001f00: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
-00001f10: 6174 6820 643d 224d 2032 2e38 3237 3230  ath d="M 2.82720
-00001f20: 3734 3065 2b30 3120 372e 3137 3237 3931  740e+01 7.172791
-00001f30: 3730 652b 3031 2051 2032 2e33 3837 3334  70e+01 Q 2.38734
-00001f40: 3836 3065 2b30 3120 372e 3232 3731 3837  860e+01 7.227187
-00001f50: 3235 652b 3031 2c20 312e 3936 3935 3831  25e+01, 1.969581
-00001f60: 3230 652b 3031 2037 2e32 3539 3633 3534  20e+01 7.2596354
-00001f70: 3065 2b30 3120 5120 322e 3335 3332 3330  0e+01 Q 2.353230
-00001f80: 3935 652b 3031 2037 2e36 3434 3232 3631  95e+01 7.6442261
-00001f90: 3065 2b30 312c 2032 2e37 3338 3232 3434  0e+01, 2.7382244
-00001fa0: 3065 2b30 3120 382e 3032 3735 3733 3930  0e+01 8.02757390
-00001fb0: 652b 3031 2051 2032 2e37 3731 3836 3332  e+01 Q 2.7718632
-00001fc0: 3565 2b30 3120 372e 3631 3132 3338 3835  5e+01 7.61123885
-00001fd0: 652b 3031 2c20 322e 3832 3732 3037 3430  e+01, 2.82720740
-00001fe0: 652b 3031 2037 2e31 3732 3739 3137 3065  e+01 7.17279170e
-00001ff0: 2b30 3120 5a22 202f 3e0d 0a20 2020 2020  +01 Z" />..     
-00002000: 203c 7061 7468 2064 3d22 4d20 342e 3130   <path d="M 4.10
-00002010: 3030 3030 3030 652b 3031 2037 2e37 3030  000000e+01 7.700
-00002020: 3030 3030 3065 2b30 3120 5120 332e 3735  00000e+01 Q 3.75
-00002030: 3131 3634 3035 652b 3031 2037 2e36 3737  116405e+01 7.677
-00002040: 3737 3430 3565 2b30 312c 2033 2e34 3131  77405e+01, 3.411
-00002050: 3136 3937 3065 2b30 3120 372e 3536 3239  16970e+01 7.5629
-00002060: 3833 3130 652b 3031 2051 2033 2e35 3834  8310e+01 Q 3.584
-00002070: 3739 3930 3565 2b30 3120 382e 3030 3438  79905e+01 8.0048
-00002080: 3132 3030 652b 3031 2c20 332e 3736 3831  1200e+01, 3.7681
-00002090: 3832 3630 652b 3031 2038 2e34 3134 3630  8260e+01 8.41460
-000020a0: 3030 3065 2b30 3120 5120 332e 3933 3532  000e+01 Q 3.9352
-000020b0: 3338 3335 652b 3031 2038 2e30 3732 3231  3835e+01 8.07221
-000020c0: 3834 3065 2b30 312c 2034 2e31 3030 3030  840e+01, 4.10000
-000020d0: 3030 3065 2b30 3120 372e 3730 3030 3030  000e+01 7.700000
-000020e0: 3030 652b 3031 205a 2220 2f3e 0d0a 2020  00e+01 Z" />..  
-000020f0: 2020 2020 3c70 6174 6820 643d 224d 2033      <path d="M 3
-00002100: 2e34 3131 3136 3937 3065 2b30 3120 372e  .41116970e+01 7.
-00002110: 3536 3239 3833 3130 652b 3031 2051 2033  56298310e+01 Q 3
-00002120: 2e30 3730 3231 3737 3565 2b30 3120 372e  .07021775e+01 7.
-00002130: 3830 3933 3038 3135 652b 3031 2c20 322e  80930815e+01, 2.
-00002140: 3733 3832 3234 3430 652b 3031 2038 2e30  73822440e+01 8.0
-00002150: 3237 3537 3339 3065 2b30 3120 5120 332e  2757390e+01 Q 3.
-00002160: 3235 3239 3932 3030 652b 3031 2038 2e32  25299200e+01 8.2
-00002170: 3232 3336 3633 3065 2b30 312c 2033 2e37  2236630e+01, 3.7
-00002180: 3638 3138 3236 3065 2b30 3120 382e 3431  6818260e+01 8.41
-00002190: 3436 3030 3030 652b 3031 2051 2033 2e35  460000e+01 Q 3.5
-000021a0: 3834 3739 3930 3565 2b30 3120 382e 3030  8479905e+01 8.00
-000021b0: 3438 3132 3030 652b 3031 2c20 332e 3431  481200e+01, 3.41
-000021c0: 3131 3639 3730 652b 3031 2037 2e35 3632  116970e+01 7.562
-000021d0: 3938 3331 3065 2b30 3120 5a22 202f 3e0d  98310e+01 Z" />.
-000021e0: 0a20 2020 2020 203c 7061 7468 2064 3d22  .      <path d="
-000021f0: 4d20 322e 3735 3030 3030 3030 652b 3031  M 2.75000000e+01
-00002200: 2039 2e35 3030 3030 3030 3065 2b30 3120   9.50000000e+01 
-00002210: 5120 332e 3837 3439 3939 3130 652b 3031  Q 3.87499910e+01
-00002220: 2039 2e35 3030 3030 3030 3065 2b30 312c   9.50000000e+01,
-00002230: 2034 2e39 3939 3939 3832 3065 2b30 3120   4.99999820e+01 
-00002240: 392e 3530 3030 3030 3030 652b 3031 2051  9.50000000e+01 Q
-00002250: 2034 2e33 3835 3735 3331 3565 2b30 3120   4.38575315e+01 
-00002260: 382e 3935 3639 3635 3230 652b 3031 2c20  8.95696520e+01, 
-00002270: 332e 3736 3831 3832 3630 652b 3031 2038  3.76818260e+01 8
-00002280: 2e34 3134 3630 3030 3065 2b30 3120 5120  .41460000e+01 Q 
-00002290: 332e 3235 3834 3137 3635 652b 3031 2038  3.25841765e+01 8
-000022a0: 2e39 3535 3635 3332 3765 2b30 312c 2032  .95565327e+01, 2
-000022b0: 2e37 3530 3030 3030 3065 2b30 3120 392e  .75000000e+01 9.
-000022c0: 3530 3030 3030 3030 652b 3031 205a 2220  50000000e+01 Z" 
-000022d0: 2f3e 0d0a 2020 2020 2020 3c70 6174 6820  />..      <path 
-000022e0: 643d 224d 2035 2e30 3030 3030 3030 3065  d="M 5.00000000e
-000022f0: 2b30 3020 392e 3530 3030 3030 3030 652b  +00 9.50000000e+
-00002300: 3031 2051 2031 2e36 3235 3030 3031 3365  01 Q 1.62500013e
-00002310: 2b30 3120 392e 3530 3030 3030 3030 652b  +01 9.50000000e+
-00002320: 3031 2c20 322e 3735 3030 3030 3030 652b  01, 2.75000000e+
-00002330: 3031 2039 2e35 3030 3030 3030 3065 2b30  01 9.50000000e+0
-00002340: 3120 5120 322e 3232 3530 3333 3135 652b  1 Q 2.22503315e+
-00002350: 3031 2038 2e38 3939 3432 3230 3465 2b30  01 8.89942204e+0
-00002360: 312c 2031 2e37 3030 3036 3633 3065 2b30  1, 1.70006630e+0
-00002370: 3120 382e 3239 3838 3433 3830 652b 3031  1 8.29884380e+01
-00002380: 2051 2031 2e31 3030 3033 3331 3965 2b30   Q 1.10003319e+0
-00002390: 3120 382e 3839 3934 3232 3034 652b 3031  1 8.89942204e+01
-000023a0: 2c20 352e 3030 3030 3030 3030 652b 3030  , 5.00000000e+00
-000023b0: 2039 2e35 3030 3030 3030 3065 2b30 3120   9.50000000e+01 
-000023c0: 5a22 202f 3e0d 0a20 2020 2020 203c 7061  Z" />..      <pa
-000023d0: 7468 2064 3d22 4d20 312e 3730 3030 3636  th d="M 1.700066
-000023e0: 3330 652b 3031 2038 2e32 3938 3834 3338  30e+01 8.2988438
-000023f0: 3065 2b30 3120 5120 322e 3232 3530 3333  0e+01 Q 2.225033
-00002400: 3135 652b 3031 2038 2e38 3939 3432 3230  15e+01 8.8994220
-00002410: 3465 2b30 312c 2032 2e37 3530 3030 3030  4e+01, 2.7500000
-00002420: 3065 2b30 3120 392e 3530 3030 3030 3030  0e+01 9.50000000
-00002430: 652b 3031 2051 2032 2e37 3435 3731 3535  e+01 Q 2.7457155
-00002440: 3565 2b30 3120 382e 3736 3237 3537 3736  5e+01 8.76275776
-00002450: 652b 3031 2c20 322e 3733 3832 3234 3430  e+01, 2.73822440
-00002460: 652b 3031 2038 2e30 3237 3537 3339 3065  e+01 8.02757390e
-00002470: 2b30 3120 5120 322e 3231 3835 3333 3830  +01 Q 2.21853380
-00002480: 652b 3031 2038 2e31 3632 3532 3339 3565  e+01 8.16252395e
-00002490: 2b30 312c 2031 2e37 3030 3036 3633 3065  +01, 1.70006630e
-000024a0: 2b30 3120 382e 3239 3838 3433 3830 652b  +01 8.29884380e+
-000024b0: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
-000024c0: 3c70 6174 6820 643d 224d 2032 2e37 3530  <path d="M 2.750
-000024d0: 3030 3030 3065 2b30 3120 392e 3530 3030  00000e+01 9.5000
-000024e0: 3030 3030 652b 3031 2051 2033 2e32 3538  0000e+01 Q 3.258
-000024f0: 3431 3736 3565 2b30 3120 382e 3935 3536  41765e+01 8.9556
-00002500: 3533 3237 652b 3031 2c20 332e 3736 3831  5327e+01, 3.7681
-00002510: 3832 3630 652b 3031 2038 2e34 3134 3630  8260e+01 8.41460
-00002520: 3030 3065 2b30 3120 5120 332e 3235 3239  000e+01 Q 3.2529
-00002530: 3932 3030 652b 3031 2038 2e32 3232 3336  9200e+01 8.22236
-00002540: 3633 3065 2b30 312c 2032 2e37 3338 3232  630e+01, 2.73822
-00002550: 3434 3065 2b30 3120 382e 3032 3735 3733  440e+01 8.027573
-00002560: 3930 652b 3031 2051 2032 2e37 3435 3731  90e+01 Q 2.74571
-00002570: 3535 3565 2b30 3120 382e 3736 3237 3537  555e+01 8.762757
-00002580: 3736 652b 3031 2c20 322e 3735 3030 3030  76e+01, 2.750000
-00002590: 3030 652b 3031 2039 2e35 3030 3030 3030  00e+01 9.5000000
-000025a0: 3065 2b30 3120 5a22 202f 3e0d 0a20 2020  0e+01 Z" />..   
-000025b0: 2020 203c 7061 7468 2064 3d22 4d20 342e     <path d="M 4.
-000025c0: 3939 3939 3938 3230 652b 3031 2039 2e35  99999820e+01 9.5
-000025d0: 3030 3030 3030 3065 2b30 3120 5120 362e  0000000e+01 Q 6.
-000025e0: 3132 3439 3938 3230 652b 3031 2039 2e35  12499820e+01 9.5
-000025f0: 3030 3030 3030 3065 2b30 312c 2037 2e32  0000000e+01, 7.2
-00002600: 3439 3939 3931 3065 2b30 3120 392e 3530  4999910e+01 9.50
-00002610: 3030 3030 3030 652b 3031 2051 2036 2e34  000000e+01 Q 6.4
-00002620: 3739 3233 3031 3065 2b30 3120 382e 3831  7923010e+01 8.81
-00002630: 3238 3536 3438 652b 3031 2c20 352e 3731  285648e+01, 5.71
-00002640: 3037 3439 3830 652b 3031 2038 2e31 3330  074980e+01 8.130
-00002650: 3638 3837 3065 2b30 3120 5120 352e 3335  68870e+01 Q 5.35
-00002660: 3532 3934 3335 652b 3031 2038 2e38 3136  529435e+01 8.816
-00002670: 3534 3535 3865 2b30 312c 2034 2e39 3939  54558e+01, 4.999
-00002680: 3939 3832 3065 2b30 3120 392e 3530 3030  99820e+01 9.5000
-00002690: 3030 3030 652b 3031 205a 2220 2f3e 0d0a  0000e+01 Z" />..
-000026a0: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
-000026b0: 2034 2e39 3939 3939 3832 3065 2b30 3120   4.99999820e+01 
-000026c0: 392e 3530 3030 3030 3030 652b 3031 2051  9.50000000e+01 Q
-000026d0: 2035 2e33 3535 3239 3433 3565 2b30 3120   5.35529435e+01 
-000026e0: 382e 3831 3635 3435 3538 652b 3031 2c20  8.81654558e+01, 
-000026f0: 352e 3731 3037 3439 3830 652b 3031 2038  5.71074980e+01 8
-00002700: 2e31 3330 3638 3837 3065 2b30 3120 5120  .13068870e+01 Q 
-00002710: 352e 3138 3634 3836 3330 652b 3031 2038  5.18648630e+01 8
-00002720: 2e31 3931 3937 3639 3065 2b30 312c 2034  .19197690e+01, 4
-00002730: 2e36 3539 3831 3236 3065 2b30 3120 382e  .65981260e+01 8.
-00002740: 3235 3330 3434 3630 652b 3031 2051 2034  25304460e+01 Q 4
-00002750: 2e38 3330 3235 3233 3565 2b30 3120 382e  .83025235e+01 8.
-00002760: 3837 3533 3431 3732 652b 3031 2c20 342e  87534172e+01, 4.
-00002770: 3939 3939 3938 3230 652b 3031 2039 2e35  99999820e+01 9.5
-00002780: 3030 3030 3030 3065 2b30 3120 5a22 202f  0000000e+01 Z" /
-00002790: 3e0d 0a20 2020 2020 203c 7061 7468 2064  >..      <path d
-000027a0: 3d22 4d20 332e 3736 3831 3832 3630 652b  ="M 3.76818260e+
-000027b0: 3031 2038 2e34 3134 3630 3030 3065 2b30  01 8.41460000e+0
-000027c0: 3120 5120 342e 3338 3537 3533 3135 652b  1 Q 4.38575315e+
-000027d0: 3031 2038 2e39 3536 3936 3532 3065 2b30  01 8.95696520e+0
-000027e0: 312c 2034 2e39 3939 3939 3832 3065 2b30  1, 4.99999820e+0
-000027f0: 3120 392e 3530 3030 3030 3030 652b 3031  1 9.50000000e+01
-00002800: 2051 2034 2e38 3330 3235 3233 3565 2b30   Q 4.83025235e+0
-00002810: 3120 382e 3837 3533 3431 3732 652b 3031  1 8.87534172e+01
-00002820: 2c20 342e 3635 3938 3132 3630 652b 3031  , 4.65981260e+01
-00002830: 2038 2e32 3533 3034 3436 3065 2b30 3120   8.25304460e+01 
-00002840: 5120 342e 3231 3338 3537 3230 652b 3031  Q 4.21385720e+01
-00002850: 2038 2e33 3334 3635 3433 3565 2b30 312c   8.33465435e+01,
-00002860: 2033 2e37 3638 3138 3236 3065 2b30 3120   3.76818260e+01 
-00002870: 382e 3431 3436 3030 3030 652b 3031 205a  8.41460000e+01 Z
-00002880: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
-00002890: 6820 643d 224d 2037 2e32 3439 3939 3931  h d="M 7.2499991
-000028a0: 3065 2b30 3120 392e 3530 3030 3030 3030  0e+01 9.50000000
-000028b0: 652b 3031 2051 2038 2e33 3734 3939 3935  e+01 Q 8.3749995
-000028c0: 3565 2b30 3120 392e 3530 3030 3030 3030  5e+01 9.50000000
-000028d0: 652b 3031 2c20 392e 3530 3030 3030 3030  e+01, 9.50000000
-000028e0: 652b 3031 2039 2e35 3030 3030 3030 3065  e+01 9.50000000e
-000028f0: 2b30 3120 5120 382e 3834 3635 3136 3330  +01 Q 8.84651630
-00002900: 652b 3031 2038 2e38 3437 3337 3933 3165  e+01 8.84737931e
-00002910: 2b30 312c 2038 2e31 3933 3033 3335 3065  +01, 8.19303350e
-00002920: 2b30 3120 382e 3139 3437 3538 3830 652b  +01 8.19475880e+
-00002930: 3031 2051 2037 2e37 3231 3531 3633 3065  01 Q 7.72151630e
-00002940: 2b30 3120 382e 3834 3733 3739 3331 652b  +01 8.84737931e+
-00002950: 3031 2c20 372e 3234 3939 3939 3130 652b  01, 7.24999910e+
-00002960: 3031 2039 2e35 3030 3030 3030 3065 2b30  01 9.50000000e+0
-00002970: 3120 5a22 202f 3e0d 0a20 2020 2020 203c  1 Z" />..      <
-00002980: 7061 7468 2064 3d22 4d20 352e 3731 3037  path d="M 5.7107
-00002990: 3439 3830 652b 3031 2038 2e31 3330 3638  4980e+01 8.13068
-000029a0: 3837 3065 2b30 3120 5120 362e 3437 3932  870e+01 Q 6.4792
-000029b0: 3330 3130 652b 3031 2038 2e38 3132 3835  3010e+01 8.81285
-000029c0: 3634 3865 2b30 312c 2037 2e32 3439 3939  648e+01, 7.24999
-000029d0: 3931 3065 2b30 3120 392e 3530 3030 3030  910e+01 9.500000
-000029e0: 3030 652b 3031 2051 2037 2e30 3835 3434  00e+01 Q 7.08544
-000029f0: 3331 3065 2b30 3120 382e 3632 3831 3139  310e+01 8.628119
-00002a00: 3238 652b 3031 2c20 362e 3932 3038 3837  28e+01, 6.920887
-00002a10: 3130 652b 3031 2037 2e37 3536 3233 3833  10e+01 7.7562383
-00002a20: 3065 2b30 3120 5120 362e 3331 3738 3732  0e+01 Q 6.317872
-00002a30: 3235 652b 3031 2037 2e39 3435 3839 3735  25e+01 7.9458975
-00002a40: 3565 2b30 312c 2035 2e37 3130 3734 3938  5e+01, 5.7107498
-00002a50: 3065 2b30 3120 382e 3133 3036 3838 3730  0e+01 8.13068870
-00002a60: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
-00002a70: 2020 3c70 6174 6820 643d 224d 2037 2e32    <path d="M 7.2
-00002a80: 3439 3939 3931 3065 2b30 3120 392e 3530  4999910e+01 9.50
-00002a90: 3030 3030 3030 652b 3031 2051 2037 2e37  000000e+01 Q 7.7
-00002aa0: 3231 3531 3633 3065 2b30 3120 382e 3834  2151630e+01 8.84
-00002ab0: 3733 3739 3331 652b 3031 2c20 382e 3139  737931e+01, 8.19
-00002ac0: 3330 3333 3530 652b 3031 2038 2e31 3934  303350e+01 8.194
-00002ad0: 3735 3838 3065 2b30 3120 5120 372e 3535  75880e+01 Q 7.55
-00002ae0: 3639 3630 3330 652b 3031 2037 2e39 3735  696030e+01 7.975
-00002af0: 3439 3835 3565 2b30 312c 2036 2e39 3230  49855e+01, 6.920
-00002b00: 3838 3731 3065 2b30 3120 372e 3735 3632  88710e+01 7.7562
-00002b10: 3338 3330 652b 3031 2051 2037 2e30 3835  3830e+01 Q 7.085
-00002b20: 3434 3331 3065 2b30 3120 382e 3632 3831  44310e+01 8.6281
-00002b30: 3139 3238 652b 3031 2c20 372e 3234 3939  1928e+01, 7.2499
-00002b40: 3939 3130 652b 3031 2039 2e35 3030 3030  9910e+01 9.50000
-00002b50: 3030 3065 2b30 3120 5a22 202f 3e0d 0a20  000e+01 Z" />.. 
-00002b60: 2020 2020 203c 7061 7468 2064 3d22 4d20       <path d="M 
-00002b70: 322e 3330 3030 3030 3030 652b 3031 2034  2.30000000e+01 4
-00002b80: 2e30 3939 3939 3931 3065 2b30 3120 5120  .09999910e+01 Q 
-00002b90: 322e 3330 3030 3030 3030 652b 3031 2033  2.30000000e+01 3
-00002ba0: 2e36 3439 3939 3935 3565 2b30 312c 2032  .64999955e+01, 2
-00002bb0: 2e33 3030 3030 3030 3065 2b30 3120 332e  .30000000e+01 3.
-00002bc0: 3230 3030 3030 3030 652b 3031 2051 2031  20000000e+01 Q 1
-00002bd0: 2e38 3833 3235 3930 3565 2b30 3120 332e  .88325905e+01 3.
-00002be0: 3535 3535 3435 3030 652b 3031 2c20 312e  55554500e+01, 1.
-00002bf0: 3436 3635 3138 3130 652b 3031 2033 2e39  46651810e+01 3.9
-00002c00: 3131 3039 3030 3065 2b30 3120 5120 312e  1109000e+01 Q 1.
-00002c10: 3838 3332 3539 3035 652b 3031 2034 2e30  88325905e+01 4.0
-00002c20: 3035 3534 3435 3565 2b30 312c 2032 2e33  0554455e+01, 2.3
-00002c30: 3030 3030 3030 3065 2b30 3120 342e 3039  0000000e+01 4.09
-00002c40: 3939 3939 3130 652b 3031 205a 2220 2f3e  999910e+01 Z" />
-00002c50: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
-00002c60: 224d 2032 2e33 3030 3030 3030 3065 2b30  "M 2.30000000e+0
-00002c70: 3120 332e 3230 3030 3030 3030 652b 3031  1 3.20000000e+01
-00002c80: 2051 2032 2e33 3030 3030 3030 3065 2b30   Q 2.30000000e+0
-00002c90: 3120 322e 3735 3030 3030 3030 652b 3031  1 2.75000000e+01
-00002ca0: 2c20 322e 3330 3030 3030 3030 652b 3031  , 2.30000000e+01
-00002cb0: 2032 2e33 3030 3030 3030 3065 2b30 3120   2.30000000e+01 
-00002cc0: 5120 312e 3339 3939 3939 3837 652b 3031  Q 1.39999987e+01
-00002cd0: 2032 2e35 3235 3030 3030 3065 2b30 312c   2.52500000e+01,
-00002ce0: 2035 2e30 3030 3030 3030 3065 2b30 3020   5.00000000e+00 
-00002cf0: 322e 3735 3030 3030 3030 652b 3031 2051  2.75000000e+01 Q
-00002d00: 2031 2e33 3939 3939 3938 3765 2b30 3120   1.39999987e+01 
-00002d10: 322e 3937 3530 3030 3030 652b 3031 2c20  2.97500000e+01, 
-00002d20: 322e 3330 3030 3030 3030 652b 3031 2033  2.30000000e+01 3
-00002d30: 2e32 3030 3030 3030 3065 2b30 3120 5a22  .20000000e+01 Z"
-00002d40: 202f 3e0d 0a20 2020 2020 203c 7061 7468   />..      <path
-00002d50: 2064 3d22 4d20 312e 3436 3635 3138 3130   d="M 1.46651810
-00002d60: 652b 3031 2033 2e39 3131 3039 3030 3065  e+01 3.91109000e
-00002d70: 2b30 3120 5120 312e 3838 3332 3539 3035  +01 Q 1.88325905
-00002d80: 652b 3031 2033 2e35 3535 3534 3530 3065  e+01 3.55554500e
-00002d90: 2b30 312c 2032 2e33 3030 3030 3030 3065  +01, 2.30000000e
-00002da0: 2b30 3120 332e 3230 3030 3030 3030 652b  +01 3.20000000e+
-00002db0: 3031 2051 2031 2e33 3939 3939 3938 3765  01 Q 1.39999987e
-00002dc0: 2b30 3120 322e 3937 3530 3030 3030 652b  +01 2.97500000e+
-00002dd0: 3031 2c20 352e 3030 3030 3030 3030 652b  01, 5.00000000e+
-00002de0: 3030 2032 2e37 3530 3030 3030 3065 2b30  00 2.75000000e+0
-00002df0: 3120 5120 392e 3833 3235 3930 3035 652b  1 Q 9.83259005e+
-00002e00: 3030 2033 2e33 3330 3534 3530 3065 2b30  00 3.33054500e+0
-00002e10: 312c 2031 2e34 3636 3531 3831 3065 2b30  1, 1.46651810e+0
-00002e20: 3120 332e 3931 3130 3930 3030 652b 3031  1 3.91109000e+01
-00002e30: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
-00002e40: 6174 6820 643d 224d 2032 2e33 3030 3030  ath d="M 2.30000
-00002e50: 3030 3065 2b30 3120 352e 3030 3030 3030  000e+01 5.000000
-00002e60: 3030 652b 3031 2051 2032 2e33 3030 3030  00e+01 Q 2.30000
-00002e70: 3030 3065 2b30 3120 342e 3534 3939 3939  000e+01 4.549999
-00002e80: 3535 652b 3031 2c20 322e 3330 3030 3030  55e+01, 2.300000
-00002e90: 3030 652b 3031 2034 2e30 3939 3939 3931  00e+01 4.0999991
-00002ea0: 3065 2b30 3120 5120 312e 3938 3038 3638  0e+01 Q 1.980868
-00002eb0: 3130 652b 3031 2034 2e33 3734 3139 3034  10e+01 4.3741904
-00002ec0: 3065 2b30 312c 2031 2e36 3631 3733 3731  0e+01, 1.6617371
-00002ed0: 3065 2b30 3120 342e 3634 3833 3831 3730  0e+01 4.64838170
-00002ee0: 652b 3031 2051 2031 2e39 3830 3733 3335  e+01 Q 1.9807335
-00002ef0: 3565 2b30 3120 342e 3832 3432 3133 3335  5e+01 4.82421335
-00002f00: 652b 3031 2c20 322e 3330 3030 3030 3030  e+01, 2.30000000
-00002f10: 652b 3031 2035 2e30 3030 3030 3030 3065  e+01 5.00000000e
-00002f20: 2b30 3120 5a22 202f 3e0d 0a20 2020 2020  +01 Z" />..     
-00002f30: 203c 7061 7468 2064 3d22 4d20 322e 3330   <path d="M 2.30
-00002f40: 3030 3030 3030 652b 3031 2034 2e30 3939  000000e+01 4.099
-00002f50: 3939 3931 3065 2b30 3120 5120 312e 3838  99910e+01 Q 1.88
-00002f60: 3332 3539 3035 652b 3031 2034 2e30 3035  325905e+01 4.005
-00002f70: 3534 3435 3565 2b30 312c 2031 2e34 3636  54455e+01, 1.466
-00002f80: 3531 3831 3065 2b30 3120 332e 3931 3130  51810e+01 3.9110
-00002f90: 3930 3030 652b 3031 2051 2031 2e35 3634  9000e+01 Q 1.564
-00002fa0: 3132 3731 3565 2b30 3120 342e 3237 3937  12715e+01 4.2797
-00002fb0: 3335 3835 652b 3031 2c20 312e 3636 3137  3585e+01, 1.6617
-00002fc0: 3337 3130 652b 3031 2034 2e36 3438 3338  3710e+01 4.64838
-00002fd0: 3137 3065 2b30 3120 5120 312e 3938 3038  170e+01 Q 1.9808
-00002fe0: 3638 3130 652b 3031 2034 2e33 3734 3139  6810e+01 4.37419
-00002ff0: 3034 3065 2b30 312c 2032 2e33 3030 3030  040e+01, 2.30000
-00003000: 3030 3065 2b30 3120 342e 3039 3939 3939  000e+01 4.099999
-00003010: 3130 652b 3031 205a 2220 2f3e 0d0a 2020  10e+01 Z" />..  
-00003020: 2020 2020 3c70 6174 6820 643d 224d 2032      <path d="M 2
-00003030: 2e33 3030 3030 3030 3065 2b30 3120 352e  .30000000e+01 5.
-00003040: 3930 3030 3030 3030 652b 3031 2051 2032  90000000e+01 Q 2
-00003050: 2e33 3030 3030 3030 3065 2b30 3120 352e  .30000000e+01 5.
-00003060: 3435 3030 3030 3030 652b 3031 2c20 322e  45000000e+01, 2.
-00003070: 3330 3030 3030 3030 652b 3031 2035 2e30  30000000e+01 5.0
-00003080: 3030 3030 3030 3065 2b30 3120 5120 322e  0000000e+01 Q 2.
-00003090: 3030 3330 3033 3630 652b 3031 2035 2e31  00300360e+01 5.1
-000030a0: 3630 3934 3631 3065 2b30 312c 2031 2e37  6094610e+01, 1.7
-000030b0: 3035 3537 3631 3065 2b30 3120 352e 3332  0557610e+01 5.32
-000030c0: 3134 3232 3430 652b 3031 2051 2032 2e30  142240e+01 Q 2.0
-000030d0: 3030 3533 3830 3565 2b30 3120 352e 3631  0053805e+01 5.61
-000030e0: 3036 3931 3430 652b 3031 2c20 322e 3330  069140e+01, 2.30
-000030f0: 3030 3030 3030 652b 3031 2035 2e39 3030  000000e+01 5.900
-00003100: 3030 3030 3065 2b30 3120 5a22 202f 3e0d  00000e+01 Z" />.
-00003110: 0a20 2020 2020 203c 7061 7468 2064 3d22  .      <path d="
-00003120: 4d20 322e 3330 3030 3030 3030 652b 3031  M 2.30000000e+01
-00003130: 2035 2e30 3030 3030 3030 3065 2b30 3120   5.00000000e+01 
-00003140: 5120 312e 3938 3037 3333 3535 652b 3031  Q 1.98073355e+01
-00003150: 2034 2e38 3234 3231 3333 3565 2b30 312c   4.82421335e+01,
-00003160: 2031 2e36 3631 3733 3731 3065 2b30 3120   1.66173710e+01 
-00003170: 342e 3634 3833 3831 3730 652b 3031 2051  4.64838170e+01 Q
-00003180: 2031 2e36 3833 3937 3631 3065 2b30 3120   1.68397610e+01 
-00003190: 342e 3938 3439 3839 3830 652b 3031 2c20  4.98498980e+01, 
-000031a0: 312e 3730 3535 3736 3130 652b 3031 2035  1.70557610e+01 5
-000031b0: 2e33 3231 3432 3234 3065 2b30 3120 5120  .32142240e+01 Q 
-000031c0: 322e 3030 3330 3033 3630 652b 3031 2035  2.00300360e+01 5
-000031d0: 2e31 3630 3934 3631 3065 2b30 312c 2032  .16094610e+01, 2
-000031e0: 2e33 3030 3030 3030 3065 2b30 3120 352e  .30000000e+01 5.
-000031f0: 3030 3030 3030 3030 652b 3031 205a 2220  00000000e+01 Z" 
-00003200: 2f3e 0d0a 2020 2020 2020 3c70 6174 6820  />..      <path 
-00003210: 643d 224d 2035 2e30 3030 3030 3030 3065  d="M 5.00000000e
-00003220: 2b30 3020 322e 3735 3030 3030 3030 652b  +00 2.75000000e+
-00003230: 3031 2051 2035 2e30 3030 3030 3030 3065  01 Q 5.00000000e
-00003240: 2b30 3020 332e 3837 3439 3939 3130 652b  +00 3.87499910e+
-00003250: 3031 2c20 352e 3030 3030 3030 3030 652b  01, 5.00000000e+
-00003260: 3030 2034 2e39 3939 3939 3832 3065 2b30  00 4.99999820e+0
-00003270: 3120 5120 392e 3833 3235 3930 3035 652b  1 Q 9.83259005e+
-00003280: 3030 2034 2e34 3535 3534 3336 3565 2b30  00 4.45554365e+0
-00003290: 312c 2031 2e34 3636 3531 3831 3065 2b30  1, 1.46651810e+0
-000032a0: 3120 332e 3931 3130 3930 3030 652b 3031  1 3.91109000e+01
-000032b0: 2051 2039 2e38 3332 3539 3030 3565 2b30   Q 9.83259005e+0
-000032c0: 3020 332e 3333 3035 3435 3030 652b 3031  0 3.33054500e+01
-000032d0: 2c20 352e 3030 3030 3030 3030 652b 3030  , 5.00000000e+00
-000032e0: 2032 2e37 3530 3030 3030 3065 2b30 3120   2.75000000e+01 
-000032f0: 5a22 202f 3e0d 0a20 2020 2020 203c 7061  Z" />..      <pa
-00003300: 7468 2064 3d22 4d20 352e 3030 3030 3030  th d="M 5.000000
-00003310: 3030 652b 3030 2035 2e30 3030 3030 3030  00e+00 5.0000000
-00003320: 3065 2b30 3020 5120 352e 3030 3030 3030  0e+00 Q 5.000000
-00003330: 3030 652b 3030 2031 2e36 3235 3030 3030  00e+00 1.6250000
-00003340: 3065 2b30 312c 2035 2e30 3030 3030 3030  0e+01, 5.0000000
-00003350: 3065 2b30 3020 322e 3735 3030 3030 3030  0e+00 2.75000000
-00003360: 652b 3031 2051 2031 2e33 3939 3939 3938  e+01 Q 1.3999998
-00003370: 3765 2b30 3120 322e 3532 3530 3030 3030  7e+01 2.52500000
-00003380: 652b 3031 2c20 322e 3330 3030 3030 3030  e+01, 2.30000000
-00003390: 652b 3031 2032 2e33 3030 3030 3030 3065  e+01 2.30000000e
-000033a0: 2b30 3120 5120 312e 3339 3939 3939 3837  +01 Q 1.39999987
-000033b0: 652b 3031 2031 2e34 3030 3030 3030 3065  e+01 1.40000000e
-000033c0: 2b30 312c 2035 2e30 3030 3030 3030 3065  +01, 5.00000000e
-000033d0: 2b30 3020 352e 3030 3030 3030 3030 652b  +00 5.00000000e+
-000033e0: 3030 205a 2220 2f3e 0d0a 2020 2020 2020  00 Z" />..      
-000033f0: 3c70 6174 6820 643d 224d 2035 2e30 3030  <path d="M 5.000
-00003400: 3030 3030 3065 2b30 3020 372e 3234 3939  00000e+00 7.2499
-00003410: 3939 3130 652b 3031 2051 2031 2e30 3337  9910e+01 Q 1.037
-00003420: 3436 3938 3865 2b30 3120 362e 3733 3634  46988e+01 6.7364
-00003430: 3936 3930 652b 3031 2c20 312e 3537 3431  9690e+01, 1.5741
-00003440: 3836 3930 652b 3031 2036 2e32 3231 3734  8690e+01 6.22174
-00003450: 3139 3065 2b30 3120 5120 312e 3033 3939  190e+01 Q 1.0399
-00003460: 3838 3136 652b 3031 2035 2e36 3039 3739  8816e+01 5.60979
-00003470: 3332 3065 2b30 312c 2035 2e30 3030 3030  320e+01, 5.00000
-00003480: 3030 3065 2b30 3020 342e 3939 3939 3938  000e+00 4.999998
-00003490: 3230 652b 3031 2051 2035 2e30 3030 3030  20e+01 Q 5.00000
-000034a0: 3030 3065 2b30 3020 362e 3132 3439 3938  000e+00 6.124998
-000034b0: 3230 652b 3031 2c20 352e 3030 3030 3030  20e+01, 5.000000
-000034c0: 3030 652b 3030 2037 2e32 3439 3939 3931  00e+00 7.2499991
-000034d0: 3065 2b30 3120 5a22 202f 3e0d 0a20 2020  0e+01 Z" />..   
-000034e0: 2020 203c 7061 7468 2064 3d22 4d20 312e     <path d="M 1.
-000034f0: 3730 3535 3736 3130 652b 3031 2035 2e33  70557610e+01 5.3
-00003500: 3231 3432 3234 3065 2b30 3120 5120 312e  2142240e+01 Q 1.
-00003510: 3130 3237 3536 3832 652b 3031 2035 2e31  10275682e+01 5.1
-00003520: 3630 3533 3330 3065 2b30 312c 2035 2e30  6053300e+01, 5.0
-00003530: 3030 3030 3030 3065 2b30 3020 342e 3939  0000000e+00 4.99
-00003540: 3939 3938 3230 652b 3031 2051 2031 2e30  999820e+01 Q 1.0
-00003550: 3339 3938 3831 3665 2b30 3120 352e 3630  3998816e+01 5.60
-00003560: 3937 3933 3230 652b 3031 2c20 312e 3537  979320e+01, 1.57
-00003570: 3431 3836 3930 652b 3031 2036 2e32 3231  418690e+01 6.221
-00003580: 3734 3139 3065 2b30 3120 5120 312e 3633  74190e+01 Q 1.63
-00003590: 3937 3933 3735 652b 3031 2035 2e37 3730  979375e+01 5.770
-000035a0: 3535 3937 3565 2b30 312c 2031 2e37 3035  55975e+01, 1.705
-000035b0: 3537 3631 3065 2b30 3120 352e 3332 3134  57610e+01 5.3214
-000035c0: 3232 3430 652b 3031 205a 2220 2f3e 0d0a  2240e+01 Z" />..
-000035d0: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
-000035e0: 2031 2e36 3631 3733 3731 3065 2b30 3120   1.66173710e+01 
-000035f0: 342e 3634 3833 3831 3730 652b 3031 2051  4.64838170e+01 Q
-00003600: 2031 2e30 3830 3836 3833 3765 2b30 3120   1.08086837e+01 
-00003610: 342e 3832 3431 3839 3530 652b 3031 2c20  4.82418950e+01, 
-00003620: 352e 3030 3030 3030 3030 652b 3030 2034  5.00000000e+00 4
-00003630: 2e39 3939 3939 3832 3065 2b30 3120 5120  .99999820e+01 Q 
-00003640: 312e 3130 3237 3536 3832 652b 3031 2035  1.10275682e+01 5
-00003650: 2e31 3630 3533 3330 3065 2b30 312c 2031  .16053300e+01, 1
-00003660: 2e37 3035 3537 3631 3065 2b30 3120 352e  .70557610e+01 5.
-00003670: 3332 3134 3232 3430 652b 3031 2051 2031  32142240e+01 Q 1
-00003680: 2e36 3833 3937 3631 3065 2b30 3120 342e  .68397610e+01 4.
-00003690: 3938 3439 3839 3830 652b 3031 2c20 312e  98498980e+01, 1.
-000036a0: 3636 3137 3337 3130 652b 3031 2034 2e36  66173710e+01 4.6
-000036b0: 3438 3338 3137 3065 2b30 3120 5a22 202f  4838170e+01 Z" /
-000036c0: 3e0d 0a20 2020 2020 203c 7061 7468 2064  >..      <path d
-000036d0: 3d22 4d20 312e 3436 3635 3138 3130 652b  ="M 1.46651810e+
-000036e0: 3031 2033 2e39 3131 3039 3030 3065 2b30  01 3.91109000e+0
-000036f0: 3120 5120 392e 3833 3235 3930 3035 652b  1 Q 9.83259005e+
-00003700: 3030 2034 2e34 3535 3534 3336 3565 2b30  00 4.45554365e+0
-00003710: 312c 2035 2e30 3030 3030 3030 3065 2b30  1, 5.00000000e+0
-00003720: 3020 342e 3939 3939 3938 3230 652b 3031  0 4.99999820e+01
-00003730: 2051 2031 2e30 3830 3836 3833 3765 2b30   Q 1.08086837e+0
-00003740: 3120 342e 3832 3431 3839 3530 652b 3031  1 4.82418950e+01
-00003750: 2c20 312e 3636 3137 3337 3130 652b 3031  , 1.66173710e+01
-00003760: 2034 2e36 3438 3338 3137 3065 2b30 3120   4.64838170e+01 
-00003770: 5120 312e 3536 3431 3237 3135 652b 3031  Q 1.56412715e+01
-00003780: 2034 2e32 3739 3733 3538 3565 2b30 312c   4.27973585e+01,
-00003790: 2031 2e34 3636 3531 3831 3065 2b30 3120   1.46651810e+01 
-000037a0: 332e 3931 3130 3930 3030 652b 3031 205a  3.91109000e+01 Z
-000037b0: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
-000037c0: 6820 643d 224d 2035 2e30 3030 3030 3030  h d="M 5.0000000
-000037d0: 3065 2b30 3020 372e 3234 3939 3939 3130  0e+00 7.24999910
-000037e0: 652b 3031 2051 2035 2e30 3030 3030 3030  e+01 Q 5.0000000
-000037f0: 3065 2b30 3020 382e 3337 3439 3939 3639  0e+00 8.37499969
-00003800: 652b 3031 2c20 352e 3030 3030 3030 3030  e+01, 5.00000000
-00003810: 652b 3030 2039 2e35 3030 3030 3030 3065  e+00 9.50000000e
-00003820: 2b30 3120 5120 312e 3130 3030 3333 3139  +01 Q 1.10003319
-00003830: 652b 3031 2038 2e38 3939 3432 3230 3465  e+01 8.89942204e
-00003840: 2b30 312c 2031 2e37 3030 3036 3633 3065  +01, 1.70006630e
-00003850: 2b30 3120 382e 3239 3838 3433 3830 652b  +01 8.29884380e+
-00003860: 3031 2051 2031 2e31 3030 3033 3331 3965  01 Q 1.10003319e
-00003870: 2b30 3120 372e 3737 3434 3231 3435 652b  +01 7.77442145e+
-00003880: 3031 2c20 352e 3030 3030 3030 3030 652b  01, 5.00000000e+
-00003890: 3030 2037 2e32 3439 3939 3931 3065 2b30  00 7.24999910e+0
-000038a0: 3120 5a22 202f 3e0d 0a20 2020 2020 203c  1 Z" />..      <
-000038b0: 7061 7468 2064 3d22 4d20 352e 3030 3030  path d="M 5.0000
-000038c0: 3030 3030 652b 3030 2037 2e32 3439 3939  0000e+00 7.24999
-000038d0: 3931 3065 2b30 3120 5120 312e 3130 3030  910e+01 Q 1.1000
-000038e0: 3333 3139 652b 3031 2037 2e37 3734 3432  3319e+01 7.77442
-000038f0: 3134 3565 2b30 312c 2031 2e37 3030 3036  145e+01, 1.70006
-00003900: 3633 3065 2b30 3120 382e 3239 3838 3433  630e+01 8.298843
-00003910: 3830 652b 3031 2051 2031 2e38 3335 3433  80e+01 Q 1.83543
-00003920: 3938 3065 2b30 3120 372e 3737 3938 3334  980e+01 7.779834
-00003930: 3935 652b 3031 2c20 312e 3936 3935 3831  95e+01, 1.969581
-00003940: 3230 652b 3031 2037 2e32 3539 3633 3534  20e+01 7.2596354
-00003950: 3065 2b30 3120 5120 312e 3233 3539 3338  0e+01 Q 1.235938
-00003960: 3836 652b 3031 2037 2e32 3532 3937 3736  86e+01 7.2529776
-00003970: 3565 2b30 312c 2035 2e30 3030 3030 3030  5e+01, 5.0000000
-00003980: 3065 2b30 3020 372e 3234 3939 3939 3130  0e+00 7.24999910
-00003990: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
-000039a0: 2020 3c70 6174 6820 643d 224d 2031 2e35    <path d="M 1.5
-000039b0: 3734 3138 3639 3065 2b30 3120 362e 3232  7418690e+01 6.22
-000039c0: 3137 3431 3930 652b 3031 2051 2031 2e30  174190e+01 Q 1.0
-000039d0: 3337 3436 3938 3865 2b30 3120 362e 3733  3746988e+01 6.73
-000039e0: 3634 3936 3930 652b 3031 2c20 352e 3030  649690e+01, 5.00
-000039f0: 3030 3030 3030 652b 3030 2037 2e32 3439  000000e+00 7.249
-00003a00: 3939 3931 3065 2b30 3120 5120 312e 3233  99910e+01 Q 1.23
-00003a10: 3539 3338 3836 652b 3031 2037 2e32 3532  593886e+01 7.252
-00003a20: 3937 3736 3565 2b30 312c 2031 2e39 3639  97765e+01, 1.969
-00003a30: 3538 3132 3065 2b30 3120 372e 3235 3936  58120e+01 7.2596
-00003a40: 3335 3430 652b 3031 2051 2031 2e37 3639  3540e+01 Q 1.769
-00003a50: 3431 3736 3065 2b30 3120 362e 3734 3130  41760e+01 6.7410
-00003a60: 3935 3435 652b 3031 2c20 312e 3537 3431  9545e+01, 1.5741
-00003a70: 3836 3930 652b 3031 2036 2e32 3231 3734  8690e+01 6.22174
-00003a80: 3139 3065 2b30 3120 5a22 202f 3e0d 0a20  190e+01 Z" />.. 
-00003a90: 2020 2020 203c 7061 7468 2064 3d22 4d20       <path d="M 
-00003aa0: 312e 3537 3431 3836 3930 652b 3031 2036  1.57418690e+01 6
-00003ab0: 2e32 3231 3734 3139 3065 2b30 3120 5120  .22174190e+01 Q 
-00003ac0: 312e 3932 3632 3437 3130 652b 3031 2036  1.92624710e+01 6
-00003ad0: 2e30 3539 3532 3435 3565 2b30 312c 2032  .05952455e+01, 2
-00003ae0: 2e33 3030 3030 3030 3065 2b30 3120 352e  .30000000e+01 5.
-00003af0: 3930 3030 3030 3030 652b 3031 2051 2032  90000000e+01 Q 2
-00003b00: 2e30 3030 3533 3830 3565 2b30 3120 352e  .00053805e+01 5.
-00003b10: 3631 3036 3931 3430 652b 3031 2c20 312e  61069140e+01, 1.
-00003b20: 3730 3535 3736 3130 652b 3031 2035 2e33  70557610e+01 5.3
-00003b30: 3231 3432 3234 3065 2b30 3120 5120 312e  2142240e+01 Q 1.
-00003b40: 3633 3937 3933 3735 652b 3031 2035 2e37  63979375e+01 5.7
-00003b50: 3730 3535 3937 3565 2b30 312c 2031 2e35  7055975e+01, 1.5
-00003b60: 3734 3138 3639 3065 2b30 3120 362e 3232  7418690e+01 6.22
-00003b70: 3137 3431 3930 652b 3031 205a 2220 2f3e  174190e+01 Z" />
-00003b80: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
-00003b90: 224d 2034 2e36 3539 3831 3236 3065 2b30  "M 4.65981260e+0
-00003ba0: 3120 382e 3235 3330 3434 3630 652b 3031  1 8.25304460e+01
-00003bb0: 2051 2034 2e33 3739 3139 3537 3565 2b30   Q 4.37919575e+0
-00003bc0: 3120 372e 3939 3430 3531 3630 652b 3031  1 7.99405160e+01
-00003bd0: 2c20 342e 3130 3030 3030 3030 652b 3031  , 4.10000000e+01
-00003be0: 2037 2e37 3030 3030 3030 3065 2b30 3120   7.70000000e+01 
-00003bf0: 5120 332e 3933 3532 3338 3335 652b 3031  Q 3.93523835e+01
-00003c00: 2038 2e30 3732 3231 3834 3065 2b30 312c   8.07221840e+01,
-00003c10: 2033 2e37 3638 3138 3236 3065 2b30 3120   3.76818260e+01 
-00003c20: 382e 3431 3436 3030 3030 652b 3031 2051  8.41460000e+01 Q
-00003c30: 2034 2e32 3133 3835 3732 3065 2b30 3120   4.21385720e+01 
-00003c40: 382e 3333 3436 3534 3335 652b 3031 2c20  8.33465435e+01, 
-00003c50: 342e 3635 3938 3132 3630 652b 3031 2038  4.65981260e+01 8
-00003c60: 2e32 3533 3034 3436 3065 2b30 3120 5a22  .25304460e+01 Z"
-00003c70: 202f 3e0d 0a20 2020 2020 203c 7061 7468   />..      <path
-00003c80: 2064 3d22 4d20 362e 3538 3838 3330 3330   d="M 6.58883030
-00003c90: 652b 3031 2035 2e37 3632 3938 3331 3065  e+01 5.76298310e
-00003ca0: 2b30 3120 5120 362e 3234 3838 3335 3935  +01 Q 6.24883595
-00003cb0: 652b 3031 2035 2e38 3737 3737 3430 3565  e+01 5.87777405e
-00003cc0: 2b30 312c 2035 2e39 3030 3030 3030 3065  +01, 5.90000000e
-00003cd0: 2b30 3120 352e 3930 3030 3030 3030 652b  +01 5.90000000e+
-00003ce0: 3031 2051 2036 2e32 3635 3936 3131 3565  01 Q 6.26596115e
-00003cf0: 2b30 3120 362e 3236 3733 3331 3430 652b  +01 6.26733140e+
-00003d00: 3031 2c20 362e 3630 3039 3837 3530 652b  01, 6.60098750e+
-00003d10: 3031 2036 2e36 3033 3831 3632 3065 2b30  01 6.60381620e+0
-00003d20: 3120 5120 362e 3630 3338 3435 3930 652b  1 Q 6.60384590e+
-00003d30: 3031 2036 2e31 3935 3030 3234 3565 2b30  01 6.19500245e+0
-00003d40: 312c 2036 2e35 3838 3833 3033 3065 2b30  1, 6.58883030e+0
-00003d50: 3120 352e 3736 3239 3833 3130 652b 3031  1 5.76298310e+01
-00003d60: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
-00003d70: 6174 6820 643d 224d 2038 2e34 3134 3730  ath d="M 8.41470
-00003d80: 3938 3065 2b30 3120 332e 3736 3833 3136  980e+01 3.768316
-00003d90: 3730 652b 3031 2051 2038 2e30 3732 3237  70e+01 Q 8.07227
-00003da0: 3234 3065 2b30 3120 332e 3933 3533 3036  240e+01 3.935306
-00003db0: 3330 652b 3031 2c20 372e 3730 3030 3030  30e+01, 7.700000
-00003dc0: 3030 652b 3031 2034 2e31 3030 3030 3030  00e+01 4.1000000
-00003dd0: 3065 2b30 3120 5120 372e 3939 3339 3839  0e+01 Q 7.993989
-00003de0: 3935 652b 3031 2034 2e33 3739 3238 3335  95e+01 4.3792835
-00003df0: 3065 2b30 312c 2038 2e32 3532 3931 3935  0e+01, 8.2529195
-00003e00: 3065 2b30 3120 342e 3635 3939 3835 3430  0e+01 4.65998540
-00003e10: 652b 3031 2051 2038 2e33 3334 3634 3632  e+01 Q 8.3346462
-00003e20: 3565 2b30 3120 342e 3231 3430 3130 3635  5e+01 4.21401065
-00003e30: 652b 3031 2c20 382e 3431 3437 3039 3830  e+01, 8.41470980
-00003e40: 652b 3031 2033 2e37 3638 3331 3637 3065  e+01 3.76831670e
-00003e50: 2b30 3120 5a22 202f 3e0d 0a20 2020 2020  +01 Z" />..     
-00003e60: 203c 7061 7468 2064 3d22 4d20 372e 3536   <path d="M 7.56
-00003e70: 3239 3833 3130 652b 3031 2033 2e34 3131  298310e+01 3.411
-00003e80: 3136 3937 3065 2b30 3120 5120 372e 3637  16970e+01 Q 7.67
-00003e90: 3737 3734 3035 652b 3031 2033 2e37 3531  777405e+01 3.751
-00003ea0: 3136 3430 3565 2b30 312c 2037 2e37 3030  16405e+01, 7.700
-00003eb0: 3030 3030 3065 2b30 3120 342e 3130 3030  00000e+01 4.1000
-00003ec0: 3030 3030 652b 3031 2051 2038 2e30 3732  0000e+01 Q 8.072
-00003ed0: 3237 3234 3065 2b30 3120 332e 3933 3533  27240e+01 3.9353
-00003ee0: 3036 3330 652b 3031 2c20 382e 3431 3437  0630e+01, 8.4147
-00003ef0: 3039 3830 652b 3031 2033 2e37 3638 3331  0980e+01 3.76831
-00003f00: 3637 3065 2b30 3120 5120 382e 3030 3438  670e+01 Q 8.0048
-00003f10: 3731 3835 652b 3031 2033 2e35 3834 3836  7185e+01 3.58486
-00003f20: 3536 3565 2b30 312c 2037 2e35 3632 3938  565e+01, 7.56298
-00003f30: 3331 3065 2b30 3120 332e 3431 3131 3639  310e+01 3.411169
-00003f40: 3730 652b 3031 205a 2220 2f3e 0d0a 2020  70e+01 Z" />..  
-00003f50: 2020 2020 3c70 6174 6820 643d 224d 2037      <path d="M 7
-00003f60: 2e37 3030 3030 3030 3065 2b30 3120 342e  .70000000e+01 4.
-00003f70: 3130 3030 3030 3030 652b 3031 2051 2037  10000000e+01 Q 7
-00003f80: 2e36 3737 3737 3430 3565 2b30 3120 342e  .67777405e+01 4.
-00003f90: 3434 3838 3335 3935 652b 3031 2c20 372e  44883595e+01, 7.
-00003fa0: 3536 3239 3833 3130 652b 3031 2034 2e37  56298310e+01 4.7
-00003fb0: 3838 3833 3033 3065 2b30 3120 5120 372e  8883030e+01 Q 7.
-00003fc0: 3932 3030 3237 3530 652b 3031 2034 2e37  92002750e+01 4.7
-00003fd0: 3239 3739 3339 3065 2b30 312c 2038 2e32  2979390e+01, 8.2
-00003fe0: 3532 3931 3935 3065 2b30 3120 342e 3635  5291950e+01 4.65
-00003ff0: 3939 3835 3430 652b 3031 2051 2037 2e39  998540e+01 Q 7.9
-00004000: 3933 3938 3939 3565 2b30 3120 342e 3337  9398995e+01 4.37
-00004010: 3932 3833 3530 652b 3031 2c20 372e 3730  928350e+01, 7.70
-00004020: 3030 3030 3030 652b 3031 2034 2e31 3030  000000e+01 4.100
-00004030: 3030 3030 3065 2b30 3120 5a22 202f 3e0d  00000e+01 Z" />.
-00004040: 0a20 2020 2020 203c 7061 7468 2064 3d22  .      <path d="
-00004050: 4d20 352e 3930 3030 3030 3030 652b 3031  M 5.90000000e+01
-00004060: 2032 2e33 3030 3030 3030 3065 2b30 3120   2.30000000e+01 
-00004070: 5120 362e 3035 3935 3835 3735 652b 3031  Q 6.05958575e+01
-00004080: 2031 2e39 3236 3330 3437 3065 2b30 312c   1.92630470e+01,
-00004090: 2036 2e32 3231 3836 3433 3065 2b30 3120   6.22186430e+01 
-000040a0: 312e 3537 3433 3035 3730 652b 3031 2051  1.57430570e+01 Q
-000040b0: 2035 2e37 3730 3632 3134 3065 2b30 3120   5.77062140e+01 
-000040c0: 312e 3633 3938 3534 3035 652b 3031 2c20  1.63985405e+01, 
-000040d0: 352e 3332 3134 3233 3330 652b 3031 2031  5.32142330e+01 1
-000040e0: 2e37 3035 3537 3730 3065 2b30 3120 5120  .70557700e+01 Q 
-000040f0: 352e 3631 3036 3932 3330 652b 3031 2032  5.61069230e+01 2
-00004100: 2e30 3030 3533 3835 3065 2b30 312c 2035  .00053850e+01, 5
-00004110: 2e39 3030 3030 3030 3065 2b30 3120 322e  .90000000e+01 2.
-00004120: 3330 3030 3030 3030 652b 3031 205a 2220  30000000e+01 Z" 
-00004130: 2f3e 0d0a 2020 2020 2020 3c70 6174 6820  />..      <path 
-00004140: 643d 224d 2035 2e39 3030 3030 3030 3065  d="M 5.90000000e
-00004150: 2b30 3120 322e 3330 3030 3030 3030 652b  +01 2.30000000e+
-00004160: 3031 2051 2036 2e32 3438 3833 3539 3565  01 Q 6.24883595e
-00004170: 2b30 3120 322e 3332 3232 3235 3935 652b  +01 2.32222595e+
-00004180: 3031 2c20 362e 3538 3838 3330 3330 652b  01, 6.58883030e+
-00004190: 3031 2032 2e34 3337 3031 3639 3065 2b30  01 2.43701690e+0
-000041a0: 3120 5120 362e 3431 3036 3437 3835 652b  1 Q 6.41064785e+
-000041b0: 3031 2031 2e39 3839 3332 3138 3065 2b30  01 1.98932180e+0
-000041c0: 312c 2036 2e32 3231 3836 3433 3065 2b30  1, 6.22186430e+0
-000041d0: 3120 312e 3537 3433 3035 3730 652b 3031  1 1.57430570e+01
-000041e0: 2051 2036 2e30 3539 3538 3537 3565 2b30   Q 6.05958575e+0
-000041f0: 3120 312e 3932 3633 3034 3730 652b 3031  1 1.92630470e+01
-00004200: 2c20 352e 3930 3030 3030 3030 652b 3031  , 5.90000000e+01
-00004210: 2032 2e33 3030 3030 3030 3065 2b30 3120   2.30000000e+01 
-00004220: 5a22 202f 3e0d 0a20 2020 2020 203c 7061  Z" />..      <pa
-00004230: 7468 2064 3d22 4d20 352e 3030 3030 3030  th d="M 5.000000
-00004240: 3030 652b 3031 2032 2e33 3030 3030 3030  00e+01 2.3000000
-00004250: 3065 2b30 3120 5120 352e 3435 3030 3030  0e+01 Q 5.450000
-00004260: 3030 652b 3031 2032 2e33 3030 3030 3030  00e+01 2.3000000
-00004270: 3065 2b30 312c 2035 2e39 3030 3030 3030  0e+01, 5.9000000
-00004280: 3065 2b30 3120 322e 3330 3030 3030 3030  0e+01 2.30000000
-00004290: 652b 3031 2051 2035 2e36 3130 3639 3233  e+01 Q 5.6106923
-000042a0: 3065 2b30 3120 322e 3030 3035 3338 3530  0e+01 2.00053850
-000042b0: 652b 3031 2c20 352e 3332 3134 3233 3330  e+01, 5.32142330
-000042c0: 652b 3031 2031 2e37 3035 3537 3730 3065  e+01 1.70557700e
-000042d0: 2b30 3120 5120 352e 3136 3039 3437 3435  +01 Q 5.16094745
-000042e0: 652b 3031 2032 2e30 3033 3030 3435 3065  e+01 2.00300450e
-000042f0: 2b30 312c 2035 2e30 3030 3030 3030 3065  +01, 5.00000000e
-00004300: 2b30 3120 322e 3330 3030 3030 3030 652b  +01 2.30000000e+
-00004310: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
-00004320: 3c70 6174 6820 643d 224d 2035 2e37 3130  <path d="M 5.710
-00004330: 3734 3938 3065 2b30 3120 382e 3133 3036  74980e+01 8.1306
-00004340: 3838 3730 652b 3031 2051 2036 2e33 3137  8870e+01 Q 6.317
-00004350: 3837 3232 3565 2b30 3120 372e 3934 3538  87225e+01 7.9458
-00004360: 3937 3535 652b 3031 2c20 362e 3932 3038  9755e+01, 6.9208
-00004370: 3837 3130 652b 3031 2037 2e37 3536 3233  8710e+01 7.75623
-00004380: 3833 3065 2b30 3120 5120 362e 3439 3430  830e+01 Q 6.4940
-00004390: 3133 3935 652b 3031 2037 2e35 3031 3033  1395e+01 7.50103
-000043a0: 3838 3065 2b30 312c 2036 2e30 3637 3837  880e+01, 6.06787
-000043b0: 3631 3065 2b30 3120 372e 3234 3236 3636  610e+01 7.242666
-000043c0: 3830 652b 3031 2051 2035 2e38 3838 3737  80e+01 Q 5.88877
-000043d0: 3032 3565 2b30 3120 372e 3638 3733 3836  025e+01 7.687386
-000043e0: 3035 652b 3031 2c20 352e 3731 3037 3439  05e+01, 5.710749
-000043f0: 3830 652b 3031 2038 2e31 3330 3638 3837  80e+01 8.1306887
-00004400: 3065 2b30 3120 5a22 202f 3e0d 0a20 2020  0e+01 Z" />..   
-00004410: 2020 203c 7061 7468 2064 3d22 4d20 322e     <path d="M 2.
-00004420: 3733 3832 3234 3430 652b 3031 2038 2e30  73822440e+01 8.0
-00004430: 3237 3537 3339 3065 2b30 3120 5120 322e  2757390e+01 Q 2.
-00004440: 3335 3332 3330 3935 652b 3031 2037 2e36  35323095e+01 7.6
-00004450: 3434 3232 3631 3065 2b30 312c 2031 2e39  4422610e+01, 1.9
-00004460: 3639 3538 3132 3065 2b30 3120 372e 3235  6958120e+01 7.25
-00004470: 3936 3335 3430 652b 3031 2051 2031 2e38  963540e+01 Q 1.8
-00004480: 3335 3433 3938 3065 2b30 3120 372e 3737  3543980e+01 7.77
-00004490: 3938 3334 3935 652b 3031 2c20 312e 3730  983495e+01, 1.70
-000044a0: 3030 3636 3330 652b 3031 2038 2e32 3938  006630e+01 8.298
-000044b0: 3834 3338 3065 2b30 3120 5120 322e 3231  84380e+01 Q 2.21
-000044c0: 3835 3333 3830 652b 3031 2038 2e31 3632  853380e+01 8.162
-000044d0: 3532 3339 3565 2b30 312c 2032 2e37 3338  52395e+01, 2.738
-000044e0: 3232 3434 3065 2b30 3120 382e 3032 3735  22440e+01 8.0275
-000044f0: 3733 3930 652b 3031 205a 2220 2f3e 0d0a  7390e+01 Z" />..
-00004500: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
-00004510: 2038 2e31 3933 3033 3335 3065 2b30 3120   8.19303350e+01 
-00004520: 382e 3139 3437 3538 3830 652b 3031 2051  8.19475880e+01 Q
-00004530: 2037 2e39 3733 3235 3438 3565 2b30 3120   7.97325485e+01 
-00004540: 372e 3535 3932 3034 3435 652b 3031 2c20  7.55920445e+01, 
-00004550: 372e 3735 3334 3736 3230 652b 3031 2036  7.75347620e+01 6
-00004560: 2e39 3233 3634 3932 3065 2b30 3120 5120  .92364920e+01 Q 
-00004570: 372e 3333 3731 3832 3130 652b 3031 2037  7.33718210e+01 7
-00004580: 2e33 3339 3934 3432 3065 2b30 312c 2036  .33994420e+01, 6
-00004590: 2e39 3230 3838 3731 3065 2b30 3120 372e  .92088710e+01 7.
-000045a0: 3735 3632 3338 3330 652b 3031 2051 2037  75623830e+01 Q 7
-000045b0: 2e35 3536 3936 3033 3065 2b30 3120 372e  .55696030e+01 7.
-000045c0: 3937 3534 3938 3535 652b 3031 2c20 382e  97549855e+01, 8.
-000045d0: 3139 3330 3333 3530 652b 3031 2038 2e31  19303350e+01 8.1
-000045e0: 3934 3735 3838 3065 2b30 3120 5a22 202f  9475880e+01 Z" /
-000045f0: 3e0d 0a20 2020 2020 203c 7061 7468 2064  >..      <path d
-00004600: 3d22 4d20 342e 3130 3030 3030 3930 652b  ="M 4.10000090e+
-00004610: 3031 2032 2e33 3030 3030 3030 3065 2b30  01 2.30000000e+0
-00004620: 3120 5120 342e 3337 3431 3932 3230 652b  1 Q 4.37419220e+
-00004630: 3031 2031 2e39 3830 3836 3831 3065 2b30  01 1.98086810e+0
-00004640: 312c 2034 2e36 3438 3338 3335 3065 2b30  1, 4.64838350e+0
-00004650: 3120 312e 3636 3137 3337 3130 652b 3031  1 1.66173710e+01
-00004660: 2051 2034 2e32 3739 3733 3736 3565 2b30   Q 4.27973765e+0
-00004670: 3120 312e 3536 3431 3237 3135 652b 3031  1 1.56412715e+01
-00004680: 2c20 332e 3931 3130 3931 3830 652b 3031  , 3.91109180e+01
-00004690: 2031 2e34 3636 3531 3831 3065 2b30 3120   1.46651810e+01 
-000046a0: 5120 342e 3030 3535 3436 3335 652b 3031  Q 4.00554635e+01
-000046b0: 2031 2e38 3833 3235 3930 3565 2b30 312c   1.88325905e+01,
-000046c0: 2034 2e31 3030 3030 3039 3065 2b30 3120   4.10000090e+01 
-000046d0: 322e 3330 3030 3030 3030 652b 3031 205a  2.30000000e+01 Z
-000046e0: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
-000046f0: 6820 643d 224d 2033 2e32 3030 3030 3030  h d="M 3.2000000
-00004700: 3065 2b30 3120 322e 3330 3030 3030 3030  0e+01 2.30000000
-00004710: 652b 3031 2051 2033 2e36 3530 3030 3034  e+01 Q 3.6500004
-00004720: 3565 2b30 3120 322e 3330 3030 3030 3030  5e+01 2.30000000
-00004730: 652b 3031 2c20 342e 3130 3030 3030 3930  e+01, 4.10000090
-00004740: 652b 3031 2032 2e33 3030 3030 3030 3065  e+01 2.30000000e
-00004750: 2b30 3120 5120 342e 3030 3535 3436 3335  +01 Q 4.00554635
-00004760: 652b 3031 2031 2e38 3833 3235 3930 3565  e+01 1.88325905e
-00004770: 2b30 312c 2033 2e39 3131 3039 3138 3065  +01, 3.91109180e
-00004780: 2b30 3120 312e 3436 3635 3138 3130 652b  +01 1.46651810e+
-00004790: 3031 2051 2033 2e35 3535 3534 3633 3565  01 Q 3.55554635e
-000047a0: 2b30 3120 312e 3838 3332 3539 3035 652b  +01 1.88325905e+
-000047b0: 3031 2c20 332e 3230 3030 3030 3030 652b  01, 3.20000000e+
-000047c0: 3031 2032 2e33 3030 3030 3030 3065 2b30  01 2.30000000e+0
-000047d0: 3120 5a22 202f 3e0d 0a20 2020 2020 203c  1 Z" />..      <
-000047e0: 7061 7468 2064 3d22 4d20 372e 3735 3334  path d="M 7.7534
-000047f0: 3736 3230 652b 3031 2036 2e39 3233 3634  7620e+01 6.92364
-00004800: 3932 3065 2b30 3120 5120 372e 3137 3738  920e+01 Q 7.1778
-00004810: 3435 3230 652b 3031 2036 2e37 3633 3830  4520e+01 6.76380
-00004820: 3734 3065 2b30 312c 2036 2e36 3030 3938  740e+01, 6.60098
-00004830: 3735 3065 2b30 3120 362e 3630 3338 3136  750e+01 6.603816
-00004840: 3230 652b 3031 2051 2036 2e37 3631 3030  20e+01 Q 6.76100
-00004850: 3231 3065 2b30 3120 372e 3138 3036 3435  210e+01 7.180645
-00004860: 3130 652b 3031 2c20 362e 3932 3038 3837  10e+01, 6.920887
-00004870: 3130 652b 3031 2037 2e37 3536 3233 3833  10e+01 7.7562383
-00004880: 3065 2b30 3120 5120 372e 3333 3731 3832  0e+01 Q 7.337182
-00004890: 3130 652b 3031 2037 2e33 3339 3934 3432  10e+01 7.3399442
-000048a0: 3065 2b30 312c 2037 2e37 3533 3437 3632  0e+01, 7.7534762
-000048b0: 3065 2b30 3120 362e 3932 3336 3439 3230  0e+01 6.92364920
-000048c0: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
-000048d0: 2020 3c70 6174 6820 643d 224d 2037 2e37    <path d="M 7.7
-000048e0: 3533 3437 3632 3065 2b30 3120 362e 3932  5347620e+01 6.92
-000048f0: 3336 3439 3230 652b 3031 2051 2037 2e39  364920e+01 Q 7.9
-00004900: 3434 3036 3734 3065 2b30 3120 362e 3331  4406740e+01 6.31
-00004910: 3937 3134 3130 652b 3031 2c20 382e 3132  971410e+01, 8.12
-00004920: 3937 3836 3930 652b 3031 2035 2e37 3131  978690e+01 5.711
-00004930: 3636 3432 3065 2b30 3120 5120 372e 3638  66420e+01 Q 7.68
-00004940: 3538 3437 3935 652b 3031 2035 2e38 3930  584795e+01 5.890
-00004950: 3332 3233 3065 2b30 312c 2037 2e32 3430  32230e+01, 7.240
-00004960: 3439 3135 3065 2b30 3120 362e 3037 3030  49150e+01 6.0700
-00004970: 3534 3130 652b 3031 2051 2037 2e34 3938  5410e+01 Q 7.498
-00004980: 3537 3233 3565 2b30 3120 362e 3439 3634  57235e+01 6.4964
-00004990: 3835 3830 652b 3031 2c20 372e 3735 3334  8580e+01, 7.7534
-000049a0: 3736 3230 652b 3031 2036 2e39 3233 3634  7620e+01 6.92364
-000049b0: 3932 3065 2b30 3120 5a22 202f 3e0d 0a20  920e+01 Z" />.. 
-000049c0: 2020 2020 203c 7061 7468 2064 3d22 4d20       <path d="M 
-000049d0: 372e 3234 3034 3931 3530 652b 3031 2036  7.24049150e+01 6
-000049e0: 2e30 3730 3035 3431 3065 2b30 3120 5120  .07005410e+01 Q 
-000049f0: 362e 3932 3030 3631 3335 652b 3031 2036  6.92006135e+01 6
-00004a00: 2e33 3337 3037 3139 3565 2b30 312c 2036  .33707195e+01, 6
-00004a10: 2e36 3030 3938 3735 3065 2b30 3120 362e  .60098750e+01 6.
-00004a20: 3630 3338 3136 3230 652b 3031 2051 2037  60381620e+01 Q 7
-00004a30: 2e31 3737 3834 3532 3065 2b30 3120 362e  .17784520e+01 6.
-00004a40: 3736 3338 3037 3430 652b 3031 2c20 372e  76380740e+01, 7.
-00004a50: 3735 3334 3736 3230 652b 3031 2036 2e39  75347620e+01 6.9
-00004a60: 3233 3634 3932 3065 2b30 3120 5120 372e  2364920e+01 Q 7.
-00004a70: 3439 3835 3732 3335 652b 3031 2036 2e34  49857235e+01 6.4
-00004a80: 3936 3438 3538 3065 2b30 312c 2037 2e32  9648580e+01, 7.2
-00004a90: 3430 3439 3135 3065 2b30 3120 362e 3037  4049150e+01 6.07
-00004aa0: 3030 3534 3130 652b 3031 205a 2220 2f3e  005410e+01 Z" />
-00004ab0: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
-00004ac0: 224d 2036 2e36 3030 3938 3735 3065 2b30  "M 6.60098750e+0
-00004ad0: 3120 362e 3630 3338 3136 3230 652b 3031  1 6.60381620e+01
-00004ae0: 2051 2036 2e33 3334 3536 3539 3065 2b30   Q 6.33456590e+0
-00004af0: 3120 362e 3932 3235 3631 3535 652b 3031  1 6.92256155e+01
-00004b00: 2c20 362e 3036 3738 3736 3130 652b 3031  , 6.06787610e+01
-00004b10: 2037 2e32 3432 3636 3638 3065 2b30 3120   7.24266680e+01 
-00004b20: 5120 362e 3439 3430 3133 3935 652b 3031  Q 6.49401395e+01
-00004b30: 2037 2e35 3031 3033 3838 3065 2b30 312c   7.50103880e+01,
-00004b40: 2036 2e39 3230 3838 3731 3065 2b30 3120   6.92088710e+01 
-00004b50: 372e 3735 3632 3338 3330 652b 3031 2051  7.75623830e+01 Q
-00004b60: 2036 2e37 3631 3030 3231 3065 2b30 3120   6.76100210e+01 
-00004b70: 372e 3138 3036 3435 3130 652b 3031 2c20  7.18064510e+01, 
-00004b80: 362e 3630 3039 3837 3530 652b 3031 2036  6.60098750e+01 6
-00004b90: 2e36 3033 3831 3632 3065 2b30 3120 5a22  .60381620e+01 Z"
-00004ba0: 202f 3e0d 0a20 2020 2020 203c 7061 7468   />..      <path
-00004bb0: 2064 3d22 4d20 372e 3236 3031 3133 3330   d="M 7.26011330
-00004bc0: 652b 3031 2031 2e39 3730 3035 3436 3065  e+01 1.97005460e
-00004bd0: 2b30 3120 5120 372e 3634 3437 3033 3130  +01 Q 7.64470310
-00004be0: 652b 3031 2032 2e33 3533 3730 3834 3065  e+01 2.35370840e
-00004bf0: 2b30 312c 2038 2e30 3238 3034 3832 3065  +01, 8.02804820e
-00004c00: 2b30 3120 322e 3733 3837 3032 3330 652b  +01 2.73870230e+
-00004c10: 3031 2051 2038 2e31 3633 3038 3238 3565  01 Q 8.16308285e
-00004c20: 2b30 3120 322e 3231 3930 3932 3730 652b  +01 2.21909270e+
-00004c30: 3031 2c20 382e 3239 3934 3834 3630 652b  01, 8.29948460e+
-00004c40: 3031 2031 2e37 3030 3730 3731 3065 2b30  01 1.70070710e+0
-00004c50: 3120 5120 372e 3738 3033 3934 3330 652b  1 Q 7.78039430e+
-00004c60: 3031 2031 2e38 3335 3939 3832 3565 2b30  01 1.83599825e+0
-00004c70: 312c 2037 2e32 3630 3131 3333 3065 2b30  1, 7.26011330e+0
-00004c80: 3120 312e 3937 3030 3534 3630 652b 3031  1 1.97005460e+01
-00004c90: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
-00004ca0: 6174 6820 643d 224d 2038 2e30 3238 3034  ath d="M 8.02804
-00004cb0: 3832 3065 2b30 3120 322e 3733 3837 3032  820e+01 2.738702
-00004cc0: 3330 652b 3031 2051 2037 2e38 3039 3534  30e+01 Q 7.80954
-00004cd0: 3033 3565 2b30 3120 332e 3037 3034 3631  035e+01 3.070461
-00004ce0: 3230 652b 3031 2c20 372e 3536 3239 3833  20e+01, 7.562983
-00004cf0: 3130 652b 3031 2033 2e34 3131 3136 3937  10e+01 3.4111697
-00004d00: 3065 2b30 3120 5120 382e 3030 3438 3731  0e+01 Q 8.004871
-00004d10: 3835 652b 3031 2033 2e35 3834 3836 3536  85e+01 3.5848656
-00004d20: 3565 2b30 312c 2038 2e34 3134 3730 3938  5e+01, 8.4147098
-00004d30: 3065 2b30 3120 332e 3736 3833 3136 3730  0e+01 3.76831670
-00004d40: 652b 3031 2051 2038 2e32 3232 3635 3734  e+01 Q 8.2226574
-00004d50: 3565 2b30 3120 332e 3235 3332 3939 3335  5e+01 3.25329935
-00004d60: 652b 3031 2c20 382e 3032 3830 3438 3230  e+01, 8.02804820
-00004d70: 652b 3031 2032 2e37 3338 3730 3233 3065  e+01 2.73870230e
-00004d80: 2b30 3120 5a22 202f 3e0d 0a20 2020 2020  +01 Z" />..     
-00004d90: 203c 7061 7468 2064 3d22 4d20 342e 3634   <path d="M 4.64
-00004da0: 3833 3833 3530 652b 3031 2031 2e36 3631  838350e+01 1.661
-00004db0: 3733 3731 3065 2b30 3120 5120 342e 3832  73710e+01 Q 4.82
-00004dc0: 3432 3134 3235 652b 3031 2031 2e39 3830  421425e+01 1.980
-00004dd0: 3733 3335 3565 2b30 312c 2035 2e30 3030  73355e+01, 5.000
-00004de0: 3030 3030 3065 2b30 3120 322e 3330 3030  00000e+01 2.3000
-00004df0: 3030 3030 652b 3031 2051 2035 2e31 3630  0000e+01 Q 5.160
-00004e00: 3934 3734 3565 2b30 3120 322e 3030 3330  94745e+01 2.0030
-00004e10: 3034 3530 652b 3031 2c20 352e 3332 3134  0450e+01, 5.3214
-00004e20: 3233 3330 652b 3031 2031 2e37 3035 3537  2330e+01 1.70557
-00004e30: 3730 3065 2b30 3120 5120 342e 3938 3439  700e+01 Q 4.9849
-00004e40: 3931 3630 652b 3031 2031 2e36 3833 3937  9160e+01 1.68397
-00004e50: 3631 3065 2b30 312c 2034 2e36 3438 3338  610e+01, 4.64838
-00004e60: 3335 3065 2b30 3120 312e 3636 3137 3337  350e+01 1.661737
-00004e70: 3130 652b 3031 205a 2220 2f3e 0d0a 2020  10e+01 Z" />..  
-00004e80: 2020 2020 3c70 6174 6820 643d 224d 2034      <path d="M 4
-00004e90: 2e31 3030 3030 3039 3065 2b30 3120 322e  .10000090e+01 2.
-00004ea0: 3330 3030 3030 3030 652b 3031 2051 2034  30000000e+01 Q 4
-00004eb0: 2e35 3530 3030 3034 3565 2b30 3120 322e  .55000045e+01 2.
-00004ec0: 3330 3030 3030 3030 652b 3031 2c20 352e  30000000e+01, 5.
-00004ed0: 3030 3030 3030 3030 652b 3031 2032 2e33  00000000e+01 2.3
-00004ee0: 3030 3030 3030 3065 2b30 3120 5120 342e  0000000e+01 Q 4.
-00004ef0: 3832 3432 3134 3235 652b 3031 2031 2e39  82421425e+01 1.9
-00004f00: 3830 3733 3335 3565 2b30 312c 2034 2e36  8073355e+01, 4.6
-00004f10: 3438 3338 3335 3065 2b30 3120 312e 3636  4838350e+01 1.66
-00004f20: 3137 3337 3130 652b 3031 2051 2034 2e33  173710e+01 Q 4.3
-00004f30: 3734 3139 3232 3065 2b30 3120 312e 3938  7419220e+01 1.98
-00004f40: 3038 3638 3130 652b 3031 2c20 342e 3130  086810e+01, 4.10
-00004f50: 3030 3030 3930 652b 3031 2032 2e33 3030  000090e+01 2.300
-00004f60: 3030 3030 3065 2b30 3120 5a22 202f 3e0d  00000e+01 Z" />.
-00004f70: 0a20 2020 2020 203c 7061 7468 2064 3d22  .      <path d="
-00004f80: 4d20 372e 3137 3237 3932 3630 652b 3031  M 7.17279260e+01
-00004f90: 2032 2e38 3237 3230 3833 3065 2b30 3120   2.82720830e+01 
-00004fa0: 5120 372e 3631 3134 3834 3130 652b 3031  Q 7.61148410e+01
-00004fb0: 2032 2e37 3732 3039 3935 3065 2b30 312c   2.77209950e+01,
-00004fc0: 2038 2e30 3238 3034 3832 3065 2b30 3120   8.02804820e+01 
-00004fd0: 322e 3733 3837 3032 3330 652b 3031 2051  2.73870230e+01 Q
-00004fe0: 2037 2e36 3434 3730 3331 3065 2b30 3120   7.64470310e+01 
-00004ff0: 322e 3335 3337 3038 3430 652b 3031 2c20  2.35370840e+01, 
-00005000: 372e 3236 3031 3133 3330 652b 3031 2031  7.26011330e+01 1
-00005010: 2e39 3730 3035 3436 3065 2b30 3120 5120  .97005460e+01 Q 
-00005020: 372e 3232 3734 3233 3530 652b 3031 2032  7.22742350e+01 2
-00005030: 2e33 3837 3539 3433 3065 2b30 312c 2037  .38759430e+01, 7
-00005040: 2e31 3732 3739 3236 3065 2b30 3120 322e  .17279260e+01 2.
-00005050: 3832 3732 3038 3330 652b 3031 205a 2220  82720830e+01 Z" 
-00005060: 2f3e 0d0a 2020 2020 2020 3c70 6174 6820  />..      <path 
-00005070: 643d 224d 2037 2e31 3732 3739 3236 3065  d="M 7.17279260e
-00005080: 2b30 3120 322e 3832 3732 3038 3330 652b  +01 2.82720830e+
-00005090: 3031 2051 2037 2e34 3037 3230 3132 3065  01 Q 7.40720120e
-000050a0: 2b30 3120 332e 3039 3437 3533 3130 652b  +01 3.09475310e+
-000050b0: 3031 2c20 372e 3536 3239 3833 3130 652b  01, 7.56298310e+
-000050c0: 3031 2033 2e34 3131 3136 3937 3065 2b30  01 3.41116970e+0
-000050d0: 3120 5120 372e 3830 3935 3430 3335 652b  1 Q 7.80954035e+
-000050e0: 3031 2033 2e30 3730 3436 3132 3065 2b30  01 3.07046120e+0
-000050f0: 312c 2038 2e30 3238 3034 3832 3065 2b30  1, 8.02804820e+0
-00005100: 3120 322e 3733 3837 3032 3330 652b 3031  1 2.73870230e+01
-00005110: 2051 2037 2e36 3131 3438 3431 3065 2b30   Q 7.61148410e+0
-00005120: 3120 322e 3737 3230 3939 3530 652b 3031  1 2.77209950e+01
-00005130: 2c20 372e 3137 3237 3932 3630 652b 3031  , 7.17279260e+01
-00005140: 2032 2e38 3237 3230 3833 3065 2b30 3120   2.82720830e+01 
-00005150: 5a22 202f 3e0d 0a20 2020 2020 203c 7061  Z" />..      <pa
-00005160: 7468 2064 3d22 4d20 362e 3538 3838 3330  th d="M 6.588830
-00005170: 3330 652b 3031 2032 2e34 3337 3031 3639  30e+01 2.4370169
-00005180: 3065 2b30 3120 5120 362e 3932 3930 3530  0e+01 Q 6.929050
-00005190: 3535 652b 3031 2032 2e31 3839 3833 3233  55e+01 2.1898323
-000051a0: 3565 2b30 312c 2037 2e32 3630 3131 3333  5e+01, 7.2601133
-000051b0: 3065 2b30 3120 312e 3937 3030 3534 3630  0e+01 1.97005460
-000051c0: 652b 3031 2051 2036 2e37 3431 3339 3536  e+01 Q 6.7413956
-000051d0: 3065 2b30 3120 312e 3736 3937 3132 3830  0e+01 1.76971280
-000051e0: 652b 3031 2c20 362e 3232 3138 3634 3330  e+01, 6.22186430
-000051f0: 652b 3031 2031 2e35 3734 3330 3537 3065  e+01 1.57430570e
-00005200: 2b30 3120 5120 362e 3431 3036 3437 3835  +01 Q 6.41064785
-00005210: 652b 3031 2031 2e39 3839 3332 3138 3065  e+01 1.98932180e
-00005220: 2b30 312c 2036 2e35 3838 3833 3033 3065  +01, 6.58883030e
-00005230: 2b30 3120 322e 3433 3730 3136 3930 652b  +01 2.43701690e+
-00005240: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
-00005250: 3c70 6174 6820 643d 224d 2036 2e35 3838  <path d="M 6.588
-00005260: 3833 3033 3065 2b30 3120 322e 3433 3730  83030e+01 2.4370
-00005270: 3136 3930 652b 3031 2051 2036 2e39 3035  1690e+01 Q 6.905
-00005280: 3234 3639 3065 2b30 3120 322e 3539 3237  24690e+01 2.5927
-00005290: 3938 3830 652b 3031 2c20 372e 3137 3237  9880e+01, 7.1727
-000052a0: 3932 3630 652b 3031 2032 2e38 3237 3230  9260e+01 2.82720
-000052b0: 3833 3065 2b30 3120 5120 372e 3232 3734  830e+01 Q 7.2274
-000052c0: 3233 3530 652b 3031 2032 2e33 3837 3539  2350e+01 2.38759
-000052d0: 3433 3065 2b30 312c 2037 2e32 3630 3131  430e+01, 7.26011
-000052e0: 3333 3065 2b30 3120 312e 3937 3030 3534  330e+01 1.970054
-000052f0: 3630 652b 3031 2051 2036 2e39 3239 3035  60e+01 Q 6.92905
-00005300: 3035 3565 2b30 3120 322e 3138 3938 3332  055e+01 2.189832
-00005310: 3335 652b 3031 2c20 362e 3538 3838 3330  35e+01, 6.588830
-00005320: 3330 652b 3031 2032 2e34 3337 3031 3639  30e+01 2.4370169
-00005330: 3065 2b30 3120 5a22 202f 3e0d 0a20 2020  0e+01 Z" />..   
-00005340: 2020 203c 7061 7468 2064 3d22 4d20 372e     <path d="M 7.
-00005350: 3536 3239 3833 3130 652b 3031 2034 2e37  56298310e+01 4.7
-00005360: 3838 3833 3033 3065 2b30 3120 5120 372e  8883030e+01 Q 7.
-00005370: 3836 3136 3333 3235 652b 3031 2035 2e32  86163325e+01 5.2
-00005380: 3536 3531 3830 3065 2b30 312c 2038 2e31  5651800e+01, 8.1
-00005390: 3239 3738 3639 3065 2b30 3120 352e 3731  2978690e+01 5.71
-000053a0: 3136 3634 3230 652b 3031 2051 2038 2e31  166420e+01 Q 8.1
-000053b0: 3931 3436 3334 3565 2b30 3120 352e 3138  9146345e+01 5.18
-000053c0: 3730 3331 3730 652b 3031 2c20 382e 3235  703170e+01, 8.25
-000053d0: 3239 3139 3530 652b 3031 2034 2e36 3539  291950e+01 4.659
-000053e0: 3938 3534 3065 2b30 3120 5120 372e 3932  98540e+01 Q 7.92
-000053f0: 3030 3237 3530 652b 3031 2034 2e37 3239  002750e+01 4.729
-00005400: 3739 3339 3065 2b30 312c 2037 2e35 3632  79390e+01, 7.562
-00005410: 3938 3331 3065 2b30 3120 342e 3738 3838  98310e+01 4.7888
-00005420: 3330 3330 652b 3031 205a 2220 2f3e 0d0a  3030e+01 Z" />..
-00005430: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
-00005440: 2037 2e31 3732 3739 3137 3065 2b30 3120   7.17279170e+01 
-00005450: 352e 3337 3237 3932 3630 652b 3031 2051  5.37279260e+01 Q
-00005460: 2037 2e32 3137 3637 3936 3565 2b30 3120   7.21767965e+01 
-00005470: 352e 3733 3131 3633 3135 652b 3031 2c20  5.73116315e+01, 
-00005480: 372e 3234 3034 3931 3530 652b 3031 2036  7.24049150e+01 6
-00005490: 2e30 3730 3035 3431 3065 2b30 3120 5120  .07005410e+01 Q 
-000054a0: 372e 3638 3538 3437 3935 652b 3031 2035  7.68584795e+01 5
-000054b0: 2e38 3930 3332 3233 3065 2b30 312c 2038  .89032230e+01, 8
-000054c0: 2e31 3239 3738 3639 3065 2b30 3120 352e  .12978690e+01 5.
-000054d0: 3731 3136 3634 3230 652b 3031 2051 2037  71166420e+01 Q 7
-000054e0: 2e36 3632 3337 3836 3565 2b30 3120 352e  .66237865e+01 5.
-000054f0: 3535 3231 3531 3335 652b 3031 2c20 372e  55215135e+01, 7.
-00005500: 3137 3237 3931 3730 652b 3031 2035 2e33  17279170e+01 5.3
-00005510: 3732 3739 3236 3065 2b30 3120 5a22 202f  7279260e+01 Z" /
-00005520: 3e0d 0a20 2020 2020 203c 7061 7468 2064  >..      <path d
-00005530: 3d22 4d20 372e 3536 3239 3833 3130 652b  ="M 7.56298310e+
-00005540: 3031 2034 2e37 3838 3833 3033 3065 2b30  01 4.78883030e+0
-00005550: 3120 5120 372e 3430 3732 3031 3230 652b  1 Q 7.40720120e+
-00005560: 3031 2035 2e31 3035 3234 3639 3065 2b30  01 5.10524690e+0
-00005570: 312c 2037 2e31 3732 3739 3137 3065 2b30  1, 7.17279170e+0
-00005580: 3120 352e 3337 3237 3932 3630 652b 3031  1 5.37279260e+01
-00005590: 2051 2037 2e36 3632 3337 3836 3565 2b30   Q 7.66237865e+0
-000055a0: 3120 352e 3535 3231 3531 3335 652b 3031  1 5.55215135e+01
-000055b0: 2c20 382e 3132 3937 3836 3930 652b 3031  , 8.12978690e+01
-000055c0: 2035 2e37 3131 3636 3432 3065 2b30 3120   5.71166420e+01 
-000055d0: 5120 372e 3836 3136 3333 3235 652b 3031  Q 7.86163325e+01
-000055e0: 2035 2e32 3536 3531 3830 3065 2b30 312c   5.25651800e+01,
-000055f0: 2037 2e35 3632 3938 3331 3065 2b30 3120   7.56298310e+01 
-00005600: 342e 3738 3838 3330 3330 652b 3031 205a  4.78883030e+01 Z
-00005610: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
-00005620: 6820 643d 224d 2037 2e32 3430 3439 3135  h d="M 7.2404915
-00005630: 3065 2b30 3120 362e 3037 3030 3534 3130  0e+01 6.07005410
-00005640: 652b 3031 2051 2036 2e39 3231 3539 3435  e+01 Q 6.9215945
-00005650: 3065 2b30 3120 352e 3933 3130 3834 3635  0e+01 5.93108465
-00005660: 652b 3031 2c20 362e 3538 3838 3330 3330  e+01, 6.58883030
-00005670: 652b 3031 2035 2e37 3632 3938 3331 3065  e+01 5.76298310e
-00005680: 2b30 3120 5120 362e 3630 3338 3435 3930  +01 Q 6.60384590
-00005690: 652b 3031 2036 2e31 3935 3030 3234 3565  e+01 6.19500245e
-000056a0: 2b30 312c 2036 2e36 3030 3938 3735 3065  +01, 6.60098750e
-000056b0: 2b30 3120 362e 3630 3338 3136 3230 652b  +01 6.60381620e+
-000056c0: 3031 2051 2036 2e39 3230 3036 3133 3565  01 Q 6.92006135e
-000056d0: 2b30 3120 362e 3333 3730 3731 3935 652b  +01 6.33707195e+
-000056e0: 3031 2c20 372e 3234 3034 3931 3530 652b  01, 7.24049150e+
-000056f0: 3031 2036 2e30 3730 3035 3431 3065 2b30  01 6.07005410e+0
-00005700: 3120 5a22 202f 3e0d 0a20 2020 2020 203c  1 Z" />..      <
-00005710: 7061 7468 2064 3d22 4d20 372e 3137 3237  path d="M 7.1727
-00005720: 3931 3730 652b 3031 2035 2e33 3732 3739  9170e+01 5.37279
-00005730: 3236 3065 2b30 3120 5120 362e 3930 3532  260e+01 Q 6.9052
-00005740: 3436 3930 652b 3031 2035 2e36 3037 3230  4690e+01 5.60720
-00005750: 3132 3065 2b30 312c 2036 2e35 3838 3833  120e+01, 6.58883
-00005760: 3033 3065 2b30 3120 352e 3736 3239 3833  030e+01 5.762983
-00005770: 3130 652b 3031 2051 2036 2e39 3231 3539  10e+01 Q 6.92159
-00005780: 3435 3065 2b30 3120 352e 3933 3130 3834  450e+01 5.931084
-00005790: 3635 652b 3031 2c20 372e 3234 3034 3931  65e+01, 7.240491
-000057a0: 3530 652b 3031 2036 2e30 3730 3035 3431  50e+01 6.0700541
-000057b0: 3065 2b30 3120 5120 372e 3231 3736 3739  0e+01 Q 7.217679
-000057c0: 3635 652b 3031 2035 2e37 3331 3136 3331  65e+01 5.7311631
-000057d0: 3565 2b30 312c 2037 2e31 3732 3739 3137  5e+01, 7.1727917
-000057e0: 3065 2b30 3120 352e 3337 3237 3932 3630  0e+01 5.37279260
-000057f0: 652b 3031 205a 2220 2f3e 0d0a 2020 203c  e+01 Z" />..   <
-00005800: 2f67 3e0d 0a20 2020 3c67 2069 643d 224e  /g>..   <g id="N
-00005810: 6f64 6573 2220 6669 6c6c 3d22 2361 3935  odes" fill="#a95
-00005820: 6535 6522 3e0d 0a20 2020 2020 203c 6369  e5e">..      <ci
-00005830: 7263 6c65 2063 783d 2238 2e37 3530 3030  rcle cx="8.75000
-00005840: 3033 3065 2b30 3122 2063 793d 2235 2e30  030e+01" cy="5.0
-00005850: 3030 3030 3030 3065 2b30 3022 2072 3d22  0000000e+00" r="
-00005860: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-00005870: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-00005880: 6972 636c 6520 6378 3d22 372e 3939 3939  ircle cx="7.9999
-00005890: 3939 3730 652b 3031 2220 6379 3d22 352e  9970e+01" cy="5.
-000058a0: 3030 3030 3030 3030 652b 3030 2220 723d  00000000e+00" r=
-000058b0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-000058c0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-000058d0: 6369 7263 6c65 2063 783d 2237 2e32 3530  circle cx="7.250
-000058e0: 3030 3030 3065 2b30 3122 2063 793d 2235  00000e+01" cy="5
-000058f0: 2e30 3030 3030 3030 3065 2b30 3022 2072  .00000000e+00" r
-00005900: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-00005910: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-00005920: 3c63 6972 636c 6520 6378 3d22 362e 3530  <circle cx="6.50
-00005930: 3030 3030 3330 652b 3031 2220 6379 3d22  000030e+01" cy="
-00005940: 352e 3030 3030 3030 3030 652b 3030 2220  5.00000000e+00" 
-00005950: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-00005960: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-00005970: 203c 6369 7263 6c65 2063 783d 2235 2e37   <circle cx="5.7
-00005980: 3530 3030 3135 3065 2b30 3122 2063 793d  5000150e+01" cy=
-00005990: 2235 2e30 3030 3030 3030 3065 2b30 3022  "5.00000000e+00"
-000059a0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-000059b0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-000059c0: 2020 3c63 6972 636c 6520 6378 3d22 352e    <circle cx="5.
-000059d0: 3030 3030 3031 3830 652b 3031 2220 6379  00000180e+01" cy
-000059e0: 3d22 352e 3030 3030 3030 3030 652b 3030  ="5.00000000e+00
-000059f0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-00005a00: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-00005a10: 2020 203c 6369 7263 6c65 2063 783d 2234     <circle cx="4
-00005a20: 2e32 3530 3030 3231 3065 2b30 3122 2063  .25000210e+01" c
-00005a30: 793d 2235 2e30 3030 3030 3030 3065 2b30  y="5.00000000e+0
-00005a40: 3022 2072 3d22 302e 3533 3638 3130 3436  0" r="0.53681046
-00005a50: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-00005a60: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00005a70: 332e 3530 3030 3031 3530 652b 3031 2220  3.50000150e+01" 
-00005a80: 6379 3d22 352e 3030 3030 3030 3030 652b  cy="5.00000000e+
-00005a90: 3030 2220 723d 2230 2e35 3336 3831 3034  00" r="0.5368104
-00005aa0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-00005ab0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00005ac0: 2232 2e37 3530 3030 3039 3065 2b30 3122  "2.75000090e+01"
-00005ad0: 2063 793d 2235 2e30 3030 3030 3030 3065   cy="5.00000000e
-00005ae0: 2b30 3022 2072 3d22 302e 3533 3638 3130  +00" r="0.536810
-00005af0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-00005b00: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00005b10: 3d22 322e 3030 3030 3030 3330 652b 3031  ="2.00000030e+01
-00005b20: 2220 6379 3d22 352e 3030 3030 3030 3030  " cy="5.00000000
-00005b30: 652b 3030 2220 723d 2230 2e35 3336 3831  e+00" r="0.53681
-00005b40: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-00005b50: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00005b60: 783d 2231 2e32 3530 3030 3033 3365 2b30  x="1.25000033e+0
-00005b70: 3122 2063 793d 2235 2e30 3030 3030 3030  1" cy="5.0000000
-00005b80: 3065 2b30 3022 2072 3d22 302e 3533 3638  0e+00" r="0.5368
-00005b90: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-00005ba0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00005bb0: 6378 3d22 342e 3333 3233 3134 3330 652b  cx="4.33231430e+
-00005bc0: 3031 2220 6379 3d22 372e 3730 3030 3030  01" cy="7.700000
-00005bd0: 3030 652b 3031 2220 723d 2230 2e35 3336  00e+01" r="0.536
-00005be0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-00005bf0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00005c00: 2063 783d 2234 2e35 3635 3335 3736 3065   cx="4.56535760e
-00005c10: 2b30 3122 2063 793d 2237 2e36 3535 3534  +01" cy="7.65554
-00005c20: 3831 3065 2b30 3122 2072 3d22 302e 3533  810e+01" r="0.53
-00005c30: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-00005c40: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00005c50: 6520 6378 3d22 342e 3738 3838 3330 3330  e cx="4.78883030
-00005c60: 652b 3031 2220 6379 3d22 372e 3536 3239  e+01" cy="7.5629
-00005c70: 3833 3130 652b 3031 2220 723d 2230 2e35  8310e+01" r="0.5
-00005c80: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-00005c90: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00005ca0: 6c65 2063 783d 2235 2e30 3036 3438 3435  le cx="5.0064845
-00005cb0: 3065 2b30 3122 2063 793d 2237 2e34 3732  0e+01" cy="7.472
-00005cc0: 3832 3734 3065 2b30 3122 2072 3d22 302e  82740e+01" r="0.
-00005cd0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-00005ce0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00005cf0: 636c 6520 6378 3d22 352e 3230 3430 3039  cle cx="5.204009
-00005d00: 3330 652b 3031 2220 6379 3d22 372e 3334  30e+01" cy="7.34
-00005d10: 3135 3735 3030 652b 3031 2220 723d 2230  157500e+01" r="0
-00005d20: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-00005d30: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00005d40: 7263 6c65 2063 783d 2235 2e33 3732 3739  rcle cx="5.37279
-00005d50: 3137 3065 2b30 3122 2063 793d 2237 2e31  170e+01" cy="7.1
-00005d60: 3732 3739 3236 3065 2b30 3122 2072 3d22  7279260e+01" r="
-00005d70: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-00005d80: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-00005d90: 6972 636c 6520 6378 3d22 352e 3534 3135  ircle cx="5.5415
-00005da0: 3735 3030 652b 3031 2220 6379 3d22 372e  7500e+01" cy="7.
-00005db0: 3030 3430 3039 3330 652b 3031 2220 723d  00400930e+01" r=
-00005dc0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-00005dd0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-00005de0: 6369 7263 6c65 2063 783d 2235 2e36 3732  circle cx="5.672
-00005df0: 3832 3734 3065 2b30 3122 2063 793d 2236  82740e+01" cy="6
-00005e00: 2e38 3036 3438 3435 3065 2b30 3122 2072  .80648450e+01" r
-00005e10: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-00005e20: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-00005e30: 3c63 6972 636c 6520 6378 3d22 352e 3736  <circle cx="5.76
-00005e40: 3239 3833 3130 652b 3031 2220 6379 3d22  298310e+01" cy="
-00005e50: 362e 3538 3838 3330 3330 652b 3031 2220  6.58883030e+01" 
-00005e60: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-00005e70: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-00005e80: 203c 6369 7263 6c65 2063 783d 2235 2e38   <circle cx="5.8
-00005e90: 3535 3534 3831 3065 2b30 3122 2063 793d  5554810e+01" cy=
-00005ea0: 2236 2e33 3635 3335 3736 3065 2b30 3122  "6.36535760e+01"
-00005eb0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-00005ec0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-00005ed0: 2020 3c63 6972 636c 6520 6378 3d22 352e    <circle cx="5.
-00005ee0: 3930 3030 3030 3030 652b 3031 2220 6379  90000000e+01" cy
-00005ef0: 3d22 362e 3133 3233 3134 3330 652b 3031  ="6.13231430e+01
-00005f00: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-00005f10: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-00005f20: 2020 203c 6369 7263 6c65 2063 783d 2239     <circle cx="9
-00005f30: 2e35 3030 3030 3030 3065 2b30 3122 2063  .50000000e+01" c
-00005f40: 793d 2238 2e37 3530 3030 3030 3365 2b30  y="8.75000003e+0
-00005f50: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-00005f60: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-00005f70: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00005f80: 392e 3530 3030 3030 3030 652b 3031 2220  9.50000000e+01" 
-00005f90: 6379 3d22 372e 3939 3939 3939 3730 652b  cy="7.99999970e+
-00005fa0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-00005fb0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-00005fc0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00005fd0: 2239 2e35 3030 3030 3030 3065 2b30 3122  "9.50000000e+01"
-00005fe0: 2063 793d 2237 2e32 3530 3030 3030 3065   cy="7.25000000e
-00005ff0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-00006000: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-00006010: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00006020: 3d22 392e 3530 3030 3030 3030 652b 3031  ="9.50000000e+01
-00006030: 2220 6379 3d22 362e 3530 3030 3030 3330  " cy="6.50000030
-00006040: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-00006050: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-00006060: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00006070: 783d 2239 2e35 3030 3030 3030 3065 2b30  x="9.50000000e+0
-00006080: 3122 2063 793d 2235 2e37 3530 3030 3135  1" cy="5.7500015
-00006090: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-000060a0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-000060b0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-000060c0: 6378 3d22 392e 3530 3030 3030 3030 652b  cx="9.50000000e+
-000060d0: 3031 2220 6379 3d22 352e 3030 3030 3031  01" cy="5.000001
-000060e0: 3830 652b 3031 2220 723d 2230 2e35 3336  80e+01" r="0.536
-000060f0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-00006100: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00006110: 2063 783d 2239 2e35 3030 3030 3030 3065   cx="9.50000000e
-00006120: 2b30 3122 2063 793d 2234 2e32 3530 3030  +01" cy="4.25000
-00006130: 3231 3065 2b30 3122 2072 3d22 302e 3533  210e+01" r="0.53
-00006140: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-00006150: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00006160: 6520 6378 3d22 392e 3530 3030 3030 3030  e cx="9.50000000
-00006170: 652b 3031 2220 6379 3d22 332e 3530 3030  e+01" cy="3.5000
-00006180: 3031 3530 652b 3031 2220 723d 2230 2e35  0150e+01" r="0.5
-00006190: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-000061a0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-000061b0: 6c65 2063 783d 2239 2e35 3030 3030 3030  le cx="9.5000000
-000061c0: 3065 2b30 3122 2063 793d 2232 2e37 3530  0e+01" cy="2.750
-000061d0: 3030 3039 3065 2b30 3122 2072 3d22 302e  00090e+01" r="0.
-000061e0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-000061f0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00006200: 636c 6520 6378 3d22 392e 3530 3030 3030  cle cx="9.500000
-00006210: 3030 652b 3031 2220 6379 3d22 322e 3030  00e+01" cy="2.00
-00006220: 3030 3030 3330 652b 3031 2220 723d 2230  000030e+01" r="0
-00006230: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-00006240: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00006250: 7263 6c65 2063 783d 2239 2e35 3030 3030  rcle cx="9.50000
-00006260: 3030 3065 2b30 3122 2063 793d 2231 2e32  000e+01" cy="1.2
-00006270: 3530 3030 3036 3065 2b30 3122 2072 3d22  5000060e+01" r="
-00006280: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-00006290: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-000062a0: 6972 636c 6520 6378 3d22 322e 3330 3030  ircle cx="2.3000
-000062b0: 3030 3030 652b 3031 2220 6379 3d22 362e  0000e+01" cy="6.
-000062c0: 3133 3233 3134 3330 652b 3031 2220 723d  13231430e+01" r=
-000062d0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-000062e0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-000062f0: 6369 7263 6c65 2063 783d 2232 2e33 3434  circle cx="2.344
-00006300: 3435 3139 3065 2b30 3122 2063 793d 2236  45190e+01" cy="6
-00006310: 2e33 3635 3335 3736 3065 2b30 3122 2072  .36535760e+01" r
-00006320: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-00006330: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-00006340: 3c63 6972 636c 6520 6378 3d22 322e 3433  <circle cx="2.43
-00006350: 3730 3136 3930 652b 3031 2220 6379 3d22  701690e+01" cy="
-00006360: 362e 3538 3838 3330 3330 652b 3031 2220  6.58883030e+01" 
-00006370: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-00006380: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-00006390: 203c 6369 7263 6c65 2063 783d 2232 2e35   <circle cx="2.5
-000063a0: 3237 3137 3236 3065 2b30 3122 2063 793d  2717260e+01" cy=
-000063b0: 2236 2e38 3036 3438 3435 3065 2b30 3122  "6.80648450e+01"
-000063c0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-000063d0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-000063e0: 2020 3c63 6972 636c 6520 6378 3d22 322e    <circle cx="2.
-000063f0: 3635 3834 3235 3030 652b 3031 2220 6379  65842500e+01" cy
-00006400: 3d22 372e 3030 3430 3039 3330 652b 3031  ="7.00400930e+01
-00006410: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-00006420: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-00006430: 2020 203c 6369 7263 6c65 2063 783d 2232     <circle cx="2
-00006440: 2e38 3237 3230 3734 3065 2b30 3122 2063  .82720740e+01" c
-00006450: 793d 2237 2e31 3732 3739 3137 3065 2b30  y="7.17279170e+0
-00006460: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-00006470: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-00006480: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00006490: 322e 3939 3539 3930 3730 652b 3031 2220  2.99599070e+01" 
-000064a0: 6379 3d22 372e 3334 3135 3735 3030 652b  cy="7.34157500e+
-000064b0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-000064c0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-000064d0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-000064e0: 2233 2e31 3933 3531 3535 3065 2b30 3122  "3.19351550e+01"
-000064f0: 2063 793d 2237 2e34 3732 3832 3734 3065   cy="7.47282740e
-00006500: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-00006510: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-00006520: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00006530: 3d22 332e 3431 3131 3639 3730 652b 3031  ="3.41116970e+01
-00006540: 2220 6379 3d22 372e 3536 3239 3833 3130  " cy="7.56298310
-00006550: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-00006560: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-00006570: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00006580: 783d 2233 2e36 3334 3634 3234 3065 2b30  x="3.63464240e+0
-00006590: 3122 2063 793d 2237 2e36 3535 3534 3831  1" cy="7.6555481
-000065a0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-000065b0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-000065c0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-000065d0: 6378 3d22 332e 3836 3736 3835 3730 652b  cx="3.86768570e+
-000065e0: 3031 2220 6379 3d22 372e 3730 3030 3030  01" cy="7.700000
-000065f0: 3030 652b 3031 2220 723d 2230 2e35 3336  00e+01" r="0.536
-00006600: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-00006610: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00006620: 2063 783d 2231 2e32 3439 3939 3939 3765   cx="1.24999997e
-00006630: 2b30 3122 2063 793d 2239 2e35 3030 3030  +01" cy="9.50000
-00006640: 3030 3065 2b30 3122 2072 3d22 302e 3533  000e+01" r="0.53
-00006650: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-00006660: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00006670: 6520 6378 3d22 322e 3030 3030 3030 3330  e cx="2.00000030
-00006680: 652b 3031 2220 6379 3d22 392e 3530 3030  e+01" cy="9.5000
-00006690: 3030 3030 652b 3031 2220 723d 2230 2e35  0000e+01" r="0.5
-000066a0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-000066b0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-000066c0: 6c65 2063 783d 2232 2e37 3530 3030 3030  le cx="2.7500000
-000066d0: 3065 2b30 3122 2063 793d 2239 2e35 3030  0e+01" cy="9.500
-000066e0: 3030 3030 3065 2b30 3122 2072 3d22 302e  00000e+01" r="0.
-000066f0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-00006700: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00006710: 636c 6520 6378 3d22 332e 3439 3939 3939  cle cx="3.499999
-00006720: 3730 652b 3031 2220 6379 3d22 392e 3530  70e+01" cy="9.50
-00006730: 3030 3030 3030 652b 3031 2220 723d 2230  000000e+01" r="0
-00006740: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-00006750: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00006760: 7263 6c65 2063 783d 2234 2e32 3439 3939  rcle cx="4.24999
-00006770: 3835 3065 2b30 3122 2063 793d 2239 2e35  850e+01" cy="9.5
-00006780: 3030 3030 3030 3065 2b30 3122 2072 3d22  0000000e+01" r="
-00006790: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-000067a0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-000067b0: 6972 636c 6520 6378 3d22 342e 3939 3939  ircle cx="4.9999
-000067c0: 3938 3230 652b 3031 2220 6379 3d22 392e  9820e+01" cy="9.
-000067d0: 3530 3030 3030 3030 652b 3031 2220 723d  50000000e+01" r=
-000067e0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-000067f0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-00006800: 6369 7263 6c65 2063 783d 2235 2e37 3439  circle cx="5.749
-00006810: 3939 3739 3065 2b30 3122 2063 793d 2239  99790e+01" cy="9
-00006820: 2e35 3030 3030 3030 3065 2b30 3122 2072  .50000000e+01" r
-00006830: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-00006840: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-00006850: 3c63 6972 636c 6520 6378 3d22 362e 3439  <circle cx="6.49
-00006860: 3939 3938 3530 652b 3031 2220 6379 3d22  999850e+01" cy="
-00006870: 392e 3530 3030 3030 3030 652b 3031 2220  9.50000000e+01" 
-00006880: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-00006890: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-000068a0: 203c 6369 7263 6c65 2063 783d 2237 2e32   <circle cx="7.2
-000068b0: 3439 3939 3931 3065 2b30 3122 2063 793d  4999910e+01" cy=
-000068c0: 2239 2e35 3030 3030 3030 3065 2b30 3122  "9.50000000e+01"
-000068d0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-000068e0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-000068f0: 2020 3c63 6972 636c 6520 6378 3d22 372e    <circle cx="7.
-00006900: 3939 3939 3939 3730 652b 3031 2220 6379  99999970e+01" cy
-00006910: 3d22 392e 3530 3030 3030 3030 652b 3031  ="9.50000000e+01
-00006920: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-00006930: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-00006940: 2020 203c 6369 7263 6c65 2063 783d 2238     <circle cx="8
-00006950: 2e37 3439 3939 3934 3065 2b30 3122 2063  .74999940e+01" c
-00006960: 793d 2239 2e35 3030 3030 3030 3065 2b30  y="9.50000000e+0
-00006970: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-00006980: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-00006990: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-000069a0: 322e 3330 3030 3030 3030 652b 3031 2220  2.30000000e+01" 
-000069b0: 6379 3d22 322e 3539 3939 3939 3730 652b  cy="2.59999970e+
-000069c0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-000069d0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-000069e0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-000069f0: 2232 2e33 3030 3030 3030 3065 2b30 3122  "2.30000000e+01"
-00006a00: 2063 793d 2232 2e39 3030 3030 3033 3065   cy="2.90000030e
-00006a10: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-00006a20: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-00006a30: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00006a40: 3d22 322e 3330 3030 3030 3030 652b 3031  ="2.30000000e+01
-00006a50: 2220 6379 3d22 332e 3230 3030 3030 3030  " cy="3.20000000
-00006a60: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-00006a70: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-00006a80: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00006a90: 783d 2232 2e33 3030 3030 3030 3065 2b30  x="2.30000000e+0
-00006aa0: 3122 2063 793d 2233 2e34 3939 3939 3937  1" cy="3.4999997
-00006ab0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-00006ac0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-00006ad0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00006ae0: 6378 3d22 322e 3330 3030 3030 3030 652b  cx="2.30000000e+
-00006af0: 3031 2220 6379 3d22 332e 3739 3939 3939  01" cy="3.799999
-00006b00: 3430 652b 3031 2220 723d 2230 2e35 3336  40e+01" r="0.536
-00006b10: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-00006b20: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00006b30: 2063 783d 2232 2e33 3030 3030 3030 3065   cx="2.30000000e
-00006b40: 2b30 3122 2063 793d 2234 2e30 3939 3939  +01" cy="4.09999
-00006b50: 3931 3065 2b30 3122 2072 3d22 302e 3533  910e+01" r="0.53
-00006b60: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-00006b70: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00006b80: 6520 6378 3d22 322e 3330 3030 3030 3030  e cx="2.30000000
-00006b90: 652b 3031 2220 6379 3d22 342e 3339 3939  e+01" cy="4.3999
-00006ba0: 3939 3730 652b 3031 2220 723d 2230 2e35  9970e+01" r="0.5
-00006bb0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-00006bc0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00006bd0: 6c65 2063 783d 2232 2e33 3030 3030 3030  le cx="2.3000000
-00006be0: 3065 2b30 3122 2063 793d 2234 2e36 3939  0e+01" cy="4.699
-00006bf0: 3939 3934 3065 2b30 3122 2072 3d22 302e  99940e+01" r="0.
-00006c00: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-00006c10: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00006c20: 636c 6520 6378 3d22 322e 3330 3030 3030  cle cx="2.300000
-00006c30: 3030 652b 3031 2220 6379 3d22 352e 3030  00e+01" cy="5.00
-00006c40: 3030 3030 3030 652b 3031 2220 723d 2230  000000e+01" r="0
-00006c50: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-00006c60: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00006c70: 7263 6c65 2063 783d 2232 2e33 3030 3030  rcle cx="2.30000
-00006c80: 3030 3065 2b30 3122 2063 793d 2235 2e32  000e+01" cy="5.2
-00006c90: 3939 3939 3937 3065 2b30 3122 2072 3d22  9999970e+01" r="
-00006ca0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-00006cb0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-00006cc0: 6972 636c 6520 6378 3d22 322e 3330 3030  ircle cx="2.3000
-00006cd0: 3030 3030 652b 3031 2220 6379 3d22 352e  0000e+01" cy="5.
-00006ce0: 3630 3030 3030 3330 652b 3031 2220 723d  60000030e+01" r=
-00006cf0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-00006d00: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-00006d10: 6369 7263 6c65 2063 783d 2235 2e30 3030  circle cx="5.000
-00006d20: 3030 3030 3065 2b30 3022 2063 793d 2231  00000e+00" cy="1
-00006d30: 2e32 3439 3939 3937 3065 2b30 3122 2072  .24999970e+01" r
-00006d40: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-00006d50: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-00006d60: 3c63 6972 636c 6520 6378 3d22 352e 3030  <circle cx="5.00
-00006d70: 3030 3030 3030 652b 3030 2220 6379 3d22  000000e+00" cy="
-00006d80: 322e 3030 3030 3030 3330 652b 3031 2220  2.00000030e+01" 
-00006d90: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-00006da0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-00006db0: 203c 6369 7263 6c65 2063 783d 2235 2e30   <circle cx="5.0
-00006dc0: 3030 3030 3030 3065 2b30 3022 2063 793d  0000000e+00" cy=
-00006dd0: 2232 2e37 3530 3030 3030 3065 2b30 3122  "2.75000000e+01"
-00006de0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-00006df0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-00006e00: 2020 3c63 6972 636c 6520 6378 3d22 352e    <circle cx="5.
-00006e10: 3030 3030 3030 3030 652b 3030 2220 6379  00000000e+00" cy
-00006e20: 3d22 332e 3439 3939 3939 3730 652b 3031  ="3.49999970e+01
-00006e30: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-00006e40: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-00006e50: 2020 203c 6369 7263 6c65 2063 783d 2235     <circle cx="5
-00006e60: 2e30 3030 3030 3030 3065 2b30 3022 2063  .00000000e+00" c
-00006e70: 793d 2234 2e32 3439 3939 3835 3065 2b30  y="4.24999850e+0
-00006e80: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-00006e90: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-00006ea0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00006eb0: 352e 3030 3030 3030 3030 652b 3030 2220  5.00000000e+00" 
-00006ec0: 6379 3d22 342e 3939 3939 3938 3230 652b  cy="4.99999820e+
-00006ed0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-00006ee0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-00006ef0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00006f00: 2235 2e30 3030 3030 3030 3065 2b30 3022  "5.00000000e+00"
-00006f10: 2063 793d 2235 2e37 3439 3939 3739 3065   cy="5.74999790e
-00006f20: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-00006f30: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-00006f40: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00006f50: 3d22 352e 3030 3030 3030 3030 652b 3030  ="5.00000000e+00
-00006f60: 2220 6379 3d22 362e 3439 3939 3938 3530  " cy="6.49999850
-00006f70: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-00006f80: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-00006f90: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00006fa0: 783d 2235 2e30 3030 3030 3030 3065 2b30  x="5.00000000e+0
-00006fb0: 3022 2063 793d 2237 2e32 3439 3939 3931  0" cy="7.2499991
-00006fc0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-00006fd0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-00006fe0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00006ff0: 6378 3d22 352e 3030 3030 3030 3030 652b  cx="5.00000000e+
-00007000: 3030 2220 6379 3d22 372e 3939 3939 3939  00" cy="7.999999
-00007010: 3730 652b 3031 2220 723d 2230 2e35 3336  70e+01" r="0.536
-00007020: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-00007030: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00007040: 2063 783d 2235 2e30 3030 3030 3030 3065   cx="5.00000000e
-00007050: 2b30 3022 2063 793d 2238 2e37 3439 3939  +00" cy="8.74999
-00007060: 3936 3765 2b30 3122 2072 3d22 302e 3533  967e+01" r="0.53
-00007070: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-00007080: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00007090: 6520 6378 3d22 392e 3530 3030 3030 3030  e cx="9.50000000
-000070a0: 652b 3031 2220 6379 3d22 392e 3530 3030  e+01" cy="9.5000
-000070b0: 3030 3030 652b 3031 2220 723d 2230 2e35  0000e+01" r="0.5
-000070c0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-000070d0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-000070e0: 6c65 2063 783d 2239 2e35 3030 3030 3030  le cx="9.5000000
-000070f0: 3065 2b30 3122 2063 793d 2235 2e30 3030  0e+01" cy="5.000
-00007100: 3030 3030 3065 2b30 3022 2072 3d22 302e  00000e+00" r="0.
-00007110: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-00007120: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00007130: 636c 6520 6378 3d22 352e 3030 3030 3030  cle cx="5.000000
-00007140: 3030 652b 3030 2220 6379 3d22 392e 3530  00e+00" cy="9.50
-00007150: 3030 3030 3030 652b 3031 2220 723d 2230  000000e+01" r="0
-00007160: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-00007170: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00007180: 7263 6c65 2063 783d 2235 2e30 3030 3030  rcle cx="5.00000
-00007190: 3030 3065 2b30 3022 2063 793d 2235 2e30  000e+00" cy="5.0
-000071a0: 3030 3030 3030 3065 2b30 3022 2072 3d22  0000000e+00" r="
-000071b0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-000071c0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-000071d0: 6972 636c 6520 6378 3d22 322e 3330 3030  ircle cx="2.3000
-000071e0: 3030 3030 652b 3031 2220 6379 3d22 322e  0000e+01" cy="2.
-000071f0: 3330 3030 3030 3030 652b 3031 2220 723d  30000000e+01" r=
-00007200: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-00007210: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-00007220: 6369 7263 6c65 2063 783d 2232 2e33 3030  circle cx="2.300
-00007230: 3030 3030 3065 2b30 3122 2063 793d 2235  00000e+01" cy="5
-00007240: 2e39 3030 3030 3030 3065 2b30 3122 2072  .90000000e+01" r
-00007250: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-00007260: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-00007270: 3c63 6972 636c 6520 6378 3d22 342e 3130  <circle cx="4.10
-00007280: 3030 3030 3030 652b 3031 2220 6379 3d22  000000e+01" cy="
-00007290: 372e 3730 3030 3030 3030 652b 3031 2220  7.70000000e+01" 
-000072a0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-000072b0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-000072c0: 203c 6369 7263 6c65 2063 783d 2235 2e39   <circle cx="5.9
-000072d0: 3030 3030 3030 3065 2b30 3122 2063 793d  0000000e+01" cy=
-000072e0: 2235 2e39 3030 3030 3030 3065 2b30 3122  "5.90000000e+01"
-000072f0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-00007300: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-00007310: 2020 3c63 6972 636c 6520 6378 3d22 372e    <circle cx="7.
-00007320: 3730 3030 3030 3030 652b 3031 2220 6379  70000000e+01" cy
-00007330: 3d22 342e 3130 3030 3030 3030 652b 3031  ="4.10000000e+01
-00007340: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-00007350: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-00007360: 2020 203c 6369 7263 6c65 2063 783d 2235     <circle cx="5
-00007370: 2e39 3030 3030 3030 3065 2b30 3122 2063  .90000000e+01" c
-00007380: 793d 2232 2e33 3030 3030 3030 3065 2b30  y="2.30000000e+0
-00007390: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-000073a0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-000073b0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-000073c0: 352e 3731 3037 3439 3830 652b 3031 2220  5.71074980e+01" 
-000073d0: 6379 3d22 382e 3133 3036 3838 3730 652b  cy="8.13068870e+
-000073e0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-000073f0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-00007400: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00007410: 2231 2e37 3030 3036 3633 3065 2b30 3122  "1.70006630e+01"
-00007420: 2063 793d 2238 2e32 3938 3834 3338 3065   cy="8.29884380e
-00007430: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-00007440: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-00007450: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00007460: 3d22 382e 3139 3330 3333 3530 652b 3031  ="8.19303350e+01
-00007470: 2220 6379 3d22 382e 3139 3437 3538 3830  " cy="8.19475880
-00007480: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-00007490: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-000074a0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-000074b0: 783d 2233 2e39 3131 3039 3138 3065 2b30  x="3.91109180e+0
-000074c0: 3122 2063 793d 2231 2e34 3636 3531 3831  1" cy="1.4665181
-000074d0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-000074e0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-000074f0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00007500: 6378 3d22 372e 3735 3334 3736 3230 652b  cx="7.75347620e+
-00007510: 3031 2220 6379 3d22 362e 3932 3336 3439  01" cy="6.923649
-00007520: 3230 652b 3031 2220 723d 2230 2e35 3336  20e+01" r="0.536
-00007530: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-00007540: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00007550: 2063 783d 2236 2e39 3230 3838 3731 3065   cx="6.92088710e
-00007560: 2b30 3122 2063 793d 2237 2e37 3536 3233  +01" cy="7.75623
-00007570: 3833 3065 2b30 3122 2072 3d22 302e 3533  830e+01" r="0.53
-00007580: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-00007590: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-000075a0: 6520 6378 3d22 312e 3730 3535 3736 3130  e cx="1.70557610
-000075b0: 652b 3031 2220 6379 3d22 352e 3332 3134  e+01" cy="5.3214
-000075c0: 3232 3430 652b 3031 2220 723d 2230 2e35  2240e+01" r="0.5
-000075d0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-000075e0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-000075f0: 6c65 2063 783d 2232 2e37 3338 3232 3434  le cx="2.7382244
-00007600: 3065 2b30 3122 2063 793d 2238 2e30 3237  0e+01" cy="8.027
-00007610: 3537 3339 3065 2b30 3122 2072 3d22 302e  57390e+01" r="0.
-00007620: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-00007630: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00007640: 636c 6520 6378 3d22 372e 3235 3434 3338  cle cx="7.254438
-00007650: 3830 652b 3031 2220 6379 3d22 312e 3438  80e+01" cy="1.48
-00007660: 3039 3937 3330 652b 3031 2220 723d 2230  099730e+01" r="0
-00007670: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-00007680: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00007690: 7263 6c65 2063 783d 2238 2e32 3939 3438  rcle cx="8.29948
-000076a0: 3436 3065 2b30 3122 2063 793d 2231 2e37  460e+01" cy="1.7
-000076b0: 3030 3730 3731 3065 2b30 3122 2072 3d22  0070710e+01" r="
-000076c0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-000076d0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-000076e0: 6972 636c 6520 6378 3d22 372e 3934 3936  ircle cx="7.9496
-000076f0: 3536 3430 652b 3031 2220 6379 3d22 312e  5640e+01" cy="1.
-00007700: 3330 3034 3731 3730 652b 3031 2220 723d  30047170e+01" r=
-00007710: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-00007720: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-00007730: 6369 7263 6c65 2063 783d 2238 2e34 3134  circle cx="8.414
-00007740: 3730 3938 3065 2b30 3122 2063 793d 2233  70980e+01" cy="3
-00007750: 2e37 3638 3331 3637 3065 2b30 3122 2072  .76831670e+01" r
-00007760: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-00007770: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-00007780: 3c63 6972 636c 6520 6378 3d22 372e 3235  <circle cx="7.25
-00007790: 3139 3931 3730 652b 3031 2220 6379 3d22  199170e+01" cy="
-000077a0: 392e 3931 3335 3332 3030 652b 3030 2220  9.91353200e+00" 
-000077b0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-000077c0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-000077d0: 203c 6369 7263 6c65 2063 783d 2234 2e32   <circle cx="4.2
-000077e0: 3734 3036 3138 3065 2b30 3122 2063 793d  7406180e+01" cy=
-000077f0: 2231 2e31 3434 3334 3531 3065 2b30 3122  "1.14434510e+01"
-00007800: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-00007810: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-00007820: 2020 3c63 6972 636c 6520 6378 3d22 342e    <circle cx="4.
-00007830: 3635 3938 3132 3630 652b 3031 2220 6379  65981260e+01" cy
-00007840: 3d22 382e 3235 3330 3434 3630 652b 3031  ="8.25304460e+01
-00007850: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-00007860: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-00007870: 2020 203c 6369 7263 6c65 2063 783d 2234     <circle cx="4
-00007880: 2e36 3337 3033 3138 3065 2b30 3122 2063  .63703180e+01" c
-00007890: 793d 2238 2e32 3231 3733 3030 3065 2b30  y="8.22173000e+0
-000078a0: 3022 2072 3d22 302e 3533 3638 3130 3436  0" r="0.53681046
-000078b0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-000078c0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-000078d0: 342e 3634 3833 3833 3530 652b 3031 2220  4.64838350e+01" 
-000078e0: 6379 3d22 312e 3636 3137 3337 3130 652b  cy="1.66173710e+
-000078f0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-00007900: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-00007910: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00007920: 2238 2e30 3238 3034 3832 3065 2b30 3122  "8.02804820e+01"
-00007930: 2063 793d 2232 2e37 3338 3730 3233 3065   cy="2.73870230e
-00007940: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-00007950: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-00007960: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00007970: 3d22 312e 3537 3431 3836 3930 652b 3031  ="1.57418690e+01
-00007980: 2220 6379 3d22 362e 3232 3137 3431 3930  " cy="6.22174190
-00007990: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-000079a0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-000079b0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-000079c0: 783d 2231 2e39 3639 3538 3132 3065 2b30  x="1.96958120e+0
-000079d0: 3122 2063 793d 2237 2e32 3539 3633 3534  1" cy="7.2596354
-000079e0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-000079f0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-00007a00: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00007a10: 6378 3d22 362e 3232 3138 3634 3330 652b  cx="6.22186430e+
-00007a20: 3031 2220 6379 3d22 312e 3537 3433 3035  01" cy="1.574305
-00007a30: 3730 652b 3031 2220 723d 2230 2e35 3336  70e+01" r="0.536
-00007a40: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-00007a50: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00007a60: 2063 783d 2231 2e36 3631 3733 3731 3065   cx="1.66173710e
-00007a70: 2b30 3122 2063 793d 2234 2e36 3438 3338  +01" cy="4.64838
-00007a80: 3137 3065 2b30 3122 2072 3d22 302e 3533  170e+01" r="0.53
-00007a90: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-00007aa0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00007ab0: 6520 6378 3d22 362e 3536 3534 3136 3830  e cx="6.56541680
-00007ac0: 652b 3031 2220 6379 3d22 312e 3231 3539  e+01" cy="1.2159
-00007ad0: 3530 3930 652b 3031 2220 723d 2230 2e35  5090e+01" r="0.5
-00007ae0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-00007af0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00007b00: 6c65 2063 783d 2236 2e30 3637 3837 3631  le cx="6.0678761
-00007b10: 3065 2b30 3122 2063 793d 2237 2e32 3432  0e+01" cy="7.242
-00007b20: 3636 3638 3065 2b30 3122 2072 3d22 302e  66680e+01" r="0.
-00007b30: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-00007b40: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00007b50: 636c 6520 6378 3d22 372e 3236 3031 3133  cle cx="7.260113
-00007b60: 3330 652b 3031 2220 6379 3d22 312e 3937  30e+01" cy="1.97
-00007b70: 3030 3534 3630 652b 3031 2220 723d 2230  005460e+01" r="0
-00007b80: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-00007b90: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00007ba0: 7263 6c65 2063 783d 2238 2e31 3239 3738  rcle cx="8.12978
-00007bb0: 3639 3065 2b30 3122 2063 793d 2235 2e37  690e+01" cy="5.7
-00007bc0: 3131 3636 3432 3065 2b30 3122 2072 3d22  1166420e+01" r="
-00007bd0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-00007be0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-00007bf0: 6972 636c 6520 6378 3d22 362e 3630 3039  ircle cx="6.6009
-00007c00: 3837 3530 652b 3031 2220 6379 3d22 362e  8750e+01" cy="6.
-00007c10: 3630 3338 3136 3230 652b 3031 2220 723d  60381620e+01" r=
-00007c20: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-00007c30: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-00007c40: 6369 7263 6c65 2063 783d 2233 2e37 3638  circle cx="3.768
-00007c50: 3138 3236 3065 2b30 3122 2063 793d 2238  18260e+01" cy="8
-00007c60: 2e34 3134 3630 3030 3065 2b30 3122 2072  .41460000e+01" r
-00007c70: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-00007c80: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-00007c90: 3c63 6972 636c 6520 6378 3d22 362e 3930  <circle cx="6.90
-00007ca0: 3737 3030 3330 652b 3031 2220 6379 3d22  770030e+01" cy="
-00007cb0: 382e 3539 3130 3930 3030 652b 3030 2220  8.59109000e+00" 
-00007cc0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-00007cd0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-00007ce0: 203c 6369 7263 6c65 2063 783d 2238 2e32   <circle cx="8.2
-00007cf0: 3532 3931 3935 3065 2b30 3122 2063 793d  5291950e+01" cy=
-00007d00: 2234 2e36 3539 3938 3534 3065 2b30 3122  "4.65998540e+01"
-00007d10: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-00007d20: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-00007d30: 2020 3c63 6972 636c 6520 6378 3d22 312e    <circle cx="1.
-00007d40: 3436 3635 3138 3130 652b 3031 2220 6379  46651810e+01" cy
-00007d50: 3d22 332e 3931 3130 3930 3030 652b 3031  ="3.91109000e+01
-00007d60: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-00007d70: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-00007d80: 2020 203c 6369 7263 6c65 2063 783d 2237     <circle cx="7
-00007d90: 2e35 3939 3832 3832 3065 2b30 3122 2063  .59982820e+01" c
-00007da0: 793d 2239 2e30 3032 3335 3430 3065 2b30  y="9.00235400e+0
-00007db0: 3022 2072 3d22 302e 3533 3638 3130 3436  0" r="0.53681046
-00007dc0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-00007dd0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00007de0: 372e 3234 3034 3931 3530 652b 3031 2220  7.24049150e+01" 
-00007df0: 6379 3d22 362e 3037 3030 3534 3130 652b  cy="6.07005410e+
-00007e00: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-00007e10: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-00007e20: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00007e30: 2234 2e37 3535 3535 3139 3065 2b30 3122  "4.75555190e+01"
-00007e40: 2063 793d 2237 2e38 3039 3931 3631 3065   cy="7.80991610e
-00007e50: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-00007e60: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-00007e70: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00007e80: 3d22 352e 3838 3937 3438 3130 652b 3031  ="5.88974810e+01
-00007e90: 2220 6379 3d22 362e 3831 3436 3935 3230  " cy="6.81469520
-00007ea0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-00007eb0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-00007ec0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00007ed0: 783d 2236 2e33 3237 3836 3633 3065 2b30  x="6.32786630e+0
-00007ee0: 3122 2063 793d 2236 2e36 3033 3438 3431  1" cy="6.6034841
-00007ef0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-00007f00: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-00007f10: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00007f20: 6378 3d22 392e 3036 3433 3434 3230 652b  cx="9.06434420e+
-00007f30: 3031 2220 6379 3d22 372e 3536 3439 3139  01" cy="7.564919
-00007f40: 3930 652b 3031 2220 723d 2230 2e35 3336  90e+01" r="0.536
-00007f50: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-00007f60: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00007f70: 2063 783d 2235 2e38 3132 3732 3730 3065   cx="5.81272700e
-00007f80: 2b30 3122 2063 793d 2231 2e32 3139 3531  +01" cy="1.21951
-00007f90: 3538 3065 2b30 3122 2072 3d22 302e 3533  580e+01" r="0.53
-00007fa0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-00007fb0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00007fc0: 6520 6378 3d22 342e 3736 3535 3839 3630  e cx="4.76558960
-00007fd0: 652b 3031 2220 6379 3d22 312e 3237 3434  e+01" cy="1.2744
-00007fe0: 3931 3430 652b 3031 2220 723d 2230 2e35  9140e+01" r="0.5
-00007ff0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-00008000: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00008010: 6c65 2063 783d 2235 2e34 3036 3938 3435  le cx="5.4069845
-00008020: 3065 2b30 3122 2063 793d 2238 2e36 3035  0e+01" cy="8.605
-00008030: 3830 3530 3065 2b30 3022 2072 3d22 302e  80500e+00" r="0.
-00008040: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-00008050: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00008060: 636c 6520 6378 3d22 352e 3130 3730 3937  cle cx="5.107097
-00008070: 3330 652b 3031 2220 6379 3d22 392e 3032  30e+01" cy="9.02
-00008080: 3037 3638 3030 652b 3030 2220 723d 2230  076800e+00" r="0
-00008090: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-000080a0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-000080b0: 7263 6c65 2063 783d 2233 2e31 3337 3033  rcle cx="3.13703
-000080c0: 3135 3065 2b30 3122 2063 793d 2238 2e32  150e+01" cy="8.2
-000080d0: 3231 3733 3030 3065 2b30 3022 2072 3d22  2173000e+00" r="
-000080e0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-000080f0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-00008100: 6972 636c 6520 6378 3d22 382e 3632 3836  ircle cx="8.6286
-00008110: 3838 3430 652b 3031 2220 6379 3d22 372e  8840e+01" cy="7.
-00008120: 3837 3938 3338 3930 652b 3031 2220 723d  87983890e+01" r=
-00008130: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-00008140: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-00008150: 6369 7263 6c65 2063 783d 2238 2e33 3335  circle cx="8.335
-00008160: 3635 3131 3065 2b30 3122 2063 793d 2237  65110e+01" cy="7
-00008170: 2e30 3332 3433 3331 3065 2b30 3122 2072  .03243310e+01" r
-00008180: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-00008190: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-000081a0: 3c63 6972 636c 6520 6378 3d22 382e 3931  <circle cx="8.91
-000081b0: 3738 3235 3130 652b 3031 2220 6379 3d22  782510e+01" cy="
-000081c0: 372e 3134 3132 3136 3130 652b 3031 2220  7.14121610e+01" 
-000081d0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-000081e0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-000081f0: 203c 6369 7263 6c65 2063 783d 2232 2e36   <circle cx="2.6
-00008200: 3030 3030 3036 3065 2b30 3122 2063 793d  0000060e+01" cy=
-00008210: 2231 2e31 3030 3030 3033 3065 2b30 3122  "1.10000030e+01"
-00008220: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-00008230: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-00008240: 2020 3c63 6972 636c 6520 6378 3d22 352e    <circle cx="5.
-00008250: 3539 3932 3031 3130 652b 3031 2220 6379  59920110e+01" cy
-00008260: 3d22 372e 3831 3636 3430 3030 652b 3031  ="7.81664000e+01
-00008270: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-00008280: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-00008290: 2020 203c 6369 7263 6c65 2063 783d 2235     <circle cx="5
-000082a0: 2e32 3133 3937 3332 3065 2b30 3122 2063  .21397320e+01" c
-000082b0: 793d 2231 2e33 3033 3433 3831 3065 2b30  y="1.30343810e+0
-000082c0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-000082d0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-000082e0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-000082f0: 352e 3530 3431 3937 3130 652b 3031 2220  5.50419710e+01" 
-00008300: 6379 3d22 372e 3530 3930 3437 3030 652b  cy="7.50904700e+
-00008310: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-00008320: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-00008330: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00008340: 2235 2e36 3137 3736 3039 3065 2b30 3122  "5.61776090e+01"
-00008350: 2063 793d 2237 2e32 3134 3733 3038 3065   cy="7.21473080e
-00008360: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-00008370: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-00008380: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00008390: 3d22 352e 3834 3232 3933 3830 652b 3031  ="5.84229380e+01
-000083a0: 2220 6379 3d22 372e 3232 3237 3636 3930  " cy="7.22276690
-000083b0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-000083c0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-000083d0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-000083e0: 783d 2235 2e31 3034 3432 3937 3065 2b30  x="5.10442970e+0
-000083f0: 3122 2063 793d 2237 2e37 3831 3536 3730  1" cy="7.7815670
-00008400: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-00008410: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-00008420: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00008430: 6378 3d22 352e 3937 3033 3233 3330 652b  cx="5.97032330e+
-00008440: 3031 2220 6379 3d22 372e 3033 3037 3331  01" cy="7.030731
-00008450: 3230 652b 3031 2220 723d 2230 2e35 3336  20e+01" r="0.536
-00008460: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-00008470: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00008480: 2063 783d 2236 2e30 3539 3232 3731 3065   cx="6.05922710e
-00008490: 2b30 3122 2063 793d 2236 2e36 3036 3938  +01" cy="6.60698
-000084a0: 3738 3065 2b30 3122 2072 3d22 302e 3533  780e+01" r="0.53
-000084b0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-000084c0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-000084d0: 6520 6378 3d22 342e 3838 3237 3935 3730  e cx="4.88279570
-000084e0: 652b 3031 2220 6379 3d22 382e 3837 3234  e+01" cy="8.8724
-000084f0: 3537 3030 652b 3030 2220 723d 2230 2e35  5700e+00" r="0.5
-00008500: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-00008510: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00008520: 6c65 2063 783d 2233 2e30 3530 3030 3036  le cx="3.0500006
-00008530: 3065 2b30 3122 2063 793d 2231 2e36 3939  0e+01" cy="1.699
-00008540: 3939 3937 3065 2b30 3122 2072 3d22 302e  99970e+01" r="0.
-00008550: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-00008560: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00008570: 636c 6520 6378 3d22 342e 3730 3338 3634  cle cx="4.703864
-00008580: 3030 652b 3031 2220 6379 3d22 382e 3033  00e+01" cy="8.03
-00008590: 3032 3830 3230 652b 3031 2220 723d 2230  028020e+01" r="0
-000085a0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-000085b0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-000085c0: 7263 6c65 2063 783d 2232 2e34 3530 3030  rcle cx="2.45000
-000085d0: 3033 3065 2b30 3122 2063 793d 2231 2e36  030e+01" cy="1.6
-000085e0: 3939 3939 3937 3065 2b30 3122 2072 3d22  9999970e+01" r="
-000085f0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-00008600: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-00008610: 6972 636c 6520 6378 3d22 332e 3532 3430  ircle cx="3.5240
-00008620: 3632 3130 652b 3031 2220 6379 3d22 312e  6210e+01" cy="1.
-00008630: 3134 3433 3435 3130 652b 3031 2220 723d  14434510e+01" r=
-00008640: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-00008650: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-00008660: 6369 7263 6c65 2063 783d 2235 2e33 3231  circle cx="5.321
-00008670: 3432 3333 3065 2b30 3122 2063 793d 2231  42330e+01" cy="1
-00008680: 2e37 3035 3537 3730 3065 2b30 3122 2072  .70557700e+01" r
-00008690: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-000086a0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-000086b0: 3c63 6972 636c 6520 6378 3d22 322e 3930  <circle cx="2.90
-000086c0: 3030 3031 3230 652b 3031 2220 6379 3d22  000120e+01" cy="
-000086d0: 312e 3130 3030 3030 3330 652b 3031 2220  1.10000030e+01" 
-000086e0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-000086f0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-00008700: 203c 6369 7263 6c65 2063 783d 2235 2e34   <circle cx="5.4
-00008710: 3037 3637 3438 3065 2b30 3122 2063 793d  0767480e+01" cy=
-00008720: 2237 2e39 3432 3539 3431 3065 2b30 3122  "7.94259410e+01"
-00008730: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-00008740: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-00008750: 2020 3c63 6972 636c 6520 6378 3d22 392e    <circle cx="9.
-00008760: 3133 3634 3030 3930 652b 3031 2220 6379  13640090e+01" cy
-00008770: 3d22 332e 3038 3930 3533 3430 652b 3031  ="3.08905340e+01
-00008780: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-00008790: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-000087a0: 2020 203c 6369 7263 6c65 2063 783d 2232     <circle cx="2
-000087b0: 2e31 3232 3232 3339 3065 2b30 3122 2063  .12222390e+01" c
-000087c0: 793d 2236 2e34 3739 3235 3335 3065 2b30  y="6.47925350e+0
-000087d0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-000087e0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-000087f0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00008800: 312e 3835 3632 3932 3830 652b 3031 2220  1.85629280e+01" 
-00008810: 6379 3d22 362e 3334 3139 3138 3930 652b  cy="6.34191890e+
-00008820: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-00008830: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-00008840: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00008850: 2238 2e35 3838 3039 3933 3065 2b30 3122  "8.58809930e+01"
-00008860: 2063 793d 2235 2e34 3734 3433 3530 3065   cy="5.47443500e
-00008870: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-00008880: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-00008890: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-000088a0: 3d22 392e 3030 3831 3134 3930 652b 3031  ="9.00811490e+01
-000088b0: 2220 6379 3d22 322e 3734 3733 3631 3230  " cy="2.74736120
-000088c0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-000088d0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-000088e0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-000088f0: 783d 2238 2e37 3735 3031 3637 3065 2b30  x="8.77501670e+0
-00008900: 3122 2063 793d 2233 2e34 3237 3931 3738  1" cy="3.4279178
-00008910: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-00008920: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-00008930: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00008940: 6378 3d22 332e 3138 3236 3132 3030 652b  cx="3.18261200e+
-00008950: 3031 2220 6379 3d22 372e 3734 3039 3633  01" cy="7.740963
-00008960: 3530 652b 3031 2220 723d 2230 2e35 3336  50e+01" r="0.536
-00008970: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-00008980: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00008990: 2063 783d 2232 2e31 3230 3530 3232 3065   cx="2.12050220e
-000089a0: 2b30 3122 2063 793d 2237 2e30 3430 3736  +01" cy="7.04076
-000089b0: 3137 3065 2b30 3122 2072 3d22 302e 3533  170e+01" r="0.53
-000089c0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-000089d0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-000089e0: 6520 6378 3d22 332e 3531 3833 3534 3330  e cx="3.51835430
-000089f0: 652b 3031 2220 6379 3d22 372e 3837 3330  e+01" cy="7.8730
-00008a00: 3338 3530 652b 3031 2220 723d 2230 2e35  3850e+01" r="0.5
-00008a10: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-00008a20: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00008a30: 6c65 2063 783d 2238 2e35 3137 3837 3332  le cx="8.5178732
-00008a40: 3065 2b30 3122 2063 793d 2232 2e37 3434  0e+01" cy="2.744
-00008a50: 3534 3639 3065 2b30 3122 2072 3d22 302e  54690e+01" r="0.
-00008a60: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-00008a70: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00008a80: 636c 6520 6378 3d22 382e 3737 3636 3435  cle cx="8.776645
-00008a90: 3730 652b 3031 2220 6379 3d22 342e 3138  70e+01" cy="4.18
-00008aa0: 3035 3934 3130 652b 3031 2220 723d 2230  059410e+01" r="0
-00008ab0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-00008ac0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00008ad0: 7263 6c65 2063 783d 2232 2e37 3636 3537  rcle cx="2.76657
-00008ae0: 3236 3065 2b30 3122 2063 793d 2237 2e37  260e+01" cy="7.7
-00008af0: 3439 3031 3430 3065 2b30 3122 2072 3d22  4901400e+01" r="
-00008b00: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-00008b10: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-00008b20: 6972 636c 6520 6378 3d22 332e 3635 3132  ircle cx="3.6512
-00008b30: 3433 3830 652b 3031 2220 6379 3d22 382e  4380e+01" cy="8.
-00008b40: 3133 3635 3835 3530 652b 3031 2220 723d  13658550e+01" r=
-00008b50: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-00008b60: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-00008b70: 6369 7263 6c65 2063 783d 2232 2e34 3030  circle cx="2.400
-00008b80: 3032 3234 3065 2b30 3122 2063 793d 2239  02240e+01" cy="9
-00008b90: 2e30 3939 3631 3436 3665 2b30 3122 2072  .09961466e+01" r
-00008ba0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-00008bb0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-00008bc0: 3c63 6972 636c 6520 6378 3d22 392e 3133  <circle cx="9.13
-00008bd0: 3733 3934 3530 652b 3031 2220 6379 3d22  739450e+01" cy="
-00008be0: 342e 3539 3130 3531 3730 652b 3031 2220  4.59105170e+01" 
-00008bf0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-00008c00: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-00008c10: 203c 6369 7263 6c65 2063 783d 2232 2e37   <circle cx="2.7
-00008c20: 3737 3135 3339 3065 2b30 3122 2063 793d  7715390e+01" cy=
-00008c30: 2237 2e34 3733 3436 3337 3065 2b30 3122  "7.47346370e+01"
-00008c40: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-00008c50: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-00008c60: 2020 3c63 6972 636c 6520 6378 3d22 392e    <circle cx="9.
-00008c70: 3039 3938 3238 3530 652b 3031 2220 6379  09982850e+01" cy
-00008c80: 3d22 322e 3430 3032 3336 3630 652b 3031  ="2.40023660e+01
-00008c90: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-00008ca0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-00008cb0: 2020 203c 6369 7263 6c65 2063 783d 2232     <circle cx="2
-00008cc0: 2e39 3537 3832 3335 3065 2b30 3122 2063  .95782350e+01" c
-00008cd0: 793d 2237 2e38 3737 3635 3238 3065 2b30  y="7.87765280e+0
-00008ce0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-00008cf0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-00008d00: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00008d10: 322e 3035 3030 3433 3930 652b 3031 2220  2.05004390e+01" 
-00008d20: 6379 3d22 382e 3639 3932 3239 3431 652b  cy="8.69922941e+
-00008d30: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-00008d40: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-00008d50: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00008d60: 2239 2e30 3434 3039 3432 3065 2b30 3122  "9.04409420e+01"
-00008d70: 2063 793d 2235 2e32 3337 3037 3236 3065   cy="5.23707260e
-00008d80: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-00008d90: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-00008da0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00008db0: 3d22 392e 3038 3334 3439 3430 652b 3031  ="9.08344940e+01
-00008dc0: 2220 6379 3d22 342e 3838 3730 3932 3330  " cy="4.88709230
-00008dd0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-00008de0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-00008df0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00008e00: 783d 2232 2e32 3538 3639 3930 3065 2b30  x="2.25869900e+0
-00008e10: 3122 2063 793d 2236 2e38 3136 3835 3334  1" cy="6.8168534
-00008e20: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-00008e30: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-00008e40: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00008e50: 6378 3d22 322e 3234 3931 3535 3430 652b  cx="2.24915540e+
-00008e60: 3031 2220 6379 3d22 372e 3233 3230 3334  01" cy="7.232034
-00008e70: 3230 652b 3031 2220 723d 2230 2e35 3336  20e+01" r="0.536
-00008e80: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-00008e90: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00008ea0: 2063 783d 2239 2e30 3430 3439 3630 3065   cx="9.04049600e
-00008eb0: 2b30 3122 2063 793d 2236 2e37 3335 3935  +01" cy="6.73595
-00008ec0: 3639 3065 2b30 3122 2072 3d22 302e 3533  690e+01" r="0.53
-00008ed0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-00008ee0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00008ef0: 6520 6378 3d22 322e 3532 3535 3431 3830  e cx="2.52554180
-00008f00: 652b 3031 2220 6379 3d22 372e 3232 3233  e+01" cy="7.2223
-00008f10: 3430 3330 652b 3031 2220 723d 2230 2e35  4030e+01" r="0.5
-00008f20: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-00008f30: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00008f40: 6c65 2063 783d 2238 2e35 3834 3332 3131  le cx="8.5843211
-00008f50: 3065 2b30 3122 2063 793d 2236 2e32 3233  0e+01" cy="6.223
-00008f60: 3431 3737 3065 2b30 3122 2072 3d22 302e  41770e+01" r="0.
-00008f70: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-00008f80: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00008f90: 636c 6520 6378 3d22 382e 3636 3731 3039  cle cx="8.667109
-00008fa0: 3430 652b 3031 2220 6379 3d22 342e 3737  40e+01" cy="4.77
-00008fb0: 3335 3837 3930 652b 3031 2220 723d 2230  358790e+01" r="0
-00008fc0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-00008fd0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00008fe0: 7263 6c65 2063 783d 2238 2e36 3939 3635  rcle cx="8.69965
-00008ff0: 3631 3065 2b30 3122 2063 793d 2232 2e30  610e+01" cy="2.0
-00009000: 3530 3437 3134 3065 2b30 3122 2072 3d22  5047140e+01" r="
-00009010: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-00009020: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-00009030: 6972 636c 6520 6378 3d22 342e 3737 3334  ircle cx="4.7734
-00009040: 3731 3830 652b 3031 2220 6379 3d22 382e  7180e+01" cy="8.
-00009050: 3636 3731 3932 3734 652b 3031 2220 723d  66719274e+01" r=
-00009060: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-00009070: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-00009080: 6369 7263 6c65 2063 783d 2232 2e37 3437  circle cx="2.747
-00009090: 3230 3139 3065 2b30 3122 2063 793d 2239  20190e+01" cy="9
-000090a0: 2e30 3037 3935 3733 3165 2b30 3122 2072  .00795731e+01" r
-000090b0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-000090c0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-000090d0: 3c63 6972 636c 6520 6378 3d22 332e 3432  <circle cx="3.42
-000090e0: 3738 3236 3930 652b 3031 2220 6379 3d22  782690e+01" cy="
-000090f0: 382e 3737 3439 3432 3435 652b 3031 2220  8.77494245e+01" 
-00009100: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-00009110: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-00009120: 203c 6369 7263 6c65 2063 783d 2232 2e30   <circle cx="2.0
-00009130: 3837 3234 3534 3065 2b30 3122 2063 793d  8724540e+01" cy=
-00009140: 2234 2e32 3832 3739 3336 3065 2b30 3122  "4.28279360e+01"
-00009150: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-00009160: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-00009170: 2020 3c63 6972 636c 6520 6378 3d22 312e    <circle cx="1.
-00009180: 3639 3939 3939 3730 652b 3031 2220 6379  69999970e+01" cy
-00009190: 3d22 332e 3034 3939 3939 3730 652b 3031  ="3.04999970e+01
-000091a0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-000091b0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-000091c0: 2020 203c 6369 7263 6c65 2063 783d 2235     <circle cx="5
-000091d0: 2e32 3336 3736 3537 3065 2b30 3122 2063  .23676570e+01" c
-000091e0: 793d 2239 2e30 3434 3339 3333 3665 2b30  y="9.04439336e+0
-000091f0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-00009200: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-00009210: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00009220: 322e 3734 3432 3239 3230 652b 3031 2220  2.74422920e+01" 
-00009230: 6379 3d22 382e 3531 3735 3538 3230 652b  cy="8.51755820e+
-00009240: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-00009250: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-00009260: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00009270: 2231 2e38 3734 3439 3038 3065 2b30 3122  "1.87449080e+01"
-00009280: 2063 793d 2234 2e34 3635 3538 3732 3065   cy="4.46558720e
-00009290: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-000092a0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-000092b0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-000092c0: 3d22 322e 3032 3231 3732 3730 652b 3031  ="2.02217270e+01
-000092d0: 2220 6379 3d22 332e 3433 3730 3330 3330  " cy="3.43703030
-000092e0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-000092f0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-00009300: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00009310: 783d 2231 2e37 3434 3334 3534 3065 2b30  x="1.74434540e+0
-00009320: 3122 2063 793d 2233 2e36 3734 3035 3937  1" cy="3.6740597
-00009330: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-00009340: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-00009350: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00009360: 6378 3d22 312e 3734 3433 3435 3430 652b  cx="1.74434540e+
-00009370: 3031 2220 6379 3d22 332e 3937 3430 3539  01" cy="3.974059
-00009380: 3430 652b 3031 2220 723d 2230 2e35 3336  40e+01" r="0.536
-00009390: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-000093a0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-000093b0: 2063 783d 2232 2e30 3232 3137 3237 3065   cx="2.02217270e
-000093c0: 2b30 3122 2063 793d 2234 2e30 3337 3032  +01" cy="4.03702
-000093d0: 3937 3065 2b30 3122 2072 3d22 302e 3533  970e+01" r="0.53
-000093e0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-000093f0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00009400: 6520 6378 3d22 322e 3130 3230 3736 3530  e cx="2.10207650
-00009410: 652b 3031 2220 6379 3d22 352e 3130 3734  e+01" cy="5.1074
-00009420: 3234 3930 652b 3031 2220 723d 2230 2e35  2490e+01" r="0.5
-00009430: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-00009440: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00009450: 6c65 2063 783d 2231 2e39 3033 3933 3037  le cx="1.9039307
-00009460: 3065 2b30 3122 2063 793d 2235 2e32 3134  0e+01" cy="5.214
-00009470: 3436 3733 3065 2b30 3122 2072 3d22 302e  46730e+01" r="0.
-00009480: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-00009490: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-000094a0: 636c 6520 6378 3d22 372e 3033 3035 3930  cle cx="7.030590
-000094b0: 3830 652b 3031 2220 6379 3d22 382e 3333  80e+01" cy="8.33
-000094c0: 3734 3932 3530 652b 3031 2220 723d 2230  749250e+01" r="0
-000094d0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-000094e0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-000094f0: 7263 6c65 2063 783d 2235 2e34 3733 3832  rcle cx="5.47382
-00009500: 3330 3065 2b30 3122 2063 793d 2238 2e35  300e+01" cy="8.5
-00009510: 3838 3639 3738 3065 2b30 3122 2072 3d22  8869780e+01" r="
-00009520: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-00009530: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-00009540: 6972 636c 6520 6378 3d22 372e 3837 3836  ircle cx="7.8786
-00009550: 3838 3730 652b 3031 2220 6379 3d22 382e  8870e+01" cy="8.
-00009560: 3632 3938 3339 3035 652b 3031 2220 723d  62983905e+01" r=
-00009570: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-00009580: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-00009590: 6369 7263 6c65 2063 783d 2237 2e31 3430  circle cx="7.140
-000095a0: 3239 3534 3065 2b30 3122 2063 793d 2238  29540e+01" cy="8
-000095b0: 2e39 3138 3734 3630 3765 2b30 3122 2072  .91874607e+01" r
-000095c0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-000095d0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-000095e0: 3c63 6972 636c 6520 6378 3d22 332e 3038  <circle cx="3.08
-000095f0: 3930 3038 3430 652b 3031 2220 6379 3d22  900840e+01" cy="
-00009600: 392e 3133 3633 3634 3039 652b 3031 2220  9.13636409e+01" 
-00009610: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-00009620: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-00009630: 203c 6369 7263 6c65 2063 783d 2234 2e35   <circle cx="4.5
-00009640: 3931 3030 3430 3065 2b30 3122 2063 793d  9100400e+01" cy=
-00009650: 2239 2e31 3337 3335 3737 3865 2b30 3122  "9.13735778e+01"
-00009660: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-00009670: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-00009680: 2020 3c63 6972 636c 6520 6378 3d22 372e    <circle cx="7.
-00009690: 3536 3433 3433 3930 652b 3031 2220 6379  56434390e+01" cy
-000096a0: 3d22 392e 3036 3439 3139 3537 652b 3031  ="9.06491957e+01
-000096b0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-000096c0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-000096d0: 2020 203c 6369 7263 6c65 2063 783d 2234     <circle cx="4
-000096e0: 2e38 3837 3033 3239 3065 2b30 3122 2063  .88703290e+01" c
-000096f0: 793d 2239 2e30 3833 3439 3037 3165 2b30  y="9.08349071e+0
-00009700: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-00009710: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-00009720: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00009730: 342e 3138 3035 3032 3330 652b 3031 2220  4.18050230e+01" 
-00009740: 6379 3d22 382e 3737 3635 3732 3632 652b  cy="8.77657262e+
-00009750: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-00009760: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-00009770: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00009780: 2236 2e32 3232 3830 3933 3065 2b30 3122  "6.22280930e+01"
-00009790: 2063 793d 2238 2e35 3834 3931 3837 3065   cy="8.58491870e
-000097a0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-000097b0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-000097c0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-000097d0: 3d22 362e 3733 3536 3530 3930 652b 3031  ="6.73565090e+01
-000097e0: 2220 6379 3d22 392e 3034 3037 3934 3236  " cy="9.04079426
-000097f0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-00009800: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-00009810: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00009820: 783d 2231 2e31 3030 3030 3030 3365 2b30  x="1.10000003e+0
-00009830: 3122 2063 793d 2232 2e39 3030 3030 3033  1" cy="2.9000003
-00009840: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-00009850: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-00009860: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00009870: 6378 3d22 382e 3639 3936 3536 3130 652b  cx="8.69965610e+
-00009880: 3031 2220 6379 3d22 312e 3330 3034 3731  01" cy="1.300471
-00009890: 3730 652b 3031 2220 723d 2230 2e35 3336  70e+01" r="0.536
-000098a0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-000098b0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-000098c0: 2063 783d 2239 2e30 3939 3832 3835 3065   cx="9.09982850e
-000098d0: 2b30 3122 2063 793d 2239 2e30 3032 3335  +01" cy="9.00235
-000098e0: 3430 3065 2b30 3022 2072 3d22 302e 3533  400e+00" r="0.53
-000098f0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-00009900: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00009910: 6520 6378 3d22 312e 3438 3036 3832 3330  e cx="1.48068230
-00009920: 652b 3031 2220 6379 3d22 372e 3235 3431  e+01" cy="7.2541
-00009930: 3232 3030 652b 3031 2220 723d 2230 2e35  2200e+01" r="0.5
-00009940: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-00009950: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00009960: 6c65 2063 783d 2238 2e32 3231 3732 3634  le cx="8.2217264
-00009970: 3065 2b30 3022 2063 793d 2234 2e36 3337  0e+00" cy="4.637
-00009980: 3032 3832 3065 2b30 3122 2072 3d22 302e  02820e+01" r="0.
-00009990: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-000099a0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-000099b0: 636c 6520 6378 3d22 312e 3330 3030 3434  cle cx="1.300044
-000099c0: 3239 652b 3031 2220 6379 3d22 382e 3639  29e+01" cy="8.69
-000099d0: 3932 3239 3431 652b 3031 2220 723d 2230  922941e+01" r="0
-000099e0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-000099f0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00009a00: 7263 6c65 2063 783d 2239 2e30 3030 3232  rcle cx="9.00022
-00009a10: 3130 3065 2b30 3022 2063 793d 2239 2e30  100e+00" cy="9.0
-00009a20: 3939 3631 3436 3665 2b30 3122 2072 3d22  9961466e+01" r="
-00009a30: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-00009a40: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-00009a50: 6972 636c 6520 6378 3d22 382e 3539 3036  ircle cx="8.5906
-00009a60: 3932 3230 652b 3030 2220 6379 3d22 362e  9220e+00" cy="6.
-00009a70: 3930 3736 3538 3930 652b 3031 2220 723d  90765890e+01" r=
-00009a80: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-00009a90: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-00009aa0: 6369 7263 6c65 2063 783d 2231 2e33 3033  circle cx="1.303
-00009ab0: 3433 3734 3765 2b30 3122 2063 793d 2235  43747e+01" cy="5
-00009ac0: 2e32 3133 3937 3134 3065 2b30 3122 2072  .21397140e+01" r
-00009ad0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-00009ae0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-00009af0: 3c63 6972 636c 6520 6378 3d22 312e 3639  <circle cx="1.69
-00009b00: 3939 3939 3730 652b 3031 2220 6379 3d22  999970e+01" cy="
-00009b10: 322e 3435 3030 3030 3330 652b 3031 2220  2.45000030e+01" 
-00009b20: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-00009b30: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-00009b40: 203c 6369 7263 6c65 2063 783d 2238 2e32   <circle cx="8.2
-00009b50: 3231 3732 3634 3065 2b30 3022 2063 793d  2172640e+00" cy=
-00009b60: 2233 2e31 3337 3032 3937 3065 2b30 3122  "3.13702970e+01"
-00009b70: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-00009b80: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-00009b90: 2020 3c63 6972 636c 6520 6378 3d22 312e    <circle cx="1.
-00009ba0: 3134 3433 3435 3337 652b 3031 2220 6379  14434537e+01" cy
-00009bb0: 3d22 332e 3532 3430 3630 3330 652b 3031  ="3.52406030e+01
-00009bc0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-00009bd0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-00009be0: 2020 203c 6369 7263 6c65 2063 783d 2231     <circle cx="1
-00009bf0: 2e38 3734 3338 3931 3065 2b30 3122 2063  .87438910e+01" c
-00009c00: 793d 2234 2e37 3635 3533 3536 3065 2b30  y="4.76553560e+0
-00009c10: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-00009c20: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-00009c30: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-00009c40: 392e 3032 3037 3631 3730 652b 3030 2220  9.02076170e+00" 
-00009c50: 6379 3d22 352e 3130 3730 3934 3630 652b  cy="5.10709460e+
-00009c60: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-00009c70: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-00009c80: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-00009c90: 2231 2e32 3139 3433 3634 3265 2b30 3122  "1.21943642e+01"
-00009ca0: 2063 793d 2235 2e38 3132 3634 3531 3065   cy="5.81264510e
-00009cb0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-00009cc0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-00009cd0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-00009ce0: 3d22 382e 3837 3234 3536 3130 652b 3030  ="8.87245610e+00
-00009cf0: 2220 6379 3d22 342e 3838 3237 3932 3130  " cy="4.88279210
-00009d00: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-00009d10: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-00009d20: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-00009d30: 783d 2231 2e32 3734 3439 3131 3365 2b30  x="1.27449113e+0
-00009d40: 3122 2063 793d 2234 2e37 3635 3538 3639  1" cy="4.7655869
-00009d50: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-00009d60: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-00009d70: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-00009d80: 6378 3d22 392e 3030 3032 3231 3030 652b  cx="9.00022100e+
-00009d90: 3030 2220 6379 3d22 372e 3539 3936 3134  00" cy="7.599614
-00009da0: 3030 652b 3031 2220 723d 2230 2e35 3336  00e+01" r="0.536
-00009db0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-00009dc0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-00009dd0: 2063 783d 2232 2e30 3837 3037 3830 3065   cx="2.08707800e
-00009de0: 2b30 3122 2063 793d 2234 2e38 3832 3839  +01" cy="4.88289
-00009df0: 3131 3065 2b30 3122 2072 3d22 302e 3533  110e+01" r="0.53
-00009e00: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-00009e10: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-00009e20: 6520 6378 3d22 382e 3630 3533 3939 3130  e cx="8.60539910
-00009e30: 652b 3030 2220 6379 3d22 352e 3430 3639  e+00" cy="5.4069
-00009e40: 3431 3330 652b 3031 2220 723d 2230 2e35  4130e+01" r="0.5
-00009e50: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-00009e60: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-00009e70: 6c65 2063 783d 2231 2e32 3135 3837 3035  le cx="1.2158705
-00009e80: 3365 2b30 3122 2063 793d 2236 2e35 3635  3e+01" cy="6.565
-00009e90: 3333 3439 3065 2b30 3122 2072 3d22 302e  33490e+01" r="0.
-00009ea0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-00009eb0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-00009ec0: 636c 6520 6378 3d22 392e 3931 3139 3534  cle cx="9.911954
-00009ed0: 3330 652b 3030 2220 6379 3d22 372e 3235  30e+00" cy="7.25
-00009ee0: 3138 3333 3330 652b 3031 2220 723d 2230  183330e+01" r="0
-00009ef0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-00009f00: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-00009f10: 7263 6c65 2063 783d 2238 2e36 3238 3638  rcle cx="8.62868
-00009f20: 3834 3065 2b30 3122 2063 793d 2238 2e36  840e+01" cy="8.6
-00009f30: 3239 3833 3930 3565 2b30 3122 2072 3d22  2983905e+01" r="
-00009f40: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-00009f50: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-00009f60: 6972 636c 6520 6378 3d22 312e 3134 3433  ircle cx="1.1443
-00009f70: 3435 3337 652b 3031 2220 6379 3d22 342e  4537e+01" cy="4.
-00009f80: 3237 3430 3539 3130 652b 3031 2220 723d  27405910e+01" r=
-00009f90: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-00009fa0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-00009fb0: 6369 7263 6c65 2063 783d 2239 2e30 3634  circle cx="9.064
-00009fc0: 3334 3432 3065 2b30 3122 2063 793d 2239  34420e+01" cy="9
-00009fd0: 2e30 3634 3931 3935 3765 2b30 3122 2072  .06491957e+01" r
-00009fe0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-00009ff0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000a000: 3c63 6972 636c 6520 6378 3d22 312e 3330  <circle cx="1.30
-0000a010: 3030 3434 3239 652b 3031 2220 6379 3d22  004429e+01" cy="
-0000a020: 372e 3934 3932 3238 3930 652b 3031 2220  7.94922890e+01" 
-0000a030: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000a040: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000a050: 203c 6369 7263 6c65 2063 783d 2231 2e31   <circle cx="1.1
-0000a060: 3030 3030 3030 3365 2b30 3122 2063 793d  0000003e+01" cy=
-0000a070: 2232 2e35 3939 3939 3937 3065 2b30 3122  "2.59999970e+01"
-0000a080: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000a090: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000a0a0: 2020 3c63 6972 636c 6520 6378 3d22 382e    <circle cx="8.
-0000a0b0: 3037 3331 3931 3330 652b 3031 2220 6379  07319130e+01" cy
-0000a0c0: 3d22 342e 3437 3733 3430 3330 652b 3031  ="4.47734030e+01
-0000a0d0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000a0e0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000a0f0: 2020 203c 6369 7263 6c65 2063 783d 2238     <circle cx="8
-0000a100: 2e31 3833 3032 3832 3065 2b30 3122 2063  .18302820e+01" c
-0000a110: 793d 2233 2e38 3737 3037 3039 3065 2b30  y="3.87707090e+0
-0000a120: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000a130: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000a140: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000a150: 312e 3831 3134 3833 3630 652b 3031 2220  1.81148360e+01" 
-0000a160: 6379 3d22 362e 3131 3536 3533 3530 652b  cy="6.11565350e+
-0000a170: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000a180: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000a190: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000a1a0: 2231 2e36 3939 3939 3937 3065 2b30 3122  "1.69999970e+01"
-0000a1b0: 2063 793d 2231 2e36 3939 3939 3937 3065   cy="1.69999970e
-0000a1c0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000a1d0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000a1e0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000a1f0: 3d22 342e 3437 3732 3232 3430 652b 3031  ="4.47722240e+01
-0000a200: 2220 6379 3d22 382e 3037 3332 3737 3730  " cy="8.07327770
-0000a210: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000a220: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000a230: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000a240: 783d 2237 2e39 3631 3531 3636 3065 2b30  x="7.96151660e+0
-0000a250: 3122 2063 793d 2233 2e39 3933 3534 3137  1" cy="3.9935417
-0000a260: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000a270: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000a280: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000a290: 6378 3d22 362e 3030 3334 3335 3230 652b  cx="6.00343520e+
-0000a2a0: 3031 2220 6379 3d22 322e 3034 3130 3437  01" cy="2.041047
-0000a2b0: 3530 652b 3031 2220 723d 2230 2e35 3336  50e+01" r="0.536
-0000a2c0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000a2d0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000a2e0: 2063 783d 2237 2e39 3134 3738 3836 3065   cx="7.91478860e
-0000a2f0: 2b30 3122 2063 793d 2234 2e32 3831 3232  +01" cy="4.28122
-0000a300: 3637 3065 2b30 3122 2072 3d22 302e 3533  670e+01" r="0.53
-0000a310: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000a320: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000a330: 6520 6378 3d22 312e 3930 3237 3932 3230  e cx="1.90279220
-0000a340: 652b 3031 2220 6379 3d22 352e 3531 3336  e+01" cy="5.5136
-0000a350: 3939 3330 652b 3031 2220 723d 2230 2e35  9930e+01" r="0.5
-0000a360: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000a370: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000a380: 6c65 2063 783d 2236 2e31 3135 3832 3030  le cx="6.1158200
-0000a390: 3065 2b30 3122 2063 793d 2238 2e30 3037  0e+01" cy="8.007
-0000a3a0: 3238 3730 3065 2b30 3122 2072 3d22 302e  28700e+01" r="0.
-0000a3b0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000a3c0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000a3d0: 636c 6520 6378 3d22 352e 3031 3131 3231  cle cx="5.011121
-0000a3e0: 3330 652b 3031 2220 6379 3d22 382e 3231  30e+01" cy="8.21
-0000a3f0: 3135 3739 3830 652b 3031 2220 723d 2230  157980e+01" r="0
-0000a400: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000a410: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000a420: 7263 6c65 2063 783d 2235 2e38 3330 3132  rcle cx="5.83012
-0000a430: 3637 3065 2b30 3122 2063 793d 2237 2e38  670e+01" cy="7.8
-0000a440: 3335 3539 3736 3065 2b30 3122 2072 3d22  3559760e+01" r="
-0000a450: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000a460: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000a470: 6972 636c 6520 6378 3d22 362e 3131 3537  ircle cx="6.1157
-0000a480: 3336 3330 652b 3031 2220 6379 3d22 312e  3630e+01" cy="1.
-0000a490: 3831 3135 3631 3930 652b 3031 2220 723d  81156190e+01" r=
-0000a4a0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000a4b0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000a4c0: 6369 7263 6c65 2063 783d 2235 2e39 3437  circle cx="5.947
-0000a4d0: 3431 3338 3065 2b30 3122 2063 793d 2237  41380e+01" cy="7
-0000a4e0: 2e35 3339 3137 3435 3065 2b30 3122 2072  .53917450e+01" r
-0000a4f0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000a500: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000a510: 3c63 6972 636c 6520 6378 3d22 352e 3336  <circle cx="5.36
-0000a520: 3138 3531 3330 652b 3031 2220 6379 3d22  185130e+01" cy="
-0000a530: 382e 3137 3233 3734 3030 652b 3031 2220  8.17237400e+01" 
-0000a540: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000a550: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000a560: 203c 6369 7263 6c65 2063 783d 2232 2e33   <circle cx="2.3
-0000a570: 3931 3433 3733 3065 2b30 3122 2063 793d  9143730e+01" cy=
-0000a580: 2238 2e31 3137 3139 3233 3065 2b30 3122  "8.11719230e+01"
-0000a590: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000a5a0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000a5b0: 2020 3c63 6972 636c 6520 6378 3d22 342e    <circle cx="4.
-0000a5c0: 3238 3131 3639 3130 652b 3031 2220 6379  28116910e+01" cy
-0000a5d0: 3d22 372e 3931 3438 3235 3530 652b 3031  ="7.91482550e+01
-0000a5e0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000a5f0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000a600: 2020 203c 6369 7263 6c65 2063 783d 2232     <circle cx="2
-0000a610: 2e30 3938 3238 3339 3065 2b30 3122 2063  .09828390e+01" c
-0000a620: 793d 2235 2e37 3037 3638 3335 3065 2b30  y="5.70768350e+0
-0000a630: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000a640: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000a650: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000a660: 322e 3034 3536 3330 3330 652b 3031 2220  2.04563030e+01" 
-0000a670: 6379 3d22 382e 3230 3738 3535 3630 652b  cy="8.20785560e+
-0000a680: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000a690: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000a6a0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000a6b0: 2233 2e38 3736 3937 3931 3065 2b30 3122  "3.87697910e+01"
-0000a6c0: 2063 793d 2238 2e31 3832 3935 3434 3065   cy="8.18295440e
-0000a6d0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000a6e0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000a6f0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000a700: 3d22 332e 3939 3334 3937 3630 652b 3031  ="3.99349760e+01
-0000a710: 2220 6379 3d22 372e 3936 3134 3832 3430  " cy="7.96148240
-0000a720: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000a730: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000a740: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000a750: 783d 2232 2e30 3431 3031 3036 3065 2b30  x="2.04101060e+0
-0000a760: 3122 2063 793d 2236 2e30 3033 3339 3536  1" cy="6.0033956
-0000a770: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000a780: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000a790: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000a7a0: 6378 3d22 362e 3136 3033 3637 3330 652b  cx="6.16036730e+
-0000a7b0: 3031 2220 6379 3d22 362e 3136 3131 3731  01" cy="6.161171
-0000a7c0: 3030 652b 3031 2220 723d 2230 2e35 3336  00e+01" r="0.536
-0000a7d0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000a7e0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000a7f0: 2063 783d 2236 2e33 3731 3535 3530 3065   cx="6.37155500e
-0000a800: 2b30 3122 2063 793d 2236 2e33 3733 3439  +01" cy="6.37349
-0000a810: 3138 3065 2b30 3122 2072 3d22 302e 3533  180e+01" r="0.53
-0000a820: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000a830: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000a840: 6520 6378 3d22 352e 3730 3736 3834 3430  e cx="5.70768440
-0000a850: 652b 3031 2220 6379 3d22 322e 3039 3832  e+01" cy="2.0982
-0000a860: 3834 3830 652b 3031 2220 723d 2230 2e35  8480e+01" r="0.5
-0000a870: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000a880: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000a890: 6c65 2063 783d 2235 2e35 3133 3730 3032  le cx="5.5137002
-0000a8a0: 3065 2b30 3122 2063 793d 2231 2e39 3032  0e+01" cy="1.902
-0000a8b0: 3739 3232 3065 2b30 3122 2072 3d22 302e  79220e+01" r="0.
-0000a8c0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000a8d0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000a8e0: 636c 6520 6378 3d22 362e 3531 3939 3234  cle cx="6.519924
-0000a8f0: 3530 652b 3031 2220 6379 3d22 372e 3838  50e+01" cy="7.88
-0000a900: 3435 3038 3130 652b 3031 2220 723d 2230  450810e+01" r="0
-0000a910: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000a920: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000a930: 7263 6c65 2063 783d 2231 2e31 3030 3030  rcle cx="1.10000
-0000a940: 3030 3365 2b30 3122 2063 793d 2231 2e31  003e+01" cy="1.1
-0000a950: 3030 3030 3033 3065 2b30 3122 2072 3d22  0000030e+01" r="
-0000a960: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000a970: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000a980: 6972 636c 6520 6378 3d22 362e 3730 3830  ircle cx="6.7080
-0000a990: 3636 3830 652b 3031 2220 6379 3d22 362e  6680e+01" cy="6.
-0000a9a0: 3938 3831 3030 3930 652b 3031 2220 723d  98810090e+01" r=
-0000a9b0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000a9c0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000a9d0: 6369 7263 6c65 2063 783d 2234 2e30 3337  circle cx="4.037
-0000a9e0: 3033 3135 3065 2b30 3122 2063 793d 2232  03150e+01" cy="2
-0000a9f0: 2e30 3232 3137 3237 3065 2b30 3122 2072  .02217270e+01" r
-0000aa00: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000aa10: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000aa20: 3c63 6972 636c 6520 6378 3d22 382e 3030  <circle cx="8.00
-0000aa30: 3537 3634 3230 652b 3031 2220 6379 3d22  576420e+01" cy="
-0000aa40: 362e 3131 3733 3533 3630 652b 3031 2220  6.11735360e+01" 
-0000aa50: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000aa60: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000aa70: 203c 6369 7263 6c65 2063 783d 2231 2e36   <circle cx="1.6
-0000aa80: 3136 3533 3931 3065 2b30 3122 2063 793d  1653910e+01" cy=
-0000aa90: 2235 2e39 3230 3031 3630 3065 2b30 3122  "5.92001600e+01"
-0000aaa0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000aab0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000aac0: 2020 3c63 6972 636c 6520 6378 3d22 362e    <circle cx="6.
-0000aad0: 3335 3134 3137 3530 652b 3031 2220 6379  35141750e+01" cy
-0000aae0: 3d22 372e 3431 3439 3732 3730 652b 3031  ="7.41497270e+01
-0000aaf0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000ab00: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000ab10: 2020 203c 6369 7263 6c65 2063 783d 2231     <circle cx="1
-0000ab20: 2e36 3633 3034 3834 3065 2b30 3122 2063  .66304840e+01" c
-0000ab30: 793d 2235 2e36 3231 3130 3335 3065 2b30  y="5.62110350e+0
-0000ab40: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000ab50: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000ab60: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000ab70: 342e 3135 3638 3535 3730 652b 3031 2220  4.15685570e+01" 
-0000ab80: 6379 3d22 312e 3533 3135 3930 3830 652b  cy="1.53159080e+
-0000ab90: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000aba0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000abb0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000abc0: 2234 2e34 3032 3631 3936 3065 2b30 3122  "4.40261960e+01"
-0000abd0: 2063 793d 2231 2e35 3936 3636 3335 3065   cy="1.59666350e
-0000abe0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000abf0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000ac00: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000ac10: 3d22 312e 3838 3034 3636 3830 652b 3031  ="1.88046680e+01
-0000ac20: 2220 6379 3d22 372e 3630 3637 3531 3030  " cy="7.60675100
-0000ac30: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000ac40: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000ac50: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000ac60: 783d 2236 2e38 3133 3933 3734 3065 2b30  x="6.81393740e+0
-0000ac70: 3122 2063 793d 2237 2e33 3733 3138 3933  1" cy="7.3731893
-0000ac80: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000ac90: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000aca0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000acb0: 6378 3d22 372e 3334 3439 3335 3630 652b  cx="7.34493560e+
-0000acc0: 3031 2220 6379 3d22 372e 3930 3234 3131  01" cy="7.902411
-0000acd0: 3830 652b 3031 2220 723d 2230 2e35 3336  80e+01" r="0.536
-0000ace0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000acf0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000ad00: 2063 783d 2231 2e37 3930 3431 3238 3065   cx="1.79041280e
-0000ad10: 2b30 3122 2063 793d 2237 2e39 3532 3931  +01" cy="7.95291
-0000ad20: 3839 3065 2b30 3122 2072 3d22 302e 3533  890e+01" r="0.53
-0000ad30: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000ad40: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000ad50: 6520 6378 3d22 372e 3437 3539 3436 3830  e cx="7.47594680
-0000ad60: 652b 3031 2220 6379 3d22 372e 3230 3131  e+01" cy="7.2011
-0000ad70: 3739 3530 652b 3031 2220 723d 2230 2e35  7950e+01" r="0.5
-0000ad80: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000ad90: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000ada0: 6c65 2063 783d 2237 2e31 3938 3431 3734  le cx="7.1984174
-0000adb0: 3065 2b30 3122 2063 793d 2237 2e34 3738  0e+01" cy="7.478
-0000adc0: 3730 3839 3065 2b30 3122 2072 3d22 302e  70890e+01" r="0.
-0000add0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000ade0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000adf0: 636c 6520 6378 3d22 332e 3637 3430 3631  cle cx="3.674061
-0000ae00: 3530 652b 3031 2220 6379 3d22 312e 3734  50e+01" cy="1.74
-0000ae10: 3433 3435 3430 652b 3031 2220 723d 2230  434540e+01" r="0
-0000ae20: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000ae30: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000ae40: 7263 6c65 2063 783d 2237 2e38 3832 3337  rcle cx="7.88237
-0000ae50: 3036 3065 2b30 3122 2063 793d 2236 2e35  060e+01" cy="6.5
-0000ae60: 3232 3037 3436 3065 2b30 3122 2072 3d22  2207460e+01" r="
-0000ae70: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000ae80: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000ae90: 6972 636c 6520 6378 3d22 372e 3337 3034  ircle cx="7.3704
-0000aea0: 3032 3030 652b 3031 2220 6379 3d22 362e  0200e+01" cy="6.
-0000aeb0: 3831 3637 3234 3730 652b 3031 2220 723d  81672470e+01" r=
-0000aec0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000aed0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000aee0: 6369 7263 6c65 2063 783d 2236 2e39 3835  circle cx="6.985
-0000aef0: 3238 3834 3065 2b30 3122 2063 793d 2236  28840e+01" cy="6
-0000af00: 2e37 3130 3839 3031 3065 2b30 3122 2072  .71089010e+01" r
-0000af10: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000af20: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000af30: 3c63 6972 636c 6520 6378 3d22 382e 3034  <circle cx="8.04
-0000af40: 3635 3134 3430 652b 3031 2220 6379 3d22  651440e+01" cy="
-0000af50: 372e 3737 3130 3535 3930 652b 3031 2220  7.77105590e+01" 
-0000af60: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000af70: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000af80: 203c 6369 7263 6c65 2063 783d 2237 2e37   <circle cx="7.7
-0000af90: 3638 3938 3530 3065 2b30 3122 2063 793d  6898500e+01" cy=
-0000afa0: 2238 2e30 3438 3538 3533 3065 2b30 3122  "8.04858530e+01"
-0000afb0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000afc0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000afd0: 2020 3c63 6972 636c 6520 6378 3d22 332e    <circle cx="3.
-0000afe0: 3433 3730 3331 3230 652b 3031 2220 6379  43703120e+01" cy
-0000aff0: 3d22 322e 3032 3231 3732 3730 652b 3031  ="2.02217270e+01
-0000b000: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000b010: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000b020: 2020 203c 6369 7263 6c65 2063 783d 2237     <circle cx="7
-0000b030: 2e35 3834 3533 3939 3065 2b30 3122 2063  .58453990e+01" c
-0000b040: 793d 2236 2e36 3339 3137 3930 3065 2b30  y="6.63917900e+0
-0000b050: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000b060: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000b070: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000b080: 372e 3839 3939 3935 3330 652b 3031 2220  7.89999530e+01" 
-0000b090: 6379 3d22 372e 3334 3733 3533 3030 652b  cy="7.34735300e+
-0000b0a0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000b0b0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000b0c0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000b0d0: 2233 2e39 3734 3036 3132 3065 2b30 3122  "3.97406120e+01"
-0000b0e0: 2063 793d 2231 2e37 3434 3334 3534 3065   cy="1.74434540e
-0000b0f0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000b100: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000b110: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000b120: 3d22 372e 3431 3236 3034 3830 652b 3031  ="7.41260480e+01
-0000b130: 2220 6379 3d22 362e 3335 3337 3932 3630  " cy="6.35379260
-0000b140: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000b150: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000b160: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000b170: 783d 2236 2e36 3336 3631 3034 3065 2b30  x="6.63661040e+0
-0000b180: 3122 2063 793d 2237 2e35 3837 3130 3439  1" cy="7.5871049
-0000b190: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000b1a0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000b1b0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000b1c0: 6378 3d22 372e 3630 3732 3832 3930 652b  cx="7.60728290e+
-0000b1d0: 3031 2220 6379 3d22 312e 3838 3039 3937  01" cy="1.880997
-0000b1e0: 3830 652b 3031 2220 723d 2230 2e35 3336  80e+01" r="0.536
-0000b1f0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000b200: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000b210: 2063 783d 2238 2e33 3631 3338 3636 3065   cx="8.36138660e
-0000b220: 2b30 3122 2063 793d 2234 2e30 3635 3739  +01" cy="4.06579
-0000b230: 3535 3065 2b30 3122 2072 3d22 302e 3533  550e+01" r="0.53
-0000b240: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000b250: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000b260: 6520 6378 3d22 342e 3837 3238 3131 3130  e cx="4.87281110
-0000b270: 652b 3031 2220 6379 3d22 312e 3637 3635  e+01" cy="1.6765
-0000b280: 3933 3430 652b 3031 2220 723d 2230 2e35  9340e+01" r="0.5
-0000b290: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000b2a0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000b2b0: 6c65 2063 783d 2235 2e30 3937 3137 3231  le cx="5.0971721
-0000b2c0: 3065 2b30 3122 2063 793d 2231 2e36 3931  0e+01" cy="1.691
-0000b2d0: 3335 3838 3065 2b30 3122 2072 3d22 302e  35880e+01" r="0.
-0000b2e0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000b2f0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000b300: 636c 6520 6378 3d22 342e 3736 3535 3336  cle cx="4.765536
-0000b310: 3530 652b 3031 2220 6379 3d22 312e 3837  50e+01" cy="1.87
-0000b320: 3433 3839 3130 652b 3031 2220 723d 2230  438910e+01" r="0
-0000b330: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000b340: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000b350: 7263 6c65 2063 783d 2234 2e30 3635 3634  rcle cx="4.06564
-0000b360: 3739 3065 2b30 3122 2063 793d 2238 2e33  790e+01" cy="8.3
-0000b370: 3631 3335 3630 3065 2b30 3122 2072 3d22  6135600e+01" r="
-0000b380: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000b390: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000b3a0: 6972 636c 6520 6378 3d22 312e 3637 3635  ircle cx="1.6765
-0000b3b0: 3933 3430 652b 3031 2220 6379 3d22 342e  9340e+01" cy="4.
-0000b3c0: 3837 3238 3039 3330 652b 3031 2220 723d  87280930e+01" r=
-0000b3d0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000b3e0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000b3f0: 6369 7263 6c65 2063 783d 2232 2e32 3235  circle cx="2.225
-0000b400: 3335 3736 3065 2b30 3122 2063 793d 2237  35760e+01" cy="7
-0000b410: 2e35 3136 3532 3837 3065 2b30 3122 2072  .51652870e+01" r
-0000b420: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000b430: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000b440: 3c63 6972 636c 6520 6378 3d22 382e 3131  <circle cx="8.11
-0000b450: 3737 3234 3230 652b 3031 2220 6379 3d22  772420e+01" cy="
-0000b460: 322e 3339 3139 3639 3230 652b 3031 2220  2.39196920e+01" 
-0000b470: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000b480: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000b490: 203c 6369 7263 6c65 2063 783d 2234 2e33   <circle cx="4.3
-0000b4a0: 3632 3036 3635 3065 2b30 3122 2063 793d  6206650e+01" cy=
-0000b4b0: 2238 2e33 3037 3935 3237 3065 2b30 3122  "8.30795270e+01"
-0000b4c0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000b4d0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000b4e0: 2020 3c63 6972 636c 6520 6378 3d22 342e    <circle cx="4.
-0000b4f0: 3838 3238 3932 3030 652b 3031 2220 6379  88289200e+01" cy
-0000b500: 3d22 322e 3038 3730 3738 3030 652b 3031  ="2.08707800e+01
-0000b510: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000b520: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000b530: 2020 203c 6369 7263 6c65 2063 783d 2231     <circle cx="1
-0000b540: 2e36 3931 3335 3838 3065 2b30 3122 2063  .69135880e+01" c
-0000b550: 793d 2235 2e30 3937 3137 3033 3065 2b30  y="5.09717030e+0
-0000b560: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000b570: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000b580: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000b590: 342e 3238 3237 3935 3430 652b 3031 2220  4.28279540e+01" 
-0000b5a0: 6379 3d22 322e 3038 3732 3435 3430 652b  cy="2.08724540e+
-0000b5b0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000b5c0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000b5d0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000b5e0: 2234 2e34 3635 3538 3930 3065 2b30 3122  "4.46558900e+01"
-0000b5f0: 2063 793d 2231 2e38 3734 3439 3038 3065   cy="1.87449080e
-0000b600: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000b610: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000b620: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000b630: 3d22 372e 3737 3234 3033 3230 652b 3031  ="7.77240320e+01
-0000b640: 2220 6379 3d22 322e 3438 3135 3739 3530  " cy="2.48157950
-0000b650: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000b660: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000b670: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000b680: 783d 2237 2e38 3733 3038 3938 3065 2b30  x="7.87308980e+0
-0000b690: 3122 2063 793d 2233 2e35 3138 3339 3339  1" cy="3.5183939
-0000b6a0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000b6b0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000b6c0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000b6d0: 6378 3d22 332e 3432 3431 3639 3330 652b  cx="3.42416930e+
-0000b6e0: 3031 2220 6379 3d22 382e 3238 3732 3933  01" cy="8.287293
-0000b6f0: 3230 652b 3031 2220 723d 2230 2e35 3336  20e+01" r="0.536
-0000b700: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000b710: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000b720: 2063 783d 2237 2e35 3137 3030 3330 3065   cx="7.51700300e
-0000b730: 2b30 3122 2063 793d 2232 2e32 3235 3833  +01" cy="2.22583
-0000b740: 3733 3065 2b30 3122 2072 3d22 302e 3533  730e+01" r="0.53
-0000b750: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000b760: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000b770: 6520 6378 3d22 382e 3230 3834 3431 3530  e cx="8.20844150
-0000b780: 652b 3031 2220 6379 3d22 322e 3034 3632  e+01" cy="2.0462
-0000b790: 3136 3230 652b 3031 2220 723d 2230 2e35  1620e+01" r="0.5
-0000b7a0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000b7b0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000b7c0: 6c65 2063 783d 2233 2e30 3831 3831 3437  le cx="3.0818147
-0000b7d0: 3065 2b30 3122 2063 793d 2238 2e31 3537  0e+01" cy="8.157
-0000b7e0: 3433 3934 3065 2b30 3122 2072 3d22 302e  43940e+01" r="0.
-0000b7f0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000b800: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000b810: 636c 6520 6378 3d22 322e 3438 3131 3034  cle cx="2.481104
-0000b820: 3330 652b 3031 2220 6379 3d22 372e 3737  30e+01" cy="7.77
-0000b830: 3139 3233 3530 652b 3031 2220 723d 2230  192350e+01" r="0
-0000b840: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000b850: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000b860: 7263 6c65 2063 783d 2237 2e39 3533 3530  rcle cx="7.95350
-0000b870: 3537 3065 2b30 3122 2063 793d 2231 2e37  570e+01" cy="1.7
-0000b880: 3930 3939 3837 3065 2b30 3122 2072 3d22  9099870e+01" r="
-0000b890: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000b8a0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000b8b0: 6972 636c 6520 6378 3d22 382e 3238 3735  ircle cx="8.2875
-0000b8c0: 3235 3430 652b 3031 2220 6379 3d22 332e  2540e+01" cy="3.
-0000b8d0: 3432 3434 3139 3530 652b 3031 2220 723d  42441950e+01" r=
-0000b8e0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000b8f0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000b900: 6369 7263 6c65 2063 783d 2238 2e31 3537  circle cx="8.157
-0000b910: 3738 3935 3065 2b30 3122 2063 793d 2233  78950e+01" cy="3
-0000b920: 2e30 3832 3137 3932 3065 2b30 3122 2072  .08217920e+01" r
-0000b930: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000b940: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000b950: 3c63 6972 636c 6520 6378 3d22 382e 3330  <circle cx="8.30
-0000b960: 3739 3035 3930 652b 3031 2220 6379 3d22  790590e+01" cy="
-0000b970: 342e 3336 3232 3235 3830 652b 3031 2220  4.36222580e+01" 
-0000b980: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000b990: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000b9a0: 203c 6369 7263 6c65 2063 783d 2238 2e31   <circle cx="8.1
-0000b9b0: 3336 3635 3339 3065 2b30 3122 2063 793d  3665390e+01" cy=
-0000b9c0: 2233 2e36 3531 3333 3734 3065 2b30 3122  "3.65133740e+01"
-0000b9d0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000b9e0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000b9f0: 2020 3c63 6972 636c 6520 6378 3d22 362e    <circle cx="6.
-0000ba00: 3234 3538 3039 3730 652b 3031 2220 6379  24580970e+01" cy
-0000ba10: 3d22 372e 3032 3831 3032 3330 652b 3031  ="7.02810230e+01
-0000ba20: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000ba30: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000ba40: 2020 203c 6369 7263 6c65 2063 783d 2237     <circle cx="7
-0000ba50: 2e32 3332 3336 3237 3065 2b30 3122 2063  .23236270e+01" c
-0000ba60: 793d 2232 2e32 3439 3437 3034 3065 2b30  y="2.24947040e+0
-0000ba70: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000ba80: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000ba90: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000baa0: 372e 3437 3336 3430 3130 652b 3031 2220  7.47364010e+01" 
-0000bab0: 6379 3d22 322e 3737 3732 3937 3930 652b  cy="2.77729790e+
-0000bac0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000bad0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000bae0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000baf0: 2237 2e38 3136 3035 3134 3065 2b30 3122  "7.81605140e+01"
-0000bb00: 2063 793d 2235 2e35 3939 3833 3536 3065   cy="5.59983560e
-0000bb10: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000bb20: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000bb30: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000bb40: 3d22 312e 3833 3631 3338 3230 652b 3031  ="1.83613820e+01
-0000bb50: 2220 6379 3d22 362e 3931 3336 3136 3030  " cy="6.91361600
-0000bb60: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000bb70: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000bb80: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000bb90: 783d 2237 2e37 3439 3332 3831 3065 2b30  x="7.74932810e+0
-0000bba0: 3122 2063 793d 2232 2e37 3636 3930 3131  1" cy="2.7669011
-0000bbb0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000bbc0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000bbd0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000bbe0: 6378 3d22 362e 3931 3339 3735 3130 652b  cx="6.91397510e+
-0000bbf0: 3031 2220 6379 3d22 312e 3833 3634 3931  01" cy="1.836491
-0000bc00: 3930 652b 3031 2220 723d 2230 2e35 3336  90e+01" r="0.536
-0000bc10: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000bc20: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000bc30: 2063 783d 2236 2e35 3638 3831 3631 3065   cx="6.56881610e
-0000bc40: 2b30 3122 2063 793d 2231 2e37 3032 3933  +01" cy="1.70293
-0000bc50: 3337 3065 2b30 3122 2072 3d22 302e 3533  370e+01" r="0.53
-0000bc60: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000bc70: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000bc80: 6520 6378 3d22 352e 3932 3030 3937 3030  e cx="5.92009700
-0000bc90: 652b 3031 2220 6379 3d22 312e 3631 3636  e+01" cy="1.6166
-0000bca0: 3138 3330 652b 3031 2220 723d 2230 2e35  1830e+01" r="0.5
-0000bcb0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000bcc0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000bcd0: 6c65 2063 783d 2237 2e32 3232 3438 3433  le cx="7.2224843
-0000bce0: 3065 2b30 3122 2063 793d 2232 2e35 3235  0e+01" cy="2.525
-0000bcf0: 3731 3832 3065 2b30 3122 2072 3d22 302e  71820e+01" r="0.
-0000bd00: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000bd10: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000bd20: 636c 6520 6378 3d22 312e 3730 3236 3937  cle cx="1.702697
-0000bd30: 3030 652b 3031 2220 6379 3d22 362e 3536  00e+01" cy="6.56
-0000bd40: 3835 3734 3930 652b 3031 2220 723d 2230  857490e+01" r="0
-0000bd50: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000bd60: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000bd70: 7263 6c65 2063 783d 2237 2e30 3431 3038  rcle cx="7.04108
-0000bd80: 3339 3065 2b30 3122 2063 793d 2232 2e31  390e+01" cy="2.1
-0000bd90: 3230 3832 3038 3065 2b30 3122 2072 3d22  2082080e+01" r="
-0000bda0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000bdb0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000bdc0: 6972 636c 6520 6378 3d22 362e 3831 3730  ircle cx="6.8170
-0000bdd0: 3137 3230 652b 3031 2220 6379 3d22 322e  1720e+01" cy="2.
-0000bde0: 3235 3838 3433 3930 652b 3031 2220 723d  25884390e+01" r=
-0000bdf0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000be00: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000be10: 6369 7263 6c65 2063 783d 2237 2e38 3334  circle cx="7.834
-0000be20: 3236 3131 3065 2b30 3122 2063 793d 2235  26110e+01" cy="5
-0000be30: 2e38 3331 3436 3332 3065 2b30 3122 2072  .83146320e+01" r
-0000be40: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000be50: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000be60: 3c63 6972 636c 6520 6378 3d22 372e 3533  <circle cx="7.53
-0000be70: 3734 3334 3830 652b 3031 2220 6379 3d22  743480e+01" cy="
-0000be80: 352e 3934 3931 3831 3430 652b 3031 2220  5.94918140e+01" 
-0000be90: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000bea0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000beb0: 203c 6369 7263 6c65 2063 783d 2237 2e37   <circle cx="7.7
-0000bec0: 3431 3130 3834 3065 2b30 3122 2063 793d  4110840e+01" cy=
-0000bed0: 2233 2e31 3832 3737 3637 3065 2b30 3122  "3.18277670e+01"
-0000bee0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000bef0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000bf00: 2020 3c63 6972 636c 6520 6378 3d22 362e    <circle cx="6.
-0000bf10: 3334 3230 3035 3330 652b 3031 2220 6379  34200530e+01" cy
-0000bf20: 3d22 312e 3835 3633 3636 3630 652b 3031  ="1.85636660e+01
-0000bf30: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000bf40: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000bf50: 2020 203c 6369 7263 6c65 2063 783d 2231     <circle cx="1
-0000bf60: 2e35 3331 3539 3038 3065 2b30 3122 2063  .53159080e+01" c
-0000bf70: 793d 2234 2e31 3536 3835 3339 3065 2b30  y="4.15685390e+0
-0000bf80: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000bf90: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000bfa0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000bfb0: 382e 3231 3131 3936 3430 652b 3031 2220  8.21119640e+01" 
-0000bfc0: 6379 3d22 352e 3031 3135 3430 3730 652b  cy="5.01154070e+
-0000bfd0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000bfe0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000bff0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000c000: 2231 2e35 3936 3636 3335 3065 2b30 3122  "1.59666350e+01"
-0000c010: 2063 793d 2234 2e34 3032 3631 3738 3065   cy="4.40261780e
-0000c020: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000c030: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000c040: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000c050: 3d22 382e 3137 3137 3330 3530 652b 3031  ="8.17173050e+01
-0000c060: 2220 6379 3d22 352e 3336 3235 3232 3730  " cy="5.36252270
-0000c070: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000c080: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000c090: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000c0a0: 783d 2237 2e35 3038 3730 3539 3065 2b30  x="7.50870590e+0
-0000c0b0: 3122 2063 793d 2235 2e35 3034 3436 3731  1" cy="5.5044671
-0000c0c0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000c0d0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000c0e0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000c0f0: 6378 3d22 372e 3837 3739 3732 3330 652b  cx="7.87797230e+
-0000c100: 3031 2220 6379 3d22 322e 3935 3831 3435  01" cy="2.958145
-0000c110: 3730 652b 3031 2220 723d 2230 2e35 3336  70e+01" r="0.536
-0000c120: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000c130: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000c140: 2063 783d 2237 2e39 3431 3938 3033 3065   cx="7.94198030e
-0000c150: 2b30 3122 2063 793d 2235 2e34 3038 3238  +01" cy="5.40828
-0000c160: 3935 3065 2b30 3122 2072 3d22 302e 3533  950e+01" r="0.53
-0000c170: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000c180: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000c190: 6520 6378 3d22 372e 3738 3132 3836 3230  e cx="7.78128620
-0000c1a0: 652b 3031 2220 6379 3d22 352e 3130 3437  e+01" cy="5.1047
-0000c1b0: 3436 3530 652b 3031 2220 723d 2230 2e35  4650e+01" r="0.5
-0000c1c0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000c1d0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000c1e0: 6c65 2063 783d 2235 2e36 3231 3134 3538  le cx="5.6211458
-0000c1f0: 3065 2b30 3122 2063 793d 2231 2e36 3633  0e+01" cy="1.663
-0000c200: 3038 3938 3065 2b30 3122 2072 3d22 302e  08980e+01" r="0.
-0000c210: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000c220: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000c230: 636c 6520 6378 3d22 362e 3432 3333 3232  cle cx="6.423322
-0000c240: 3130 652b 3031 2220 6379 3d22 362e 3831  10e+01" cy="6.81
-0000c250: 3730 3230 3830 652b 3031 2220 723d 2230  702080e+01" r="0
-0000c260: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000c270: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000c280: 7263 6c65 2063 783d 2236 2e34 3739 3239  rcle cx="6.47929
-0000c290: 3034 3065 2b30 3122 2063 793d 2232 2e31  040e+01" cy="2.1
-0000c2a0: 3232 3237 3730 3065 2b30 3122 2072 3d22  2227700e+01" r="
-0000c2b0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000c2c0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000c2d0: 6972 636c 6520 6378 3d22 362e 3831 3339  ircle cx="6.8139
-0000c2e0: 3139 3430 652b 3031 2220 6379 3d22 352e  1940e+01" cy="5.
-0000c2f0: 3839 3033 3538 3330 652b 3031 2220 723d  89035830e+01" r=
-0000c300: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000c310: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000c320: 6369 7263 6c65 2063 783d 2236 2e39 3130  circle cx="6.910
-0000c330: 3237 3037 3065 2b30 3122 2063 793d 2231  27070e+01" cy="1
-0000c340: 2e33 3438 3539 3032 3065 2b30 3122 2072  .34859020e+01" r
-0000c350: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000c360: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000c370: 3c63 6972 636c 6520 6378 3d22 372e 3232  <circle cx="7.22
-0000c380: 3132 3739 3230 652b 3031 2220 6379 3d22  127920e+01" cy="
-0000c390: 352e 3834 3337 3536 3330 652b 3031 2220  5.84375630e+01" 
-0000c3a0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000c3b0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000c3c0: 203c 6369 7263 6c65 2063 783d 2233 2e38   <circle cx="3.8
-0000c3d0: 3837 3033 3231 3065 2b30 3122 2063 793d  8703210e+01" cy=
-0000c3e0: 2238 2e32 3231 3733 3030 3065 2b30 3022  "8.22173000e+00"
-0000c3f0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000c400: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000c410: 2020 3c63 6972 636c 6520 6378 3d22 362e    <circle cx="6.
-0000c420: 3630 3631 3037 3630 652b 3031 2220 6379  60610760e+01" cy
-0000c430: 3d22 362e 3036 3032 3633 3930 652b 3031  ="6.06026390e+01
-0000c440: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000c450: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000c460: 2020 203c 6369 7263 6c65 2063 783d 2237     <circle cx="7
-0000c470: 2e32 3134 3038 3031 3065 2b30 3122 2063  .21408010e+01" c
-0000c480: 793d 2235 2e36 3138 3537 3030 3065 2b30  y="5.61857000e+0
-0000c490: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000c4a0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000c4b0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000c4c0: 372e 3630 3232 3237 3630 652b 3031 2220  7.60222760e+01" 
-0000c4d0: 6379 3d22 312e 3338 3937 3932 3230 652b  cy="1.38979220e+
-0000c4e0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000c4f0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000c500: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000c510: 2234 2e35 3139 3832 3537 3065 2b30 3122  "4.51982570e+01"
-0000c520: 2063 793d 2231 2e32 3039 3431 3837 3065   cy="1.20941870e
-0000c530: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000c540: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000c550: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000c560: 3d22 352e 3130 3734 3235 3830 652b 3031  ="5.10742580e+01
-0000c570: 2220 6379 3d22 322e 3130 3230 3737 3430  " cy="2.10207740
-0000c580: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000c590: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000c5a0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000c5b0: 783d 2236 2e38 3134 3432 3739 3065 2b30  x="6.81442790e+0
-0000c5c0: 3122 2063 793d 2236 2e34 3235 3936 3030  1" cy="6.4259600
-0000c5d0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000c5e0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000c5f0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000c600: 6378 3d22 372e 3830 3938 3538 3530 652b  cx="7.80985850e+
-0000c610: 3031 2220 6379 3d22 342e 3735 3536 3034  01" cy="4.755604
-0000c620: 3130 652b 3031 2220 723d 2230 2e35 3336  10e+01" r="0.536
-0000c630: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000c640: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000c650: 2063 783d 2237 2e30 3235 3639 3438 3065   cx="7.02569480e
-0000c660: 2b30 3122 2063 793d 2236 2e32 3438 3138  +01" cy="6.24818
-0000c670: 3339 3065 2b30 3122 2072 3d22 302e 3533  390e+01" r="0.53
-0000c680: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000c690: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000c6a0: 6520 6378 3d22 352e 3231 3434 3639 3130  e cx="5.21446910
-0000c6b0: 652b 3031 2220 6379 3d22 312e 3930 3339  e+01" cy="1.9039
-0000c6c0: 3331 3630 652b 3031 2220 723d 2230 2e35  3160e+01" r="0.5
-0000c6d0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000c6e0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000c6f0: 6c65 2063 783d 2236 2e31 3536 3237 3431  le cx="6.1562741
-0000c700: 3065 2b30 3122 2063 793d 2238 2e35 3734  0e+01" cy="8.574
-0000c710: 3432 3230 3065 2b30 3022 2072 3d22 302e  42200e+00" r="0.
-0000c720: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000c730: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000c740: 636c 6520 6378 3d22 362e 3630 3135 3834  cle cx="6.601584
-0000c750: 3230 652b 3031 2220 6379 3d22 362e 3332  20e+01" cy="6.32
-0000c760: 3937 3431 3030 652b 3031 2220 723d 2230  974100e+01" r="0
-0000c770: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000c780: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000c790: 7263 6c65 2063 783d 2237 2e30 3239 3236  rcle cx="7.02926
-0000c7a0: 3936 3065 2b30 3122 2063 793d 2235 2e39  960e+01" cy="5.9
-0000c7b0: 3731 3831 3130 3065 2b30 3122 2072 3d22  7181100e+01" r="
-0000c7c0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000c7d0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000c7e0: 6972 636c 6520 6378 3d22 382e 3033 3031  ircle cx="8.0301
-0000c7f0: 3936 3530 652b 3031 2220 6379 3d22 342e  9650e+01" cy="4.
-0000c800: 3730 3339 3833 3730 652b 3031 2220 723d  70398370e+01" r=
-0000c810: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000c820: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000c830: 6369 7263 6c65 2063 783d 2238 2e33 3439  circle cx="8.349
-0000c840: 3832 3739 3065 2b30 3122 2063 793d 2239  82790e+01" cy="9
-0000c850: 2e30 3032 3335 3430 3065 2b30 3022 2072  .00235400e+00" r
-0000c860: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000c870: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000c880: 3c63 6972 636c 6520 6378 3d22 352e 3734  <circle cx="5.74
-0000c890: 3132 3736 3930 652b 3031 2220 6379 3d22  127690e+01" cy="
-0000c8a0: 372e 3030 3635 3536 3330 652b 3031 2220  7.00655630e+01" 
-0000c8b0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000c8c0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000c8d0: 203c 6369 7263 6c65 2063 783d 2235 2e35   <circle cx="5.5
-0000c8e0: 3133 3735 3531 3065 2b30 3122 2063 793d  1375510e+01" cy=
-0000c8f0: 2231 2e32 3632 3234 3531 3065 2b30 3122  "1.26224510e+01"
-0000c900: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000c910: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000c920: 2020 3c63 6972 636c 6520 6378 3d22 352e    <circle cx="5.
-0000c930: 3035 3130 3231 3030 652b 3031 2220 6379  05102100e+01" cy
-0000c940: 3d22 372e 3938 3239 3731 3730 652b 3031  ="7.98297170e+01
-0000c950: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000c960: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000c970: 2020 203c 6369 7263 6c65 2063 783d 2236     <circle cx="6
-0000c980: 2e31 3431 3832 3733 3065 2b30 3122 2063  .14182730e+01" c
-0000c990: 793d 2236 2e38 3130 3938 3336 3065 2b30  y="6.81098360e+0
-0000c9a0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000c9b0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000c9c0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000c9d0: 332e 3238 3730 3330 3930 652b 3031 2220  3.28703090e+01" 
-0000c9e0: 6379 3d22 312e 3432 3231 3732 3430 652b  cy="1.42217240e+
-0000c9f0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000ca00: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000ca10: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000ca20: 2235 2e32 3930 3130 3639 3065 2b30 3122  "5.29010690e+01"
-0000ca30: 2063 793d 2237 2e36 3230 3234 3734 3065   cy="7.62024740e
-0000ca40: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000ca50: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000ca60: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000ca70: 3d22 312e 3835 3030 3030 3030 652b 3031  ="1.85000000e+01
-0000ca80: 2220 6379 3d22 312e 3130 3030 3030 3330  " cy="1.10000030
-0000ca90: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000caa0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000cab0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000cac0: 783d 2239 2e30 3433 3037 3930 3065 2b30  x="9.04307900e+0
-0000cad0: 3122 2063 793d 2235 2e39 3838 3139 3733  1" cy="5.9881973
-0000cae0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000caf0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000cb00: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000cb10: 6378 3d22 342e 3531 3838 3931 3530 652b  cx="4.51889150e+
-0000cb20: 3031 2220 6379 3d22 372e 3834 3535 3934  01" cy="7.845594
-0000cb30: 3830 652b 3031 2220 723d 2230 2e35 3336  80e+01" r="0.536
-0000cb40: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000cb50: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000cb60: 2063 783d 2236 2e30 3834 3531 3731 3065   cx="6.08451710e
-0000cb70: 2b30 3122 2063 793d 2236 2e33 3736 3439  +01" cy="6.37649
-0000cb80: 3432 3065 2b30 3122 2072 3d22 302e 3533  420e+01" r="0.53
-0000cb90: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000cba0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000cbb0: 6520 6378 3d22 352e 3731 3630 3937 3630  e cx="5.71609760
-0000cbc0: 652b 3031 2220 6379 3d22 372e 3531 3338  e+01" cy="7.5138
-0000cbd0: 3333 3230 652b 3031 2220 723d 2230 2e35  3320e+01" r="0.5
-0000cbe0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000cbf0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000cc00: 6c65 2063 783d 2234 2e39 3839 3733 3337  le cx="4.9897337
-0000cc10: 3065 2b30 3122 2063 793d 2231 2e32 3838  0e+01" cy="1.288
-0000cc20: 3937 3936 3065 2b30 3122 2072 3d22 302e  97960e+01" r="0.
-0000cc30: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000cc40: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000cc50: 636c 6520 6378 3d22 322e 3735 3030 3030  cle cx="2.750000
-0000cc60: 3930 652b 3031 2220 6379 3d22 312e 3639  90e+01" cy="1.69
-0000cc70: 3939 3939 3730 652b 3031 2220 723d 2230  999970e+01" r="0
-0000cc80: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000cc90: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000cca0: 7263 6c65 2063 783d 2232 2e31 3030 3538  rcle cx="2.10058
-0000ccb0: 3739 3065 2b30 3122 2063 793d 2236 2e32  790e+01" cy="6.2
-0000ccc0: 3338 3833 3536 3065 2b30 3122 2072 3d22  3883560e+01" r="
-0000ccd0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000cce0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000ccf0: 6972 636c 6520 6378 3d22 312e 3939 3438  ircle cx="1.9948
-0000cd00: 3038 3230 652b 3031 2220 6379 3d22 362e  0820e+01" cy="6.
-0000cd10: 3639 3131 3637 3530 652b 3031 2220 723d  69116750e+01" r=
-0000cd20: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000cd30: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000cd40: 6369 7263 6c65 2063 783d 2238 2e36 3237  circle cx="8.627
-0000cd50: 3734 3739 3065 2b30 3122 2063 793d 2235  74790e+01" cy="5
-0000cd60: 2e31 3233 3530 3037 3065 2b30 3122 2072  .12350070e+01" r
-0000cd70: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000cd80: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000cd90: 3c63 6972 636c 6520 6378 3d22 322e 3939  <circle cx="2.99
-0000cda0: 3030 3136 3530 652b 3031 2220 6379 3d22  001650e+01" cy="
-0000cdb0: 372e 3539 3131 3139 3830 652b 3031 2220  7.59111980e+01" 
-0000cdc0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000cdd0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000cde0: 203c 6369 7263 6c65 2063 783d 2232 2e35   <circle cx="2.5
-0000cdf0: 3133 3234 3432 3065 2b30 3122 2063 793d  1324420e+01" cy=
-0000ce00: 2237 2e34 3835 3134 3132 3065 2b30 3122  "7.48514120e+01"
-0000ce10: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000ce20: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000ce30: 2020 3c63 6972 636c 6520 6378 3d22 332e    <circle cx="3.
-0000ce40: 3735 3930 3333 3230 652b 3031 2220 6379  75903320e+01" cy
-0000ce50: 3d22 372e 3839 3533 3030 3930 652b 3031  ="7.89530090e+01
-0000ce60: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000ce70: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000ce80: 2020 203c 6369 7263 6c65 2063 783d 2233     <circle cx="3
-0000ce90: 2e33 3035 3333 3531 3065 2b30 3122 2063  .30533510e+01" c
-0000cea0: 793d 2237 2e39 3939 3630 3832 3065 2b30  y="7.99960820e+0
-0000ceb0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000cec0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000ced0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000cee0: 392e 3036 3433 3434 3230 652b 3031 2220  9.06434420e+01" 
-0000cef0: 6379 3d22 382e 3331 3439 3139 3630 652b  cy="8.31491960e+
-0000cf00: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000cf10: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000cf20: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000cf30: 2238 2e34 3832 3137 3032 3065 2b30 3122  "8.48217020e+01"
-0000cf40: 2063 793d 2237 2e34 3536 3133 3630 3065   cy="7.45613600e
-0000cf50: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000cf60: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000cf70: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000cf80: 3d22 392e 3133 3837 3935 3830 652b 3031  ="9.13879580e+01
-0000cf90: 2220 6379 3d22 332e 3833 3930 3537 3630  " cy="3.83905760
-0000cfa0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000cfb0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000cfc0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000cfd0: 783d 2238 2e36 3436 3930 3632 3065 2b30  x="8.64690620e+0
-0000cfe0: 3122 2063 793d 2233 2e30 3835 3735 3439  1" cy="3.0857549
-0000cff0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000d000: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000d010: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000d020: 6378 3d22 382e 3630 3935 3832 3330 652b  cx="8.60958230e+
-0000d030: 3031 2220 6379 3d22 322e 3339 3733 3635  01" cy="2.397365
-0000d040: 3630 652b 3031 2220 723d 2230 2e35 3336  60e+01" r="0.536
-0000d050: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000d060: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000d070: 2063 783d 2238 2e37 3232 3036 3136 3065   cx="8.72206160e
-0000d080: 2b30 3122 2063 793d 2234 2e34 3737 3136  +01" cy="4.47716
-0000d090: 3330 3065 2b30 3122 2072 3d22 302e 3533  300e+01" r="0.53
-0000d0a0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000d0b0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000d0c0: 6520 6378 3d22 322e 3430 3830 3630 3330  e cx="2.40806030
-0000d0d0: 652b 3031 2220 6379 3d22 372e 3030 3933  e+01" cy="7.0093
-0000d0e0: 3832 3330 652b 3031 2220 723d 2230 2e35  8230e+01" r="0.5
-0000d0f0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000d100: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000d110: 6c65 2063 783d 2239 2e30 3939 3832 3835  le cx="9.0998285
-0000d120: 3065 2b30 3122 2063 793d 2231 2e36 3530  0e+01" cy="1.650
-0000d130: 3233 3630 3065 2b30 3122 2072 3d22 302e  23600e+01" r="0.
-0000d140: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000d150: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000d160: 636c 6520 6378 3d22 382e 3436 3031 3237  cle cx="8.460127
-0000d170: 3430 652b 3031 2220 6379 3d22 362e 3632  40e+01" cy="6.62
-0000d180: 3739 3033 3830 652b 3031 2220 723d 2230  790380e+01" r="0
-0000d190: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000d1a0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000d1b0: 7263 6c65 2063 783d 2232 2e30 3837 3330  rcle cx="2.08730
-0000d1c0: 3636 3065 2b30 3122 2063 793d 2234 2e35  660e+01" cy="4.5
-0000d1d0: 3832 3833 3230 3065 2b30 3122 2072 3d22  8283200e+01" r="
-0000d1e0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000d1f0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000d200: 6972 636c 6520 6378 3d22 312e 3830 3934  ircle cx="1.8094
-0000d210: 3138 3130 652b 3031 2220 6379 3d22 342e  1810e+01" cy="4.
-0000d220: 3231 3938 3233 3330 652b 3031 2220 723d  21982330e+01" r=
-0000d230: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000d240: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000d250: 6369 7263 6c65 2063 783d 2232 2e30 3232  circle cx="2.022
-0000d260: 3137 3237 3065 2b30 3122 2063 793d 2233  17270e+01" cy="3
-0000d270: 2e37 3337 3033 3030 3065 2b30 3122 2072  .73703000e+01" r
-0000d280: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000d290: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000d2a0: 3c63 6972 636c 6520 6378 3d22 352e 3132  <circle cx="5.12
-0000d2b0: 3331 3338 3030 652b 3031 2220 6379 3d22  313800e+01" cy="
-0000d2c0: 382e 3632 3830 3838 3931 652b 3031 2220  8.62808891e+01" 
-0000d2d0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000d2e0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000d2f0: 203c 6369 7263 6c65 2063 783d 2235 2e39   <circle cx="5.9
-0000d300: 3837 3839 3133 3065 2b30 3122 2063 793d  8789130e+01" cy=
-0000d310: 2239 2e30 3433 3337 3830 3765 2b30 3122  "9.04337807e+01"
-0000d320: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000d330: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000d340: 2020 3c63 6972 636c 6520 6378 3d22 312e    <circle cx="1.
-0000d350: 3639 3939 3939 3730 652b 3031 2220 6379  69999970e+01" cy
-0000d360: 3d22 322e 3735 3030 3030 3030 652b 3031  ="2.75000000e+01
-0000d370: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000d380: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000d390: 2020 203c 6369 7263 6c65 2063 783d 2238     <circle cx="8
-0000d3a0: 2e33 3134 3334 3435 3065 2b30 3122 2063  .31434450e+01" c
-0000d3b0: 793d 2239 2e30 3634 3931 3935 3765 2b30  y="9.06491957e+0
-0000d3c0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000d3d0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000d3e0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000d3f0: 322e 3130 3234 3036 3830 652b 3031 2220  2.10240680e+01" 
-0000d400: 6379 3d22 352e 3430 3738 3534 3830 652b  cy="5.40785480e+
-0000d410: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000d420: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000d430: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000d440: 2234 2e34 3737 3035 3935 3065 2b30 3122  "4.47705950e+01"
-0000d450: 2063 793d 2238 2e37 3232 3036 3733 3665   cy="8.72206736e
-0000d460: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000d470: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000d480: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000d490: 3d22 362e 3632 3636 3735 3330 652b 3031  ="6.62667530e+01
-0000d4a0: 2220 6379 3d22 382e 3436 3133 3337 3030  " cy="8.46133700
-0000d4b0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000d4c0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000d4d0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000d4e0: 783d 2237 2e34 3534 3634 3032 3065 2b30  x="7.45464020e+0
-0000d4f0: 3122 2063 793d 2238 2e34 3833 3636 3630  1" cy="8.4836660
-0000d500: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000d510: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000d520: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000d530: 6378 3d22 332e 3038 3535 3531 3530 652b  cx="3.08555150e+
-0000d540: 3031 2220 6379 3d22 382e 3634 3637 3132  01" cy="8.646712
-0000d550: 3838 652b 3031 2220 723d 2230 2e35 3336  88e+01" r="0.536
-0000d560: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000d570: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000d580: 2063 783d 2232 2e33 3936 3939 3330 3065   cx="2.39699300e
-0000d590: 2b30 3122 2063 793d 2238 2e36 3039 3231  +01" cy="8.60921
-0000d5a0: 3137 3765 2b30 3122 2072 3d22 302e 3533  177e+01" r="0.53
-0000d5b0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000d5c0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000d5d0: 6520 6378 3d22 312e 3635 3030 3231 3830  e cx="1.65002180
-0000d5e0: 652b 3031 2220 6379 3d22 392e 3039 3936  e+01" cy="9.0996
-0000d5f0: 3134 3636 652b 3031 2220 723d 2230 2e35  1466e+01" r="0.5
-0000d600: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000d610: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000d620: 6c65 2063 783d 2231 2e34 3232 3137 3234  le cx="1.4221724
-0000d630: 3065 2b30 3122 2063 793d 2233 2e32 3837  0e+01" cy="3.287
-0000d640: 3033 3030 3065 2b30 3122 2072 3d22 302e  03000e+01" r="0.
-0000d650: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000d660: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000d670: 636c 6520 6378 3d22 332e 3833 3930 3130  cle cx="3.839010
-0000d680: 3830 652b 3031 2220 6379 3d22 392e 3133  80e+01" cy="9.13
-0000d690: 3837 3539 3137 652b 3031 2220 723d 2230  875917e+01" r="0
-0000d6a0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000d6b0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000d6c0: 7263 6c65 2063 783d 2236 2e33 3735 3539  rcle cx="6.37559
-0000d6d0: 3333 3065 2b30 3122 2063 793d 2236 2e30  330e+01" cy="6.0
-0000d6e0: 3835 3430 3237 3065 2b30 3122 2072 3d22  8540270e+01" r="
-0000d6f0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000d700: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000d710: 6972 636c 6520 6378 3d22 312e 3130 3030  ircle cx="1.1000
-0000d720: 3030 3033 652b 3031 2220 6379 3d22 312e  0003e+01" cy="1.
-0000d730: 3835 3030 3030 3030 652b 3031 2220 723d  85000000e+01" r=
-0000d740: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000d750: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000d760: 6369 7263 6c65 2063 783d 2238 2e32 3231  circle cx="8.221
-0000d770: 3732 3634 3065 2b30 3022 2063 793d 2233  72640e+00" cy="3
-0000d780: 2e38 3837 3032 3934 3065 2b30 3122 2072  .88702940e+01" r
-0000d790: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000d7a0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000d7b0: 3c63 6972 636c 6520 6378 3d22 312e 3236  <circle cx="1.26
-0000d7c0: 3232 3034 3234 652b 3031 2220 6379 3d22  220424e+01" cy="
-0000d7d0: 352e 3531 3337 3132 3830 652b 3031 2220  5.51371280e+01" 
-0000d7e0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000d7f0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000d800: 203c 6369 7263 6c65 2063 783d 2231 2e32   <circle cx="1.2
-0000d810: 3039 3431 3832 3565 2b30 3122 2063 793d  0941825e+01" cy=
-0000d820: 2234 2e35 3139 3832 3330 3065 2b30 3122  "4.51982300e+01"
-0000d830: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000d840: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000d850: 2020 3c63 6972 636c 6520 6378 3d22 382e    <circle cx="8.
-0000d860: 3537 3430 3236 3930 652b 3030 2220 6379  57402690e+00" cy
-0000d870: 3d22 362e 3135 3632 3331 3830 652b 3031  ="6.15623180e+01
-0000d880: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000d890: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000d8a0: 2020 203c 6369 7263 6c65 2063 783d 2238     <circle cx="8
-0000d8b0: 2e31 3231 3537 3839 3065 2b30 3122 2063  .12157890e+01" c
-0000d8c0: 793d 2234 2e31 3735 3032 3934 3065 2b30  y="4.17502940e+0
-0000d8d0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000d8e0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000d8f0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000d900: 342e 3137 3439 3238 3630 652b 3031 2220  4.17492860e+01" 
-0000d910: 6379 3d22 382e 3132 3135 3833 3430 652b  cy="8.12158340e+
-0000d920: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000d930: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000d940: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000d950: 2231 2e38 3839 3231 3834 3065 2b30 3122  "1.88921840e+01"
-0000d960: 2063 793d 2234 2e39 3839 3939 3635 3065   cy="4.98999650e
-0000d970: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000d980: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000d990: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000d9a0: 3d22 372e 3834 3535 3631 3530 652b 3031  ="7.84556150e+01
-0000d9b0: 2220 6379 3d22 342e 3531 3839 3530 3030  " cy="4.51895000
-0000d9c0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000d9d0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000d9e0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000d9f0: 783d 2231 2e32 3838 3937 3934 3265 2b30  x="1.28897942e+0
-0000da00: 3122 2063 793d 2234 2e39 3839 3733 3130  1" cy="4.9897310
-0000da10: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000da20: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000da30: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000da40: 6378 3d22 372e 3839 3533 3334 3230 652b  cx="7.89533420e+
-0000da50: 3031 2220 6379 3d22 332e 3735 3930 3738  01" cy="3.759078
-0000da60: 3230 652b 3031 2220 723d 2230 2e35 3336  20e+01" r="0.536
-0000da70: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000da80: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000da90: 2063 783d 2231 2e38 3631 3638 3734 3065   cx="1.86168740e
-0000daa0: 2b30 3122 2063 793d 2235 2e38 3132 3231  +01" cy="5.81221
-0000dab0: 3034 3065 2b30 3122 2072 3d22 302e 3533  040e+01" r="0.53
-0000dac0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000dad0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000dae0: 6520 6378 3d22 312e 3338 3934 3231 3331  e cx="1.38942131
-0000daf0: 652b 3031 2220 6379 3d22 372e 3630 3138  e+01" cy="7.6018
-0000db00: 3534 3130 652b 3031 2220 723d 2230 2e35  5410e+01" r="0.5
-0000db10: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000db20: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000db30: 6c65 2063 783d 2239 2e30 3030 3232 3130  le cx="9.0002210
-0000db40: 3065 2b30 3022 2063 793d 2238 2e33 3439  0e+00" cy="8.349
-0000db50: 3631 3436 3065 2b30 3122 2072 3d22 302e  61460e+01" r="0.
-0000db60: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000db70: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000db80: 636c 6520 6378 3d22 312e 3334 3833 3933  cle cx="1.348393
-0000db90: 3139 652b 3031 2220 6379 3d22 362e 3931  19e+01" cy="6.91
-0000dba0: 3030 3731 3830 652b 3031 2220 723d 2230  007180e+01" r="0
-0000dbb0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000dbc0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000dbd0: 7263 6c65 2063 783d 2234 2e39 3839 3939  rcle cx="4.98999
-0000dbe0: 3833 3065 2b30 3122 2063 793d 2231 2e38  830e+01" cy="1.8
-0000dbf0: 3839 3231 3834 3065 2b30 3122 2072 3d22  8921840e+01" r="
-0000dc00: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000dc10: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000dc20: 6972 636c 6520 6378 3d22 372e 3632 3234  ircle cx="7.6224
-0000dc30: 3635 3930 652b 3031 2220 6379 3d22 372e  6590e+01" cy="7.
-0000dc40: 3632 3438 3832 3430 652b 3031 2220 723d  62488240e+01" r=
-0000dc50: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000dc60: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000dc70: 6369 7263 6c65 2063 783d 2236 2e32 3338  circle cx="6.238
-0000dc80: 3837 3631 3065 2b30 3122 2063 793d 2232  87610e+01" cy="2
-0000dc90: 2e31 3030 3632 3438 3065 2b30 3122 2072  .10062480e+01" r
-0000dca0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000dcb0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000dcc0: 3c63 6972 636c 6520 6378 3d22 322e 3133  <circle cx="2.13
-0000dcd0: 3630 3230 3930 652b 3031 2220 6379 3d22  602090e+01" cy="
-0000dce0: 372e 3836 3139 3531 3430 652b 3031 2220  7.86195140e+01" 
-0000dcf0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000dd00: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000dd10: 203c 6369 7263 6c65 2063 783d 2234 2e32   <circle cx="4.2
-0000dd20: 3139 3832 3531 3065 2b30 3122 2063 793d  1982510e+01" cy=
-0000dd30: 2231 2e38 3039 3431 3831 3065 2b30 3122  "1.80941810e+01"
-0000dd40: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000dd50: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000dd60: 2020 3c63 6972 636c 6520 6378 3d22 352e    <circle cx="5.
-0000dd70: 3831 3232 3530 3930 652b 3031 2220 6379  81225090e+01" cy
-0000dd80: 3d22 312e 3836 3137 3238 3830 652b 3031  ="1.86172880e+01
-0000dd90: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000dda0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000ddb0: 2020 203c 6369 7263 6c65 2063 783d 2233     <circle cx="3
-0000ddc0: 2e37 3337 3033 3039 3065 2b30 3122 2063  .73703090e+01" c
-0000ddd0: 793d 2232 2e30 3232 3137 3237 3065 2b30  y="2.02217270e+0
-0000dde0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000ddf0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000de00: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000de10: 342e 3538 3238 3332 3930 652b 3031 2220  4.58283290e+01" 
-0000de20: 6379 3d22 322e 3038 3733 3036 3630 652b  cy="2.08730660e+
-0000de30: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000de40: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000de50: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000de60: 2236 2e35 3239 3534 3436 3065 2b30 3122  "6.52954460e+01"
-0000de70: 2063 793d 2237 2e32 3031 3530 3038 3065   cy="7.20150080e
-0000de80: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000de90: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000dea0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000deb0: 3d22 372e 3139 3839 3038 3830 652b 3031  ="7.19890880e+01
-0000dec0: 2220 6379 3d22 362e 3533 3231 3333 3930  " cy="6.53213390
-0000ded0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000dee0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000def0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000df00: 783d 2235 2e34 3037 3835 3537 3065 2b30  x="5.40785570e+0
-0000df10: 3122 2063 793d 2232 2e31 3032 3430 3638  1" cy="2.1024068
-0000df20: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000df30: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000df40: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000df50: 6378 3d22 372e 3039 3135 3930 3130 652b  cx="7.09159010e+
-0000df60: 3031 2220 6379 3d22 372e 3039 3433 3738  01" cy="7.094378
-0000df70: 3330 652b 3031 2220 723d 2230 2e35 3336  30e+01" r="0.536
-0000df80: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000df90: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000dfa0: 2063 783d 2236 2e32 3333 3436 3938 3065   cx="6.23346980e
-0000dfb0: 2b30 3122 2063 793d 2237 2e37 3130 3731  +01" cy="7.71071
-0000dfc0: 3237 3065 2b30 3122 2072 3d22 302e 3533  270e+01" r="0.53
-0000dfd0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000dfe0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000dff0: 6520 6378 3d22 372e 3730 3837 3733 3230  e cx="7.70877320
-0000e000: 652b 3031 2220 6379 3d22 362e 3233 3534  e+01" cy="6.2354
-0000e010: 3236 3430 652b 3031 2220 723d 2230 2e35  2640e+01" r="0.5
-0000e020: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000e030: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000e040: 6c65 2063 783d 2237 2e38 3632 3438 3135  le cx="7.8624815
-0000e050: 3065 2b30 3122 2063 793d 2232 2e31 3336  0e+01" cy="2.136
-0000e060: 3535 3139 3065 2b30 3122 2072 3d22 302e  55190e+01" r="0.
-0000e070: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000e080: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000e090: 636c 6520 6378 3d22 372e 3939 3938 3034  cle cx="7.999804
-0000e0a0: 3430 652b 3031 2220 6379 3d22 332e 3330  40e+01" cy="3.30
-0000e0b0: 3535 3332 3230 652b 3031 2220 723d 2230  553220e+01" r="0
-0000e0c0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000e0d0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000e0e0: 7263 6c65 2063 783d 2236 2e38 3039 3336  rcle cx="6.80936
-0000e0f0: 3831 3065 2b30 3122 2063 793d 2236 2e31  810e+01" cy="6.1
-0000e100: 3433 3436 3335 3065 2b30 3122 2072 3d22  4346350e+01" r="
-0000e110: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000e120: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000e130: 6972 636c 6520 6378 3d22 372e 3030 3537  ircle cx="7.0057
-0000e140: 3939 3430 652b 3031 2220 6379 3d22 352e  9940e+01" cy="5.
-0000e150: 3734 3139 3936 3030 652b 3031 2220 723d  74199600e+01" r=
-0000e160: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000e170: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000e180: 6369 7263 6c65 2063 783d 2236 2e36 3931  circle cx="6.691
-0000e190: 3336 3130 3065 2b30 3122 2063 793d 2231  36100e+01" cy="1
-0000e1a0: 2e39 3935 3030 3830 3065 2b30 3122 2072  .99500800e+01" r
-0000e1b0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000e1c0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000e1d0: 3c63 6972 636c 6520 6378 3d22 372e 3531  <circle cx="7.51
-0000e1e0: 3238 3039 3030 652b 3031 2220 6379 3d22  280900e+01" cy="
-0000e1f0: 352e 3731 3730 3834 3930 652b 3031 2220  5.71708490e+01" 
-0000e200: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000e210: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000e220: 203c 6369 7263 6c65 2063 783d 2237 2e36   <circle cx="7.6
-0000e230: 3139 3934 3638 3065 2b30 3122 2063 793d  1994680e+01" cy=
-0000e240: 2235 2e32 3930 3431 3734 3065 2b30 3122  "5.29041740e+01"
-0000e250: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000e260: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000e270: 2020 3c63 6972 636c 6520 6378 3d22 372e    <circle cx="7.
-0000e280: 3539 3132 3732 3830 652b 3031 2220 6379  59127280e+01" cy
-0000e290: 3d22 322e 3939 3031 3833 3030 652b 3031  ="2.99018300e+01
-0000e2a0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000e2b0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000e2c0: 2020 203c 6369 7263 6c65 2063 783d 2237     <circle cx="7
-0000e2d0: 2e30 3039 3534 3739 3065 2b30 3122 2063  .00954790e+01" c
-0000e2e0: 793d 2232 2e34 3038 3231 3432 3065 2b30  y="2.40821420e+0
-0000e2f0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000e300: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000e310: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000e320: 372e 3938 3236 3339 3630 652b 3031 2220  7.98263960e+01" 
-0000e330: 6379 3d22 352e 3035 3133 3831 3030 652b  cy="5.05138100e+
-0000e340: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000e350: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000e360: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000e370: 2237 2e34 3835 3435 3038 3065 2b30 3122  "7.48545080e+01"
-0000e380: 2063 793d 2232 2e35 3133 3535 3437 3065   cy="2.51355470e
-0000e390: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000e3a0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000e3b0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000e3c0: 3d22 372e 3730 3030 3030 3030 652b 3031  ="7.70000000e+01
-0000e3d0: 2220 6379 3d22 332e 3836 3736 3835 3730  " cy="3.86768570
-0000e3e0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000e3f0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000e400: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000e410: 783d 2237 2e36 3535 3534 3831 3065 2b30  x="7.65554810e+0
-0000e420: 3122 2063 793d 2233 2e36 3334 3634 3234  1" cy="3.6346424
-0000e430: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000e440: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000e450: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000e460: 6378 3d22 372e 3536 3239 3833 3130 652b  cx="7.56298310e+
-0000e470: 3031 2220 6379 3d22 332e 3431 3131 3639  01" cy="3.411169
-0000e480: 3730 652b 3031 2220 723d 2230 2e35 3336  70e+01" r="0.536
-0000e490: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000e4a0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000e4b0: 2063 783d 2237 2e34 3732 3832 3734 3065   cx="7.47282740e
-0000e4c0: 2b30 3122 2063 793d 2233 2e31 3933 3531  +01" cy="3.19351
-0000e4d0: 3535 3065 2b30 3122 2072 3d22 302e 3533  550e+01" r="0.53
-0000e4e0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000e4f0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000e500: 6520 6378 3d22 372e 3334 3135 3735 3030  e cx="7.34157500
-0000e510: 652b 3031 2220 6379 3d22 322e 3939 3539  e+01" cy="2.9959
-0000e520: 3930 3730 652b 3031 2220 723d 2230 2e35  9070e+01" r="0.5
-0000e530: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000e540: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000e550: 6c65 2063 783d 2237 2e31 3732 3739 3236  le cx="7.1727926
-0000e560: 3065 2b30 3122 2063 793d 2232 2e38 3237  0e+01" cy="2.827
-0000e570: 3230 3833 3065 2b30 3122 2072 3d22 302e  20830e+01" r="0.
-0000e580: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000e590: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000e5a0: 636c 6520 6378 3d22 372e 3030 3430 3039  cle cx="7.004009
-0000e5b0: 3330 652b 3031 2220 6379 3d22 322e 3635  30e+01" cy="2.65
-0000e5c0: 3834 3235 3030 652b 3031 2220 723d 2230  842500e+01" r="0
-0000e5d0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000e5e0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000e5f0: 7263 6c65 2063 783d 2236 2e38 3036 3438  rcle cx="6.80648
-0000e600: 3435 3065 2b30 3122 2063 793d 2232 2e35  450e+01" cy="2.5
-0000e610: 3237 3137 3236 3065 2b30 3122 2072 3d22  2717260e+01" r="
-0000e620: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000e630: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000e640: 6972 636c 6520 6378 3d22 362e 3538 3838  ircle cx="6.5888
-0000e650: 3330 3330 652b 3031 2220 6379 3d22 322e  3030e+01" cy="2.
-0000e660: 3433 3730 3136 3930 652b 3031 2220 723d  43701690e+01" r=
-0000e670: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000e680: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000e690: 6369 7263 6c65 2063 783d 2236 2e33 3635  circle cx="6.365
-0000e6a0: 3335 3736 3065 2b30 3122 2063 793d 2232  35760e+01" cy="2
-0000e6b0: 2e33 3434 3435 3139 3065 2b30 3122 2072  .34445190e+01" r
-0000e6c0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000e6d0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000e6e0: 3c63 6972 636c 6520 6378 3d22 362e 3133  <circle cx="6.13
-0000e6f0: 3233 3134 3330 652b 3031 2220 6379 3d22  231430e+01" cy="
-0000e700: 322e 3330 3030 3030 3030 652b 3031 2220  2.30000000e+01" 
-0000e710: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000e720: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000e730: 203c 6369 7263 6c65 2063 783d 2235 2e36   <circle cx="5.6
-0000e740: 3030 3030 3033 3065 2b30 3122 2063 793d  0000030e+01" cy=
-0000e750: 2232 2e33 3030 3030 3030 3065 2b30 3122  "2.30000000e+01"
-0000e760: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000e770: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000e780: 2020 3c63 6972 636c 6520 6378 3d22 352e    <circle cx="5.
-0000e790: 3239 3939 3939 3730 652b 3031 2220 6379  29999970e+01" cy
-0000e7a0: 3d22 322e 3330 3030 3030 3030 652b 3031  ="2.30000000e+01
-0000e7b0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000e7c0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000e7d0: 2020 203c 6369 7263 6c65 2063 783d 2235     <circle cx="5
-0000e7e0: 2e30 3030 3030 3030 3065 2b30 3122 2063  .00000000e+01" c
-0000e7f0: 793d 2232 2e33 3030 3030 3030 3065 2b30  y="2.30000000e+0
-0000e800: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000e810: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000e820: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000e830: 342e 3730 3030 3030 3330 652b 3031 2220  4.70000030e+01" 
-0000e840: 6379 3d22 322e 3330 3030 3030 3030 652b  cy="2.30000000e+
-0000e850: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000e860: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000e870: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000e880: 2234 2e34 3030 3030 3036 3065 2b30 3122  "4.40000060e+01"
-0000e890: 2063 793d 2232 2e33 3030 3030 3030 3065   cy="2.30000000e
-0000e8a0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000e8b0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000e8c0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000e8d0: 3d22 342e 3130 3030 3030 3930 652b 3031  ="4.10000090e+01
-0000e8e0: 2220 6379 3d22 322e 3330 3030 3030 3030  " cy="2.30000000
-0000e8f0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000e900: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000e910: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
-0000e920: 783d 2233 2e38 3030 3030 3033 3065 2b30  x="3.80000030e+0
-0000e930: 3122 2063 793d 2232 2e33 3030 3030 3030  1" cy="2.3000000
-0000e940: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
-0000e950: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
-0000e960: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
-0000e970: 6378 3d22 332e 3530 3030 3030 3630 652b  cx="3.50000060e+
-0000e980: 3031 2220 6379 3d22 322e 3330 3030 3030  01" cy="2.300000
-0000e990: 3030 652b 3031 2220 723d 2230 2e35 3336  00e+01" r="0.536
-0000e9a0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
-0000e9b0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
-0000e9c0: 2063 783d 2233 2e32 3030 3030 3030 3065   cx="3.20000000e
-0000e9d0: 2b30 3122 2063 793d 2232 2e33 3030 3030  +01" cy="2.30000
-0000e9e0: 3030 3065 2b30 3122 2072 3d22 302e 3533  000e+01" r="0.53
-0000e9f0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
-0000ea00: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
-0000ea10: 6520 6378 3d22 322e 3930 3030 3030 3330  e cx="2.90000030
-0000ea20: 652b 3031 2220 6379 3d22 322e 3330 3030  e+01" cy="2.3000
-0000ea30: 3030 3030 652b 3031 2220 723d 2230 2e35  0000e+01" r="0.5
-0000ea40: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
-0000ea50: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
-0000ea60: 6c65 2063 783d 2232 2e35 3939 3939 3937  le cx="2.5999997
-0000ea70: 3065 2b30 3122 2063 793d 2232 2e33 3030  0e+01" cy="2.300
-0000ea80: 3030 3030 3065 2b30 3122 2072 3d22 302e  00000e+01" r="0.
-0000ea90: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
-0000eaa0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
-0000eab0: 636c 6520 6378 3d22 362e 3133 3233 3134  cle cx="6.132314
-0000eac0: 3330 652b 3031 2220 6379 3d22 352e 3930  30e+01" cy="5.90
-0000ead0: 3030 3030 3030 652b 3031 2220 723d 2230  000000e+01" r="0
-0000eae0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
-0000eaf0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
-0000eb00: 7263 6c65 2063 783d 2236 2e33 3635 3335  rcle cx="6.36535
-0000eb10: 3736 3065 2b30 3122 2063 793d 2235 2e38  760e+01" cy="5.8
-0000eb20: 3535 3534 3831 3065 2b30 3122 2072 3d22  5554810e+01" r="
-0000eb30: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
-0000eb40: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
-0000eb50: 6972 636c 6520 6378 3d22 362e 3538 3838  ircle cx="6.5888
-0000eb60: 3330 3330 652b 3031 2220 6379 3d22 352e  3030e+01" cy="5.
-0000eb70: 3736 3239 3833 3130 652b 3031 2220 723d  76298310e+01" r=
-0000eb80: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
-0000eb90: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
-0000eba0: 6369 7263 6c65 2063 783d 2236 2e38 3036  circle cx="6.806
-0000ebb0: 3438 3435 3065 2b30 3122 2063 793d 2235  48450e+01" cy="5
-0000ebc0: 2e36 3732 3832 3734 3065 2b30 3122 2072  .67282740e+01" r
-0000ebd0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
-0000ebe0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
-0000ebf0: 3c63 6972 636c 6520 6378 3d22 372e 3030  <circle cx="7.00
-0000ec00: 3430 3039 3330 652b 3031 2220 6379 3d22  400930e+01" cy="
-0000ec10: 352e 3534 3135 3735 3030 652b 3031 2220  5.54157500e+01" 
-0000ec20: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
-0000ec30: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
-0000ec40: 203c 6369 7263 6c65 2063 783d 2237 2e31   <circle cx="7.1
-0000ec50: 3732 3739 3137 3065 2b30 3122 2063 793d  7279170e+01" cy=
-0000ec60: 2235 2e33 3732 3739 3236 3065 2b30 3122  "5.37279260e+01"
-0000ec70: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
-0000ec80: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
-0000ec90: 2020 3c63 6972 636c 6520 6378 3d22 372e    <circle cx="7.
-0000eca0: 3334 3135 3735 3030 652b 3031 2220 6379  34157500e+01" cy
-0000ecb0: 3d22 352e 3230 3430 3039 3330 652b 3031  ="5.20400930e+01
-0000ecc0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
-0000ecd0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
-0000ece0: 2020 203c 6369 7263 6c65 2063 783d 2237     <circle cx="7
-0000ecf0: 2e34 3732 3832 3734 3065 2b30 3122 2063  .47282740e+01" c
-0000ed00: 793d 2235 2e30 3036 3438 3435 3065 2b30  y="5.00648450e+0
-0000ed10: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
-0000ed20: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
-0000ed30: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
-0000ed40: 372e 3536 3239 3833 3130 652b 3031 2220  7.56298310e+01" 
-0000ed50: 6379 3d22 342e 3738 3838 3330 3330 652b  cy="4.78883030e+
-0000ed60: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
-0000ed70: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
-0000ed80: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
-0000ed90: 2237 2e36 3535 3534 3831 3065 2b30 3122  "7.65554810e+01"
-0000eda0: 2063 793d 2234 2e35 3635 3335 3736 3065   cy="4.56535760e
-0000edb0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
-0000edc0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
-0000edd0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
-0000ede0: 3d22 372e 3730 3030 3030 3030 652b 3031  ="7.70000000e+01
-0000edf0: 2220 6379 3d22 342e 3333 3233 3134 3330  " cy="4.33231430
-0000ee00: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
-0000ee10: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
-0000ee20: 0a20 2020 3c2f 673e 0d0a 3c2f 7376 673e  .   </g>..</svg>
+00001130: 3636 3830 652b 3031 2051 2035 2e39 3032  6680e+01 Q 5.902
+00001140: 3732 3035 3865 2b30 3120 372e 3232 3933  72058e+01 7.2293
+00001150: 3932 3432 652b 3031 2c20 352e 3733 3139  9242e+01, 5.7319
+00001160: 3538 3533 652b 3031 2037 2e32 3136 3337  5853e+01 7.21637
+00001170: 3534 3665 2b30 3120 5120 352e 3536 3133  546e+01 Q 5.5613
+00001180: 3739 3031 652b 3031 2037 2e32 3033 3536  7901e+01 7.20356
+00001190: 3338 3065 2b30 312c 2035 2e33 3732 3739  380e+01, 5.37279
+000011a0: 3137 3065 2b30 3120 372e 3137 3237 3932  170e+01 7.172792
+000011b0: 3630 652b 3031 205a 2220 2f3e 0d0a 2020  60e+01 Z" />..  
+000011c0: 2020 2020 3c70 6174 6820 643d 224d 2035      <path d="M 5
+000011d0: 2e39 3030 3030 3030 3065 2b30 3120 352e  .90000000e+01 5.
+000011e0: 3930 3030 3030 3030 652b 3031 2051 2035  90000000e+01 Q 5
+000011f0: 2e39 3030 3531 3730 3765 2b30 3120 362e  .90051707e+01 6.
+00001200: 3036 3630 3833 3437 652b 3031 2c20 352e  06608347e+01, 5.
+00001210: 3836 3734 3439 3433 652b 3031 2036 2e32  86744943e+01 6.2
+00001220: 3430 3736 3636 3065 2b30 3120 5120 352e  4076660e+01 Q 5.
+00001230: 3833 3431 3631 3635 652b 3031 2036 2e34  83416165e+01 6.4
+00001240: 3135 3633 3331 3165 2b30 312c 2035 2e37  1563311e+01, 5.7
+00001250: 3632 3938 3331 3065 2b30 3120 362e 3538  6298310e+01 6.58
+00001260: 3838 3330 3330 652b 3031 2051 2035 2e39  883030e+01 Q 5.9
+00001270: 3930 3439 3233 3265 2b30 3120 362e 3630  9049232e+01 6.60
+00001280: 3139 3532 3736 652b 3031 2c20 362e 3139  195276e+01, 6.19
+00001290: 3335 3132 3638 652b 3031 2036 2e36 3033  351268e+01 6.603
+000012a0: 3037 3833 3165 2b30 3120 5120 362e 3339  07831e+01 Q 6.39
+000012b0: 3834 3034 3632 652b 3031 2036 2e36 3034  840462e+01 6.604
+000012c0: 3334 3530 3065 2b30 312c 2036 2e36 3030  34500e+01, 6.600
+000012d0: 3938 3735 3065 2b30 3120 362e 3630 3338  98750e+01 6.6038
+000012e0: 3136 3230 652b 3031 204c 2035 2e39 3030  1620e+01 L 5.900
+000012f0: 3030 3030 3065 2b30 3120 352e 3930 3030  00000e+01 5.9000
+00001300: 3030 3030 652b 3031 205a 2220 2f3e 0d0a  0000e+01 Z" />..
+00001310: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
+00001320: 2035 2e37 3632 3938 3331 3065 2b30 3120   5.76298310e+01 
+00001330: 362e 3538 3838 3330 3330 652b 3031 2051  6.58883030e+01 Q
+00001340: 2035 2e38 3536 3637 3439 3465 2b30 3120   5.85667494e+01 
+00001350: 362e 3735 3932 3835 3938 652b 3031 2c20  6.75928598e+01, 
+00001360: 352e 3932 3733 3437 3930 652b 3031 2036  5.92734790e+01 6
+00001370: 2e39 3233 3231 3239 3165 2b30 3120 5120  .92321291e+01 Q 
+00001380: 352e 3939 3738 3637 3631 652b 3031 2037  5.99786761e+01 7
+00001390: 2e30 3836 3633 3137 3065 2b30 312c 2036  .08663170e+01, 6
+000013a0: 2e30 3637 3837 3631 3065 2b30 3120 372e  .06787610e+01 7.
+000013b0: 3234 3236 3636 3830 652b 3031 204c 2036  24266680e+01 L 6
+000013c0: 2e36 3030 3938 3735 3065 2b30 3120 362e  .60098750e+01 6.
+000013d0: 3630 3338 3136 3230 652b 3031 2051 2036  60381620e+01 Q 6
+000013e0: 2e33 3938 3430 3436 3265 2b30 3120 362e  .39840462e+01 6.
+000013f0: 3630 3433 3435 3030 652b 3031 2c20 362e  60434500e+01, 6.
+00001400: 3139 3335 3132 3638 652b 3031 2036 2e36  19351268e+01 6.6
+00001410: 3033 3037 3833 3165 2b30 3120 5120 352e  0307831e+01 Q 5.
+00001420: 3939 3034 3932 3332 652b 3031 2036 2e36  99049232e+01 6.6
+00001430: 3031 3935 3237 3665 2b30 312c 2035 2e37  0195276e+01, 5.7
+00001440: 3632 3938 3331 3065 2b30 3120 362e 3538  6298310e+01 6.58
+00001450: 3838 3330 3330 652b 3031 205a 2220 2f3e  883030e+01 Z" />
+00001460: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
+00001470: 224d 2039 2e35 3030 3030 3030 3065 2b30  "M 9.50000000e+0
+00001480: 3120 372e 3235 3030 3030 3030 652b 3031  1 7.25000000e+01
+00001490: 204c 2039 2e35 3030 3030 3030 3065 2b30   L 9.50000000e+0
+000014a0: 3120 352e 3030 3030 3031 3830 652b 3031  1 5.00000180e+01
+000014b0: 204c 2038 2e31 3239 3738 3639 3065 2b30   L 8.12978690e+0
+000014c0: 3120 352e 3731 3136 3634 3230 652b 3031  1 5.71166420e+01
+000014d0: 2051 2038 2e34 3832 3132 3830 3265 2b30   Q 8.48212802e+0
+000014e0: 3120 362e 3130 3833 3839 3730 652b 3031  1 6.10838970e+01
+000014f0: 2c20 382e 3831 3839 3332 3532 652b 3031  , 8.81893252e+01
+00001500: 2036 2e34 3836 3630 3738 3965 2b30 3120   6.48660789e+01 
+00001510: 5120 392e 3135 3633 3230 3032 652b 3031  Q 9.15632002e+01
+00001520: 2036 2e38 3635 3439 3232 3865 2b30 312c   6.86549228e+01,
+00001530: 2039 2e35 3030 3030 3030 3065 2b30 3120   9.50000000e+01 
+00001540: 372e 3235 3030 3030 3030 652b 3031 205a  7.25000000e+01 Z
+00001550: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+00001560: 6820 643d 224d 2039 2e35 3030 3030 3030  h d="M 9.5000000
+00001570: 3065 2b30 3120 392e 3530 3030 3030 3030  0e+01 9.50000000
+00001580: 652b 3031 204c 2039 2e35 3030 3030 3030  e+01 L 9.5000000
+00001590: 3065 2b30 3120 372e 3235 3030 3030 3030  0e+01 7.25000000
+000015a0: 652b 3031 204c 2038 2e31 3933 3033 3335  e+01 L 8.1930335
+000015b0: 3065 2b30 3120 382e 3139 3437 3538 3830  0e+01 8.19475880
+000015c0: 652b 3031 204c 2039 2e35 3030 3030 3030  e+01 L 9.5000000
+000015d0: 3065 2b30 3120 392e 3530 3030 3030 3030  0e+01 9.50000000
+000015e0: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
+000015f0: 2020 3c70 6174 6820 643d 224d 2038 2e31    <path d="M 8.1
+00001600: 3933 3033 3335 3065 2b30 3120 382e 3139  9303350e+01 8.19
+00001610: 3437 3538 3830 652b 3031 204c 2039 2e35  475880e+01 L 9.5
+00001620: 3030 3030 3030 3065 2b30 3120 372e 3235  0000000e+01 7.25
+00001630: 3030 3030 3030 652b 3031 204c 2037 2e37  000000e+01 L 7.7
+00001640: 3533 3437 3632 3065 2b30 3120 362e 3932  5347620e+01 6.92
+00001650: 3336 3439 3230 652b 3031 204c 2038 2e31  364920e+01 L 8.1
+00001660: 3933 3033 3335 3065 2b30 3120 382e 3139  9303350e+01 8.19
+00001670: 3437 3538 3830 652b 3031 205a 2220 2f3e  475880e+01 Z" />
+00001680: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
+00001690: 224d 2039 2e35 3030 3030 3030 3065 2b30  "M 9.50000000e+0
+000016a0: 3120 372e 3235 3030 3030 3030 652b 3031  1 7.25000000e+01
+000016b0: 2051 2039 2e31 3536 3332 3030 3265 2b30   Q 9.15632002e+0
+000016c0: 3120 362e 3836 3534 3932 3238 652b 3031  1 6.86549228e+01
+000016d0: 2c20 382e 3831 3839 3332 3532 652b 3031  , 8.81893252e+01
+000016e0: 2036 2e34 3836 3630 3738 3965 2b30 3120   6.48660789e+01 
+000016f0: 5120 382e 3438 3231 3238 3032 652b 3031  Q 8.48212802e+01
+00001700: 2036 2e31 3038 3338 3937 3065 2b30 312c   6.10838970e+01,
+00001710: 2038 2e31 3239 3738 3639 3065 2b30 3120   8.12978690e+01 
+00001720: 352e 3731 3136 3634 3230 652b 3031 2051  5.71166420e+01 Q
+00001730: 2038 2e30 3336 3238 3136 3265 2b30 3120   8.03628162e+01 
+00001740: 362e 3031 3832 3433 3034 652b 3031 2c20  6.01824304e+01, 
+00001750: 372e 3934 3138 3738 3636 652b 3031 2036  7.94187866e+01 6
+00001760: 2e33 3234 3237 3638 3565 2b30 3120 5120  .32427685e+01 Q 
+00001770: 372e 3834 3731 3733 3634 652b 3031 2036  7.84717364e+01 6
+00001780: 2e36 3331 3137 3137 3165 2b30 312c 2037  .63117171e+01, 7
+00001790: 2e37 3533 3437 3632 3065 2b30 3120 362e  .75347620e+01 6.
+000017a0: 3932 3336 3439 3230 652b 3031 204c 2039  92364920e+01 L 9
+000017b0: 2e35 3030 3030 3030 3065 2b30 3120 372e  .50000000e+01 7.
+000017c0: 3235 3030 3030 3030 652b 3031 205a 2220  25000000e+01 Z" 
+000017d0: 2f3e 0d0a 2020 2020 2020 3c70 6174 6820  />..      <path 
+000017e0: 643d 224d 2039 2e35 3030 3030 3030 3065  d="M 9.50000000e
+000017f0: 2b30 3120 352e 3030 3030 3031 3830 652b  +01 5.00000180e+
+00001800: 3031 204c 2039 2e35 3030 3030 3030 3065  01 L 9.50000000e
+00001810: 2b30 3120 322e 3735 3030 3030 3930 652b  +01 2.75000090e+
+00001820: 3031 2051 2039 2e32 3330 3438 3632 3165  01 Q 9.23048621e
+00001830: 2b30 3120 332e 3030 3132 3933 3730 652b  +01 3.00129370e+
+00001840: 3031 2c20 382e 3936 3032 3630 3033 652b  01, 8.96026003e+
+00001850: 3031 2033 2e32 3534 3736 3939 3865 2b30  01 3.25476998e+0
+00001860: 3120 5120 382e 3638 3837 3135 3530 652b  1 Q 8.68871550e+
+00001870: 3031 2033 2e35 3039 3438 3033 3265 2b30  01 3.50948032e+0
+00001880: 312c 2038 2e34 3134 3730 3938 3065 2b30  1, 8.41470980e+0
+00001890: 3120 332e 3736 3833 3136 3730 652b 3031  1 3.76831670e+01
+000018a0: 2051 2038 2e36 3839 3531 3136 3365 2b30   Q 8.68951163e+0
+000018b0: 3120 342e 3038 3134 3339 3232 652b 3031  1 4.08143922e+01
+000018c0: 2c20 382e 3936 3035 3131 3132 652b 3031  , 8.96051112e+01
+000018d0: 2034 2e33 3839 3237 3537 3465 2b30 3120   4.38927574e+01 
+000018e0: 5120 392e 3233 3138 3433 3237 652b 3031  Q 9.23184327e+01
+000018f0: 2034 2e36 3937 3438 3337 3365 2b30 312c   4.69748373e+01,
+00001900: 2039 2e35 3030 3030 3030 3065 2b30 3120   9.50000000e+01 
+00001910: 352e 3030 3030 3031 3830 652b 3031 205a  5.00000180e+01 Z
+00001920: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+00001930: 6820 643d 224d 2039 2e35 3030 3030 3030  h d="M 9.5000000
+00001940: 3065 2b30 3120 352e 3030 3030 3031 3830  0e+01 5.00000180
+00001950: 652b 3031 2051 2039 2e32 3331 3834 3332  e+01 Q 9.2318432
+00001960: 3765 2b30 3120 342e 3639 3734 3833 3733  7e+01 4.69748373
+00001970: 652b 3031 2c20 382e 3936 3035 3131 3132  e+01, 8.96051112
+00001980: 652b 3031 2034 2e33 3839 3237 3537 3465  e+01 4.38927574e
+00001990: 2b30 3120 5120 382e 3638 3935 3131 3633  +01 Q 8.68951163
+000019a0: 652b 3031 2034 2e30 3831 3433 3932 3265  e+01 4.08143922e
+000019b0: 2b30 312c 2038 2e34 3134 3730 3938 3065  +01, 8.41470980e
+000019c0: 2b30 3120 332e 3736 3833 3136 3730 652b  +01 3.76831670e+
+000019d0: 3031 204c 2038 2e32 3532 3931 3935 3065  01 L 8.25291950e
+000019e0: 2b30 3120 342e 3635 3939 3835 3430 652b  +01 4.65998540e+
+000019f0: 3031 204c 2039 2e35 3030 3030 3030 3065  01 L 9.50000000e
+00001a00: 2b30 3120 352e 3030 3030 3031 3830 652b  +01 5.00000180e+
+00001a10: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
+00001a20: 3c70 6174 6820 643d 224d 2038 2e31 3239  <path d="M 8.129
+00001a30: 3738 3639 3065 2b30 3120 352e 3731 3136  78690e+01 5.7116
+00001a40: 3634 3230 652b 3031 204c 2039 2e35 3030  6420e+01 L 9.500
+00001a50: 3030 3030 3065 2b30 3120 352e 3030 3030  00000e+01 5.0000
+00001a60: 3031 3830 652b 3031 204c 2038 2e32 3532  0180e+01 L 8.252
+00001a70: 3931 3935 3065 2b30 3120 342e 3635 3939  91950e+01 4.6599
+00001a80: 3835 3430 652b 3031 2051 2038 2e32 3232  8540e+01 Q 8.222
+00001a90: 3034 3234 3065 2b30 3120 342e 3932 3134  04240e+01 4.9214
+00001aa0: 3137 3038 652b 3031 2c20 382e 3139 3134  1708e+01, 8.1914
+00001ab0: 3633 3737 652b 3031 2035 2e31 3836 3438  6377e+01 5.18648
+00001ac0: 3537 3765 2b30 3120 5120 382e 3136 3038  577e+01 Q 8.1608
+00001ad0: 3838 3632 652b 3031 2035 2e34 3531 3532  8862e+01 5.45152
+00001ae0: 3039 3065 2b30 312c 2038 2e31 3239 3738  090e+01, 8.12978
+00001af0: 3639 3065 2b30 3120 352e 3731 3136 3634  690e+01 5.711664
+00001b00: 3230 652b 3031 205a 2220 2f3e 0d0a 2020  20e+01 Z" />..  
+00001b10: 2020 2020 3c70 6174 6820 643d 224d 2039      <path d="M 9
+00001b20: 2e35 3030 3030 3030 3065 2b30 3120 322e  .50000000e+01 2.
+00001b30: 3735 3030 3030 3930 652b 3031 204c 2039  75000090e+01 L 9
+00001b40: 2e35 3030 3030 3030 3065 2b30 3120 352e  .50000000e+01 5.
+00001b50: 3030 3030 3030 3030 652b 3030 204c 2038  00000000e+00 L 8
+00001b60: 2e32 3939 3438 3436 3065 2b30 3120 312e  .29948460e+01 1.
+00001b70: 3730 3037 3037 3130 652b 3031 204c 2039  70070710e+01 L 9
+00001b80: 2e35 3030 3030 3030 3065 2b30 3120 322e  .50000000e+01 2.
+00001b90: 3735 3030 3030 3930 652b 3031 205a 2220  75000090e+01 Z" 
+00001ba0: 2f3e 0d0a 2020 2020 2020 3c70 6174 6820  />..      <path 
+00001bb0: 643d 224d 2039 2e35 3030 3030 3030 3065  d="M 9.50000000e
+00001bc0: 2b30 3120 322e 3735 3030 3030 3930 652b  +01 2.75000090e+
+00001bd0: 3031 204c 2038 2e32 3939 3438 3436 3065  01 L 8.29948460e
+00001be0: 2b30 3120 312e 3730 3037 3037 3130 652b  +01 1.70070710e+
+00001bf0: 3031 204c 2038 2e30 3238 3034 3832 3065  01 L 8.02804820e
+00001c00: 2b30 3120 322e 3733 3837 3032 3330 652b  +01 2.73870230e+
+00001c10: 3031 2051 2038 2e34 3036 3836 3032 3065  01 Q 8.40686020e
+00001c20: 2b30 3120 322e 3734 3331 3134 3635 652b  +01 2.74311465e+
+00001c30: 3031 2c20 382e 3737 3035 3731 3437 652b  01, 8.77057147e+
+00001c40: 3031 2032 2e37 3435 3631 3033 3865 2b30  01 2.74561038e+0
+00001c50: 3120 5120 392e 3133 3436 3435 3735 652b  1 Q 9.13464575e+
+00001c60: 3031 2032 2e37 3438 3132 3639 3365 2b30  01 2.74812693e+0
+00001c70: 312c 2039 2e35 3030 3030 3030 3065 2b30  1, 9.50000000e+0
+00001c80: 3120 322e 3735 3030 3030 3930 652b 3031  1 2.75000090e+01
+00001c90: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00001ca0: 6174 6820 643d 224d 2038 2e34 3134 3730  ath d="M 8.41470
+00001cb0: 3938 3065 2b30 3120 332e 3736 3833 3136  980e+01 3.768316
+00001cc0: 3730 652b 3031 2051 2038 2e36 3838 3731  70e+01 Q 8.68871
+00001cd0: 3535 3065 2b30 3120 332e 3530 3934 3830  550e+01 3.509480
+00001ce0: 3332 652b 3031 2c20 382e 3936 3032 3630  32e+01, 8.960260
+00001cf0: 3033 652b 3031 2033 2e32 3534 3736 3939  03e+01 3.2547699
+00001d00: 3865 2b30 3120 5120 392e 3233 3034 3836  8e+01 Q 9.230486
+00001d10: 3231 652b 3031 2033 2e30 3031 3239 3337  21e+01 3.0012937
+00001d20: 3065 2b30 312c 2039 2e35 3030 3030 3030  0e+01, 9.5000000
+00001d30: 3065 2b30 3120 322e 3735 3030 3030 3930  0e+01 2.75000090
+00001d40: 652b 3031 2051 2039 2e31 3334 3634 3537  e+01 Q 9.1346457
+00001d50: 3565 2b30 3120 322e 3734 3831 3236 3933  5e+01 2.74812693
+00001d60: 652b 3031 2c20 382e 3737 3035 3731 3437  e+01, 8.77057147
+00001d70: 652b 3031 2032 2e37 3435 3631 3033 3865  e+01 2.74561038e
+00001d80: 2b30 3120 5120 382e 3430 3638 3630 3230  +01 Q 8.40686020
+00001d90: 652b 3031 2032 2e37 3433 3131 3436 3565  e+01 2.74311465e
+00001da0: 2b30 312c 2038 2e30 3238 3034 3832 3065  +01, 8.02804820e
+00001db0: 2b30 3120 322e 3733 3837 3032 3330 652b  +01 2.73870230e+
+00001dc0: 3031 2051 2038 2e31 3235 3730 3630 3165  01 Q 8.12570601e
+00001dd0: 2b30 3120 322e 3939 3639 3335 3935 652b  +01 2.99693595e+
+00001de0: 3031 2c20 382e 3232 3332 3337 3438 652b  01, 8.22323748e+
+00001df0: 3031 2033 2e32 3535 3734 3230 3765 2b30  01 3.25574207e+0
+00001e00: 3120 5120 382e 3332 3033 3136 3030 652b  1 Q 8.32031600e+
+00001e10: 3031 2033 2e35 3133 3336 3235 3465 2b30  01 3.51336254e+0
+00001e20: 312c 2038 2e34 3134 3730 3938 3065 2b30  1, 8.41470980e+0
+00001e30: 3120 332e 3736 3833 3136 3730 652b 3031  1 3.76831670e+01
+00001e40: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00001e50: 6174 6820 643d 224d 2032 2e38 3237 3230  ath d="M 2.82720
+00001e60: 3734 3065 2b30 3120 372e 3137 3237 3931  740e+01 7.172791
+00001e70: 3730 652b 3031 2051 2032 2e37 3030 3039  70e+01 Q 2.70009
+00001e80: 3735 3265 2b30 3120 372e 3034 3534 3937  752e+01 7.045497
+00001e90: 3235 652b 3031 2c20 322e 3630 3134 3436  25e+01, 2.601446
+00001ea0: 3536 652b 3031 2036 2e38 3937 3136 3434  56e+01 6.8971644
+00001eb0: 3965 2b30 3120 5120 322e 3530 3330 3339  9e+01 Q 2.503039
+00001ec0: 3531 652b 3031 2036 2e37 3438 3735 3833  51e+01 6.7487583
+00001ed0: 3965 2b30 312c 2032 2e34 3337 3031 3639  9e+01, 2.4370169
+00001ee0: 3065 2b30 3120 362e 3538 3838 3330 3330  0e+01 6.58883030
+00001ef0: 652b 3031 2051 2032 2e33 3032 3334 3634  e+01 Q 2.3023464
+00001f00: 3365 2b30 3120 362e 3736 3334 3038 3432  3e+01 6.76340842
+00001f10: 652b 3031 2c20 322e 3139 3036 3932 3638  e+01, 2.19069268
+00001f20: 652b 3031 2036 2e39 3331 3131 3636 3065  e+01 6.93111660e
+00001f30: 2b30 3120 5120 322e 3037 3930 3139 3136  +01 Q 2.07901916
+00001f40: 652b 3031 2037 2e30 3938 3632 3438 3165  e+01 7.09862481e
+00001f50: 2b30 312c 2031 2e39 3639 3538 3132 3065  +01, 1.96958120e
+00001f60: 2b30 3120 372e 3235 3936 3335 3430 652b  +01 7.25963540e+
+00001f70: 3031 2051 2032 2e31 3733 3233 3732 3965  01 Q 2.17323729e
+00001f80: 2b30 3120 372e 3234 3131 3132 3339 652b  +01 7.24111239e+
+00001f90: 3031 2c20 322e 3338 3331 3331 3434 652b  01, 2.38313144e+
+00001fa0: 3031 2037 2e32 3235 3035 3536 3265 2b30  01 7.22505562e+0
+00001fb0: 3120 5120 322e 3539 3237 3137 3438 652b  1 Q 2.59271748e+
+00001fc0: 3031 2037 2e32 3039 3333 3139 3165 2b30  01 7.20933191e+0
+00001fd0: 312c 2032 2e38 3237 3230 3734 3065 2b30  1, 2.82720740e+0
+00001fe0: 3120 372e 3137 3237 3931 3730 652b 3031  1 7.17279170e+01
+00001ff0: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00002000: 6174 6820 643d 224d 2032 2e34 3337 3031  ath d="M 2.43701
+00002010: 3639 3065 2b30 3120 362e 3538 3838 3330  690e+01 6.588830
+00002020: 3330 652b 3031 2051 2032 2e33 3635 3833  30e+01 Q 2.36583
+00002030: 3833 3565 2b30 3120 362e 3431 3536 3333  835e+01 6.415633
+00002040: 3131 652b 3031 2c20 322e 3333 3235 3530  11e+01, 2.332550
+00002050: 3537 652b 3031 2036 2e32 3430 3736 3636  57e+01 6.2407666
+00002060: 3065 2b30 3120 5120 322e 3239 3934 3832  0e+01 Q 2.299482
+00002070: 3933 652b 3031 2036 2e30 3636 3038 3334  93e+01 6.0660834
+00002080: 3765 2b30 312c 2032 2e33 3030 3030 3030  7e+01, 2.3000000
+00002090: 3065 2b30 3120 352e 3930 3030 3030 3030  0e+01 5.90000000
+000020a0: 652b 3031 2051 2032 2e31 3132 3035 3534  e+01 Q 2.1120554
+000020b0: 3565 2b30 3120 352e 3937 3539 3039 3036  5e+01 5.97590906
+000020c0: 652b 3031 2c20 312e 3932 3937 3132 3837  e+01, 1.92971287
+000020d0: 652b 3031 2036 2e30 3539 3537 3739 3165  e+01 6.05957791e
+000020e0: 2b30 3120 5120 312e 3734 3936 3534 3334  +01 Q 1.74965434
+000020f0: 652b 3031 2036 2e31 3432 3331 3531 3365  e+01 6.14231513e
+00002100: 2b30 312c 2031 2e35 3734 3138 3639 3065  +01, 1.57418690e
+00002110: 2b30 3120 362e 3232 3137 3431 3930 652b  +01 6.22174190e+
+00002120: 3031 2051 2031 2e37 3830 3931 3931 3465  01 Q 1.78091914e
+00002130: 2b30 3120 362e 3331 3139 3532 3231 652b  +01 6.31195221e+
+00002140: 3031 2c20 312e 3938 3733 3138 3538 652b  01, 1.98731858e+
+00002150: 3031 2036 2e34 3036 3635 3233 3565 2b30  01 6.40665235e+0
+00002160: 3120 5120 322e 3139 3139 3133 3936 652b  1 Q 2.19191396e+
+00002170: 3031 2036 2e35 3031 3030 3333 3465 2b30  01 6.50100334e+0
+00002180: 312c 2032 2e34 3337 3031 3639 3065 2b30  1, 2.43701690e+0
+00002190: 3120 362e 3538 3838 3330 3330 652b 3031  1 6.58883030e+01
+000021a0: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+000021b0: 6174 6820 643d 224d 2031 2e39 3639 3538  ath d="M 1.96958
+000021c0: 3132 3065 2b30 3120 372e 3235 3936 3335  120e+01 7.259635
+000021d0: 3430 652b 3031 2051 2032 2e30 3739 3031  40e+01 Q 2.07901
+000021e0: 3931 3665 2b30 3120 372e 3039 3836 3234  916e+01 7.098624
+000021f0: 3831 652b 3031 2c20 322e 3139 3036 3932  81e+01, 2.190692
+00002200: 3638 652b 3031 2036 2e39 3331 3131 3636  68e+01 6.9311166
+00002210: 3065 2b30 3120 5120 322e 3330 3233 3436  0e+01 Q 2.302346
+00002220: 3433 652b 3031 2036 2e37 3633 3430 3834  43e+01 6.7634084
+00002230: 3265 2b30 312c 2032 2e34 3337 3031 3639  2e+01, 2.4370169
+00002240: 3065 2b30 3120 362e 3538 3838 3330 3330  0e+01 6.58883030
+00002250: 652b 3031 2051 2032 2e31 3931 3931 3339  e+01 Q 2.1919139
+00002260: 3665 2b30 3120 362e 3530 3130 3033 3334  6e+01 6.50100334
+00002270: 652b 3031 2c20 312e 3938 3733 3138 3538  e+01, 1.98731858
+00002280: 652b 3031 2036 2e34 3036 3635 3233 3565  e+01 6.40665235e
+00002290: 2b30 3120 5120 312e 3738 3039 3139 3134  +01 Q 1.78091914
+000022a0: 652b 3031 2036 2e33 3131 3935 3232 3165  e+01 6.31195221e
+000022b0: 2b30 312c 2031 2e35 3734 3138 3639 3065  +01, 1.57418690e
+000022c0: 2b30 3120 362e 3232 3137 3431 3930 652b  +01 6.22174190e+
+000022d0: 3031 2051 2031 2e36 3639 3130 3538 3065  01 Q 1.66910580e
+000022e0: 2b30 3120 362e 3437 3734 3734 3937 652b  +01 6.47747497e+
+000022f0: 3031 2c20 312e 3736 3837 3730 3935 652b  01, 1.76877095e+
+00002300: 3031 2036 2e37 3337 3638 3531 3565 2b30  01 6.73768515e+0
+00002310: 3120 5120 312e 3836 3838 3832 3636 652b  1 Q 1.86888266e+
+00002320: 3031 2036 2e39 3939 3031 3733 3465 2b30  01 6.99901734e+0
+00002330: 312c 2031 2e39 3639 3538 3132 3065 2b30  1, 1.96958120e+0
+00002340: 3120 372e 3235 3936 3335 3430 652b 3031  1 7.25963540e+01
+00002350: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00002360: 6174 6820 643d 224d 2033 2e34 3131 3136  ath d="M 3.41116
+00002370: 3937 3065 2b30 3120 372e 3536 3239 3833  970e+01 7.562983
+00002380: 3130 652b 3031 2051 2033 2e32 3531 3234  10e+01 Q 3.25124
+00002390: 3136 3465 2b30 3120 372e 3439 3639 3630  164e+01 7.496960
+000023a0: 3532 652b 3031 2c20 332e 3130 3238 3335  52e+01, 3.102835
+000023b0: 3430 652b 3031 2037 2e33 3938 3535 3333  40e+01 7.3985533
+000023c0: 3265 2b30 3120 5120 322e 3935 3435 3032  2e+01 Q 2.954502
+000023d0: 3530 652b 3031 2037 2e32 3939 3930 3232  50e+01 7.2999022
+000023e0: 3365 2b30 312c 2032 2e38 3237 3230 3734  3e+01, 2.8272074
+000023f0: 3065 2b30 3120 372e 3137 3237 3931 3730  0e+01 7.17279170
+00002400: 652b 3031 2051 2032 2e37 3930 3235 3634  e+01 Q 2.7902564
+00002410: 3565 2b30 3120 372e 3430 3634 3736 3431  5e+01 7.40647641
+00002420: 652b 3031 2c20 322e 3737 3339 3536 3335  e+01, 2.77395635
+00002430: 652b 3031 2037 2e36 3135 3239 3638 3765  e+01 7.61529687e
+00002440: 2b30 3120 5120 322e 3735 3733 3234 3838  +01 Q 2.75732488
+00002450: 652b 3031 2037 2e38 3234 3436 3031 3765  e+01 7.82446017e
+00002460: 2b30 312c 2032 2e37 3338 3232 3434 3065  +01, 2.73822440e
+00002470: 2b30 3120 382e 3032 3735 3733 3930 652b  +01 8.02757390e+
+00002480: 3031 2051 2032 2e38 3939 3730 3836 3965  01 Q 2.89970869e
+00002490: 2b30 3120 372e 3931 3839 3731 3630 652b  +01 7.91897160e+
+000024a0: 3031 2c20 332e 3036 3739 3231 3631 652b  01, 3.06792161e+
+000024b0: 3031 2037 2e38 3038 3037 3833 3465 2b30  01 7.80807834e+0
+000024c0: 3120 5120 332e 3233 3634 3435 3533 652b  1 Q 3.23644553e+
+000024d0: 3031 2037 2e36 3937 3132 3632 3365 2b30  01 7.69712623e+0
+000024e0: 312c 2033 2e34 3131 3136 3937 3065 2b30  1, 3.41116970e+0
+000024f0: 3120 372e 3536 3239 3833 3130 652b 3031  1 7.56298310e+01
+00002500: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00002510: 6174 6820 643d 224d 2032 2e38 3237 3230  ath d="M 2.82720
+00002520: 3734 3065 2b30 3120 372e 3137 3237 3931  740e+01 7.172791
+00002530: 3730 652b 3031 2051 2032 2e35 3932 3731  70e+01 Q 2.59271
+00002540: 3734 3865 2b30 3120 372e 3230 3933 3331  748e+01 7.209331
+00002550: 3931 652b 3031 2c20 322e 3338 3331 3331  91e+01, 2.383131
+00002560: 3434 652b 3031 2037 2e32 3235 3035 3536  44e+01 7.2250556
+00002570: 3265 2b30 3120 5120 322e 3137 3332 3337  2e+01 Q 2.173237
+00002580: 3239 652b 3031 2037 2e32 3431 3131 3233  29e+01 7.2411123
+00002590: 3965 2b30 312c 2031 2e39 3639 3538 3132  9e+01, 1.9695812
+000025a0: 3065 2b30 3120 372e 3235 3936 3335 3430  0e+01 7.25963540
+000025b0: 652b 3031 204c 2032 2e37 3338 3232 3434  e+01 L 2.7382244
+000025c0: 3065 2b30 3120 382e 3032 3735 3733 3930  0e+01 8.02757390
+000025d0: 652b 3031 2051 2032 2e37 3537 3332 3438  e+01 Q 2.7573248
+000025e0: 3865 2b30 3120 372e 3832 3434 3630 3137  8e+01 7.82446017
+000025f0: 652b 3031 2c20 322e 3737 3339 3536 3335  e+01, 2.77395635
+00002600: 652b 3031 2037 2e36 3135 3239 3638 3765  e+01 7.61529687e
+00002610: 2b30 3120 5120 322e 3739 3032 3536 3435  +01 Q 2.79025645
+00002620: 652b 3031 2037 2e34 3036 3437 3634 3165  e+01 7.40647641e
+00002630: 2b30 312c 2032 2e38 3237 3230 3734 3065  +01, 2.82720740e
+00002640: 2b30 3120 372e 3137 3237 3931 3730 652b  +01 7.17279170e+
+00002650: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
+00002660: 3c70 6174 6820 643d 224d 2034 2e31 3030  <path d="M 4.100
+00002670: 3030 3030 3065 2b30 3120 372e 3730 3030  00000e+01 7.7000
+00002680: 3030 3030 652b 3031 2051 2033 2e39 3333  0000e+01 Q 3.933
+00002690: 3931 3635 3365 2b30 3120 372e 3730 3035  91653e+01 7.7005
+000026a0: 3137 3037 652b 3031 2c20 332e 3735 3932  1707e+01, 3.7592
+000026b0: 3333 3430 652b 3031 2037 2e36 3637 3434  3340e+01 7.66744
+000026c0: 3934 3365 2b30 3120 5120 332e 3538 3433  943e+01 Q 3.5843
+000026d0: 3636 3839 652b 3031 2037 2e36 3334 3136  6689e+01 7.63416
+000026e0: 3136 3565 2b30 312c 2033 2e34 3131 3136  165e+01, 3.41116
+000026f0: 3937 3065 2b30 3120 372e 3536 3239 3833  970e+01 7.562983
+00002700: 3130 652b 3031 2051 2033 2e34 3936 3539  10e+01 Q 3.49659
+00002710: 3634 3665 2b30 3120 372e 3830 3335 3331  646e+01 7.803531
+00002720: 3433 652b 3031 2c20 332e 3538 3830 3639  43e+01, 3.588069
+00002730: 3830 652b 3031 2038 2e30 3035 3638 3730  80e+01 8.0056870
+00002740: 3965 2b30 3120 5120 332e 3638 3031 3239  9e+01 Q 3.680129
+00002750: 3335 652b 3031 2038 2e32 3130 3035 3138  35e+01 8.2100518
+00002760: 3965 2b30 312c 2033 2e37 3638 3138 3236  9e+01, 3.7681826
+00002770: 3065 2b30 3120 382e 3431 3436 3030 3030  0e+01 8.41460000
+00002780: 652b 3031 2051 2033 2e38 3439 3238 3338  e+01 Q 3.8492838
+00002790: 3765 2b30 3120 382e 3234 3436 3231 3334  7e+01 8.24462134
+000027a0: 652b 3031 2c20 332e 3933 3533 3036 3735  e+01, 3.93530675
+000027b0: 652b 3031 2038 2e30 3637 3438 3539 3365  e+01 8.06748593e
+000027c0: 2b30 3120 5120 342e 3032 3238 3936 3930  +01 Q 4.02289690
+000027d0: 652b 3031 2037 2e38 3836 3633 3531 3165  e+01 7.88663511e
+000027e0: 2b30 312c 2034 2e31 3030 3030 3030 3065  +01, 4.10000000e
+000027f0: 2b30 3120 372e 3730 3030 3030 3030 652b  +01 7.70000000e+
+00002800: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
+00002810: 3c70 6174 6820 643d 224d 2033 2e34 3131  <path d="M 3.411
+00002820: 3136 3937 3065 2b30 3120 372e 3536 3239  16970e+01 7.5629
+00002830: 3833 3130 652b 3031 2051 2033 2e32 3336  8310e+01 Q 3.236
+00002840: 3434 3535 3365 2b30 3120 372e 3639 3731  44553e+01 7.6971
+00002850: 3236 3233 652b 3031 2c20 332e 3036 3739  2623e+01, 3.0679
+00002860: 3231 3631 652b 3031 2037 2e38 3038 3037  2161e+01 7.80807
+00002870: 3833 3465 2b30 3120 5120 322e 3839 3937  834e+01 Q 2.8997
+00002880: 3038 3639 652b 3031 2037 2e39 3138 3937  0869e+01 7.91897
+00002890: 3136 3065 2b30 312c 2032 2e37 3338 3232  160e+01, 2.73822
+000028a0: 3434 3065 2b30 3120 382e 3032 3735 3733  440e+01 8.027573
+000028b0: 3930 652b 3031 2051 2032 2e39 3936 3535  90e+01 Q 2.99655
+000028c0: 3438 3365 2b30 3120 382e 3132 3533 3239  483e+01 8.125329
+000028d0: 3132 652b 3031 2c20 332e 3235 3534 3235  12e+01, 3.255425
+000028e0: 3636 652b 3031 2038 2e32 3232 3934 3330  66e+01 8.2229430
+000028f0: 3965 2b30 3120 5120 332e 3531 3331 3335  9e+01 Q 3.513135
+00002900: 3539 652b 3031 2038 2e33 3230 3131 3331  59e+01 8.3201131
+00002910: 3865 2b30 312c 2033 2e37 3638 3138 3236  8e+01, 3.7681826
+00002920: 3065 2b30 3120 382e 3431 3436 3030 3030  0e+01 8.41460000
+00002930: 652b 3031 2051 2033 2e36 3830 3132 3933  e+01 Q 3.6801293
+00002940: 3565 2b30 3120 382e 3231 3030 3531 3839  5e+01 8.21005189
+00002950: 652b 3031 2c20 332e 3538 3830 3639 3830  e+01, 3.58806980
+00002960: 652b 3031 2038 2e30 3035 3638 3730 3965  e+01 8.00568709e
+00002970: 2b30 3120 5120 332e 3439 3635 3936 3436  +01 Q 3.49659646
+00002980: 652b 3031 2037 2e38 3033 3533 3134 3365  e+01 7.80353143e
+00002990: 2b30 312c 2033 2e34 3131 3136 3937 3065  +01, 3.41116970e
+000029a0: 2b30 3120 372e 3536 3239 3833 3130 652b  +01 7.56298310e+
+000029b0: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
+000029c0: 3c70 6174 6820 643d 224d 2032 2e37 3530  <path d="M 2.750
+000029d0: 3030 3030 3065 2b30 3120 392e 3530 3030  00000e+01 9.5000
+000029e0: 3030 3030 652b 3031 204c 2034 2e39 3939  0000e+01 L 4.999
+000029f0: 3939 3832 3065 2b30 3120 392e 3530 3030  99820e+01 9.5000
+00002a00: 3030 3030 652b 3031 2051 2034 2e36 3937  0000e+01 Q 4.697
+00002a10: 3434 3532 3465 2b30 3120 392e 3233 3138  44524e+01 9.2318
+00002a20: 3134 3138 652b 3031 2c20 342e 3338 3932  1418e+01, 4.3892
+00002a30: 3037 3331 652b 3031 2038 2e39 3630 3435  0731e+01 8.96045
+00002a40: 3731 3765 2b30 3120 5120 342e 3038 3133  717e+01 Q 4.0813
+00002a50: 3435 3731 652b 3031 2038 2e36 3839 3433  4571e+01 8.68943
+00002a60: 3730 3865 2b30 312c 2033 2e37 3638 3138  708e+01, 3.76818
+00002a70: 3236 3065 2b30 3120 382e 3431 3436 3030  260e+01 8.414600
+00002a80: 3030 652b 3031 2051 2033 2e35 3039 3337  00e+01 Q 3.50937
+00002a90: 3337 3665 2b30 3120 382e 3638 3836 3338  376e+01 8.688638
+00002aa0: 3632 652b 3031 2c20 332e 3235 3437 3031  62e+01, 3.254701
+00002ab0: 3335 652b 3031 2038 2e39 3630 3230 3634  35e+01 8.9602064
+00002ac0: 3765 2b30 3120 5120 332e 3030 3132 3630  7e+01 Q 3.001260
+00002ad0: 3531 652b 3031 2039 2e32 3330 3435 3832  51e+01 9.2304582
+00002ae0: 3765 2b30 312c 2032 2e37 3530 3030 3030  7e+01, 2.7500000
+00002af0: 3065 2b30 3120 392e 3530 3030 3030 3030  0e+01 9.50000000
+00002b00: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
+00002b10: 2020 3c70 6174 6820 643d 224d 2035 2e30    <path d="M 5.0
+00002b20: 3030 3030 3030 3065 2b30 3020 392e 3530  0000000e+00 9.50
+00002b30: 3030 3030 3030 652b 3031 204c 2032 2e37  000000e+01 L 2.7
+00002b40: 3530 3030 3030 3065 2b30 3120 392e 3530  5000000e+01 9.50
+00002b50: 3030 3030 3030 652b 3031 204c 2031 2e37  000000e+01 L 1.7
+00002b60: 3030 3036 3633 3065 2b30 3120 382e 3239  0006630e+01 8.29
+00002b70: 3838 3433 3830 652b 3031 204c 2035 2e30  884380e+01 L 5.0
+00002b80: 3030 3030 3030 3065 2b30 3020 392e 3530  0000000e+00 9.50
+00002b90: 3030 3030 3030 652b 3031 205a 2220 2f3e  000000e+01 Z" />
+00002ba0: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
+00002bb0: 224d 2031 2e37 3030 3036 3633 3065 2b30  "M 1.70006630e+0
+00002bc0: 3120 382e 3239 3838 3433 3830 652b 3031  1 8.29884380e+01
+00002bd0: 204c 2032 2e37 3530 3030 3030 3065 2b30   L 2.75000000e+0
+00002be0: 3120 392e 3530 3030 3030 3030 652b 3031  1 9.50000000e+01
+00002bf0: 2051 2032 2e37 3438 3030 3834 3165 2b30   Q 2.74800841e+0
+00002c00: 3120 392e 3133 3435 3237 3339 652b 3031  1 9.13452739e+01
+00002c10: 2c20 322e 3734 3533 3734 3035 652b 3031  , 2.74537405e+01
+00002c20: 2038 2e37 3730 3333 3932 3065 2b30 3120   8.77033920e+01 
+00002c30: 5120 322e 3734 3237 3630 3731 652b 3031  Q 2.74276071e+01
+00002c40: 2038 2e34 3036 3532 3033 3965 2b30 312c   8.40652039e+01,
+00002c50: 2032 2e37 3338 3232 3434 3065 2b30 3120   2.73822440e+01 
+00002c60: 382e 3032 3735 3733 3930 652b 3031 204c  8.02757390e+01 L
+00002c70: 2031 2e37 3030 3036 3633 3065 2b30 3120   1.70006630e+01 
+00002c80: 382e 3239 3838 3433 3830 652b 3031 205a  8.29884380e+01 Z
+00002c90: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+00002ca0: 6820 643d 224d 2032 2e37 3530 3030 3030  h d="M 2.7500000
+00002cb0: 3065 2b30 3120 392e 3530 3030 3030 3030  0e+01 9.50000000
+00002cc0: 652b 3031 2051 2033 2e30 3031 3236 3035  e+01 Q 3.0012605
+00002cd0: 3165 2b30 3120 392e 3233 3034 3538 3237  1e+01 9.23045827
+00002ce0: 652b 3031 2c20 332e 3235 3437 3031 3335  e+01, 3.25470135
+00002cf0: 652b 3031 2038 2e39 3630 3230 3634 3765  e+01 8.96020647e
+00002d00: 2b30 3120 5120 332e 3530 3933 3733 3736  +01 Q 3.50937376
+00002d10: 652b 3031 2038 2e36 3838 3633 3836 3265  e+01 8.68863862e
+00002d20: 2b30 312c 2033 2e37 3638 3138 3236 3065  +01, 3.76818260e
+00002d30: 2b30 3120 382e 3431 3436 3030 3030 652b  +01 8.41460000e+
+00002d40: 3031 2051 2033 2e35 3133 3133 3535 3965  01 Q 3.51313559e
+00002d50: 2b30 3120 382e 3332 3031 3133 3138 652b  +01 8.32011318e+
+00002d60: 3031 2c20 332e 3235 3534 3235 3636 652b  01, 3.25542566e+
+00002d70: 3031 2038 2e32 3232 3934 3330 3965 2b30  01 8.22294309e+0
+00002d80: 3120 5120 322e 3939 3635 3534 3833 652b  1 Q 2.99655483e+
+00002d90: 3031 2038 2e31 3235 3332 3931 3265 2b30  01 8.12532912e+0
+00002da0: 312c 2032 2e37 3338 3232 3434 3065 2b30  1, 2.73822440e+0
+00002db0: 3120 382e 3032 3735 3733 3930 652b 3031  1 8.02757390e+01
+00002dc0: 2051 2032 2e37 3432 3736 3037 3165 2b30   Q 2.74276071e+0
+00002dd0: 3120 382e 3430 3635 3230 3339 652b 3031  1 8.40652039e+01
+00002de0: 2c20 322e 3734 3533 3734 3035 652b 3031  , 2.74537405e+01
+00002df0: 2038 2e37 3730 3333 3932 3065 2b30 3120   8.77033920e+01 
+00002e00: 5120 322e 3734 3830 3038 3431 652b 3031  Q 2.74800841e+01
+00002e10: 2039 2e31 3334 3532 3733 3965 2b30 312c   9.13452739e+01,
+00002e20: 2032 2e37 3530 3030 3030 3065 2b30 3120   2.75000000e+01 
+00002e30: 392e 3530 3030 3030 3030 652b 3031 205a  9.50000000e+01 Z
+00002e40: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+00002e50: 6820 643d 224d 2034 2e39 3939 3939 3832  h d="M 4.9999982
+00002e60: 3065 2b30 3120 392e 3530 3030 3030 3030  0e+01 9.50000000
+00002e70: 652b 3031 204c 2037 2e32 3439 3939 3931  e+01 L 7.2499991
+00002e80: 3065 2b30 3120 392e 3530 3030 3030 3030  0e+01 9.50000000
+00002e90: 652b 3031 2051 2036 2e38 3635 3235 3832  e+01 Q 6.8652582
+00002ea0: 3865 2b30 3120 392e 3135 3635 3338 3530  8e+01 9.15653850
+00002eb0: 652b 3031 2c20 362e 3438 3631 3436 3334  e+01, 6.48614634
+00002ec0: 652b 3031 2038 2e38 3139 3337 3030 3365  e+01 8.81937003e
+00002ed0: 2b30 3120 5120 362e 3130 3736 3938 3134  +01 Q 6.10769814
+00002ee0: 652b 3031 2038 2e34 3832 3738 3135 3665  e+01 8.48278156e
+00002ef0: 2b30 312c 2035 2e37 3130 3734 3938 3065  +01, 5.71074980e
+00002f00: 2b30 3120 382e 3133 3036 3838 3730 652b  +01 8.13068870e+
+00002f10: 3031 204c 2034 2e39 3939 3939 3832 3065  01 L 4.99999820e
+00002f20: 2b30 3120 392e 3530 3030 3030 3030 652b  +01 9.50000000e+
+00002f30: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
+00002f40: 3c70 6174 6820 643d 224d 2034 2e39 3939  <path d="M 4.999
+00002f50: 3939 3832 3065 2b30 3120 392e 3530 3030  99820e+01 9.5000
+00002f60: 3030 3030 652b 3031 204c 2035 2e37 3130  0000e+01 L 5.710
+00002f70: 3734 3938 3065 2b30 3120 382e 3133 3036  74980e+01 8.1306
+00002f80: 3838 3730 652b 3031 2051 2035 2e34 3530  8870e+01 Q 5.450
+00002f90: 3739 3834 3665 2b30 3120 382e 3136 3135  79846e+01 8.1615
+00002fa0: 3936 3535 652b 3031 2c20 352e 3138 3539  9655e+01, 5.1859
+00002fb0: 3232 3435 652b 3031 2038 2e31 3931 3937  2245e+01 8.19197
+00002fc0: 3930 3965 2b30 3120 5120 342e 3932 3130  909e+01 Q 4.9210
+00002fd0: 3636 3936 652b 3031 2038 2e32 3232 3335  6696e+01 8.22235
+00002fe0: 3838 3365 2b30 312c 2034 2e36 3539 3831  883e+01, 4.65981
+00002ff0: 3236 3065 2b30 3120 382e 3235 3330 3434  260e+01 8.253044
+00003000: 3630 652b 3031 204c 2034 2e39 3939 3939  60e+01 L 4.99999
+00003010: 3832 3065 2b30 3120 392e 3530 3030 3030  820e+01 9.500000
+00003020: 3030 652b 3031 205a 2220 2f3e 0d0a 2020  00e+01 Z" />..  
+00003030: 2020 2020 3c70 6174 6820 643d 224d 2033      <path d="M 3
+00003040: 2e37 3638 3138 3236 3065 2b30 3120 382e  .76818260e+01 8.
+00003050: 3431 3436 3030 3030 652b 3031 2051 2034  41460000e+01 Q 4
+00003060: 2e30 3831 3334 3537 3165 2b30 3120 382e  .08134571e+01 8.
+00003070: 3638 3934 3337 3038 652b 3031 2c20 342e  68943708e+01, 4.
+00003080: 3338 3932 3037 3331 652b 3031 2038 2e39  38920731e+01 8.9
+00003090: 3630 3435 3731 3765 2b30 3120 5120 342e  6045717e+01 Q 4.
+000030a0: 3639 3734 3435 3234 652b 3031 2039 2e32  69744524e+01 9.2
+000030b0: 3331 3831 3431 3865 2b30 312c 2034 2e39  3181418e+01, 4.9
+000030c0: 3939 3939 3832 3065 2b30 3120 392e 3530  9999820e+01 9.50
+000030d0: 3030 3030 3030 652b 3031 204c 2034 2e36  000000e+01 L 4.6
+000030e0: 3539 3831 3236 3065 2b30 3120 382e 3235  5981260e+01 8.25
+000030f0: 3330 3434 3630 652b 3031 204c 2033 2e37  304460e+01 L 3.7
+00003100: 3638 3138 3236 3065 2b30 3120 382e 3431  6818260e+01 8.41
+00003110: 3436 3030 3030 652b 3031 205a 2220 2f3e  460000e+01 Z" />
+00003120: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
+00003130: 224d 2037 2e32 3439 3939 3931 3065 2b30  "M 7.24999910e+0
+00003140: 3120 392e 3530 3030 3030 3030 652b 3031  1 9.50000000e+01
+00003150: 204c 2039 2e35 3030 3030 3030 3065 2b30   L 9.50000000e+0
+00003160: 3120 392e 3530 3030 3030 3030 652b 3031  1 9.50000000e+01
+00003170: 204c 2038 2e31 3933 3033 3335 3065 2b30   L 8.19303350e+0
+00003180: 3120 382e 3139 3437 3538 3830 652b 3031  1 8.19475880e+01
+00003190: 204c 2037 2e32 3439 3939 3931 3065 2b30   L 7.24999910e+0
+000031a0: 3120 392e 3530 3030 3030 3030 652b 3031  1 9.50000000e+01
+000031b0: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+000031c0: 6174 6820 643d 224d 2035 2e37 3130 3734  ath d="M 5.71074
+000031d0: 3938 3065 2b30 3120 382e 3133 3036 3838  980e+01 8.130688
+000031e0: 3730 652b 3031 2051 2036 2e31 3037 3639  70e+01 Q 6.10769
+000031f0: 3831 3465 2b30 3120 382e 3438 3237 3831  814e+01 8.482781
+00003200: 3536 652b 3031 2c20 362e 3438 3631 3436  56e+01, 6.486146
+00003210: 3334 652b 3031 2038 2e38 3139 3337 3030  34e+01 8.8193700
+00003220: 3365 2b30 3120 5120 362e 3836 3532 3538  3e+01 Q 6.865258
+00003230: 3238 652b 3031 2039 2e31 3536 3533 3835  28e+01 9.1565385
+00003240: 3065 2b30 312c 2037 2e32 3439 3939 3931  0e+01, 7.2499991
+00003250: 3065 2b30 3120 392e 3530 3030 3030 3030  0e+01 9.50000000
+00003260: 652b 3031 204c 2036 2e39 3230 3838 3731  e+01 L 6.9208871
+00003270: 3065 2b30 3120 372e 3735 3632 3338 3330  0e+01 7.75623830
+00003280: 652b 3031 2051 2036 2e36 3238 3834 3833  e+01 Q 6.6288483
+00003290: 3665 2b30 3120 372e 3834 3934 3833 3535  6e+01 7.84948355
+000032a0: 652b 3031 2c20 362e 3332 3234 3230 3833  e+01, 6.32242083
+000032b0: 652b 3031 2037 2e39 3433 3731 3933 3165  e+01 7.94371931e
+000032c0: 2b30 3120 5120 362e 3031 3638 3532 3736  +01 Q 6.01685276
+000032d0: 652b 3031 2038 2e30 3337 3635 3435 3165  e+01 8.03765451e
+000032e0: 2b30 312c 2035 2e37 3130 3734 3938 3065  +01, 5.71074980e
+000032f0: 2b30 3120 382e 3133 3036 3838 3730 652b  +01 8.13068870e+
+00003300: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
+00003310: 3c70 6174 6820 643d 224d 2037 2e32 3439  <path d="M 7.249
+00003320: 3939 3931 3065 2b30 3120 392e 3530 3030  99910e+01 9.5000
+00003330: 3030 3030 652b 3031 204c 2038 2e31 3933  0000e+01 L 8.193
+00003340: 3033 3335 3065 2b30 3120 382e 3139 3437  03350e+01 8.1947
+00003350: 3538 3830 652b 3031 204c 2036 2e39 3230  5880e+01 L 6.920
+00003360: 3838 3731 3065 2b30 3120 372e 3735 3632  88710e+01 7.7562
+00003370: 3338 3330 652b 3031 204c 2037 2e32 3439  3830e+01 L 7.249
+00003380: 3939 3931 3065 2b30 3120 392e 3530 3030  99910e+01 9.5000
+00003390: 3030 3030 652b 3031 205a 2220 2f3e 0d0a  0000e+01 Z" />..
+000033a0: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
+000033b0: 2032 2e33 3030 3030 3030 3065 2b30 3120   2.30000000e+01 
+000033c0: 342e 3039 3939 3939 3130 652b 3031 204c  4.09999910e+01 L
+000033d0: 2032 2e33 3030 3030 3030 3065 2b30 3120   2.30000000e+01 
+000033e0: 332e 3230 3030 3030 3030 652b 3031 204c  3.20000000e+01 L
+000033f0: 2031 2e34 3636 3531 3831 3065 2b30 3120   1.46651810e+01 
+00003400: 332e 3931 3130 3930 3030 652b 3031 204c  3.91109000e+01 L
+00003410: 2032 2e33 3030 3030 3030 3065 2b30 3120   2.30000000e+01 
+00003420: 342e 3039 3939 3939 3130 652b 3031 205a  4.09999910e+01 Z
+00003430: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+00003440: 6820 643d 224d 2032 2e33 3030 3030 3030  h d="M 2.3000000
+00003450: 3065 2b30 3120 332e 3230 3030 3030 3030  0e+01 3.20000000
+00003460: 652b 3031 204c 2032 2e33 3030 3030 3030  e+01 L 2.3000000
+00003470: 3065 2b30 3120 322e 3330 3030 3030 3030  0e+01 2.30000000
+00003480: 652b 3031 204c 2035 2e30 3030 3030 3030  e+01 L 5.0000000
+00003490: 3065 2b30 3020 322e 3735 3030 3030 3030  0e+00 2.75000000
+000034a0: 652b 3031 204c 2032 2e33 3030 3030 3030  e+01 L 2.3000000
+000034b0: 3065 2b30 3120 332e 3230 3030 3030 3030  0e+01 3.20000000
+000034c0: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
+000034d0: 2020 3c70 6174 6820 643d 224d 2031 2e34    <path d="M 1.4
+000034e0: 3636 3531 3831 3065 2b30 3120 332e 3931  6651810e+01 3.91
+000034f0: 3130 3930 3030 652b 3031 204c 2032 2e33  109000e+01 L 2.3
+00003500: 3030 3030 3030 3065 2b30 3120 332e 3230  0000000e+01 3.20
+00003510: 3030 3030 3030 652b 3031 204c 2035 2e30  000000e+01 L 5.0
+00003520: 3030 3030 3030 3065 2b30 3020 322e 3735  0000000e+00 2.75
+00003530: 3030 3030 3030 652b 3031 204c 2031 2e34  000000e+01 L 1.4
+00003540: 3636 3531 3831 3065 2b30 3120 332e 3931  6651810e+01 3.91
+00003550: 3130 3930 3030 652b 3031 205a 2220 2f3e  109000e+01 Z" />
+00003560: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
+00003570: 224d 2032 2e33 3030 3030 3030 3065 2b30  "M 2.30000000e+0
+00003580: 3120 352e 3030 3030 3030 3030 652b 3031  1 5.00000000e+01
+00003590: 204c 2032 2e33 3030 3030 3030 3065 2b30   L 2.30000000e+0
+000035a0: 3120 342e 3039 3939 3939 3130 652b 3031  1 4.09999910e+01
+000035b0: 204c 2031 2e36 3631 3733 3731 3065 2b30   L 1.66173710e+0
+000035c0: 3120 342e 3634 3833 3831 3730 652b 3031  1 4.64838170e+01
+000035d0: 204c 2032 2e33 3030 3030 3030 3065 2b30   L 2.30000000e+0
+000035e0: 3120 352e 3030 3030 3030 3030 652b 3031  1 5.00000000e+01
+000035f0: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00003600: 6174 6820 643d 224d 2032 2e33 3030 3030  ath d="M 2.30000
+00003610: 3030 3065 2b30 3120 342e 3039 3939 3939  000e+01 4.099999
+00003620: 3130 652b 3031 204c 2031 2e34 3636 3531  10e+01 L 1.46651
+00003630: 3831 3065 2b30 3120 332e 3931 3130 3930  810e+01 3.911090
+00003640: 3030 652b 3031 204c 2031 2e36 3631 3733  00e+01 L 1.66173
+00003650: 3731 3065 2b30 3120 342e 3634 3833 3831  710e+01 4.648381
+00003660: 3730 652b 3031 204c 2032 2e33 3030 3030  70e+01 L 2.30000
+00003670: 3030 3065 2b30 3120 342e 3039 3939 3939  000e+01 4.099999
+00003680: 3130 652b 3031 205a 2220 2f3e 0d0a 2020  10e+01 Z" />..  
+00003690: 2020 2020 3c70 6174 6820 643d 224d 2032      <path d="M 2
+000036a0: 2e33 3030 3030 3030 3065 2b30 3120 352e  .30000000e+01 5.
+000036b0: 3930 3030 3030 3030 652b 3031 204c 2032  90000000e+01 L 2
+000036c0: 2e33 3030 3030 3030 3065 2b30 3120 352e  .30000000e+01 5.
+000036d0: 3030 3030 3030 3030 652b 3031 204c 2031  00000000e+01 L 1
+000036e0: 2e37 3035 3537 3631 3065 2b30 3120 352e  .70557610e+01 5.
+000036f0: 3332 3134 3232 3430 652b 3031 2051 2031  32142240e+01 Q 1
+00003700: 2e38 3532 3635 3130 3065 2b30 3120 352e  .85265100e+01 5.
+00003710: 3436 3531 3538 3535 652b 3031 2c20 322e  46515855e+01, 2.
+00003720: 3030 3130 3330 3435 652b 3031 2035 2e36  00103045e+01 5.6
+00003730: 3130 3631 3934 3465 2b30 3120 5120 322e  1061944e+01 Q 2.
+00003740: 3135 3032 3135 3630 652b 3031 2035 2e37  15021560e+01 5.7
+00003750: 3536 3835 3639 3665 2b30 312c 2032 2e33  5685696e+01, 2.3
+00003760: 3030 3030 3030 3065 2b30 3120 352e 3930  0000000e+01 5.90
+00003770: 3030 3030 3030 652b 3031 205a 2220 2f3e  000000e+01 Z" />
+00003780: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
+00003790: 224d 2032 2e33 3030 3030 3030 3065 2b30  "M 2.30000000e+0
+000037a0: 3120 352e 3030 3030 3030 3030 652b 3031  1 5.00000000e+01
+000037b0: 204c 2031 2e36 3631 3733 3731 3065 2b30   L 1.66173710e+0
+000037c0: 3120 342e 3634 3833 3831 3730 652b 3031  1 4.64838170e+01
+000037d0: 204c 2031 2e37 3035 3537 3631 3065 2b30   L 1.70557610e+0
+000037e0: 3120 352e 3332 3134 3232 3430 652b 3031  1 5.32142240e+01
+000037f0: 204c 2032 2e33 3030 3030 3030 3065 2b30   L 2.30000000e+0
+00003800: 3120 352e 3030 3030 3030 3030 652b 3031  1 5.00000000e+01
+00003810: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00003820: 6174 6820 643d 224d 2035 2e30 3030 3030  ath d="M 5.00000
+00003830: 3030 3065 2b30 3020 322e 3735 3030 3030  000e+00 2.750000
+00003840: 3030 652b 3031 204c 2035 2e30 3030 3030  00e+01 L 5.00000
+00003850: 3030 3065 2b30 3020 342e 3939 3939 3938  000e+00 4.999998
+00003860: 3230 652b 3031 204c 2031 2e34 3636 3531  20e+01 L 1.46651
+00003870: 3831 3065 2b30 3120 332e 3931 3130 3930  810e+01 3.911090
+00003880: 3030 652b 3031 204c 2035 2e30 3030 3030  00e+01 L 5.00000
+00003890: 3030 3065 2b30 3020 322e 3735 3030 3030  000e+00 2.750000
+000038a0: 3030 652b 3031 205a 2220 2f3e 0d0a 2020  00e+01 Z" />..  
+000038b0: 2020 2020 3c70 6174 6820 643d 224d 2035      <path d="M 5
+000038c0: 2e30 3030 3030 3030 3065 2b30 3020 352e  .00000000e+00 5.
+000038d0: 3030 3030 3030 3030 652b 3030 204c 2035  00000000e+00 L 5
+000038e0: 2e30 3030 3030 3030 3065 2b30 3020 322e  .00000000e+00 2.
+000038f0: 3735 3030 3030 3030 652b 3031 204c 2032  75000000e+01 L 2
+00003900: 2e33 3030 3030 3030 3065 2b30 3120 322e  .30000000e+01 2.
+00003910: 3330 3030 3030 3030 652b 3031 204c 2035  30000000e+01 L 5
+00003920: 2e30 3030 3030 3030 3065 2b30 3020 352e  .00000000e+00 5.
+00003930: 3030 3030 3030 3030 652b 3030 205a 2220  00000000e+00 Z" 
+00003940: 2f3e 0d0a 2020 2020 2020 3c70 6174 6820  />..      <path 
+00003950: 643d 224d 2035 2e30 3030 3030 3030 3065  d="M 5.00000000e
+00003960: 2b30 3020 372e 3234 3939 3939 3130 652b  +00 7.24999910e+
+00003970: 3031 204c 2031 2e35 3734 3138 3639 3065  01 L 1.57418690e
+00003980: 2b30 3120 362e 3232 3137 3431 3930 652b  +01 6.22174190e+
+00003990: 3031 2051 2031 2e33 3033 3633 3331 3065  01 Q 1.30363310e
+000039a0: 2b30 3120 352e 3930 3939 3938 3737 652b  +01 5.90999877e+
+000039b0: 3031 2c20 312e 3033 3731 3430 3832 652b  01, 1.03714082e+
+000039c0: 3031 2035 2e36 3037 3634 3133 3365 2b30  01 5.60764133e+0
+000039d0: 3120 5120 372e 3730 3033 3839 3734 652b  1 Q 7.70038974e+
+000039e0: 3030 2035 2e33 3034 3536 3335 3065 2b30  00 5.30456350e+0
+000039f0: 312c 2035 2e30 3030 3030 3030 3065 2b30  1, 5.00000000e+0
+00003a00: 3020 342e 3939 3939 3938 3230 652b 3031  0 4.99999820e+01
+00003a10: 204c 2035 2e30 3030 3030 3030 3065 2b30   L 5.00000000e+0
+00003a20: 3020 372e 3234 3939 3939 3130 652b 3031  0 7.24999910e+01
+00003a30: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00003a40: 6174 6820 643d 224d 2031 2e37 3035 3537  ath d="M 1.70557
+00003a50: 3631 3065 2b30 3120 352e 3332 3134 3232  610e+01 5.321422
+00003a60: 3430 652b 3031 204c 2035 2e30 3030 3030  40e+01 L 5.00000
+00003a70: 3030 3065 2b30 3020 342e 3939 3939 3938  000e+00 4.999998
+00003a80: 3230 652b 3031 2051 2037 2e37 3030 3338  20e+01 Q 7.70038
+00003a90: 3937 3465 2b30 3020 352e 3330 3435 3633  974e+00 5.304563
+00003aa0: 3530 652b 3031 2c20 312e 3033 3731 3430  50e+01, 1.037140
+00003ab0: 3832 652b 3031 2035 2e36 3037 3634 3133  82e+01 5.6076413
+00003ac0: 3365 2b30 3120 5120 312e 3330 3336 3333  3e+01 Q 1.303633
+00003ad0: 3130 652b 3031 2035 2e39 3039 3939 3837  10e+01 5.9099987
+00003ae0: 3765 2b30 312c 2031 2e35 3734 3138 3639  7e+01, 1.5741869
+00003af0: 3065 2b30 3120 362e 3232 3137 3431 3930  0e+01 6.22174190
+00003b00: 652b 3031 2051 2031 2e36 3036 3437 3835  e+01 Q 1.6064785
+00003b10: 3465 2b30 3120 352e 3939 3336 3831 3530  4e+01 5.99368150
+00003b20: 652b 3031 2c20 312e 3634 3030 3736 3432  e+01, 1.64007642
+00003b30: 652b 3031 2035 2e37 3639 3036 3437 3565  e+01 5.76906475e
+00003b40: 2b30 3120 5120 312e 3637 3336 3135 3333  +01 Q 1.67361533
+00003b50: 652b 3031 2035 2e35 3434 3738 3733 3665  e+01 5.54478736e
+00003b60: 2b30 312c 2031 2e37 3035 3537 3631 3065  +01, 1.70557610e
+00003b70: 2b30 3120 352e 3332 3134 3232 3430 652b  +01 5.32142240e+
+00003b80: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
+00003b90: 3c70 6174 6820 643d 224d 2031 2e36 3631  <path d="M 1.661
+00003ba0: 3733 3731 3065 2b30 3120 342e 3634 3833  73710e+01 4.6483
+00003bb0: 3831 3730 652b 3031 204c 2035 2e30 3030  8170e+01 L 5.000
+00003bc0: 3030 3030 3065 2b30 3020 342e 3939 3939  00000e+00 4.9999
+00003bd0: 3938 3230 652b 3031 204c 2031 2e37 3035  9820e+01 L 1.705
+00003be0: 3537 3631 3065 2b30 3120 352e 3332 3134  57610e+01 5.3214
+00003bf0: 3232 3430 652b 3031 204c 2031 2e36 3631  2240e+01 L 1.661
+00003c00: 3733 3731 3065 2b30 3120 342e 3634 3833  73710e+01 4.6483
+00003c10: 3831 3730 652b 3031 205a 2220 2f3e 0d0a  8170e+01 Z" />..
+00003c20: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
+00003c30: 2031 2e34 3636 3531 3831 3065 2b30 3120   1.46651810e+01 
+00003c40: 332e 3931 3130 3930 3030 652b 3031 204c  3.91109000e+01 L
+00003c50: 2035 2e30 3030 3030 3030 3065 2b30 3020   5.00000000e+00 
+00003c60: 342e 3939 3939 3938 3230 652b 3031 204c  4.99999820e+01 L
+00003c70: 2031 2e36 3631 3733 3731 3065 2b30 3120   1.66173710e+01 
+00003c80: 342e 3634 3833 3831 3730 652b 3031 204c  4.64838170e+01 L
+00003c90: 2031 2e34 3636 3531 3831 3065 2b30 3120   1.46651810e+01 
+00003ca0: 332e 3931 3130 3930 3030 652b 3031 205a  3.91109000e+01 Z
+00003cb0: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+00003cc0: 6820 643d 224d 2035 2e30 3030 3030 3030  h d="M 5.0000000
+00003cd0: 3065 2b30 3020 372e 3234 3939 3939 3130  0e+00 7.24999910
+00003ce0: 652b 3031 204c 2035 2e30 3030 3030 3030  e+01 L 5.0000000
+00003cf0: 3065 2b30 3020 392e 3530 3030 3030 3030  0e+00 9.50000000
+00003d00: 652b 3031 204c 2031 2e37 3030 3036 3633  e+01 L 1.7000663
+00003d10: 3065 2b30 3120 382e 3239 3838 3433 3830  0e+01 8.29884380
+00003d20: 652b 3031 204c 2035 2e30 3030 3030 3030  e+01 L 5.0000000
+00003d30: 3065 2b30 3020 372e 3234 3939 3939 3130  0e+00 7.24999910
+00003d40: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
+00003d50: 2020 3c70 6174 6820 643d 224d 2035 2e30    <path d="M 5.0
+00003d60: 3030 3030 3030 3065 2b30 3020 372e 3234  0000000e+00 7.24
+00003d70: 3939 3939 3130 652b 3031 204c 2031 2e37  999910e+01 L 1.7
+00003d80: 3030 3036 3633 3065 2b30 3120 382e 3239  0006630e+01 8.29
+00003d90: 3838 3433 3830 652b 3031 204c 2031 2e39  884380e+01 L 1.9
+00003da0: 3639 3538 3132 3065 2b30 3120 372e 3235  6958120e+01 7.25
+00003db0: 3936 3335 3430 652b 3031 2051 2031 2e35  963540e+01 Q 1.5
+00003dc0: 3931 3338 3631 3565 2b30 3120 372e 3235  9138615e+01 7.25
+00003dd0: 3534 3736 3339 652b 3031 2c20 312e 3232  547639e+01, 1.22
+00003de0: 3836 3533 3430 652b 3031 2037 2e32 3533  865340e+01 7.253
+00003df0: 3338 3935 3365 2b30 3120 5120 382e 3635  38953e+01 Q 8.65
+00003e00: 3331 3936 3032 652b 3030 2037 2e32 3531  319602e+00 7.251
+00003e10: 3237 3839 3565 2b30 312c 2035 2e30 3030  27895e+01, 5.000
+00003e20: 3030 3030 3065 2b30 3020 372e 3234 3939  00000e+00 7.2499
+00003e30: 3939 3130 652b 3031 205a 2220 2f3e 0d0a  9910e+01 Z" />..
+00003e40: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
+00003e50: 2031 2e35 3734 3138 3639 3065 2b30 3120   1.57418690e+01 
+00003e60: 362e 3232 3137 3431 3930 652b 3031 204c  6.22174190e+01 L
+00003e70: 2035 2e30 3030 3030 3030 3065 2b30 3020   5.00000000e+00 
+00003e80: 372e 3234 3939 3939 3130 652b 3031 2051  7.24999910e+01 Q
+00003e90: 2038 2e36 3533 3139 3630 3265 2b30 3020   8.65319602e+00 
+00003ea0: 372e 3235 3132 3738 3935 652b 3031 2c20  7.25127895e+01, 
+00003eb0: 312e 3232 3836 3533 3430 652b 3031 2037  1.22865340e+01 7
+00003ec0: 2e32 3533 3338 3935 3365 2b30 3120 5120  .25338953e+01 Q 
+00003ed0: 312e 3539 3133 3836 3135 652b 3031 2037  1.59138615e+01 7
+00003ee0: 2e32 3535 3437 3633 3965 2b30 312c 2031  .25547639e+01, 1
+00003ef0: 2e39 3639 3538 3132 3065 2b30 3120 372e  .96958120e+01 7.
+00003f00: 3235 3936 3335 3430 652b 3031 2051 2031  25963540e+01 Q 1
+00003f10: 2e38 3638 3838 3236 3665 2b30 3120 362e  .86888266e+01 6.
+00003f20: 3939 3930 3137 3334 652b 3031 2c20 312e  99901734e+01, 1.
+00003f30: 3736 3837 3730 3935 652b 3031 2036 2e37  76877095e+01 6.7
+00003f40: 3337 3638 3531 3565 2b30 3120 5120 312e  3768515e+01 Q 1.
+00003f50: 3636 3931 3035 3830 652b 3031 2036 2e34  66910580e+01 6.4
+00003f60: 3737 3437 3439 3765 2b30 312c 2031 2e35  7747497e+01, 1.5
+00003f70: 3734 3138 3639 3065 2b30 3120 362e 3232  7418690e+01 6.22
+00003f80: 3137 3431 3930 652b 3031 205a 2220 2f3e  174190e+01 Z" />
+00003f90: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
+00003fa0: 224d 2031 2e35 3734 3138 3639 3065 2b30  "M 1.57418690e+0
+00003fb0: 3120 362e 3232 3137 3431 3930 652b 3031  1 6.22174190e+01
+00003fc0: 2051 2031 2e37 3439 3635 3433 3465 2b30   Q 1.74965434e+0
+00003fd0: 3120 362e 3134 3233 3135 3133 652b 3031  1 6.14231513e+01
+00003fe0: 2c20 312e 3932 3937 3132 3837 652b 3031  , 1.92971287e+01
+00003ff0: 2036 2e30 3539 3537 3739 3165 2b30 3120   6.05957791e+01 
+00004000: 5120 322e 3131 3230 3535 3435 652b 3031  Q 2.11205545e+01
+00004010: 2035 2e39 3735 3930 3930 3665 2b30 312c   5.97590906e+01,
+00004020: 2032 2e33 3030 3030 3030 3065 2b30 3120   2.30000000e+01 
+00004030: 352e 3930 3030 3030 3030 652b 3031 2051  5.90000000e+01 Q
+00004040: 2032 2e31 3530 3231 3536 3065 2b30 3120   2.15021560e+01 
+00004050: 352e 3735 3638 3536 3936 652b 3031 2c20  5.75685696e+01, 
+00004060: 322e 3030 3130 3330 3435 652b 3031 2035  2.00103045e+01 5
+00004070: 2e36 3130 3631 3934 3465 2b30 3120 5120  .61061944e+01 Q 
+00004080: 312e 3835 3236 3531 3030 652b 3031 2035  1.85265100e+01 5
+00004090: 2e34 3635 3135 3835 3565 2b30 312c 2031  .46515855e+01, 1
+000040a0: 2e37 3035 3537 3631 3065 2b30 3120 352e  .70557610e+01 5.
+000040b0: 3332 3134 3232 3430 652b 3031 2051 2031  32142240e+01 Q 1
+000040c0: 2e36 3733 3631 3533 3365 2b30 3120 352e  .67361533e+01 5.
+000040d0: 3534 3437 3837 3336 652b 3031 2c20 312e  54478736e+01, 1.
+000040e0: 3634 3030 3736 3432 652b 3031 2035 2e37  64007642e+01 5.7
+000040f0: 3639 3036 3437 3565 2b30 3120 5120 312e  6906475e+01 Q 1.
+00004100: 3630 3634 3738 3534 652b 3031 2035 2e39  60647854e+01 5.9
+00004110: 3933 3638 3135 3065 2b30 312c 2031 2e35  9368150e+01, 1.5
+00004120: 3734 3138 3639 3065 2b30 3120 362e 3232  7418690e+01 6.22
+00004130: 3137 3431 3930 652b 3031 205a 2220 2f3e  174190e+01 Z" />
+00004140: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
+00004150: 224d 2034 2e36 3539 3831 3236 3065 2b30  "M 4.65981260e+0
+00004160: 3120 382e 3235 3330 3434 3630 652b 3031  1 8.25304460e+01
+00004170: 2051 2034 2e35 3233 3138 3539 3565 2b30   Q 4.52318595e+0
+00004180: 3120 382e 3132 3138 3031 3133 652b 3031  1 8.12180113e+01
+00004190: 2c20 342e 3337 3830 3431 3931 652b 3031  , 4.37804191e+01
+000041a0: 2037 2e39 3838 3133 3939 3565 2b30 3120   7.98813995e+01 
+000041b0: 5120 342e 3233 3036 3031 3237 652b 3031  Q 4.23060127e+01
+000041c0: 2037 2e38 3531 3737 3332 3865 2b30 312c   7.85177328e+01,
+000041d0: 2034 2e31 3030 3030 3030 3065 2b30 3120   4.10000000e+01 
+000041e0: 372e 3730 3030 3030 3030 652b 3031 2051  7.70000000e+01 Q
+000041f0: 2034 2e30 3232 3839 3639 3065 2b30 3120   4.02289690e+01 
+00004200: 372e 3838 3636 3335 3131 652b 3031 2c20  7.88663511e+01, 
+00004210: 332e 3933 3533 3036 3735 652b 3031 2038  3.93530675e+01 8
+00004220: 2e30 3637 3438 3539 3365 2b30 3120 5120  .06748593e+01 Q 
+00004230: 332e 3834 3932 3833 3837 652b 3031 2038  3.84928387e+01 8
+00004240: 2e32 3434 3632 3133 3465 2b30 312c 2033  .24462134e+01, 3
+00004250: 2e37 3638 3138 3236 3065 2b30 3120 382e  .76818260e+01 8.
+00004260: 3431 3436 3030 3030 652b 3031 204c 2034  41460000e+01 L 4
+00004270: 2e36 3539 3831 3236 3065 2b30 3120 382e  .65981260e+01 8.
+00004280: 3235 3330 3434 3630 652b 3031 205a 2220  25304460e+01 Z" 
+00004290: 2f3e 0d0a 2020 2020 2020 3c70 6174 6820  />..      <path 
+000042a0: 643d 224d 2036 2e35 3838 3833 3033 3065  d="M 6.58883030e
+000042b0: 2b30 3120 352e 3736 3239 3833 3130 652b  +01 5.76298310e+
+000042c0: 3031 2051 2036 2e34 3135 3633 3331 3165  01 Q 6.41563311e
+000042d0: 2b30 3120 352e 3833 3431 3631 3635 652b  +01 5.83416165e+
+000042e0: 3031 2c20 362e 3234 3037 3636 3630 652b  01, 6.24076660e+
+000042f0: 3031 2035 2e38 3637 3434 3934 3365 2b30  01 5.86744943e+0
+00004300: 3120 5120 362e 3036 3630 3833 3437 652b  1 Q 6.06608347e+
+00004310: 3031 2035 2e39 3030 3531 3730 3765 2b30  01 5.90051707e+0
+00004320: 312c 2035 2e39 3030 3030 3030 3065 2b30  1, 5.90000000e+0
+00004330: 3120 352e 3930 3030 3030 3030 652b 3031  1 5.90000000e+01
+00004340: 204c 2036 2e36 3030 3938 3735 3065 2b30   L 6.60098750e+0
+00004350: 3120 362e 3630 3338 3136 3230 652b 3031  1 6.60381620e+01
+00004360: 2051 2036 2e36 3032 3231 3534 3665 2b30   Q 6.60221546e+0
+00004370: 3120 362e 3430 3035 3638 3037 652b 3031  1 6.40056807e+01
+00004380: 2c20 362e 3630 3136 3731 3938 652b 3031  , 6.60167198e+01
+00004390: 2036 2e31 3934 3938 3336 3765 2b30 3120   6.19498367e+01 
+000043a0: 5120 362e 3630 3132 3633 3135 652b 3031  Q 6.60126315e+01
+000043b0: 2035 2e39 3931 3233 3834 3965 2b30 312c   5.99123849e+01,
+000043c0: 2036 2e35 3838 3833 3033 3065 2b30 3120   6.58883030e+01 
+000043d0: 352e 3736 3239 3833 3130 652b 3031 205a  5.76298310e+01 Z
+000043e0: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+000043f0: 6820 643d 224d 2038 2e34 3134 3730 3938  h d="M 8.4147098
+00004400: 3065 2b30 3120 332e 3736 3833 3136 3730  0e+01 3.76831670
+00004410: 652b 3031 2051 2038 2e32 3434 3731 3439  e+01 Q 8.2447149
+00004420: 3065 2b30 3120 332e 3834 3933 3831 3036  0e+01 3.84938106
+00004430: 652b 3031 2c20 382e 3036 3735 3439 3736  e+01, 8.06754976
+00004440: 652b 3031 2033 2e39 3335 3336 3931 3565  e+01 3.93536915e
+00004450: 2b30 3120 5120 372e 3838 3636 3437 3932  +01 Q 7.88664792
+00004460: 652b 3031 2034 2e30 3232 3933 3335 3165  e+01 4.02293351e
+00004470: 2b30 312c 2037 2e37 3030 3030 3030 3065  +01, 7.70000000e
+00004480: 2b30 3120 342e 3130 3030 3030 3030 652b  +01 4.10000000e+
+00004490: 3031 2051 2037 2e38 3531 3734 3833 3865  01 Q 7.85174838e
+000044a0: 2b30 3120 342e 3233 3036 3433 3138 652b  +01 4.23064318e+
+000044b0: 3031 2c20 372e 3938 3830 3730 3339 652b  01, 7.98807039e+
+000044c0: 3031 2034 2e33 3738 3131 3931 3465 2b30  01 4.37811914e+0
+000044d0: 3120 5120 382e 3132 3137 3036 3534 652b  1 Q 8.12170654e+
+000044e0: 3031 2034 2e35 3233 3331 3739 3565 2b30  01 4.52331795e+0
+000044f0: 312c 2038 2e32 3532 3931 3935 3065 2b30  1, 8.25291950e+0
+00004500: 3120 342e 3635 3939 3835 3430 652b 3031  1 4.65998540e+01
+00004510: 204c 2038 2e34 3134 3730 3938 3065 2b30   L 8.41470980e+0
+00004520: 3120 332e 3736 3833 3136 3730 652b 3031  1 3.76831670e+01
+00004530: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00004540: 6174 6820 643d 224d 2037 2e35 3632 3938  ath d="M 7.56298
+00004550: 3331 3065 2b30 3120 332e 3431 3131 3639  310e+01 3.411169
+00004560: 3730 652b 3031 2051 2037 2e36 3334 3136  70e+01 Q 7.63416
+00004570: 3136 3565 2b30 3120 332e 3538 3433 3636  165e+01 3.584366
+00004580: 3839 652b 3031 2c20 372e 3636 3734 3439  89e+01, 7.667449
+00004590: 3433 652b 3031 2033 2e37 3539 3233 3334  43e+01 3.7592334
+000045a0: 3065 2b30 3120 5120 372e 3730 3035 3137  0e+01 Q 7.700517
+000045b0: 3037 652b 3031 2033 2e39 3333 3931 3635  07e+01 3.9339165
+000045c0: 3365 2b30 312c 2037 2e37 3030 3030 3030  3e+01, 7.7000000
+000045d0: 3065 2b30 3120 342e 3130 3030 3030 3030  0e+01 4.10000000
+000045e0: 652b 3031 2051 2037 2e38 3836 3634 3739  e+01 Q 7.8866479
+000045f0: 3265 2b30 3120 342e 3032 3239 3333 3531  2e+01 4.02293351
+00004600: 652b 3031 2c20 382e 3036 3735 3439 3736  e+01, 8.06754976
+00004610: 652b 3031 2033 2e39 3335 3336 3931 3565  e+01 3.93536915e
+00004620: 2b30 3120 5120 382e 3234 3437 3134 3930  +01 Q 8.24471490
+00004630: 652b 3031 2033 2e38 3439 3338 3130 3665  e+01 3.84938106e
+00004640: 2b30 312c 2038 2e34 3134 3730 3938 3065  +01, 8.41470980e
+00004650: 2b30 3120 332e 3736 3833 3136 3730 652b  +01 3.76831670e+
+00004660: 3031 2051 2038 2e32 3130 3231 3130 3765  01 Q 8.21021107e
+00004670: 2b30 3120 332e 3638 3032 3636 3530 652b  +01 3.68026650e+
+00004680: 3031 2c20 382e 3030 3537 3531 3138 652b  01, 8.00575118e+
+00004690: 3031 2033 2e35 3838 3134 3036 3965 2b30  01 3.58814069e+0
+000046a0: 3120 5120 372e 3830 3334 3837 3735 652b  1 Q 7.80348775e+
+000046b0: 3031 2033 2e34 3936 3539 3830 3165 2b30  01 3.49659801e+0
+000046c0: 312c 2037 2e35 3632 3938 3331 3065 2b30  1, 7.56298310e+0
+000046d0: 3120 332e 3431 3131 3639 3730 652b 3031  1 3.41116970e+01
+000046e0: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+000046f0: 6174 6820 643d 224d 2037 2e37 3030 3030  ath d="M 7.70000
+00004700: 3030 3065 2b30 3120 342e 3130 3030 3030  000e+01 4.100000
+00004710: 3030 652b 3031 2051 2037 2e37 3030 3531  00e+01 Q 7.70051
+00004720: 3730 3765 2b30 3120 342e 3236 3630 3833  707e+01 4.266083
+00004730: 3437 652b 3031 2c20 372e 3636 3734 3439  47e+01, 7.667449
+00004740: 3433 652b 3031 2034 2e34 3430 3736 3636  43e+01 4.4407666
+00004750: 3065 2b30 3120 5120 372e 3633 3431 3631  0e+01 Q 7.634161
+00004760: 3635 652b 3031 2034 2e36 3135 3633 3331  65e+01 4.6156331
+00004770: 3165 2b30 312c 2037 2e35 3632 3938 3331  1e+01, 7.5629831
+00004780: 3065 2b30 3120 342e 3738 3838 3330 3330  0e+01 4.78883030
+00004790: 652b 3031 2051 2037 2e37 3533 3239 3230  e+01 Q 7.7532920
+000047a0: 3565 2b30 3120 342e 3736 3231 3437 3633  5e+01 4.76214763
+000047b0: 652b 3031 2c20 372e 3932 3035 3933 3835  e+01, 7.92059385
+000047c0: 652b 3031 2034 2e37 3237 3736 3635 3165  e+01 4.72776651e
+000047d0: 2b30 3120 5120 382e 3038 3838 3233 3839  +01 Q 8.08882389
+000047e0: 652b 3031 2034 2e36 3933 3335 3330 3065  e+01 4.69335300e
+000047f0: 2b30 312c 2038 2e32 3532 3931 3935 3065  +01, 8.25291950e
+00004800: 2b30 3120 342e 3635 3939 3835 3430 652b  +01 4.65998540e+
+00004810: 3031 2051 2038 2e31 3231 3730 3635 3465  01 Q 8.12170654e
+00004820: 2b30 3120 342e 3532 3333 3137 3935 652b  +01 4.52331795e+
+00004830: 3031 2c20 372e 3938 3830 3730 3339 652b  01, 7.98807039e+
+00004840: 3031 2034 2e33 3738 3131 3931 3465 2b30  01 4.37811914e+0
+00004850: 3120 5120 372e 3835 3137 3438 3338 652b  1 Q 7.85174838e+
+00004860: 3031 2034 2e32 3330 3634 3331 3865 2b30  01 4.23064318e+0
+00004870: 312c 2037 2e37 3030 3030 3030 3065 2b30  1, 7.70000000e+0
+00004880: 3120 342e 3130 3030 3030 3030 652b 3031  1 4.10000000e+01
+00004890: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+000048a0: 6174 6820 643d 224d 2035 2e39 3030 3030  ath d="M 5.90000
+000048b0: 3030 3065 2b30 3120 322e 3330 3030 3030  000e+01 2.300000
+000048c0: 3030 652b 3031 2051 2035 2e39 3735 3934  00e+01 Q 5.97594
+000048d0: 3231 3965 2b30 3120 322e 3131 3230 3732  219e+01 2.112072
+000048e0: 3634 652b 3031 2c20 362e 3035 3936 3337  64e+01, 6.059637
+000048f0: 3137 652b 3031 2031 2e39 3239 3737 3434  17e+01 1.9297744
+00004900: 3665 2b30 3120 5120 362e 3134 3234 3032  6e+01 Q 6.142402
+00004910: 3530 652b 3031 2031 2e37 3439 3735 3435  50e+01 1.7497545
+00004920: 3065 2b30 312c 2036 2e32 3231 3836 3433  0e+01, 6.2218643
+00004930: 3065 2b30 3120 312e 3537 3433 3035 3730  0e+01 1.57430570
+00004940: 652b 3031 2051 2035 2e39 3933 3736 3536  e+01 Q 5.9937656
+00004950: 3565 2b30 3120 312e 3630 3635 3638 3535  5e+01 1.60656855
+00004960: 652b 3031 2c20 352e 3736 3931 3235 3430  e+01, 5.76912540
+00004970: 652b 3031 2031 2e36 3430 3133 3634 3865  e+01 1.64013648e
+00004980: 2b30 3120 5120 352e 3534 3438 3230 3932  +01 Q 5.54482092
+00004990: 652b 3031 2031 2e36 3733 3634 3630 3165  e+01 1.67364601e
+000049a0: 2b30 312c 2035 2e33 3231 3432 3333 3065  +01, 5.32142330e
+000049b0: 2b30 3120 312e 3730 3535 3737 3030 652b  +01 1.70557700e+
+000049c0: 3031 2051 2035 2e34 3635 3136 3036 3465  01 Q 5.46516064e
+000049d0: 2b30 3120 312e 3835 3236 3532 3532 652b  +01 1.85265252e+
+000049e0: 3031 2c20 352e 3631 3036 3230 3830 652b  01, 5.61062080e+
+000049f0: 3031 2032 2e30 3031 3033 3134 3765 2b30  01 2.00103147e+0
+00004a00: 3120 5120 352e 3735 3638 3535 3836 652b  1 Q 5.75685586e+
+00004a10: 3031 2032 2e31 3530 3231 3433 3465 2b30  01 2.15021434e+0
+00004a20: 312c 2035 2e39 3030 3030 3030 3065 2b30  1, 5.90000000e+0
+00004a30: 3120 322e 3330 3030 3030 3030 652b 3031  1 2.30000000e+01
+00004a40: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00004a50: 6174 6820 643d 224d 2035 2e39 3030 3030  ath d="M 5.90000
+00004a60: 3030 3065 2b30 3120 322e 3330 3030 3030  000e+01 2.300000
+00004a70: 3030 652b 3031 2051 2036 2e30 3636 3038  00e+01 Q 6.06608
+00004a80: 3334 3765 2b30 3120 322e 3239 3934 3832  347e+01 2.299482
+00004a90: 3933 652b 3031 2c20 362e 3234 3037 3636  93e+01, 6.240766
+00004aa0: 3630 652b 3031 2032 2e33 3332 3535 3035  60e+01 2.3325505
+00004ab0: 3765 2b30 3120 5120 362e 3431 3536 3333  7e+01 Q 6.415633
+00004ac0: 3131 652b 3031 2032 2e33 3635 3833 3833  11e+01 2.3658383
+00004ad0: 3565 2b30 312c 2036 2e35 3838 3833 3033  5e+01, 6.5888303
+00004ae0: 3065 2b30 3120 322e 3433 3730 3136 3930  0e+01 2.43701690
+00004af0: 652b 3031 2051 2036 2e35 3030 3939 3936  e+01 Q 6.5009996
+00004b00: 3765 2b30 3120 322e 3139 3138 3636 3636  7e+01 2.19186666
+00004b10: 652b 3031 2c20 362e 3430 3637 3133 3634  e+01, 6.40671364
+00004b20: 652b 3031 2031 2e39 3837 3337 3735 3665  e+01 1.98737756e
+00004b30: 2b30 3120 5120 362e 3331 3230 3834 3738  +01 Q 6.31208478
+00004b40: 652b 3031 2031 2e37 3831 3039 3237 3465  e+01 1.78109274e
+00004b50: 2b30 312c 2036 2e32 3231 3836 3433 3065  +01, 6.22186430e
+00004b60: 2b30 3120 312e 3537 3433 3035 3730 652b  +01 1.57430570e+
+00004b70: 3031 2051 2036 2e31 3432 3430 3235 3065  01 Q 6.14240250e
+00004b80: 2b30 3120 312e 3734 3937 3534 3530 652b  +01 1.74975450e+
+00004b90: 3031 2c20 362e 3035 3936 3337 3137 652b  01, 6.05963717e+
+00004ba0: 3031 2031 2e39 3239 3737 3434 3665 2b30  01 1.92977446e+0
+00004bb0: 3120 5120 352e 3937 3539 3432 3139 652b  1 Q 5.97594219e+
+00004bc0: 3031 2032 2e31 3132 3037 3236 3465 2b30  01 2.11207264e+0
+00004bd0: 312c 2035 2e39 3030 3030 3030 3065 2b30  1, 5.90000000e+0
+00004be0: 3120 322e 3330 3030 3030 3030 652b 3031  1 2.30000000e+01
+00004bf0: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00004c00: 6174 6820 643d 224d 2035 2e30 3030 3030  ath d="M 5.00000
+00004c10: 3030 3065 2b30 3120 322e 3330 3030 3030  000e+01 2.300000
+00004c20: 3030 652b 3031 204c 2035 2e39 3030 3030  00e+01 L 5.90000
+00004c30: 3030 3065 2b30 3120 322e 3330 3030 3030  000e+01 2.300000
+00004c40: 3030 652b 3031 2051 2035 2e37 3536 3835  00e+01 Q 5.75685
+00004c50: 3538 3665 2b30 3120 322e 3135 3032 3134  586e+01 2.150214
+00004c60: 3334 652b 3031 2c20 352e 3631 3036 3230  34e+01, 5.610620
+00004c70: 3830 652b 3031 2032 2e30 3031 3033 3134  80e+01 2.0010314
+00004c80: 3765 2b30 3120 5120 352e 3436 3531 3630  7e+01 Q 5.465160
+00004c90: 3634 652b 3031 2031 2e38 3532 3635 3235  64e+01 1.8526525
+00004ca0: 3265 2b30 312c 2035 2e33 3231 3432 3333  2e+01, 5.3214233
+00004cb0: 3065 2b30 3120 312e 3730 3535 3737 3030  0e+01 1.70557700
+00004cc0: 652b 3031 204c 2035 2e30 3030 3030 3030  e+01 L 5.0000000
+00004cd0: 3065 2b30 3120 322e 3330 3030 3030 3030  0e+01 2.30000000
+00004ce0: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
+00004cf0: 2020 3c70 6174 6820 643d 224d 2035 2e37    <path d="M 5.7
+00004d00: 3130 3734 3938 3065 2b30 3120 382e 3133  1074980e+01 8.13
+00004d10: 3036 3838 3730 652b 3031 2051 2036 2e30  068870e+01 Q 6.0
+00004d20: 3136 3835 3237 3665 2b30 3120 382e 3033  1685276e+01 8.03
+00004d30: 3736 3534 3531 652b 3031 2c20 362e 3332  765451e+01, 6.32
+00004d40: 3234 3230 3833 652b 3031 2037 2e39 3433  242083e+01 7.943
+00004d50: 3731 3933 3165 2b30 3120 5120 362e 3632  71931e+01 Q 6.62
+00004d60: 3838 3438 3336 652b 3031 2037 2e38 3439  884836e+01 7.849
+00004d70: 3438 3335 3565 2b30 312c 2036 2e39 3230  48355e+01, 6.920
+00004d80: 3838 3731 3065 2b30 3120 372e 3735 3632  88710e+01 7.7562
+00004d90: 3338 3330 652b 3031 2051 2036 2e37 3133  3830e+01 Q 6.713
+00004da0: 3931 3537 3565 2b30 3120 372e 3633 3330  91575e+01 7.6330
+00004db0: 3730 3131 652b 3031 2c20 362e 3439 3935  7011e+01, 6.4995
+00004dc0: 3132 3535 652b 3031 2037 2e35 3033 3839  1255e+01 7.50389
+00004dd0: 3737 3265 2b30 3120 5120 362e 3238 3630  772e+01 Q 6.2860
+00004de0: 3931 3532 652b 3031 2037 2e33 3735 3331  9152e+01 7.37531
+00004df0: 3034 3165 2b30 312c 2036 2e30 3637 3837  041e+01, 6.06787
+00004e00: 3631 3065 2b30 3120 372e 3234 3236 3636  610e+01 7.242666
+00004e10: 3830 652b 3031 2051 2035 2e39 3737 3231  80e+01 Q 5.97721
+00004e20: 3835 3865 2b30 3120 372e 3436 3632 3731  858e+01 7.466271
+00004e30: 3034 652b 3031 2c20 352e 3838 3830 3032  04e+01, 5.888002
+00004e40: 3637 652b 3031 2037 2e36 3839 3436 3637  67e+01 7.6894667
+00004e50: 3865 2b30 3120 5120 352e 3739 3839 3430  8e+01 Q 5.798940
+00004e60: 3137 652b 3031 2037 2e39 3132 3236 3233  17e+01 7.9122623
+00004e70: 3865 2b30 312c 2035 2e37 3130 3734 3938  8e+01, 5.7107498
+00004e80: 3065 2b30 3120 382e 3133 3036 3838 3730  0e+01 8.13068870
+00004e90: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
+00004ea0: 2020 3c70 6174 6820 643d 224d 2032 2e37    <path d="M 2.7
+00004eb0: 3338 3232 3434 3065 2b30 3120 382e 3032  3822440e+01 8.02
+00004ec0: 3735 3733 3930 652b 3031 204c 2031 2e39  757390e+01 L 1.9
+00004ed0: 3639 3538 3132 3065 2b30 3120 372e 3235  6958120e+01 7.25
+00004ee0: 3936 3335 3430 652b 3031 204c 2031 2e37  963540e+01 L 1.7
+00004ef0: 3030 3036 3633 3065 2b30 3120 382e 3239  0006630e+01 8.29
+00004f00: 3838 3433 3830 652b 3031 204c 2032 2e37  884380e+01 L 2.7
+00004f10: 3338 3232 3434 3065 2b30 3120 382e 3032  3822440e+01 8.02
+00004f20: 3735 3733 3930 652b 3031 205a 2220 2f3e  757390e+01 Z" />
+00004f30: 0d0a 2020 2020 2020 3c70 6174 6820 643d  ..      <path d=
+00004f40: 224d 2038 2e31 3933 3033 3335 3065 2b30  "M 8.19303350e+0
+00004f50: 3120 382e 3139 3437 3538 3830 652b 3031  1 8.19475880e+01
+00004f60: 204c 2037 2e37 3533 3437 3632 3065 2b30   L 7.75347620e+0
+00004f70: 3120 362e 3932 3336 3439 3230 652b 3031  1 6.92364920e+01
+00004f80: 204c 2036 2e39 3230 3838 3731 3065 2b30   L 6.92088710e+0
+00004f90: 3120 372e 3735 3632 3338 3330 652b 3031  1 7.75623830e+01
+00004fa0: 204c 2038 2e31 3933 3033 3335 3065 2b30   L 8.19303350e+0
+00004fb0: 3120 382e 3139 3437 3538 3830 652b 3031  1 8.19475880e+01
+00004fc0: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00004fd0: 6174 6820 643d 224d 2034 2e31 3030 3030  ath d="M 4.10000
+00004fe0: 3039 3065 2b30 3120 322e 3330 3030 3030  090e+01 2.300000
+00004ff0: 3030 652b 3031 204c 2034 2e36 3438 3338  00e+01 L 4.64838
+00005000: 3335 3065 2b30 3120 312e 3636 3137 3337  350e+01 1.661737
+00005010: 3130 652b 3031 204c 2033 2e39 3131 3039  10e+01 L 3.91109
+00005020: 3138 3065 2b30 3120 312e 3436 3635 3138  180e+01 1.466518
+00005030: 3130 652b 3031 204c 2034 2e31 3030 3030  10e+01 L 4.10000
+00005040: 3039 3065 2b30 3120 322e 3330 3030 3030  090e+01 2.300000
+00005050: 3030 652b 3031 205a 2220 2f3e 0d0a 2020  00e+01 Z" />..  
+00005060: 2020 2020 3c70 6174 6820 643d 224d 2033      <path d="M 3
+00005070: 2e32 3030 3030 3030 3065 2b30 3120 322e  .20000000e+01 2.
+00005080: 3330 3030 3030 3030 652b 3031 204c 2034  30000000e+01 L 4
+00005090: 2e31 3030 3030 3039 3065 2b30 3120 322e  .10000090e+01 2.
+000050a0: 3330 3030 3030 3030 652b 3031 204c 2033  30000000e+01 L 3
+000050b0: 2e39 3131 3039 3138 3065 2b30 3120 312e  .91109180e+01 1.
+000050c0: 3436 3635 3138 3130 652b 3031 204c 2033  46651810e+01 L 3
+000050d0: 2e32 3030 3030 3030 3065 2b30 3120 322e  .20000000e+01 2.
+000050e0: 3330 3030 3030 3030 652b 3031 205a 2220  30000000e+01 Z" 
+000050f0: 2f3e 0d0a 2020 2020 2020 3c70 6174 6820  />..      <path 
+00005100: 643d 224d 2037 2e37 3533 3437 3632 3065  d="M 7.75347620e
+00005110: 2b30 3120 362e 3932 3336 3439 3230 652b  +01 6.92364920e+
+00005120: 3031 2051 2037 2e34 3734 3238 3838 3465  01 Q 7.47428884e
+00005130: 2b30 3120 362e 3834 3538 3039 3637 652b  +01 6.84580967e+
+00005140: 3031 2c20 372e 3138 3431 3734 3835 652b  01, 7.18417485e+
+00005150: 3031 2036 2e37 3635 3538 3337 3965 2b30  01 6.76558379e+0
+00005160: 3120 5120 362e 3839 3431 3437 3735 652b  1 Q 6.89414775e+
+00005170: 3031 2036 2e36 3835 3339 3231 3965 2b30  01 6.68539219e+0
+00005180: 312c 2036 2e36 3030 3938 3735 3065 2b30  1, 6.60098750e+0
+00005190: 3120 362e 3630 3338 3136 3230 652b 3031  1 6.60381620e+01
+000051a0: 2051 2036 2e36 3832 3536 3737 3965 2b30   Q 6.68256779e+0
+000051b0: 3120 362e 3839 3639 3539 3333 652b 3031  1 6.89695933e+01
+000051c0: 2c20 362e 3736 3237 3831 3736 652b 3031  , 6.76278176e+01
+000051d0: 2037 2e31 3836 3937 3435 3065 2b30 3120   7.18697450e+01 
+000051e0: 5120 362e 3834 3330 3239 3133 652b 3031  Q 6.84302913e+01
+000051f0: 2037 2e34 3737 3037 3337 3065 2b30 312c   7.47707370e+01,
+00005200: 2036 2e39 3230 3838 3731 3065 2b30 3120   6.92088710e+01 
+00005210: 372e 3735 3632 3338 3330 652b 3031 204c  7.75623830e+01 L
+00005220: 2037 2e37 3533 3437 3632 3065 2b30 3120   7.75347620e+01 
+00005230: 362e 3932 3336 3439 3230 652b 3031 205a  6.92364920e+01 Z
+00005240: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+00005250: 6820 643d 224d 2037 2e37 3533 3437 3632  h d="M 7.7534762
+00005260: 3065 2b30 3120 362e 3932 3336 3439 3230  0e+01 6.92364920
+00005270: 652b 3031 2051 2037 2e38 3437 3137 3336  e+01 Q 7.8471736
+00005280: 3465 2b30 3120 362e 3633 3131 3731 3731  4e+01 6.63117171
+00005290: 652b 3031 2c20 372e 3934 3138 3738 3636  e+01, 7.94187866
+000052a0: 652b 3031 2036 2e33 3234 3237 3638 3565  e+01 6.32427685e
+000052b0: 2b30 3120 5120 382e 3033 3632 3831 3632  +01 Q 8.03628162
+000052c0: 652b 3031 2036 2e30 3138 3234 3330 3465  e+01 6.01824304e
+000052d0: 2b30 312c 2038 2e31 3239 3738 3639 3065  +01, 8.12978690e
+000052e0: 2b30 3120 352e 3731 3136 3634 3230 652b  +01 5.71166420e+
+000052f0: 3031 2051 2037 2e39 3131 3033 3238 3065  01 Q 7.91103280e
+00005300: 2b30 3120 352e 3830 3031 3730 3939 652b  +01 5.80017099e+
+00005310: 3031 2c20 372e 3638 3739 3036 3133 652b  01, 7.68790613e+
+00005320: 3031 2035 2e38 3839 3536 3032 3265 2b30  01 5.88956022e+0
+00005330: 3120 5120 372e 3436 3434 3137 3432 652b  1 Q 7.46441742e+
+00005340: 3031 2035 2e39 3739 3038 3739 3865 2b30  01 5.97908798e+0
+00005350: 312c 2037 2e32 3430 3439 3135 3065 2b30  1, 7.24049150e+0
+00005360: 3120 362e 3037 3030 3534 3130 652b 3031  1 6.07005410e+01
+00005370: 2051 2037 2e33 3732 3938 3433 3265 2b30   Q 7.37298432e+0
+00005380: 3120 362e 3238 3834 3136 3935 652b 3031  1 6.28841695e+01
+00005390: 2c20 372e 3530 3134 3235 3039 652b 3031  , 7.50142509e+01
+000053a0: 2036 2e35 3031 3938 3435 3065 2b30 3120   6.50198450e+01 
+000053b0: 5120 372e 3633 3034 3530 3631 652b 3031  Q 7.63045061e+01
+000053c0: 2036 2e37 3136 3533 3534 3665 2b30 312c   6.71653546e+01,
+000053d0: 2037 2e37 3533 3437 3632 3065 2b30 3120   7.75347620e+01 
+000053e0: 362e 3932 3336 3439 3230 652b 3031 205a  6.92364920e+01 Z
+000053f0: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+00005400: 6820 643d 224d 2037 2e32 3430 3439 3135  h d="M 7.2404915
+00005410: 3065 2b30 3120 362e 3037 3030 3534 3130  0e+01 6.07005410
+00005420: 652b 3031 204c 2036 2e36 3030 3938 3735  e+01 L 6.6009875
+00005430: 3065 2b30 3120 362e 3630 3338 3136 3230  0e+01 6.60381620
+00005440: 652b 3031 2051 2036 2e38 3934 3134 3737  e+01 Q 6.8941477
+00005450: 3565 2b30 3120 362e 3638 3533 3932 3139  5e+01 6.68539219
+00005460: 652b 3031 2c20 372e 3138 3431 3734 3835  e+01, 7.18417485
+00005470: 652b 3031 2036 2e37 3635 3538 3337 3965  e+01 6.76558379e
+00005480: 2b30 3120 5120 372e 3437 3432 3838 3834  +01 Q 7.47428884
+00005490: 652b 3031 2036 2e38 3435 3830 3936 3765  e+01 6.84580967e
+000054a0: 2b30 312c 2037 2e37 3533 3437 3632 3065  +01, 7.75347620e
+000054b0: 2b30 3120 362e 3932 3336 3439 3230 652b  +01 6.92364920e+
+000054c0: 3031 2051 2037 2e36 3330 3435 3036 3165  01 Q 7.63045061e
+000054d0: 2b30 3120 362e 3731 3635 3335 3436 652b  +01 6.71653546e+
+000054e0: 3031 2c20 372e 3530 3134 3235 3039 652b  01, 7.50142509e+
+000054f0: 3031 2036 2e35 3031 3938 3435 3065 2b30  01 6.50198450e+0
+00005500: 3120 5120 372e 3337 3239 3834 3332 652b  1 Q 7.37298432e+
+00005510: 3031 2036 2e32 3838 3431 3639 3565 2b30  01 6.28841695e+0
+00005520: 312c 2037 2e32 3430 3439 3135 3065 2b30  1, 7.24049150e+0
+00005530: 3120 362e 3037 3030 3534 3130 652b 3031  1 6.07005410e+01
+00005540: 205a 2220 2f3e 0d0a 2020 2020 2020 3c70   Z" />..      <p
+00005550: 6174 6820 643d 224d 2036 2e36 3030 3938  ath d="M 6.60098
+00005560: 3735 3065 2b30 3120 362e 3630 3338 3136  750e+01 6.603816
+00005570: 3230 652b 3031 204c 2036 2e30 3637 3837  20e+01 L 6.06787
+00005580: 3631 3065 2b30 3120 372e 3234 3236 3636  610e+01 7.242666
+00005590: 3830 652b 3031 2051 2036 2e32 3836 3039  80e+01 Q 6.28609
+000055a0: 3135 3265 2b30 3120 372e 3337 3533 3130  152e+01 7.375310
+000055b0: 3431 652b 3031 2c20 362e 3439 3935 3132  41e+01, 6.499512
+000055c0: 3535 652b 3031 2037 2e35 3033 3839 3737  55e+01 7.5038977
+000055d0: 3265 2b30 3120 5120 362e 3731 3339 3135  2e+01 Q 6.713915
+000055e0: 3735 652b 3031 2037 2e36 3333 3037 3031  75e+01 7.6330701
+000055f0: 3165 2b30 312c 2036 2e39 3230 3838 3731  1e+01, 6.9208871
+00005600: 3065 2b30 3120 372e 3735 3632 3338 3330  0e+01 7.75623830
+00005610: 652b 3031 2051 2036 2e38 3433 3032 3931  e+01 Q 6.8430291
+00005620: 3365 2b30 3120 372e 3437 3730 3733 3730  3e+01 7.47707370
+00005630: 652b 3031 2c20 362e 3736 3237 3831 3736  e+01, 6.76278176
+00005640: 652b 3031 2037 2e31 3836 3937 3435 3065  e+01 7.18697450e
+00005650: 2b30 3120 5120 362e 3638 3235 3637 3739  +01 Q 6.68256779
+00005660: 652b 3031 2036 2e38 3936 3935 3933 3365  e+01 6.89695933e
+00005670: 2b30 312c 2036 2e36 3030 3938 3735 3065  +01, 6.60098750e
+00005680: 2b30 3120 362e 3630 3338 3136 3230 652b  +01 6.60381620e+
+00005690: 3031 205a 2220 2f3e 0d0a 2020 2020 2020  01 Z" />..      
+000056a0: 3c70 6174 6820 643d 224d 2037 2e32 3630  <path d="M 7.260
+000056b0: 3131 3333 3065 2b30 3120 312e 3937 3030  11330e+01 1.9700
+000056c0: 3534 3630 652b 3031 204c 2038 2e30 3238  5460e+01 L 8.028
+000056d0: 3034 3832 3065 2b30 3120 322e 3733 3837  04820e+01 2.7387
+000056e0: 3032 3330 652b 3031 204c 2038 2e32 3939  0230e+01 L 8.299
+000056f0: 3438 3436 3065 2b30 3120 312e 3730 3037  48460e+01 1.7007
+00005700: 3037 3130 652b 3031 204c 2037 2e32 3630  0710e+01 L 7.260
+00005710: 3131 3333 3065 2b30 3120 312e 3937 3030  11330e+01 1.9700
+00005720: 3534 3630 652b 3031 205a 2220 2f3e 0d0a  5460e+01 Z" />..
+00005730: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
+00005740: 2038 2e30 3238 3034 3832 3065 2b30 3120   8.02804820e+01 
+00005750: 322e 3733 3837 3032 3330 652b 3031 2051  2.73870230e+01 Q
+00005760: 2037 2e39 3139 3333 3537 3865 2b30 3120   7.91933578e+01 
+00005770: 322e 3930 3030 3634 3538 652b 3031 2c20  2.90006458e+01, 
+00005780: 372e 3830 3833 3136 3031 652b 3031 2033  7.80831601e+01 3
+00005790: 2e30 3638 3136 3335 3465 2b30 3120 5120  .06816354e+01 Q 
+000057a0: 372e 3639 3732 3335 3737 652b 3031 2033  7.69723577e+01 3
+000057b0: 2e32 3336 3537 3439 3965 2b30 312c 2037  .23657499e+01, 7
+000057c0: 2e35 3632 3938 3331 3065 2b30 3120 332e  .56298310e+01 3.
+000057d0: 3431 3131 3639 3730 652b 3031 2051 2037  41116970e+01 Q 7
+000057e0: 2e38 3033 3438 3737 3565 2b30 3120 332e  .80348775e+01 3.
+000057f0: 3439 3635 3938 3031 652b 3031 2c20 382e  49659801e+01, 8.
+00005800: 3030 3537 3531 3138 652b 3031 2033 2e35  00575118e+01 3.5
+00005810: 3838 3134 3036 3965 2b30 3120 5120 382e  8814069e+01 Q 8.
+00005820: 3231 3032 3131 3037 652b 3031 2033 2e36  21021107e+01 3.6
+00005830: 3830 3236 3635 3065 2b30 312c 2038 2e34  8026650e+01, 8.4
+00005840: 3134 3730 3938 3065 2b30 3120 332e 3736  1470980e+01 3.76
+00005850: 3833 3136 3730 652b 3031 2051 2038 2e33  831670e+01 Q 8.3
+00005860: 3230 3331 3630 3065 2b30 3120 332e 3531  2031600e+01 3.51
+00005870: 3333 3632 3534 652b 3031 2c20 382e 3232  336254e+01, 8.22
+00005880: 3332 3337 3438 652b 3031 2033 2e32 3535  323748e+01 3.255
+00005890: 3734 3230 3765 2b30 3120 5120 382e 3132  74207e+01 Q 8.12
+000058a0: 3537 3036 3031 652b 3031 2032 2e39 3936  570601e+01 2.996
+000058b0: 3933 3539 3565 2b30 312c 2038 2e30 3238  93595e+01, 8.028
+000058c0: 3034 3832 3065 2b30 3120 322e 3733 3837  04820e+01 2.7387
+000058d0: 3032 3330 652b 3031 205a 2220 2f3e 0d0a  0230e+01 Z" />..
+000058e0: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
+000058f0: 2034 2e36 3438 3338 3335 3065 2b30 3120   4.64838350e+01 
+00005900: 312e 3636 3137 3337 3130 652b 3031 204c  1.66173710e+01 L
+00005910: 2035 2e30 3030 3030 3030 3065 2b30 3120   5.00000000e+01 
+00005920: 322e 3330 3030 3030 3030 652b 3031 204c  2.30000000e+01 L
+00005930: 2035 2e33 3231 3432 3333 3065 2b30 3120   5.32142330e+01 
+00005940: 312e 3730 3535 3737 3030 652b 3031 204c  1.70557700e+01 L
+00005950: 2034 2e36 3438 3338 3335 3065 2b30 3120   4.64838350e+01 
+00005960: 312e 3636 3137 3337 3130 652b 3031 205a  1.66173710e+01 Z
+00005970: 2220 2f3e 0d0a 2020 2020 2020 3c70 6174  " />..      <pat
+00005980: 6820 643d 224d 2034 2e31 3030 3030 3039  h d="M 4.1000009
+00005990: 3065 2b30 3120 322e 3330 3030 3030 3030  0e+01 2.30000000
+000059a0: 652b 3031 204c 2035 2e30 3030 3030 3030  e+01 L 5.0000000
+000059b0: 3065 2b30 3120 322e 3330 3030 3030 3030  0e+01 2.30000000
+000059c0: 652b 3031 204c 2034 2e36 3438 3338 3335  e+01 L 4.6483835
+000059d0: 3065 2b30 3120 312e 3636 3137 3337 3130  0e+01 1.66173710
+000059e0: 652b 3031 204c 2034 2e31 3030 3030 3039  e+01 L 4.1000009
+000059f0: 3065 2b30 3120 322e 3330 3030 3030 3030  0e+01 2.30000000
+00005a00: 652b 3031 205a 2220 2f3e 0d0a 2020 2020  e+01 Z" />..    
+00005a10: 2020 3c70 6174 6820 643d 224d 2037 2e31    <path d="M 7.1
+00005a20: 3732 3739 3236 3065 2b30 3120 322e 3832  7279260e+01 2.82
+00005a30: 3732 3038 3330 652b 3031 2051 2037 2e34  720830e+01 Q 7.4
+00005a40: 3036 3536 3438 3265 2b30 3120 322e 3739  0656482e+01 2.79
+00005a50: 3033 3737 3439 652b 3031 2c20 372e 3631  037749e+01, 7.61
+00005a60: 3535 3333 3231 652b 3031 2032 2e37 3734  553321e+01 2.774
+00005a70: 3139 3831 3665 2b30 3120 5120 372e 3832  19816e+01 Q 7.82
+00005a80: 3438 3732 3832 652b 3031 2032 2e37 3537  487282e+01 2.757
+00005a90: 3638 3538 3465 2b30 312c 2038 2e30 3238  68584e+01, 8.028
+00005aa0: 3034 3832 3065 2b30 3120 322e 3733 3837  04820e+01 2.7387
+00005ab0: 3032 3330 652b 3031 204c 2037 2e32 3630  0230e+01 L 7.260
+00005ac0: 3131 3333 3065 2b30 3120 312e 3937 3030  11330e+01 1.9700
+00005ad0: 3534 3630 652b 3031 2051 2037 2e32 3431  5460e+01 Q 7.241
+00005ae0: 3437 3335 3265 2b30 3120 322e 3137 3336  47352e+01 2.1736
+00005af0: 3530 3233 652b 3031 2c20 372e 3232 3532  5023e+01, 7.2252
+00005b00: 3937 3535 652b 3031 2032 2e33 3833 3336  9755e+01 2.38336
+00005b10: 3634 3265 2b30 3120 5120 372e 3230 3934  642e+01 Q 7.2094
+00005b20: 3532 3635 652b 3031 2032 2e35 3932 3830  5265e+01 2.59280
+00005b30: 3730 3065 2b30 312c 2037 2e31 3732 3739  700e+01, 7.17279
+00005b40: 3236 3065 2b30 3120 322e 3832 3732 3038  260e+01 2.827208
+00005b50: 3330 652b 3031 205a 2220 2f3e 0d0a 2020  30e+01 Z" />..  
+00005b60: 2020 2020 3c70 6174 6820 643d 224d 2037      <path d="M 7
+00005b70: 2e31 3732 3739 3236 3065 2b30 3120 322e  .17279260e+01 2.
+00005b80: 3832 3732 3038 3330 652b 3031 2051 2037  82720830e+01 Q 7
+00005b90: 2e32 3939 3930 3234 3865 2b30 3120 322e  .29990248e+01 2.
+00005ba0: 3935 3435 3032 3735 652b 3031 2c20 372e  95450275e+01, 7.
+00005bb0: 3339 3835 3533 3434 652b 3031 2033 2e31  39855344e+01 3.1
+00005bc0: 3032 3833 3535 3165 2b30 3120 5120 372e  0283551e+01 Q 7.
+00005bd0: 3439 3639 3630 3439 652b 3031 2033 2e32  49696049e+01 3.2
+00005be0: 3531 3234 3136 3165 2b30 312c 2037 2e35  5124161e+01, 7.5
+00005bf0: 3632 3938 3331 3065 2b30 3120 332e 3431  6298310e+01 3.41
+00005c00: 3131 3639 3730 652b 3031 2051 2037 2e36  116970e+01 Q 7.6
+00005c10: 3937 3233 3537 3765 2b30 3120 332e 3233  9723577e+01 3.23
+00005c20: 3635 3734 3939 652b 3031 2c20 372e 3830  657499e+01, 7.80
+00005c30: 3833 3136 3031 652b 3031 2033 2e30 3638  831601e+01 3.068
+00005c40: 3136 3335 3465 2b30 3120 5120 372e 3931  16354e+01 Q 7.91
+00005c50: 3933 3335 3738 652b 3031 2032 2e39 3030  933578e+01 2.900
+00005c60: 3036 3435 3865 2b30 312c 2038 2e30 3238  06458e+01, 8.028
+00005c70: 3034 3832 3065 2b30 3120 322e 3733 3837  04820e+01 2.7387
+00005c80: 3032 3330 652b 3031 2051 2037 2e38 3234  0230e+01 Q 7.824
+00005c90: 3837 3238 3265 2b30 3120 322e 3735 3736  87282e+01 2.7576
+00005ca0: 3835 3834 652b 3031 2c20 372e 3631 3535  8584e+01, 7.6155
+00005cb0: 3333 3231 652b 3031 2032 2e37 3734 3139  3321e+01 2.77419
+00005cc0: 3831 3665 2b30 3120 5120 372e 3430 3635  816e+01 Q 7.4065
+00005cd0: 3634 3832 652b 3031 2032 2e37 3930 3337  6482e+01 2.79037
+00005ce0: 3734 3965 2b30 312c 2037 2e31 3732 3739  749e+01, 7.17279
+00005cf0: 3236 3065 2b30 3120 322e 3832 3732 3038  260e+01 2.827208
+00005d00: 3330 652b 3031 205a 2220 2f3e 0d0a 2020  30e+01 Z" />..  
+00005d10: 2020 2020 3c70 6174 6820 643d 224d 2036      <path d="M 6
+00005d20: 2e35 3838 3833 3033 3065 2b30 3120 322e  .58883030e+01 2.
+00005d30: 3433 3730 3136 3930 652b 3031 2051 2036  43701690e+01 Q 6
+00005d40: 2e37 3633 3533 3332 3965 2b30 3120 322e  .76353329e+01 2.
+00005d50: 3330 3234 3539 3430 652b 3031 2c20 362e  30245940e+01, 6.
+00005d60: 3933 3133 3630 3234 652b 3031 2032 2e31  93136024e+01 2.1
+00005d70: 3930 3932 3837 3765 2b30 3120 5120 372e  9092877e+01 Q 7.
+00005d80: 3039 3839 3833 3934 652b 3031 2032 2e30  09898394e+01 2.0
+00005d90: 3739 3338 3032 3565 2b30 312c 2037 2e32  7938025e+01, 7.2
+00005da0: 3630 3131 3333 3065 2b30 3120 312e 3937  6011330e+01 1.97
+00005db0: 3030 3534 3630 652b 3031 2051 2036 2e39  005460e+01 Q 6.9
+00005dc0: 3939 3339 3331 3465 2b30 3120 312e 3836  9939314e+01 1.86
+00005dd0: 3932 3631 3131 652b 3031 2c20 362e 3733  926111e+01, 6.73
+00005de0: 3739 3938 3533 652b 3031 2031 2e37 3639  799853e+01 1.769
+00005df0: 3037 3037 3865 2b30 3120 5120 362e 3437  07078e+01 Q 6.47
+00005e00: 3736 3931 3339 652b 3031 2031 2e36 3639  769139e+01 1.669
+00005e10: 3331 3339 3965 2b30 312c 2036 2e32 3231  31399e+01, 6.221
+00005e20: 3836 3433 3065 2b30 3120 312e 3537 3433  86430e+01 1.5743
+00005e30: 3035 3730 652b 3031 2051 2036 2e33 3132  0570e+01 Q 6.312
+00005e40: 3038 3437 3865 2b30 3120 312e 3738 3130  08478e+01 1.7810
+00005e50: 3932 3734 652b 3031 2c20 362e 3430 3637  9274e+01, 6.4067
+00005e60: 3133 3634 652b 3031 2031 2e39 3837 3337  1364e+01 1.98737
+00005e70: 3735 3665 2b30 3120 5120 362e 3530 3039  756e+01 Q 6.5009
+00005e80: 3939 3637 652b 3031 2032 2e31 3931 3836  9967e+01 2.19186
+00005e90: 3636 3665 2b30 312c 2036 2e35 3838 3833  666e+01, 6.58883
+00005ea0: 3033 3065 2b30 3120 322e 3433 3730 3136  030e+01 2.437016
+00005eb0: 3930 652b 3031 205a 2220 2f3e 0d0a 2020  90e+01 Z" />..  
+00005ec0: 2020 2020 3c70 6174 6820 643d 224d 2036      <path d="M 6
+00005ed0: 2e35 3838 3833 3033 3065 2b30 3120 322e  .58883030e+01 2.
+00005ee0: 3433 3730 3136 3930 652b 3031 2051 2036  43701690e+01 Q 6
+00005ef0: 2e37 3438 3735 3833 3665 2b30 3120 322e  .74875836e+01 2.
+00005f00: 3530 3330 3339 3438 652b 3031 2c20 362e  50303948e+01, 6.
+00005f10: 3839 3731 3634 3630 652b 3031 2032 2e36  89716460e+01 2.6
+00005f20: 3031 3434 3636 3865 2b30 3120 5120 372e  0144668e+01 Q 7.
+00005f30: 3034 3534 3937 3530 652b 3031 2032 2e37  04549750e+01 2.7
+00005f40: 3030 3039 3737 3765 2b30 312c 2037 2e31  0009777e+01, 7.1
+00005f50: 3732 3739 3236 3065 2b30 3120 322e 3832  7279260e+01 2.82
+00005f60: 3732 3038 3330 652b 3031 2051 2037 2e32  720830e+01 Q 7.2
+00005f70: 3039 3435 3236 3565 2b30 3120 322e 3539  0945265e+01 2.59
+00005f80: 3238 3037 3030 652b 3031 2c20 372e 3232  280700e+01, 7.22
+00005f90: 3532 3937 3535 652b 3031 2032 2e33 3833  529755e+01 2.383
+00005fa0: 3336 3634 3265 2b30 3120 5120 372e 3234  36642e+01 Q 7.24
+00005fb0: 3134 3733 3532 652b 3031 2032 2e31 3733  147352e+01 2.173
+00005fc0: 3635 3032 3365 2b30 312c 2037 2e32 3630  65023e+01, 7.260
+00005fd0: 3131 3333 3065 2b30 3120 312e 3937 3030  11330e+01 1.9700
+00005fe0: 3534 3630 652b 3031 2051 2037 2e30 3938  5460e+01 Q 7.098
+00005ff0: 3938 3339 3465 2b30 3120 322e 3037 3933  98394e+01 2.0793
+00006000: 3830 3235 652b 3031 2c20 362e 3933 3133  8025e+01, 6.9313
+00006010: 3630 3234 652b 3031 2032 2e31 3930 3932  6024e+01 2.19092
+00006020: 3837 3765 2b30 3120 5120 362e 3736 3335  877e+01 Q 6.7635
+00006030: 3333 3239 652b 3031 2032 2e33 3032 3435  3329e+01 2.30245
+00006040: 3934 3065 2b30 312c 2036 2e35 3838 3833  940e+01, 6.58883
+00006050: 3033 3065 2b30 3120 322e 3433 3730 3136  030e+01 2.437016
+00006060: 3930 652b 3031 205a 2220 2f3e 0d0a 2020  90e+01 Z" />..  
+00006070: 2020 2020 3c70 6174 6820 643d 224d 2037      <path d="M 7
+00006080: 2e35 3632 3938 3331 3065 2b30 3120 342e  .56298310e+01 4.
+00006090: 3738 3838 3330 3330 652b 3031 2051 2037  78883030e+01 Q 7
+000060a0: 2e37 3237 3330 3035 3365 2b30 3120 352e  .72730053e+01 5.
+000060b0: 3033 3034 3632 3734 652b 3031 2c20 372e  03046274e+01, 7.
+000060c0: 3836 3039 3631 3737 652b 3031 2035 2e32  86096177e+01 5.2
+000060d0: 3630 3238 3132 3265 2b30 3120 5120 372e  6028122e+01 Q 7.
+000060e0: 3939 3434 3439 3635 652b 3031 2035 2e34  99444965e+01 5.4
+000060f0: 3839 3431 3133 3865 2b30 312c 2038 2e31  8941138e+01, 8.1
+00006100: 3239 3738 3639 3065 2b30 3120 352e 3731  2978690e+01 5.71
+00006110: 3136 3634 3230 652b 3031 2051 2038 2e31  166420e+01 Q 8.1
+00006120: 3630 3838 3836 3265 2b30 3120 352e 3435  6088862e+01 5.45
+00006130: 3135 3230 3930 652b 3031 2c20 382e 3139  152090e+01, 8.19
+00006140: 3134 3633 3737 652b 3031 2035 2e31 3836  146377e+01 5.186
+00006150: 3438 3537 3765 2b30 3120 5120 382e 3232  48577e+01 Q 8.22
+00006160: 3230 3432 3430 652b 3031 2034 2e39 3231  204240e+01 4.921
+00006170: 3431 3730 3865 2b30 312c 2038 2e32 3532  41708e+01, 8.252
+00006180: 3931 3935 3065 2b30 3120 342e 3635 3939  91950e+01 4.6599
+00006190: 3835 3430 652b 3031 2051 2038 2e30 3838  8540e+01 Q 8.088
+000061a0: 3832 3338 3965 2b30 3120 342e 3639 3333  82389e+01 4.6933
+000061b0: 3533 3030 652b 3031 2c20 372e 3932 3035  5300e+01, 7.9205
+000061c0: 3933 3835 652b 3031 2034 2e37 3237 3736  9385e+01 4.72776
+000061d0: 3635 3165 2b30 3120 5120 372e 3735 3332  651e+01 Q 7.7532
+000061e0: 3932 3035 652b 3031 2034 2e37 3632 3134  9205e+01 4.76214
+000061f0: 3736 3365 2b30 312c 2037 2e35 3632 3938  763e+01, 7.56298
+00006200: 3331 3065 2b30 3120 342e 3738 3838 3330  310e+01 4.788830
+00006210: 3330 652b 3031 205a 2220 2f3e 0d0a 2020  30e+01 Z" />..  
+00006220: 2020 2020 3c70 6174 6820 643d 224d 2037      <path d="M 7
+00006230: 2e31 3732 3739 3137 3065 2b30 3120 352e  .17279170e+01 5.
+00006240: 3337 3237 3932 3630 652b 3031 2051 2037  37279260e+01 Q 7
+00006250: 2e32 3033 3034 3536 3065 2b30 3120 352e  .20304560e+01 5.
+00006260: 3536 3139 3733 3938 652b 3031 2c20 372e  56197398e+01, 7.
+00006270: 3231 3532 3837 3135 652b 3031 2035 2e37  21528715e+01 5.7
+00006280: 3333 3039 3734 3865 2b30 3120 5120 372e  3309748e+01 Q 7.
+00006290: 3232 3737 3334 3335 652b 3031 2035 2e39  22773435e+01 5.9
+000062a0: 3034 3430 3535 3765 2b30 312c 2037 2e32  0440557e+01, 7.2
+000062b0: 3430 3439 3135 3065 2b30 3120 362e 3037  4049150e+01 6.07
+000062c0: 3030 3534 3130 652b 3031 2051 2037 2e34  005410e+01 Q 7.4
+000062d0: 3634 3431 3734 3265 2b30 3120 352e 3937  6441742e+01 5.97
+000062e0: 3930 3837 3938 652b 3031 2c20 372e 3638  908798e+01, 7.68
+000062f0: 3739 3036 3133 652b 3031 2035 2e38 3839  790613e+01 5.889
+00006300: 3536 3032 3265 2b30 3120 5120 372e 3931  56022e+01 Q 7.91
+00006310: 3130 3332 3830 652b 3031 2035 2e38 3030  103280e+01 5.800
+00006320: 3137 3039 3965 2b30 312c 2038 2e31 3239  17099e+01, 8.129
+00006330: 3738 3639 3065 2b30 3120 352e 3731 3136  78690e+01 5.7116
+00006340: 3634 3230 652b 3031 2051 2037 2e39 3030  6420e+01 Q 7.900
+00006350: 3732 3134 3165 2b30 3120 352e 3633 3131  72141e+01 5.6311
+00006360: 3739 3439 652b 3031 2c20 372e 3636 3734  7949e+01, 7.6674
+00006370: 3139 3331 652b 3031 2035 2e35 3532 3338  1931e+01 5.55238
+00006380: 3332 3165 2b30 3120 5120 372e 3433 3534  321e+01 Q 7.4354
+00006390: 3036 3331 652b 3031 2035 2e34 3734 3237  0631e+01 5.47427
+000063a0: 3830 3565 2b30 312c 2037 2e31 3732 3739  805e+01, 7.17279
+000063b0: 3137 3065 2b30 3120 352e 3337 3237 3932  170e+01 5.372792
+000063c0: 3630 652b 3031 205a 2220 2f3e 0d0a 2020  60e+01 Z" />..  
+000063d0: 2020 2020 3c70 6174 6820 643d 224d 2037      <path d="M 7
+000063e0: 2e35 3632 3938 3331 3065 2b30 3120 342e  .56298310e+01 4.
+000063f0: 3738 3838 3330 3330 652b 3031 2051 2037  78883030e+01 Q 7
+00006400: 2e34 3936 3936 3035 3265 2b30 3120 342e  .49696052e+01 4.
+00006410: 3934 3837 3538 3336 652b 3031 2c20 372e  94875836e+01, 7.
+00006420: 3339 3835 3533 3332 652b 3031 2035 2e30  39855332e+01 5.0
+00006430: 3937 3136 3436 3065 2b30 3120 5120 372e  9716460e+01 Q 7.
+00006440: 3239 3939 3032 3233 652b 3031 2035 2e32  29990223e+01 5.2
+00006450: 3435 3439 3735 3065 2b30 312c 2037 2e31  4549750e+01, 7.1
+00006460: 3732 3739 3137 3065 2b30 3120 352e 3337  7279170e+01 5.37
+00006470: 3237 3932 3630 652b 3031 2051 2037 2e34  279260e+01 Q 7.4
+00006480: 3335 3430 3633 3165 2b30 3120 352e 3437  3540631e+01 5.47
+00006490: 3432 3738 3035 652b 3031 2c20 372e 3636  427805e+01, 7.66
+000064a0: 3734 3139 3331 652b 3031 2035 2e35 3532  741931e+01 5.552
+000064b0: 3338 3332 3165 2b30 3120 5120 372e 3930  38321e+01 Q 7.90
+000064c0: 3037 3231 3431 652b 3031 2035 2e36 3331  072141e+01 5.631
+000064d0: 3137 3934 3965 2b30 312c 2038 2e31 3239  17949e+01, 8.129
+000064e0: 3738 3639 3065 2b30 3120 352e 3731 3136  78690e+01 5.7116
+000064f0: 3634 3230 652b 3031 2051 2037 2e39 3934  6420e+01 Q 7.994
+00006500: 3434 3936 3565 2b30 3120 352e 3438 3934  44965e+01 5.4894
+00006510: 3131 3338 652b 3031 2c20 372e 3836 3039  1138e+01, 7.8609
+00006520: 3631 3737 652b 3031 2035 2e32 3630 3238  6177e+01 5.26028
+00006530: 3132 3265 2b30 3120 5120 372e 3732 3733  122e+01 Q 7.7273
+00006540: 3030 3533 652b 3031 2035 2e30 3330 3436  0053e+01 5.03046
+00006550: 3237 3465 2b30 312c 2037 2e35 3632 3938  274e+01, 7.56298
+00006560: 3331 3065 2b30 3120 342e 3738 3838 3330  310e+01 4.788830
+00006570: 3330 652b 3031 205a 2220 2f3e 0d0a 2020  30e+01 Z" />..  
+00006580: 2020 2020 3c70 6174 6820 643d 224d 2037      <path d="M 7
+00006590: 2e32 3430 3439 3135 3065 2b30 3120 362e  .24049150e+01 6.
+000065a0: 3037 3030 3534 3130 652b 3031 2051 2037  07005410e+01 Q 7
+000065b0: 2e30 3834 3939 3233 3465 2b30 3120 352e  .08499234e+01 5.
+000065c0: 3939 3935 3239 3038 652b 3031 2c20 362e  99952908e+01, 6.
+000065d0: 3932 3231 3033 3737 652b 3031 2035 2e39  92210377e+01 5.9
+000065e0: 3238 3431 3833 3365 2b30 3120 5120 362e  2841833e+01 Q 6.
+000065f0: 3735 3836 3932 3235 652b 3031 2035 2e38  75869225e+01 5.8
+00006600: 3537 3134 3431 3065 2b30 312c 2036 2e35  5714410e+01, 6.5
+00006610: 3838 3833 3033 3065 2b30 3120 352e 3736  8883030e+01 5.76
+00006620: 3239 3833 3130 652b 3031 2051 2036 2e36  298310e+01 Q 6.6
+00006630: 3031 3236 3331 3565 2b30 3120 352e 3939  0126315e+01 5.99
+00006640: 3132 3338 3439 652b 3031 2c20 362e 3630  123849e+01, 6.60
+00006650: 3136 3731 3938 652b 3031 2036 2e31 3934  167198e+01 6.194
+00006660: 3938 3336 3765 2b30 3120 5120 362e 3630  98367e+01 Q 6.60
+00006670: 3232 3135 3436 652b 3031 2036 2e34 3030  221546e+01 6.400
+00006680: 3536 3830 3765 2b30 312c 2036 2e36 3030  56807e+01, 6.600
+00006690: 3938 3735 3065 2b30 3120 362e 3630 3338  98750e+01 6.6038
+000066a0: 3136 3230 652b 3031 204c 2037 2e32 3430  1620e+01 L 7.240
+000066b0: 3439 3135 3065 2b30 3120 362e 3037 3030  49150e+01 6.0700
+000066c0: 3534 3130 652b 3031 205a 2220 2f3e 0d0a  5410e+01 Z" />..
+000066d0: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
+000066e0: 2037 2e31 3732 3739 3137 3065 2b30 3120   7.17279170e+01 
+000066f0: 352e 3337 3237 3932 3630 652b 3031 2051  5.37279260e+01 Q
+00006700: 2037 2e30 3435 3439 3732 3565 2b30 3120   7.04549725e+01 
+00006710: 352e 3439 3939 3032 3438 652b 3031 2c20  5.49990248e+01, 
+00006720: 362e 3839 3731 3634 3439 652b 3031 2035  6.89716449e+01 5
+00006730: 2e35 3938 3535 3334 3465 2b30 3120 5120  .59855344e+01 Q 
+00006740: 362e 3734 3837 3538 3339 652b 3031 2035  6.74875839e+01 5
+00006750: 2e36 3936 3936 3034 3965 2b30 312c 2036  .69696049e+01, 6
+00006760: 2e35 3838 3833 3033 3065 2b30 3120 352e  .58883030e+01 5.
+00006770: 3736 3239 3833 3130 652b 3031 2051 2036  76298310e+01 Q 6
+00006780: 2e37 3538 3639 3232 3565 2b30 3120 352e  .75869225e+01 5.
+00006790: 3835 3731 3434 3130 652b 3031 2c20 362e  85714410e+01, 6.
+000067a0: 3932 3231 3033 3737 652b 3031 2035 2e39  92210377e+01 5.9
+000067b0: 3238 3431 3833 3365 2b30 3120 5120 372e  2841833e+01 Q 7.
+000067c0: 3038 3439 3932 3334 652b 3031 2035 2e39  08499234e+01 5.9
+000067d0: 3939 3532 3930 3865 2b30 312c 2037 2e32  9952908e+01, 7.2
+000067e0: 3430 3439 3135 3065 2b30 3120 362e 3037  4049150e+01 6.07
+000067f0: 3030 3534 3130 652b 3031 2051 2037 2e32  005410e+01 Q 7.2
+00006800: 3237 3733 3433 3565 2b30 3120 352e 3930  2773435e+01 5.90
+00006810: 3434 3035 3537 652b 3031 2c20 372e 3231  440557e+01, 7.21
+00006820: 3532 3837 3135 652b 3031 2035 2e37 3333  528715e+01 5.733
+00006830: 3039 3734 3865 2b30 3120 5120 372e 3230  09748e+01 Q 7.20
+00006840: 3330 3435 3630 652b 3031 2035 2e35 3631  304560e+01 5.561
+00006850: 3937 3339 3865 2b30 312c 2037 2e31 3732  97398e+01, 7.172
+00006860: 3739 3137 3065 2b30 3120 352e 3337 3237  79170e+01 5.3727
+00006870: 3932 3630 652b 3031 205a 2220 2f3e 0d0a  9260e+01 Z" />..
+00006880: 2020 203c 2f67 3e0d 0a20 2020 3c67 2069     </g>..   <g i
+00006890: 643d 224e 6f64 6573 2220 6669 6c6c 3d22  d="Nodes" fill="
+000068a0: 2361 3935 6535 6522 3e0d 0a20 2020 2020  #a95e5e">..     
+000068b0: 203c 6369 7263 6c65 2063 783d 2238 2e37   <circle cx="8.7
+000068c0: 3530 3030 3033 3065 2b30 3122 2063 793d  5000030e+01" cy=
+000068d0: 2235 2e30 3030 3030 3030 3065 2b30 3022  "5.00000000e+00"
+000068e0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+000068f0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+00006900: 2020 3c63 6972 636c 6520 6378 3d22 372e    <circle cx="7.
+00006910: 3939 3939 3939 3730 652b 3031 2220 6379  99999970e+01" cy
+00006920: 3d22 352e 3030 3030 3030 3030 652b 3030  ="5.00000000e+00
+00006930: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+00006940: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+00006950: 2020 203c 6369 7263 6c65 2063 783d 2237     <circle cx="7
+00006960: 2e32 3530 3030 3030 3065 2b30 3122 2063  .25000000e+01" c
+00006970: 793d 2235 2e30 3030 3030 3030 3065 2b30  y="5.00000000e+0
+00006980: 3022 2072 3d22 302e 3533 3638 3130 3436  0" r="0.53681046
+00006990: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+000069a0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+000069b0: 362e 3530 3030 3030 3330 652b 3031 2220  6.50000030e+01" 
+000069c0: 6379 3d22 352e 3030 3030 3030 3030 652b  cy="5.00000000e+
+000069d0: 3030 2220 723d 2230 2e35 3336 3831 3034  00" r="0.5368104
+000069e0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+000069f0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00006a00: 2235 2e37 3530 3030 3135 3065 2b30 3122  "5.75000150e+01"
+00006a10: 2063 793d 2235 2e30 3030 3030 3030 3065   cy="5.00000000e
+00006a20: 2b30 3022 2072 3d22 302e 3533 3638 3130  +00" r="0.536810
+00006a30: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+00006a40: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+00006a50: 3d22 352e 3030 3030 3031 3830 652b 3031  ="5.00000180e+01
+00006a60: 2220 6379 3d22 352e 3030 3030 3030 3030  " cy="5.00000000
+00006a70: 652b 3030 2220 723d 2230 2e35 3336 3831  e+00" r="0.53681
+00006a80: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+00006a90: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+00006aa0: 783d 2234 2e32 3530 3030 3231 3065 2b30  x="4.25000210e+0
+00006ab0: 3122 2063 793d 2235 2e30 3030 3030 3030  1" cy="5.0000000
+00006ac0: 3065 2b30 3022 2072 3d22 302e 3533 3638  0e+00" r="0.5368
+00006ad0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+00006ae0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+00006af0: 6378 3d22 332e 3530 3030 3031 3530 652b  cx="3.50000150e+
+00006b00: 3031 2220 6379 3d22 352e 3030 3030 3030  01" cy="5.000000
+00006b10: 3030 652b 3030 2220 723d 2230 2e35 3336  00e+00" r="0.536
+00006b20: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+00006b30: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+00006b40: 2063 783d 2232 2e37 3530 3030 3039 3065   cx="2.75000090e
+00006b50: 2b30 3122 2063 793d 2235 2e30 3030 3030  +01" cy="5.00000
+00006b60: 3030 3065 2b30 3022 2072 3d22 302e 3533  000e+00" r="0.53
+00006b70: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+00006b80: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+00006b90: 6520 6378 3d22 322e 3030 3030 3030 3330  e cx="2.00000030
+00006ba0: 652b 3031 2220 6379 3d22 352e 3030 3030  e+01" cy="5.0000
+00006bb0: 3030 3030 652b 3030 2220 723d 2230 2e35  0000e+00" r="0.5
+00006bc0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+00006bd0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+00006be0: 6c65 2063 783d 2231 2e32 3530 3030 3033  le cx="1.2500003
+00006bf0: 3365 2b30 3122 2063 793d 2235 2e30 3030  3e+01" cy="5.000
+00006c00: 3030 3030 3065 2b30 3022 2072 3d22 302e  00000e+00" r="0.
+00006c10: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+00006c20: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+00006c30: 636c 6520 6378 3d22 342e 3333 3233 3134  cle cx="4.332314
+00006c40: 3330 652b 3031 2220 6379 3d22 372e 3730  30e+01" cy="7.70
+00006c50: 3030 3030 3030 652b 3031 2220 723d 2230  000000e+01" r="0
+00006c60: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+00006c70: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+00006c80: 7263 6c65 2063 783d 2234 2e35 3635 3335  rcle cx="4.56535
+00006c90: 3736 3065 2b30 3122 2063 793d 2237 2e36  760e+01" cy="7.6
+00006ca0: 3535 3534 3831 3065 2b30 3122 2072 3d22  5554810e+01" r="
+00006cb0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+00006cc0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+00006cd0: 6972 636c 6520 6378 3d22 342e 3738 3838  ircle cx="4.7888
+00006ce0: 3330 3330 652b 3031 2220 6379 3d22 372e  3030e+01" cy="7.
+00006cf0: 3536 3239 3833 3130 652b 3031 2220 723d  56298310e+01" r=
+00006d00: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+00006d10: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+00006d20: 6369 7263 6c65 2063 783d 2235 2e30 3036  circle cx="5.006
+00006d30: 3438 3435 3065 2b30 3122 2063 793d 2237  48450e+01" cy="7
+00006d40: 2e34 3732 3832 3734 3065 2b30 3122 2072  .47282740e+01" r
+00006d50: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+00006d60: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+00006d70: 3c63 6972 636c 6520 6378 3d22 352e 3230  <circle cx="5.20
+00006d80: 3430 3039 3330 652b 3031 2220 6379 3d22  400930e+01" cy="
+00006d90: 372e 3334 3135 3735 3030 652b 3031 2220  7.34157500e+01" 
+00006da0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+00006db0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+00006dc0: 203c 6369 7263 6c65 2063 783d 2235 2e33   <circle cx="5.3
+00006dd0: 3732 3739 3137 3065 2b30 3122 2063 793d  7279170e+01" cy=
+00006de0: 2237 2e31 3732 3739 3236 3065 2b30 3122  "7.17279260e+01"
+00006df0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+00006e00: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+00006e10: 2020 3c63 6972 636c 6520 6378 3d22 352e    <circle cx="5.
+00006e20: 3534 3135 3735 3030 652b 3031 2220 6379  54157500e+01" cy
+00006e30: 3d22 372e 3030 3430 3039 3330 652b 3031  ="7.00400930e+01
+00006e40: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+00006e50: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+00006e60: 2020 203c 6369 7263 6c65 2063 783d 2235     <circle cx="5
+00006e70: 2e36 3732 3832 3734 3065 2b30 3122 2063  .67282740e+01" c
+00006e80: 793d 2236 2e38 3036 3438 3435 3065 2b30  y="6.80648450e+0
+00006e90: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+00006ea0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+00006eb0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+00006ec0: 352e 3736 3239 3833 3130 652b 3031 2220  5.76298310e+01" 
+00006ed0: 6379 3d22 362e 3538 3838 3330 3330 652b  cy="6.58883030e+
+00006ee0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+00006ef0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+00006f00: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00006f10: 2235 2e38 3535 3534 3831 3065 2b30 3122  "5.85554810e+01"
+00006f20: 2063 793d 2236 2e33 3635 3335 3736 3065   cy="6.36535760e
+00006f30: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+00006f40: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+00006f50: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+00006f60: 3d22 352e 3930 3030 3030 3030 652b 3031  ="5.90000000e+01
+00006f70: 2220 6379 3d22 362e 3133 3233 3134 3330  " cy="6.13231430
+00006f80: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+00006f90: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+00006fa0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+00006fb0: 783d 2239 2e35 3030 3030 3030 3065 2b30  x="9.50000000e+0
+00006fc0: 3122 2063 793d 2238 2e37 3530 3030 3030  1" cy="8.7500000
+00006fd0: 3365 2b30 3122 2072 3d22 302e 3533 3638  3e+01" r="0.5368
+00006fe0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+00006ff0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+00007000: 6378 3d22 392e 3530 3030 3030 3030 652b  cx="9.50000000e+
+00007010: 3031 2220 6379 3d22 372e 3939 3939 3939  01" cy="7.999999
+00007020: 3730 652b 3031 2220 723d 2230 2e35 3336  70e+01" r="0.536
+00007030: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+00007040: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+00007050: 2063 783d 2239 2e35 3030 3030 3030 3065   cx="9.50000000e
+00007060: 2b30 3122 2063 793d 2237 2e32 3530 3030  +01" cy="7.25000
+00007070: 3030 3065 2b30 3122 2072 3d22 302e 3533  000e+01" r="0.53
+00007080: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+00007090: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+000070a0: 6520 6378 3d22 392e 3530 3030 3030 3030  e cx="9.50000000
+000070b0: 652b 3031 2220 6379 3d22 362e 3530 3030  e+01" cy="6.5000
+000070c0: 3030 3330 652b 3031 2220 723d 2230 2e35  0030e+01" r="0.5
+000070d0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+000070e0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+000070f0: 6c65 2063 783d 2239 2e35 3030 3030 3030  le cx="9.5000000
+00007100: 3065 2b30 3122 2063 793d 2235 2e37 3530  0e+01" cy="5.750
+00007110: 3030 3135 3065 2b30 3122 2072 3d22 302e  00150e+01" r="0.
+00007120: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+00007130: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+00007140: 636c 6520 6378 3d22 392e 3530 3030 3030  cle cx="9.500000
+00007150: 3030 652b 3031 2220 6379 3d22 352e 3030  00e+01" cy="5.00
+00007160: 3030 3031 3830 652b 3031 2220 723d 2230  000180e+01" r="0
+00007170: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+00007180: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+00007190: 7263 6c65 2063 783d 2239 2e35 3030 3030  rcle cx="9.50000
+000071a0: 3030 3065 2b30 3122 2063 793d 2234 2e32  000e+01" cy="4.2
+000071b0: 3530 3030 3231 3065 2b30 3122 2072 3d22  5000210e+01" r="
+000071c0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+000071d0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+000071e0: 6972 636c 6520 6378 3d22 392e 3530 3030  ircle cx="9.5000
+000071f0: 3030 3030 652b 3031 2220 6379 3d22 332e  0000e+01" cy="3.
+00007200: 3530 3030 3031 3530 652b 3031 2220 723d  50000150e+01" r=
+00007210: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+00007220: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+00007230: 6369 7263 6c65 2063 783d 2239 2e35 3030  circle cx="9.500
+00007240: 3030 3030 3065 2b30 3122 2063 793d 2232  00000e+01" cy="2
+00007250: 2e37 3530 3030 3039 3065 2b30 3122 2072  .75000090e+01" r
+00007260: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+00007270: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+00007280: 3c63 6972 636c 6520 6378 3d22 392e 3530  <circle cx="9.50
+00007290: 3030 3030 3030 652b 3031 2220 6379 3d22  000000e+01" cy="
+000072a0: 322e 3030 3030 3030 3330 652b 3031 2220  2.00000030e+01" 
+000072b0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+000072c0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+000072d0: 203c 6369 7263 6c65 2063 783d 2239 2e35   <circle cx="9.5
+000072e0: 3030 3030 3030 3065 2b30 3122 2063 793d  0000000e+01" cy=
+000072f0: 2231 2e32 3530 3030 3036 3065 2b30 3122  "1.25000060e+01"
+00007300: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+00007310: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+00007320: 2020 3c63 6972 636c 6520 6378 3d22 322e    <circle cx="2.
+00007330: 3330 3030 3030 3030 652b 3031 2220 6379  30000000e+01" cy
+00007340: 3d22 362e 3133 3233 3134 3330 652b 3031  ="6.13231430e+01
+00007350: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+00007360: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+00007370: 2020 203c 6369 7263 6c65 2063 783d 2232     <circle cx="2
+00007380: 2e33 3434 3435 3139 3065 2b30 3122 2063  .34445190e+01" c
+00007390: 793d 2236 2e33 3635 3335 3736 3065 2b30  y="6.36535760e+0
+000073a0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+000073b0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+000073c0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+000073d0: 322e 3433 3730 3136 3930 652b 3031 2220  2.43701690e+01" 
+000073e0: 6379 3d22 362e 3538 3838 3330 3330 652b  cy="6.58883030e+
+000073f0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+00007400: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+00007410: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00007420: 2232 2e35 3237 3137 3236 3065 2b30 3122  "2.52717260e+01"
+00007430: 2063 793d 2236 2e38 3036 3438 3435 3065   cy="6.80648450e
+00007440: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+00007450: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+00007460: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+00007470: 3d22 322e 3635 3834 3235 3030 652b 3031  ="2.65842500e+01
+00007480: 2220 6379 3d22 372e 3030 3430 3039 3330  " cy="7.00400930
+00007490: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+000074a0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+000074b0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+000074c0: 783d 2232 2e38 3237 3230 3734 3065 2b30  x="2.82720740e+0
+000074d0: 3122 2063 793d 2237 2e31 3732 3739 3137  1" cy="7.1727917
+000074e0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+000074f0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+00007500: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+00007510: 6378 3d22 322e 3939 3539 3930 3730 652b  cx="2.99599070e+
+00007520: 3031 2220 6379 3d22 372e 3334 3135 3735  01" cy="7.341575
+00007530: 3030 652b 3031 2220 723d 2230 2e35 3336  00e+01" r="0.536
+00007540: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+00007550: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+00007560: 2063 783d 2233 2e31 3933 3531 3535 3065   cx="3.19351550e
+00007570: 2b30 3122 2063 793d 2237 2e34 3732 3832  +01" cy="7.47282
+00007580: 3734 3065 2b30 3122 2072 3d22 302e 3533  740e+01" r="0.53
+00007590: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+000075a0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+000075b0: 6520 6378 3d22 332e 3431 3131 3639 3730  e cx="3.41116970
+000075c0: 652b 3031 2220 6379 3d22 372e 3536 3239  e+01" cy="7.5629
+000075d0: 3833 3130 652b 3031 2220 723d 2230 2e35  8310e+01" r="0.5
+000075e0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+000075f0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+00007600: 6c65 2063 783d 2233 2e36 3334 3634 3234  le cx="3.6346424
+00007610: 3065 2b30 3122 2063 793d 2237 2e36 3535  0e+01" cy="7.655
+00007620: 3534 3831 3065 2b30 3122 2072 3d22 302e  54810e+01" r="0.
+00007630: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+00007640: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+00007650: 636c 6520 6378 3d22 332e 3836 3736 3835  cle cx="3.867685
+00007660: 3730 652b 3031 2220 6379 3d22 372e 3730  70e+01" cy="7.70
+00007670: 3030 3030 3030 652b 3031 2220 723d 2230  000000e+01" r="0
+00007680: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+00007690: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+000076a0: 7263 6c65 2063 783d 2231 2e32 3439 3939  rcle cx="1.24999
+000076b0: 3939 3765 2b30 3122 2063 793d 2239 2e35  997e+01" cy="9.5
+000076c0: 3030 3030 3030 3065 2b30 3122 2072 3d22  0000000e+01" r="
+000076d0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+000076e0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+000076f0: 6972 636c 6520 6378 3d22 322e 3030 3030  ircle cx="2.0000
+00007700: 3030 3330 652b 3031 2220 6379 3d22 392e  0030e+01" cy="9.
+00007710: 3530 3030 3030 3030 652b 3031 2220 723d  50000000e+01" r=
+00007720: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+00007730: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+00007740: 6369 7263 6c65 2063 783d 2232 2e37 3530  circle cx="2.750
+00007750: 3030 3030 3065 2b30 3122 2063 793d 2239  00000e+01" cy="9
+00007760: 2e35 3030 3030 3030 3065 2b30 3122 2072  .50000000e+01" r
+00007770: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+00007780: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+00007790: 3c63 6972 636c 6520 6378 3d22 332e 3439  <circle cx="3.49
+000077a0: 3939 3939 3730 652b 3031 2220 6379 3d22  999970e+01" cy="
+000077b0: 392e 3530 3030 3030 3030 652b 3031 2220  9.50000000e+01" 
+000077c0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+000077d0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+000077e0: 203c 6369 7263 6c65 2063 783d 2234 2e32   <circle cx="4.2
+000077f0: 3439 3939 3835 3065 2b30 3122 2063 793d  4999850e+01" cy=
+00007800: 2239 2e35 3030 3030 3030 3065 2b30 3122  "9.50000000e+01"
+00007810: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+00007820: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+00007830: 2020 3c63 6972 636c 6520 6378 3d22 342e    <circle cx="4.
+00007840: 3939 3939 3938 3230 652b 3031 2220 6379  99999820e+01" cy
+00007850: 3d22 392e 3530 3030 3030 3030 652b 3031  ="9.50000000e+01
+00007860: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+00007870: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+00007880: 2020 203c 6369 7263 6c65 2063 783d 2235     <circle cx="5
+00007890: 2e37 3439 3939 3739 3065 2b30 3122 2063  .74999790e+01" c
+000078a0: 793d 2239 2e35 3030 3030 3030 3065 2b30  y="9.50000000e+0
+000078b0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+000078c0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+000078d0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+000078e0: 362e 3439 3939 3938 3530 652b 3031 2220  6.49999850e+01" 
+000078f0: 6379 3d22 392e 3530 3030 3030 3030 652b  cy="9.50000000e+
+00007900: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+00007910: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+00007920: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00007930: 2237 2e32 3439 3939 3931 3065 2b30 3122  "7.24999910e+01"
+00007940: 2063 793d 2239 2e35 3030 3030 3030 3065   cy="9.50000000e
+00007950: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+00007960: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+00007970: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+00007980: 3d22 372e 3939 3939 3939 3730 652b 3031  ="7.99999970e+01
+00007990: 2220 6379 3d22 392e 3530 3030 3030 3030  " cy="9.50000000
+000079a0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+000079b0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+000079c0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+000079d0: 783d 2238 2e37 3439 3939 3934 3065 2b30  x="8.74999940e+0
+000079e0: 3122 2063 793d 2239 2e35 3030 3030 3030  1" cy="9.5000000
+000079f0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+00007a00: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+00007a10: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+00007a20: 6378 3d22 322e 3330 3030 3030 3030 652b  cx="2.30000000e+
+00007a30: 3031 2220 6379 3d22 322e 3539 3939 3939  01" cy="2.599999
+00007a40: 3730 652b 3031 2220 723d 2230 2e35 3336  70e+01" r="0.536
+00007a50: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+00007a60: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+00007a70: 2063 783d 2232 2e33 3030 3030 3030 3065   cx="2.30000000e
+00007a80: 2b30 3122 2063 793d 2232 2e39 3030 3030  +01" cy="2.90000
+00007a90: 3033 3065 2b30 3122 2072 3d22 302e 3533  030e+01" r="0.53
+00007aa0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+00007ab0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+00007ac0: 6520 6378 3d22 322e 3330 3030 3030 3030  e cx="2.30000000
+00007ad0: 652b 3031 2220 6379 3d22 332e 3230 3030  e+01" cy="3.2000
+00007ae0: 3030 3030 652b 3031 2220 723d 2230 2e35  0000e+01" r="0.5
+00007af0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+00007b00: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+00007b10: 6c65 2063 783d 2232 2e33 3030 3030 3030  le cx="2.3000000
+00007b20: 3065 2b30 3122 2063 793d 2233 2e34 3939  0e+01" cy="3.499
+00007b30: 3939 3937 3065 2b30 3122 2072 3d22 302e  99970e+01" r="0.
+00007b40: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+00007b50: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+00007b60: 636c 6520 6378 3d22 322e 3330 3030 3030  cle cx="2.300000
+00007b70: 3030 652b 3031 2220 6379 3d22 332e 3739  00e+01" cy="3.79
+00007b80: 3939 3939 3430 652b 3031 2220 723d 2230  999940e+01" r="0
+00007b90: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+00007ba0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+00007bb0: 7263 6c65 2063 783d 2232 2e33 3030 3030  rcle cx="2.30000
+00007bc0: 3030 3065 2b30 3122 2063 793d 2234 2e30  000e+01" cy="4.0
+00007bd0: 3939 3939 3931 3065 2b30 3122 2072 3d22  9999910e+01" r="
+00007be0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+00007bf0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+00007c00: 6972 636c 6520 6378 3d22 322e 3330 3030  ircle cx="2.3000
+00007c10: 3030 3030 652b 3031 2220 6379 3d22 342e  0000e+01" cy="4.
+00007c20: 3339 3939 3939 3730 652b 3031 2220 723d  39999970e+01" r=
+00007c30: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+00007c40: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+00007c50: 6369 7263 6c65 2063 783d 2232 2e33 3030  circle cx="2.300
+00007c60: 3030 3030 3065 2b30 3122 2063 793d 2234  00000e+01" cy="4
+00007c70: 2e36 3939 3939 3934 3065 2b30 3122 2072  .69999940e+01" r
+00007c80: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+00007c90: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+00007ca0: 3c63 6972 636c 6520 6378 3d22 322e 3330  <circle cx="2.30
+00007cb0: 3030 3030 3030 652b 3031 2220 6379 3d22  000000e+01" cy="
+00007cc0: 352e 3030 3030 3030 3030 652b 3031 2220  5.00000000e+01" 
+00007cd0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+00007ce0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+00007cf0: 203c 6369 7263 6c65 2063 783d 2232 2e33   <circle cx="2.3
+00007d00: 3030 3030 3030 3065 2b30 3122 2063 793d  0000000e+01" cy=
+00007d10: 2235 2e32 3939 3939 3937 3065 2b30 3122  "5.29999970e+01"
+00007d20: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+00007d30: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+00007d40: 2020 3c63 6972 636c 6520 6378 3d22 322e    <circle cx="2.
+00007d50: 3330 3030 3030 3030 652b 3031 2220 6379  30000000e+01" cy
+00007d60: 3d22 352e 3630 3030 3030 3330 652b 3031  ="5.60000030e+01
+00007d70: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+00007d80: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+00007d90: 2020 203c 6369 7263 6c65 2063 783d 2235     <circle cx="5
+00007da0: 2e30 3030 3030 3030 3065 2b30 3022 2063  .00000000e+00" c
+00007db0: 793d 2231 2e32 3439 3939 3937 3065 2b30  y="1.24999970e+0
+00007dc0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+00007dd0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+00007de0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+00007df0: 352e 3030 3030 3030 3030 652b 3030 2220  5.00000000e+00" 
+00007e00: 6379 3d22 322e 3030 3030 3030 3330 652b  cy="2.00000030e+
+00007e10: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+00007e20: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+00007e30: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00007e40: 2235 2e30 3030 3030 3030 3065 2b30 3022  "5.00000000e+00"
+00007e50: 2063 793d 2232 2e37 3530 3030 3030 3065   cy="2.75000000e
+00007e60: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+00007e70: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+00007e80: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+00007e90: 3d22 352e 3030 3030 3030 3030 652b 3030  ="5.00000000e+00
+00007ea0: 2220 6379 3d22 332e 3439 3939 3939 3730  " cy="3.49999970
+00007eb0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+00007ec0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+00007ed0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+00007ee0: 783d 2235 2e30 3030 3030 3030 3065 2b30  x="5.00000000e+0
+00007ef0: 3022 2063 793d 2234 2e32 3439 3939 3835  0" cy="4.2499985
+00007f00: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+00007f10: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+00007f20: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+00007f30: 6378 3d22 352e 3030 3030 3030 3030 652b  cx="5.00000000e+
+00007f40: 3030 2220 6379 3d22 342e 3939 3939 3938  00" cy="4.999998
+00007f50: 3230 652b 3031 2220 723d 2230 2e35 3336  20e+01" r="0.536
+00007f60: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+00007f70: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+00007f80: 2063 783d 2235 2e30 3030 3030 3030 3065   cx="5.00000000e
+00007f90: 2b30 3022 2063 793d 2235 2e37 3439 3939  +00" cy="5.74999
+00007fa0: 3739 3065 2b30 3122 2072 3d22 302e 3533  790e+01" r="0.53
+00007fb0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+00007fc0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+00007fd0: 6520 6378 3d22 352e 3030 3030 3030 3030  e cx="5.00000000
+00007fe0: 652b 3030 2220 6379 3d22 362e 3439 3939  e+00" cy="6.4999
+00007ff0: 3938 3530 652b 3031 2220 723d 2230 2e35  9850e+01" r="0.5
+00008000: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+00008010: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+00008020: 6c65 2063 783d 2235 2e30 3030 3030 3030  le cx="5.0000000
+00008030: 3065 2b30 3022 2063 793d 2237 2e32 3439  0e+00" cy="7.249
+00008040: 3939 3931 3065 2b30 3122 2072 3d22 302e  99910e+01" r="0.
+00008050: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+00008060: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+00008070: 636c 6520 6378 3d22 352e 3030 3030 3030  cle cx="5.000000
+00008080: 3030 652b 3030 2220 6379 3d22 372e 3939  00e+00" cy="7.99
+00008090: 3939 3939 3730 652b 3031 2220 723d 2230  999970e+01" r="0
+000080a0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+000080b0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+000080c0: 7263 6c65 2063 783d 2235 2e30 3030 3030  rcle cx="5.00000
+000080d0: 3030 3065 2b30 3022 2063 793d 2238 2e37  000e+00" cy="8.7
+000080e0: 3439 3939 3936 3765 2b30 3122 2072 3d22  4999967e+01" r="
+000080f0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+00008100: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+00008110: 6972 636c 6520 6378 3d22 392e 3530 3030  ircle cx="9.5000
+00008120: 3030 3030 652b 3031 2220 6379 3d22 392e  0000e+01" cy="9.
+00008130: 3530 3030 3030 3030 652b 3031 2220 723d  50000000e+01" r=
+00008140: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+00008150: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+00008160: 6369 7263 6c65 2063 783d 2239 2e35 3030  circle cx="9.500
+00008170: 3030 3030 3065 2b30 3122 2063 793d 2235  00000e+01" cy="5
+00008180: 2e30 3030 3030 3030 3065 2b30 3022 2072  .00000000e+00" r
+00008190: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+000081a0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+000081b0: 3c63 6972 636c 6520 6378 3d22 352e 3030  <circle cx="5.00
+000081c0: 3030 3030 3030 652b 3030 2220 6379 3d22  000000e+00" cy="
+000081d0: 392e 3530 3030 3030 3030 652b 3031 2220  9.50000000e+01" 
+000081e0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+000081f0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+00008200: 203c 6369 7263 6c65 2063 783d 2235 2e30   <circle cx="5.0
+00008210: 3030 3030 3030 3065 2b30 3022 2063 793d  0000000e+00" cy=
+00008220: 2235 2e30 3030 3030 3030 3065 2b30 3022  "5.00000000e+00"
+00008230: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+00008240: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+00008250: 2020 3c63 6972 636c 6520 6378 3d22 322e    <circle cx="2.
+00008260: 3330 3030 3030 3030 652b 3031 2220 6379  30000000e+01" cy
+00008270: 3d22 322e 3330 3030 3030 3030 652b 3031  ="2.30000000e+01
+00008280: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+00008290: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+000082a0: 2020 203c 6369 7263 6c65 2063 783d 2232     <circle cx="2
+000082b0: 2e33 3030 3030 3030 3065 2b30 3122 2063  .30000000e+01" c
+000082c0: 793d 2235 2e39 3030 3030 3030 3065 2b30  y="5.90000000e+0
+000082d0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+000082e0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+000082f0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+00008300: 342e 3130 3030 3030 3030 652b 3031 2220  4.10000000e+01" 
+00008310: 6379 3d22 372e 3730 3030 3030 3030 652b  cy="7.70000000e+
+00008320: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+00008330: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+00008340: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00008350: 2235 2e39 3030 3030 3030 3065 2b30 3122  "5.90000000e+01"
+00008360: 2063 793d 2235 2e39 3030 3030 3030 3065   cy="5.90000000e
+00008370: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+00008380: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+00008390: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+000083a0: 3d22 372e 3730 3030 3030 3030 652b 3031  ="7.70000000e+01
+000083b0: 2220 6379 3d22 342e 3130 3030 3030 3030  " cy="4.10000000
+000083c0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+000083d0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+000083e0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+000083f0: 783d 2235 2e39 3030 3030 3030 3065 2b30  x="5.90000000e+0
+00008400: 3122 2063 793d 2232 2e33 3030 3030 3030  1" cy="2.3000000
+00008410: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+00008420: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+00008430: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+00008440: 6378 3d22 352e 3731 3037 3439 3830 652b  cx="5.71074980e+
+00008450: 3031 2220 6379 3d22 382e 3133 3036 3838  01" cy="8.130688
+00008460: 3730 652b 3031 2220 723d 2230 2e35 3336  70e+01" r="0.536
+00008470: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+00008480: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+00008490: 2063 783d 2231 2e37 3030 3036 3633 3065   cx="1.70006630e
+000084a0: 2b30 3122 2063 793d 2238 2e32 3938 3834  +01" cy="8.29884
+000084b0: 3338 3065 2b30 3122 2072 3d22 302e 3533  380e+01" r="0.53
+000084c0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+000084d0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+000084e0: 6520 6378 3d22 382e 3139 3330 3333 3530  e cx="8.19303350
+000084f0: 652b 3031 2220 6379 3d22 382e 3139 3437  e+01" cy="8.1947
+00008500: 3538 3830 652b 3031 2220 723d 2230 2e35  5880e+01" r="0.5
+00008510: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+00008520: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+00008530: 6c65 2063 783d 2233 2e39 3131 3039 3138  le cx="3.9110918
+00008540: 3065 2b30 3122 2063 793d 2231 2e34 3636  0e+01" cy="1.466
+00008550: 3531 3831 3065 2b30 3122 2072 3d22 302e  51810e+01" r="0.
+00008560: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+00008570: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+00008580: 636c 6520 6378 3d22 372e 3735 3334 3736  cle cx="7.753476
+00008590: 3230 652b 3031 2220 6379 3d22 362e 3932  20e+01" cy="6.92
+000085a0: 3336 3439 3230 652b 3031 2220 723d 2230  364920e+01" r="0
+000085b0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+000085c0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+000085d0: 7263 6c65 2063 783d 2236 2e39 3230 3838  rcle cx="6.92088
+000085e0: 3731 3065 2b30 3122 2063 793d 2237 2e37  710e+01" cy="7.7
+000085f0: 3536 3233 3833 3065 2b30 3122 2072 3d22  5623830e+01" r="
+00008600: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+00008610: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+00008620: 6972 636c 6520 6378 3d22 312e 3730 3535  ircle cx="1.7055
+00008630: 3736 3130 652b 3031 2220 6379 3d22 352e  7610e+01" cy="5.
+00008640: 3332 3134 3232 3430 652b 3031 2220 723d  32142240e+01" r=
+00008650: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+00008660: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+00008670: 6369 7263 6c65 2063 783d 2232 2e37 3338  circle cx="2.738
+00008680: 3232 3434 3065 2b30 3122 2063 793d 2238  22440e+01" cy="8
+00008690: 2e30 3237 3537 3339 3065 2b30 3122 2072  .02757390e+01" r
+000086a0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+000086b0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+000086c0: 3c63 6972 636c 6520 6378 3d22 372e 3235  <circle cx="7.25
+000086d0: 3434 3338 3830 652b 3031 2220 6379 3d22  443880e+01" cy="
+000086e0: 312e 3438 3039 3937 3330 652b 3031 2220  1.48099730e+01" 
+000086f0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+00008700: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+00008710: 203c 6369 7263 6c65 2063 783d 2238 2e32   <circle cx="8.2
+00008720: 3939 3438 3436 3065 2b30 3122 2063 793d  9948460e+01" cy=
+00008730: 2231 2e37 3030 3730 3731 3065 2b30 3122  "1.70070710e+01"
+00008740: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+00008750: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+00008760: 2020 3c63 6972 636c 6520 6378 3d22 372e    <circle cx="7.
+00008770: 3934 3936 3536 3430 652b 3031 2220 6379  94965640e+01" cy
+00008780: 3d22 312e 3330 3034 3731 3730 652b 3031  ="1.30047170e+01
+00008790: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+000087a0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+000087b0: 2020 203c 6369 7263 6c65 2063 783d 2238     <circle cx="8
+000087c0: 2e34 3134 3730 3938 3065 2b30 3122 2063  .41470980e+01" c
+000087d0: 793d 2233 2e37 3638 3331 3637 3065 2b30  y="3.76831670e+0
+000087e0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+000087f0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+00008800: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+00008810: 372e 3235 3139 3931 3730 652b 3031 2220  7.25199170e+01" 
+00008820: 6379 3d22 392e 3931 3335 3332 3030 652b  cy="9.91353200e+
+00008830: 3030 2220 723d 2230 2e35 3336 3831 3034  00" r="0.5368104
+00008840: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+00008850: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00008860: 2234 2e32 3734 3036 3138 3065 2b30 3122  "4.27406180e+01"
+00008870: 2063 793d 2231 2e31 3434 3334 3531 3065   cy="1.14434510e
+00008880: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+00008890: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+000088a0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+000088b0: 3d22 342e 3635 3938 3132 3630 652b 3031  ="4.65981260e+01
+000088c0: 2220 6379 3d22 382e 3235 3330 3434 3630  " cy="8.25304460
+000088d0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+000088e0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+000088f0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+00008900: 783d 2234 2e36 3337 3033 3138 3065 2b30  x="4.63703180e+0
+00008910: 3122 2063 793d 2238 2e32 3231 3733 3030  1" cy="8.2217300
+00008920: 3065 2b30 3022 2072 3d22 302e 3533 3638  0e+00" r="0.5368
+00008930: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+00008940: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+00008950: 6378 3d22 342e 3634 3833 3833 3530 652b  cx="4.64838350e+
+00008960: 3031 2220 6379 3d22 312e 3636 3137 3337  01" cy="1.661737
+00008970: 3130 652b 3031 2220 723d 2230 2e35 3336  10e+01" r="0.536
+00008980: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+00008990: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+000089a0: 2063 783d 2238 2e30 3238 3034 3832 3065   cx="8.02804820e
+000089b0: 2b30 3122 2063 793d 2232 2e37 3338 3730  +01" cy="2.73870
+000089c0: 3233 3065 2b30 3122 2072 3d22 302e 3533  230e+01" r="0.53
+000089d0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+000089e0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+000089f0: 6520 6378 3d22 312e 3537 3431 3836 3930  e cx="1.57418690
+00008a00: 652b 3031 2220 6379 3d22 362e 3232 3137  e+01" cy="6.2217
+00008a10: 3431 3930 652b 3031 2220 723d 2230 2e35  4190e+01" r="0.5
+00008a20: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+00008a30: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+00008a40: 6c65 2063 783d 2231 2e39 3639 3538 3132  le cx="1.9695812
+00008a50: 3065 2b30 3122 2063 793d 2237 2e32 3539  0e+01" cy="7.259
+00008a60: 3633 3534 3065 2b30 3122 2072 3d22 302e  63540e+01" r="0.
+00008a70: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+00008a80: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+00008a90: 636c 6520 6378 3d22 362e 3232 3138 3634  cle cx="6.221864
+00008aa0: 3330 652b 3031 2220 6379 3d22 312e 3537  30e+01" cy="1.57
+00008ab0: 3433 3035 3730 652b 3031 2220 723d 2230  430570e+01" r="0
+00008ac0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+00008ad0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+00008ae0: 7263 6c65 2063 783d 2231 2e36 3631 3733  rcle cx="1.66173
+00008af0: 3731 3065 2b30 3122 2063 793d 2234 2e36  710e+01" cy="4.6
+00008b00: 3438 3338 3137 3065 2b30 3122 2072 3d22  4838170e+01" r="
+00008b10: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+00008b20: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+00008b30: 6972 636c 6520 6378 3d22 362e 3536 3534  ircle cx="6.5654
+00008b40: 3136 3830 652b 3031 2220 6379 3d22 312e  1680e+01" cy="1.
+00008b50: 3231 3539 3530 3930 652b 3031 2220 723d  21595090e+01" r=
+00008b60: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+00008b70: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+00008b80: 6369 7263 6c65 2063 783d 2236 2e30 3637  circle cx="6.067
+00008b90: 3837 3631 3065 2b30 3122 2063 793d 2237  87610e+01" cy="7
+00008ba0: 2e32 3432 3636 3638 3065 2b30 3122 2072  .24266680e+01" r
+00008bb0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+00008bc0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+00008bd0: 3c63 6972 636c 6520 6378 3d22 372e 3236  <circle cx="7.26
+00008be0: 3031 3133 3330 652b 3031 2220 6379 3d22  011330e+01" cy="
+00008bf0: 312e 3937 3030 3534 3630 652b 3031 2220  1.97005460e+01" 
+00008c00: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+00008c10: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+00008c20: 203c 6369 7263 6c65 2063 783d 2238 2e31   <circle cx="8.1
+00008c30: 3239 3738 3639 3065 2b30 3122 2063 793d  2978690e+01" cy=
+00008c40: 2235 2e37 3131 3636 3432 3065 2b30 3122  "5.71166420e+01"
+00008c50: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+00008c60: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+00008c70: 2020 3c63 6972 636c 6520 6378 3d22 362e    <circle cx="6.
+00008c80: 3630 3039 3837 3530 652b 3031 2220 6379  60098750e+01" cy
+00008c90: 3d22 362e 3630 3338 3136 3230 652b 3031  ="6.60381620e+01
+00008ca0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+00008cb0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+00008cc0: 2020 203c 6369 7263 6c65 2063 783d 2233     <circle cx="3
+00008cd0: 2e37 3638 3138 3236 3065 2b30 3122 2063  .76818260e+01" c
+00008ce0: 793d 2238 2e34 3134 3630 3030 3065 2b30  y="8.41460000e+0
+00008cf0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+00008d00: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+00008d10: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+00008d20: 362e 3930 3737 3030 3330 652b 3031 2220  6.90770030e+01" 
+00008d30: 6379 3d22 382e 3539 3130 3930 3030 652b  cy="8.59109000e+
+00008d40: 3030 2220 723d 2230 2e35 3336 3831 3034  00" r="0.5368104
+00008d50: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+00008d60: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00008d70: 2238 2e32 3532 3931 3935 3065 2b30 3122  "8.25291950e+01"
+00008d80: 2063 793d 2234 2e36 3539 3938 3534 3065   cy="4.65998540e
+00008d90: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+00008da0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+00008db0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+00008dc0: 3d22 312e 3436 3635 3138 3130 652b 3031  ="1.46651810e+01
+00008dd0: 2220 6379 3d22 332e 3931 3130 3930 3030  " cy="3.91109000
+00008de0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+00008df0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+00008e00: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+00008e10: 783d 2237 2e35 3939 3832 3832 3065 2b30  x="7.59982820e+0
+00008e20: 3122 2063 793d 2239 2e30 3032 3335 3430  1" cy="9.0023540
+00008e30: 3065 2b30 3022 2072 3d22 302e 3533 3638  0e+00" r="0.5368
+00008e40: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+00008e50: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+00008e60: 6378 3d22 372e 3234 3034 3931 3530 652b  cx="7.24049150e+
+00008e70: 3031 2220 6379 3d22 362e 3037 3030 3534  01" cy="6.070054
+00008e80: 3130 652b 3031 2220 723d 2230 2e35 3336  10e+01" r="0.536
+00008e90: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+00008ea0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+00008eb0: 2063 783d 2234 2e37 3535 3535 3139 3065   cx="4.75555190e
+00008ec0: 2b30 3122 2063 793d 2237 2e38 3039 3931  +01" cy="7.80991
+00008ed0: 3631 3065 2b30 3122 2072 3d22 302e 3533  610e+01" r="0.53
+00008ee0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+00008ef0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+00008f00: 6520 6378 3d22 352e 3838 3937 3438 3130  e cx="5.88974810
+00008f10: 652b 3031 2220 6379 3d22 362e 3831 3436  e+01" cy="6.8146
+00008f20: 3935 3230 652b 3031 2220 723d 2230 2e35  9520e+01" r="0.5
+00008f30: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+00008f40: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+00008f50: 6c65 2063 783d 2236 2e33 3237 3836 3633  le cx="6.3278663
+00008f60: 3065 2b30 3122 2063 793d 2236 2e36 3033  0e+01" cy="6.603
+00008f70: 3438 3431 3065 2b30 3122 2072 3d22 302e  48410e+01" r="0.
+00008f80: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+00008f90: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+00008fa0: 636c 6520 6378 3d22 392e 3036 3433 3434  cle cx="9.064344
+00008fb0: 3230 652b 3031 2220 6379 3d22 372e 3536  20e+01" cy="7.56
+00008fc0: 3439 3139 3930 652b 3031 2220 723d 2230  491990e+01" r="0
+00008fd0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+00008fe0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+00008ff0: 7263 6c65 2063 783d 2235 2e38 3132 3732  rcle cx="5.81272
+00009000: 3730 3065 2b30 3122 2063 793d 2231 2e32  700e+01" cy="1.2
+00009010: 3139 3531 3538 3065 2b30 3122 2072 3d22  1951580e+01" r="
+00009020: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+00009030: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+00009040: 6972 636c 6520 6378 3d22 342e 3736 3535  ircle cx="4.7655
+00009050: 3839 3630 652b 3031 2220 6379 3d22 312e  8960e+01" cy="1.
+00009060: 3237 3434 3931 3430 652b 3031 2220 723d  27449140e+01" r=
+00009070: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+00009080: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+00009090: 6369 7263 6c65 2063 783d 2235 2e34 3036  circle cx="5.406
+000090a0: 3938 3435 3065 2b30 3122 2063 793d 2238  98450e+01" cy="8
+000090b0: 2e36 3035 3830 3530 3065 2b30 3022 2072  .60580500e+00" r
+000090c0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+000090d0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+000090e0: 3c63 6972 636c 6520 6378 3d22 352e 3130  <circle cx="5.10
+000090f0: 3730 3937 3330 652b 3031 2220 6379 3d22  709730e+01" cy="
+00009100: 392e 3032 3037 3638 3030 652b 3030 2220  9.02076800e+00" 
+00009110: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+00009120: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+00009130: 203c 6369 7263 6c65 2063 783d 2233 2e31   <circle cx="3.1
+00009140: 3337 3033 3135 3065 2b30 3122 2063 793d  3703150e+01" cy=
+00009150: 2238 2e32 3231 3733 3030 3065 2b30 3022  "8.22173000e+00"
+00009160: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+00009170: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+00009180: 2020 3c63 6972 636c 6520 6378 3d22 382e    <circle cx="8.
+00009190: 3632 3836 3838 3430 652b 3031 2220 6379  62868840e+01" cy
+000091a0: 3d22 372e 3837 3938 3338 3930 652b 3031  ="7.87983890e+01
+000091b0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+000091c0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+000091d0: 2020 203c 6369 7263 6c65 2063 783d 2238     <circle cx="8
+000091e0: 2e33 3335 3635 3131 3065 2b30 3122 2063  .33565110e+01" c
+000091f0: 793d 2237 2e30 3332 3433 3331 3065 2b30  y="7.03243310e+0
+00009200: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+00009210: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+00009220: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+00009230: 382e 3931 3738 3235 3130 652b 3031 2220  8.91782510e+01" 
+00009240: 6379 3d22 372e 3134 3132 3136 3130 652b  cy="7.14121610e+
+00009250: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+00009260: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+00009270: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00009280: 2232 2e36 3030 3030 3036 3065 2b30 3122  "2.60000060e+01"
+00009290: 2063 793d 2231 2e31 3030 3030 3033 3065   cy="1.10000030e
+000092a0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+000092b0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+000092c0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+000092d0: 3d22 352e 3539 3932 3031 3130 652b 3031  ="5.59920110e+01
+000092e0: 2220 6379 3d22 372e 3831 3636 3430 3030  " cy="7.81664000
+000092f0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+00009300: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+00009310: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+00009320: 783d 2235 2e32 3133 3937 3332 3065 2b30  x="5.21397320e+0
+00009330: 3122 2063 793d 2231 2e33 3033 3433 3831  1" cy="1.3034381
+00009340: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+00009350: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+00009360: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+00009370: 6378 3d22 352e 3530 3431 3937 3130 652b  cx="5.50419710e+
+00009380: 3031 2220 6379 3d22 372e 3530 3930 3437  01" cy="7.509047
+00009390: 3030 652b 3031 2220 723d 2230 2e35 3336  00e+01" r="0.536
+000093a0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+000093b0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+000093c0: 2063 783d 2235 2e36 3137 3736 3039 3065   cx="5.61776090e
+000093d0: 2b30 3122 2063 793d 2237 2e32 3134 3733  +01" cy="7.21473
+000093e0: 3038 3065 2b30 3122 2072 3d22 302e 3533  080e+01" r="0.53
+000093f0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+00009400: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+00009410: 6520 6378 3d22 352e 3834 3232 3933 3830  e cx="5.84229380
+00009420: 652b 3031 2220 6379 3d22 372e 3232 3237  e+01" cy="7.2227
+00009430: 3636 3930 652b 3031 2220 723d 2230 2e35  6690e+01" r="0.5
+00009440: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+00009450: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+00009460: 6c65 2063 783d 2235 2e31 3034 3432 3937  le cx="5.1044297
+00009470: 3065 2b30 3122 2063 793d 2237 2e37 3831  0e+01" cy="7.781
+00009480: 3536 3730 3065 2b30 3122 2072 3d22 302e  56700e+01" r="0.
+00009490: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+000094a0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+000094b0: 636c 6520 6378 3d22 352e 3937 3033 3233  cle cx="5.970323
+000094c0: 3330 652b 3031 2220 6379 3d22 372e 3033  30e+01" cy="7.03
+000094d0: 3037 3331 3230 652b 3031 2220 723d 2230  073120e+01" r="0
+000094e0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+000094f0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+00009500: 7263 6c65 2063 783d 2236 2e30 3539 3232  rcle cx="6.05922
+00009510: 3731 3065 2b30 3122 2063 793d 2236 2e36  710e+01" cy="6.6
+00009520: 3036 3938 3738 3065 2b30 3122 2072 3d22  0698780e+01" r="
+00009530: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+00009540: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+00009550: 6972 636c 6520 6378 3d22 342e 3838 3237  ircle cx="4.8827
+00009560: 3935 3730 652b 3031 2220 6379 3d22 382e  9570e+01" cy="8.
+00009570: 3837 3234 3537 3030 652b 3030 2220 723d  87245700e+00" r=
+00009580: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+00009590: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+000095a0: 6369 7263 6c65 2063 783d 2233 2e30 3530  circle cx="3.050
+000095b0: 3030 3036 3065 2b30 3122 2063 793d 2231  00060e+01" cy="1
+000095c0: 2e36 3939 3939 3937 3065 2b30 3122 2072  .69999970e+01" r
+000095d0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+000095e0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+000095f0: 3c63 6972 636c 6520 6378 3d22 342e 3730  <circle cx="4.70
+00009600: 3338 3634 3030 652b 3031 2220 6379 3d22  386400e+01" cy="
+00009610: 382e 3033 3032 3830 3230 652b 3031 2220  8.03028020e+01" 
+00009620: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+00009630: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+00009640: 203c 6369 7263 6c65 2063 783d 2232 2e34   <circle cx="2.4
+00009650: 3530 3030 3033 3065 2b30 3122 2063 793d  5000030e+01" cy=
+00009660: 2231 2e36 3939 3939 3937 3065 2b30 3122  "1.69999970e+01"
+00009670: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+00009680: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+00009690: 2020 3c63 6972 636c 6520 6378 3d22 332e    <circle cx="3.
+000096a0: 3532 3430 3632 3130 652b 3031 2220 6379  52406210e+01" cy
+000096b0: 3d22 312e 3134 3433 3435 3130 652b 3031  ="1.14434510e+01
+000096c0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+000096d0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+000096e0: 2020 203c 6369 7263 6c65 2063 783d 2235     <circle cx="5
+000096f0: 2e33 3231 3432 3333 3065 2b30 3122 2063  .32142330e+01" c
+00009700: 793d 2231 2e37 3035 3537 3730 3065 2b30  y="1.70557700e+0
+00009710: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+00009720: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+00009730: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+00009740: 322e 3930 3030 3031 3230 652b 3031 2220  2.90000120e+01" 
+00009750: 6379 3d22 312e 3130 3030 3030 3330 652b  cy="1.10000030e+
+00009760: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+00009770: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+00009780: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00009790: 2235 2e34 3037 3637 3438 3065 2b30 3122  "5.40767480e+01"
+000097a0: 2063 793d 2237 2e39 3432 3539 3431 3065   cy="7.94259410e
+000097b0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+000097c0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+000097d0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+000097e0: 3d22 392e 3133 3634 3030 3930 652b 3031  ="9.13640090e+01
+000097f0: 2220 6379 3d22 332e 3038 3930 3533 3430  " cy="3.08905340
+00009800: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+00009810: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+00009820: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+00009830: 783d 2232 2e31 3232 3232 3339 3065 2b30  x="2.12222390e+0
+00009840: 3122 2063 793d 2236 2e34 3739 3235 3335  1" cy="6.4792535
+00009850: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+00009860: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+00009870: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+00009880: 6378 3d22 312e 3835 3632 3932 3830 652b  cx="1.85629280e+
+00009890: 3031 2220 6379 3d22 362e 3334 3139 3138  01" cy="6.341918
+000098a0: 3930 652b 3031 2220 723d 2230 2e35 3336  90e+01" r="0.536
+000098b0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+000098c0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+000098d0: 2063 783d 2238 2e35 3838 3039 3933 3065   cx="8.58809930e
+000098e0: 2b30 3122 2063 793d 2235 2e34 3734 3433  +01" cy="5.47443
+000098f0: 3530 3065 2b30 3122 2072 3d22 302e 3533  500e+01" r="0.53
+00009900: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+00009910: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+00009920: 6520 6378 3d22 392e 3030 3831 3134 3930  e cx="9.00811490
+00009930: 652b 3031 2220 6379 3d22 322e 3734 3733  e+01" cy="2.7473
+00009940: 3631 3230 652b 3031 2220 723d 2230 2e35  6120e+01" r="0.5
+00009950: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+00009960: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+00009970: 6c65 2063 783d 2238 2e37 3735 3031 3637  le cx="8.7750167
+00009980: 3065 2b30 3122 2063 793d 2233 2e34 3237  0e+01" cy="3.427
+00009990: 3931 3738 3065 2b30 3122 2072 3d22 302e  91780e+01" r="0.
+000099a0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+000099b0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+000099c0: 636c 6520 6378 3d22 332e 3138 3236 3132  cle cx="3.182612
+000099d0: 3030 652b 3031 2220 6379 3d22 372e 3734  00e+01" cy="7.74
+000099e0: 3039 3633 3530 652b 3031 2220 723d 2230  096350e+01" r="0
+000099f0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+00009a00: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+00009a10: 7263 6c65 2063 783d 2232 2e31 3230 3530  rcle cx="2.12050
+00009a20: 3232 3065 2b30 3122 2063 793d 2237 2e30  220e+01" cy="7.0
+00009a30: 3430 3736 3137 3065 2b30 3122 2072 3d22  4076170e+01" r="
+00009a40: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+00009a50: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+00009a60: 6972 636c 6520 6378 3d22 332e 3531 3833  ircle cx="3.5183
+00009a70: 3534 3330 652b 3031 2220 6379 3d22 372e  5430e+01" cy="7.
+00009a80: 3837 3330 3338 3530 652b 3031 2220 723d  87303850e+01" r=
+00009a90: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+00009aa0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+00009ab0: 6369 7263 6c65 2063 783d 2238 2e35 3137  circle cx="8.517
+00009ac0: 3837 3332 3065 2b30 3122 2063 793d 2232  87320e+01" cy="2
+00009ad0: 2e37 3434 3534 3639 3065 2b30 3122 2072  .74454690e+01" r
+00009ae0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+00009af0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+00009b00: 3c63 6972 636c 6520 6378 3d22 382e 3737  <circle cx="8.77
+00009b10: 3636 3435 3730 652b 3031 2220 6379 3d22  664570e+01" cy="
+00009b20: 342e 3138 3035 3934 3130 652b 3031 2220  4.18059410e+01" 
+00009b30: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+00009b40: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+00009b50: 203c 6369 7263 6c65 2063 783d 2232 2e37   <circle cx="2.7
+00009b60: 3636 3537 3236 3065 2b30 3122 2063 793d  6657260e+01" cy=
+00009b70: 2237 2e37 3439 3031 3430 3065 2b30 3122  "7.74901400e+01"
+00009b80: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+00009b90: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+00009ba0: 2020 3c63 6972 636c 6520 6378 3d22 332e    <circle cx="3.
+00009bb0: 3635 3132 3433 3830 652b 3031 2220 6379  65124380e+01" cy
+00009bc0: 3d22 382e 3133 3635 3835 3530 652b 3031  ="8.13658550e+01
+00009bd0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+00009be0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+00009bf0: 2020 203c 6369 7263 6c65 2063 783d 2232     <circle cx="2
+00009c00: 2e34 3030 3032 3234 3065 2b30 3122 2063  .40002240e+01" c
+00009c10: 793d 2239 2e30 3939 3631 3436 3665 2b30  y="9.09961466e+0
+00009c20: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+00009c30: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+00009c40: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+00009c50: 392e 3133 3733 3934 3530 652b 3031 2220  9.13739450e+01" 
+00009c60: 6379 3d22 342e 3539 3130 3531 3730 652b  cy="4.59105170e+
+00009c70: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+00009c80: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+00009c90: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+00009ca0: 2232 2e37 3737 3135 3339 3065 2b30 3122  "2.77715390e+01"
+00009cb0: 2063 793d 2237 2e34 3733 3436 3337 3065   cy="7.47346370e
+00009cc0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+00009cd0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+00009ce0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+00009cf0: 3d22 392e 3039 3938 3238 3530 652b 3031  ="9.09982850e+01
+00009d00: 2220 6379 3d22 322e 3430 3032 3336 3630  " cy="2.40023660
+00009d10: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+00009d20: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+00009d30: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+00009d40: 783d 2232 2e39 3537 3832 3335 3065 2b30  x="2.95782350e+0
+00009d50: 3122 2063 793d 2237 2e38 3737 3635 3238  1" cy="7.8776528
+00009d60: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+00009d70: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+00009d80: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+00009d90: 6378 3d22 322e 3035 3030 3433 3930 652b  cx="2.05004390e+
+00009da0: 3031 2220 6379 3d22 382e 3639 3932 3239  01" cy="8.699229
+00009db0: 3431 652b 3031 2220 723d 2230 2e35 3336  41e+01" r="0.536
+00009dc0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+00009dd0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+00009de0: 2063 783d 2239 2e30 3434 3039 3432 3065   cx="9.04409420e
+00009df0: 2b30 3122 2063 793d 2235 2e32 3337 3037  +01" cy="5.23707
+00009e00: 3236 3065 2b30 3122 2072 3d22 302e 3533  260e+01" r="0.53
+00009e10: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+00009e20: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+00009e30: 6520 6378 3d22 392e 3038 3334 3439 3430  e cx="9.08344940
+00009e40: 652b 3031 2220 6379 3d22 342e 3838 3730  e+01" cy="4.8870
+00009e50: 3932 3330 652b 3031 2220 723d 2230 2e35  9230e+01" r="0.5
+00009e60: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+00009e70: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+00009e80: 6c65 2063 783d 2232 2e32 3538 3639 3930  le cx="2.2586990
+00009e90: 3065 2b30 3122 2063 793d 2236 2e38 3136  0e+01" cy="6.816
+00009ea0: 3835 3334 3065 2b30 3122 2072 3d22 302e  85340e+01" r="0.
+00009eb0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+00009ec0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+00009ed0: 636c 6520 6378 3d22 322e 3234 3931 3535  cle cx="2.249155
+00009ee0: 3430 652b 3031 2220 6379 3d22 372e 3233  40e+01" cy="7.23
+00009ef0: 3230 3334 3230 652b 3031 2220 723d 2230  203420e+01" r="0
+00009f00: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+00009f10: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+00009f20: 7263 6c65 2063 783d 2239 2e30 3430 3439  rcle cx="9.04049
+00009f30: 3630 3065 2b30 3122 2063 793d 2236 2e37  600e+01" cy="6.7
+00009f40: 3335 3935 3639 3065 2b30 3122 2072 3d22  3595690e+01" r="
+00009f50: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+00009f60: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+00009f70: 6972 636c 6520 6378 3d22 322e 3532 3535  ircle cx="2.5255
+00009f80: 3431 3830 652b 3031 2220 6379 3d22 372e  4180e+01" cy="7.
+00009f90: 3232 3233 3430 3330 652b 3031 2220 723d  22234030e+01" r=
+00009fa0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+00009fb0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+00009fc0: 6369 7263 6c65 2063 783d 2238 2e35 3834  circle cx="8.584
+00009fd0: 3332 3131 3065 2b30 3122 2063 793d 2236  32110e+01" cy="6
+00009fe0: 2e32 3233 3431 3737 3065 2b30 3122 2072  .22341770e+01" r
+00009ff0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000a000: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000a010: 3c63 6972 636c 6520 6378 3d22 382e 3636  <circle cx="8.66
+0000a020: 3731 3039 3430 652b 3031 2220 6379 3d22  710940e+01" cy="
+0000a030: 342e 3737 3335 3837 3930 652b 3031 2220  4.77358790e+01" 
+0000a040: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000a050: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000a060: 203c 6369 7263 6c65 2063 783d 2238 2e36   <circle cx="8.6
+0000a070: 3939 3635 3631 3065 2b30 3122 2063 793d  9965610e+01" cy=
+0000a080: 2232 2e30 3530 3437 3134 3065 2b30 3122  "2.05047140e+01"
+0000a090: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000a0a0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000a0b0: 2020 3c63 6972 636c 6520 6378 3d22 342e    <circle cx="4.
+0000a0c0: 3737 3334 3731 3830 652b 3031 2220 6379  77347180e+01" cy
+0000a0d0: 3d22 382e 3636 3731 3932 3734 652b 3031  ="8.66719274e+01
+0000a0e0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000a0f0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000a100: 2020 203c 6369 7263 6c65 2063 783d 2232     <circle cx="2
+0000a110: 2e37 3437 3230 3139 3065 2b30 3122 2063  .74720190e+01" c
+0000a120: 793d 2239 2e30 3037 3935 3733 3165 2b30  y="9.00795731e+0
+0000a130: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000a140: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000a150: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000a160: 332e 3432 3738 3236 3930 652b 3031 2220  3.42782690e+01" 
+0000a170: 6379 3d22 382e 3737 3439 3432 3435 652b  cy="8.77494245e+
+0000a180: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000a190: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000a1a0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000a1b0: 2232 2e30 3837 3234 3534 3065 2b30 3122  "2.08724540e+01"
+0000a1c0: 2063 793d 2234 2e32 3832 3739 3336 3065   cy="4.28279360e
+0000a1d0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000a1e0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000a1f0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000a200: 3d22 312e 3639 3939 3939 3730 652b 3031  ="1.69999970e+01
+0000a210: 2220 6379 3d22 332e 3034 3939 3939 3730  " cy="3.04999970
+0000a220: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000a230: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000a240: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000a250: 783d 2235 2e32 3336 3736 3537 3065 2b30  x="5.23676570e+0
+0000a260: 3122 2063 793d 2239 2e30 3434 3339 3333  1" cy="9.0443933
+0000a270: 3665 2b30 3122 2072 3d22 302e 3533 3638  6e+01" r="0.5368
+0000a280: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000a290: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000a2a0: 6378 3d22 322e 3734 3432 3239 3230 652b  cx="2.74422920e+
+0000a2b0: 3031 2220 6379 3d22 382e 3531 3735 3538  01" cy="8.517558
+0000a2c0: 3230 652b 3031 2220 723d 2230 2e35 3336  20e+01" r="0.536
+0000a2d0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000a2e0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000a2f0: 2063 783d 2231 2e38 3734 3439 3038 3065   cx="1.87449080e
+0000a300: 2b30 3122 2063 793d 2234 2e34 3635 3538  +01" cy="4.46558
+0000a310: 3732 3065 2b30 3122 2072 3d22 302e 3533  720e+01" r="0.53
+0000a320: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000a330: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000a340: 6520 6378 3d22 322e 3032 3231 3732 3730  e cx="2.02217270
+0000a350: 652b 3031 2220 6379 3d22 332e 3433 3730  e+01" cy="3.4370
+0000a360: 3330 3330 652b 3031 2220 723d 2230 2e35  3030e+01" r="0.5
+0000a370: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000a380: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000a390: 6c65 2063 783d 2231 2e37 3434 3334 3534  le cx="1.7443454
+0000a3a0: 3065 2b30 3122 2063 793d 2233 2e36 3734  0e+01" cy="3.674
+0000a3b0: 3035 3937 3065 2b30 3122 2072 3d22 302e  05970e+01" r="0.
+0000a3c0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000a3d0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000a3e0: 636c 6520 6378 3d22 312e 3734 3433 3435  cle cx="1.744345
+0000a3f0: 3430 652b 3031 2220 6379 3d22 332e 3937  40e+01" cy="3.97
+0000a400: 3430 3539 3430 652b 3031 2220 723d 2230  405940e+01" r="0
+0000a410: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000a420: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000a430: 7263 6c65 2063 783d 2232 2e30 3232 3137  rcle cx="2.02217
+0000a440: 3237 3065 2b30 3122 2063 793d 2234 2e30  270e+01" cy="4.0
+0000a450: 3337 3032 3937 3065 2b30 3122 2072 3d22  3702970e+01" r="
+0000a460: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000a470: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000a480: 6972 636c 6520 6378 3d22 322e 3130 3230  ircle cx="2.1020
+0000a490: 3736 3530 652b 3031 2220 6379 3d22 352e  7650e+01" cy="5.
+0000a4a0: 3130 3734 3234 3930 652b 3031 2220 723d  10742490e+01" r=
+0000a4b0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000a4c0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000a4d0: 6369 7263 6c65 2063 783d 2231 2e39 3033  circle cx="1.903
+0000a4e0: 3933 3037 3065 2b30 3122 2063 793d 2235  93070e+01" cy="5
+0000a4f0: 2e32 3134 3436 3733 3065 2b30 3122 2072  .21446730e+01" r
+0000a500: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000a510: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000a520: 3c63 6972 636c 6520 6378 3d22 372e 3033  <circle cx="7.03
+0000a530: 3035 3930 3830 652b 3031 2220 6379 3d22  059080e+01" cy="
+0000a540: 382e 3333 3734 3932 3530 652b 3031 2220  8.33749250e+01" 
+0000a550: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000a560: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000a570: 203c 6369 7263 6c65 2063 783d 2235 2e34   <circle cx="5.4
+0000a580: 3733 3832 3330 3065 2b30 3122 2063 793d  7382300e+01" cy=
+0000a590: 2238 2e35 3838 3639 3738 3065 2b30 3122  "8.58869780e+01"
+0000a5a0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000a5b0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000a5c0: 2020 3c63 6972 636c 6520 6378 3d22 372e    <circle cx="7.
+0000a5d0: 3837 3836 3838 3730 652b 3031 2220 6379  87868870e+01" cy
+0000a5e0: 3d22 382e 3632 3938 3339 3035 652b 3031  ="8.62983905e+01
+0000a5f0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000a600: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000a610: 2020 203c 6369 7263 6c65 2063 783d 2237     <circle cx="7
+0000a620: 2e31 3430 3239 3534 3065 2b30 3122 2063  .14029540e+01" c
+0000a630: 793d 2238 2e39 3138 3734 3630 3765 2b30  y="8.91874607e+0
+0000a640: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000a650: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000a660: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000a670: 332e 3038 3930 3038 3430 652b 3031 2220  3.08900840e+01" 
+0000a680: 6379 3d22 392e 3133 3633 3634 3039 652b  cy="9.13636409e+
+0000a690: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000a6a0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000a6b0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000a6c0: 2234 2e35 3931 3030 3430 3065 2b30 3122  "4.59100400e+01"
+0000a6d0: 2063 793d 2239 2e31 3337 3335 3737 3865   cy="9.13735778e
+0000a6e0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000a6f0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000a700: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000a710: 3d22 372e 3536 3433 3433 3930 652b 3031  ="7.56434390e+01
+0000a720: 2220 6379 3d22 392e 3036 3439 3139 3537  " cy="9.06491957
+0000a730: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000a740: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000a750: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000a760: 783d 2234 2e38 3837 3033 3239 3065 2b30  x="4.88703290e+0
+0000a770: 3122 2063 793d 2239 2e30 3833 3439 3037  1" cy="9.0834907
+0000a780: 3165 2b30 3122 2072 3d22 302e 3533 3638  1e+01" r="0.5368
+0000a790: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000a7a0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000a7b0: 6378 3d22 342e 3138 3035 3032 3330 652b  cx="4.18050230e+
+0000a7c0: 3031 2220 6379 3d22 382e 3737 3635 3732  01" cy="8.776572
+0000a7d0: 3632 652b 3031 2220 723d 2230 2e35 3336  62e+01" r="0.536
+0000a7e0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000a7f0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000a800: 2063 783d 2236 2e32 3232 3830 3933 3065   cx="6.22280930e
+0000a810: 2b30 3122 2063 793d 2238 2e35 3834 3931  +01" cy="8.58491
+0000a820: 3837 3065 2b30 3122 2072 3d22 302e 3533  870e+01" r="0.53
+0000a830: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000a840: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000a850: 6520 6378 3d22 362e 3733 3536 3530 3930  e cx="6.73565090
+0000a860: 652b 3031 2220 6379 3d22 392e 3034 3037  e+01" cy="9.0407
+0000a870: 3934 3236 652b 3031 2220 723d 2230 2e35  9426e+01" r="0.5
+0000a880: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000a890: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000a8a0: 6c65 2063 783d 2231 2e31 3030 3030 3030  le cx="1.1000000
+0000a8b0: 3365 2b30 3122 2063 793d 2232 2e39 3030  3e+01" cy="2.900
+0000a8c0: 3030 3033 3065 2b30 3122 2072 3d22 302e  00030e+01" r="0.
+0000a8d0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000a8e0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000a8f0: 636c 6520 6378 3d22 382e 3639 3936 3536  cle cx="8.699656
+0000a900: 3130 652b 3031 2220 6379 3d22 312e 3330  10e+01" cy="1.30
+0000a910: 3034 3731 3730 652b 3031 2220 723d 2230  047170e+01" r="0
+0000a920: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000a930: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000a940: 7263 6c65 2063 783d 2239 2e30 3939 3832  rcle cx="9.09982
+0000a950: 3835 3065 2b30 3122 2063 793d 2239 2e30  850e+01" cy="9.0
+0000a960: 3032 3335 3430 3065 2b30 3022 2072 3d22  0235400e+00" r="
+0000a970: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000a980: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000a990: 6972 636c 6520 6378 3d22 312e 3438 3036  ircle cx="1.4806
+0000a9a0: 3832 3330 652b 3031 2220 6379 3d22 372e  8230e+01" cy="7.
+0000a9b0: 3235 3431 3232 3030 652b 3031 2220 723d  25412200e+01" r=
+0000a9c0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000a9d0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000a9e0: 6369 7263 6c65 2063 783d 2238 2e32 3231  circle cx="8.221
+0000a9f0: 3732 3634 3065 2b30 3022 2063 793d 2234  72640e+00" cy="4
+0000aa00: 2e36 3337 3032 3832 3065 2b30 3122 2072  .63702820e+01" r
+0000aa10: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000aa20: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000aa30: 3c63 6972 636c 6520 6378 3d22 312e 3330  <circle cx="1.30
+0000aa40: 3030 3434 3239 652b 3031 2220 6379 3d22  004429e+01" cy="
+0000aa50: 382e 3639 3932 3239 3431 652b 3031 2220  8.69922941e+01" 
+0000aa60: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000aa70: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000aa80: 203c 6369 7263 6c65 2063 783d 2239 2e30   <circle cx="9.0
+0000aa90: 3030 3232 3130 3065 2b30 3022 2063 793d  0022100e+00" cy=
+0000aaa0: 2239 2e30 3939 3631 3436 3665 2b30 3122  "9.09961466e+01"
+0000aab0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000aac0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000aad0: 2020 3c63 6972 636c 6520 6378 3d22 382e    <circle cx="8.
+0000aae0: 3539 3036 3932 3230 652b 3030 2220 6379  59069220e+00" cy
+0000aaf0: 3d22 362e 3930 3736 3538 3930 652b 3031  ="6.90765890e+01
+0000ab00: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000ab10: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000ab20: 2020 203c 6369 7263 6c65 2063 783d 2231     <circle cx="1
+0000ab30: 2e33 3033 3433 3734 3765 2b30 3122 2063  .30343747e+01" c
+0000ab40: 793d 2235 2e32 3133 3937 3134 3065 2b30  y="5.21397140e+0
+0000ab50: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000ab60: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000ab70: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000ab80: 312e 3639 3939 3939 3730 652b 3031 2220  1.69999970e+01" 
+0000ab90: 6379 3d22 322e 3435 3030 3030 3330 652b  cy="2.45000030e+
+0000aba0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000abb0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000abc0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000abd0: 2238 2e32 3231 3732 3634 3065 2b30 3022  "8.22172640e+00"
+0000abe0: 2063 793d 2233 2e31 3337 3032 3937 3065   cy="3.13702970e
+0000abf0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000ac00: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000ac10: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000ac20: 3d22 312e 3134 3433 3435 3337 652b 3031  ="1.14434537e+01
+0000ac30: 2220 6379 3d22 332e 3532 3430 3630 3330  " cy="3.52406030
+0000ac40: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000ac50: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000ac60: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000ac70: 783d 2231 2e38 3734 3338 3931 3065 2b30  x="1.87438910e+0
+0000ac80: 3122 2063 793d 2234 2e37 3635 3533 3536  1" cy="4.7655356
+0000ac90: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000aca0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000acb0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000acc0: 6378 3d22 392e 3032 3037 3631 3730 652b  cx="9.02076170e+
+0000acd0: 3030 2220 6379 3d22 352e 3130 3730 3934  00" cy="5.107094
+0000ace0: 3630 652b 3031 2220 723d 2230 2e35 3336  60e+01" r="0.536
+0000acf0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000ad00: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000ad10: 2063 783d 2231 2e32 3139 3433 3634 3265   cx="1.21943642e
+0000ad20: 2b30 3122 2063 793d 2235 2e38 3132 3634  +01" cy="5.81264
+0000ad30: 3531 3065 2b30 3122 2072 3d22 302e 3533  510e+01" r="0.53
+0000ad40: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000ad50: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000ad60: 6520 6378 3d22 382e 3837 3234 3536 3130  e cx="8.87245610
+0000ad70: 652b 3030 2220 6379 3d22 342e 3838 3237  e+00" cy="4.8827
+0000ad80: 3932 3130 652b 3031 2220 723d 2230 2e35  9210e+01" r="0.5
+0000ad90: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000ada0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000adb0: 6c65 2063 783d 2231 2e32 3734 3439 3131  le cx="1.2744911
+0000adc0: 3365 2b30 3122 2063 793d 2234 2e37 3635  3e+01" cy="4.765
+0000add0: 3538 3639 3065 2b30 3122 2072 3d22 302e  58690e+01" r="0.
+0000ade0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000adf0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000ae00: 636c 6520 6378 3d22 392e 3030 3032 3231  cle cx="9.000221
+0000ae10: 3030 652b 3030 2220 6379 3d22 372e 3539  00e+00" cy="7.59
+0000ae20: 3936 3134 3030 652b 3031 2220 723d 2230  961400e+01" r="0
+0000ae30: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000ae40: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000ae50: 7263 6c65 2063 783d 2232 2e30 3837 3037  rcle cx="2.08707
+0000ae60: 3830 3065 2b30 3122 2063 793d 2234 2e38  800e+01" cy="4.8
+0000ae70: 3832 3839 3131 3065 2b30 3122 2072 3d22  8289110e+01" r="
+0000ae80: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000ae90: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000aea0: 6972 636c 6520 6378 3d22 382e 3630 3533  ircle cx="8.6053
+0000aeb0: 3939 3130 652b 3030 2220 6379 3d22 352e  9910e+00" cy="5.
+0000aec0: 3430 3639 3431 3330 652b 3031 2220 723d  40694130e+01" r=
+0000aed0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000aee0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000aef0: 6369 7263 6c65 2063 783d 2231 2e32 3135  circle cx="1.215
+0000af00: 3837 3035 3365 2b30 3122 2063 793d 2236  87053e+01" cy="6
+0000af10: 2e35 3635 3333 3439 3065 2b30 3122 2072  .56533490e+01" r
+0000af20: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000af30: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000af40: 3c63 6972 636c 6520 6378 3d22 392e 3931  <circle cx="9.91
+0000af50: 3139 3534 3330 652b 3030 2220 6379 3d22  195430e+00" cy="
+0000af60: 372e 3235 3138 3333 3330 652b 3031 2220  7.25183330e+01" 
+0000af70: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000af80: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000af90: 203c 6369 7263 6c65 2063 783d 2238 2e36   <circle cx="8.6
+0000afa0: 3238 3638 3834 3065 2b30 3122 2063 793d  2868840e+01" cy=
+0000afb0: 2238 2e36 3239 3833 3930 3565 2b30 3122  "8.62983905e+01"
+0000afc0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000afd0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000afe0: 2020 3c63 6972 636c 6520 6378 3d22 312e    <circle cx="1.
+0000aff0: 3134 3433 3435 3337 652b 3031 2220 6379  14434537e+01" cy
+0000b000: 3d22 342e 3237 3430 3539 3130 652b 3031  ="4.27405910e+01
+0000b010: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000b020: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000b030: 2020 203c 6369 7263 6c65 2063 783d 2239     <circle cx="9
+0000b040: 2e30 3634 3334 3432 3065 2b30 3122 2063  .06434420e+01" c
+0000b050: 793d 2239 2e30 3634 3931 3935 3765 2b30  y="9.06491957e+0
+0000b060: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000b070: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000b080: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000b090: 312e 3330 3030 3434 3239 652b 3031 2220  1.30004429e+01" 
+0000b0a0: 6379 3d22 372e 3934 3932 3238 3930 652b  cy="7.94922890e+
+0000b0b0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000b0c0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000b0d0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000b0e0: 2231 2e31 3030 3030 3030 3365 2b30 3122  "1.10000003e+01"
+0000b0f0: 2063 793d 2232 2e35 3939 3939 3937 3065   cy="2.59999970e
+0000b100: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000b110: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000b120: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000b130: 3d22 382e 3037 3331 3931 3330 652b 3031  ="8.07319130e+01
+0000b140: 2220 6379 3d22 342e 3437 3733 3430 3330  " cy="4.47734030
+0000b150: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000b160: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000b170: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000b180: 783d 2238 2e31 3833 3032 3832 3065 2b30  x="8.18302820e+0
+0000b190: 3122 2063 793d 2233 2e38 3737 3037 3039  1" cy="3.8770709
+0000b1a0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000b1b0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000b1c0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000b1d0: 6378 3d22 312e 3831 3134 3833 3630 652b  cx="1.81148360e+
+0000b1e0: 3031 2220 6379 3d22 362e 3131 3536 3533  01" cy="6.115653
+0000b1f0: 3530 652b 3031 2220 723d 2230 2e35 3336  50e+01" r="0.536
+0000b200: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000b210: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000b220: 2063 783d 2231 2e36 3939 3939 3937 3065   cx="1.69999970e
+0000b230: 2b30 3122 2063 793d 2231 2e36 3939 3939  +01" cy="1.69999
+0000b240: 3937 3065 2b30 3122 2072 3d22 302e 3533  970e+01" r="0.53
+0000b250: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000b260: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000b270: 6520 6378 3d22 342e 3437 3732 3232 3430  e cx="4.47722240
+0000b280: 652b 3031 2220 6379 3d22 382e 3037 3332  e+01" cy="8.0732
+0000b290: 3737 3730 652b 3031 2220 723d 2230 2e35  7770e+01" r="0.5
+0000b2a0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000b2b0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000b2c0: 6c65 2063 783d 2237 2e39 3631 3531 3636  le cx="7.9615166
+0000b2d0: 3065 2b30 3122 2063 793d 2233 2e39 3933  0e+01" cy="3.993
+0000b2e0: 3534 3137 3065 2b30 3122 2072 3d22 302e  54170e+01" r="0.
+0000b2f0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000b300: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000b310: 636c 6520 6378 3d22 362e 3030 3334 3335  cle cx="6.003435
+0000b320: 3230 652b 3031 2220 6379 3d22 322e 3034  20e+01" cy="2.04
+0000b330: 3130 3437 3530 652b 3031 2220 723d 2230  104750e+01" r="0
+0000b340: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000b350: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000b360: 7263 6c65 2063 783d 2237 2e39 3134 3738  rcle cx="7.91478
+0000b370: 3836 3065 2b30 3122 2063 793d 2234 2e32  860e+01" cy="4.2
+0000b380: 3831 3232 3637 3065 2b30 3122 2072 3d22  8122670e+01" r="
+0000b390: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000b3a0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000b3b0: 6972 636c 6520 6378 3d22 312e 3930 3237  ircle cx="1.9027
+0000b3c0: 3932 3230 652b 3031 2220 6379 3d22 352e  9220e+01" cy="5.
+0000b3d0: 3531 3336 3939 3330 652b 3031 2220 723d  51369930e+01" r=
+0000b3e0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000b3f0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000b400: 6369 7263 6c65 2063 783d 2236 2e31 3135  circle cx="6.115
+0000b410: 3832 3030 3065 2b30 3122 2063 793d 2238  82000e+01" cy="8
+0000b420: 2e30 3037 3238 3730 3065 2b30 3122 2072  .00728700e+01" r
+0000b430: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000b440: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000b450: 3c63 6972 636c 6520 6378 3d22 352e 3031  <circle cx="5.01
+0000b460: 3131 3231 3330 652b 3031 2220 6379 3d22  112130e+01" cy="
+0000b470: 382e 3231 3135 3739 3830 652b 3031 2220  8.21157980e+01" 
+0000b480: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000b490: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000b4a0: 203c 6369 7263 6c65 2063 783d 2235 2e38   <circle cx="5.8
+0000b4b0: 3330 3132 3637 3065 2b30 3122 2063 793d  3012670e+01" cy=
+0000b4c0: 2237 2e38 3335 3539 3736 3065 2b30 3122  "7.83559760e+01"
+0000b4d0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000b4e0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000b4f0: 2020 3c63 6972 636c 6520 6378 3d22 362e    <circle cx="6.
+0000b500: 3131 3537 3336 3330 652b 3031 2220 6379  11573630e+01" cy
+0000b510: 3d22 312e 3831 3135 3631 3930 652b 3031  ="1.81156190e+01
+0000b520: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000b530: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000b540: 2020 203c 6369 7263 6c65 2063 783d 2235     <circle cx="5
+0000b550: 2e39 3437 3431 3338 3065 2b30 3122 2063  .94741380e+01" c
+0000b560: 793d 2237 2e35 3339 3137 3435 3065 2b30  y="7.53917450e+0
+0000b570: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000b580: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000b590: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000b5a0: 352e 3336 3138 3531 3330 652b 3031 2220  5.36185130e+01" 
+0000b5b0: 6379 3d22 382e 3137 3233 3734 3030 652b  cy="8.17237400e+
+0000b5c0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000b5d0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000b5e0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000b5f0: 2232 2e33 3931 3433 3733 3065 2b30 3122  "2.39143730e+01"
+0000b600: 2063 793d 2238 2e31 3137 3139 3233 3065   cy="8.11719230e
+0000b610: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000b620: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000b630: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000b640: 3d22 342e 3238 3131 3639 3130 652b 3031  ="4.28116910e+01
+0000b650: 2220 6379 3d22 372e 3931 3438 3235 3530  " cy="7.91482550
+0000b660: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000b670: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000b680: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000b690: 783d 2232 2e30 3938 3238 3339 3065 2b30  x="2.09828390e+0
+0000b6a0: 3122 2063 793d 2235 2e37 3037 3638 3335  1" cy="5.7076835
+0000b6b0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000b6c0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000b6d0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000b6e0: 6378 3d22 322e 3034 3536 3330 3330 652b  cx="2.04563030e+
+0000b6f0: 3031 2220 6379 3d22 382e 3230 3738 3535  01" cy="8.207855
+0000b700: 3630 652b 3031 2220 723d 2230 2e35 3336  60e+01" r="0.536
+0000b710: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000b720: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000b730: 2063 783d 2233 2e38 3736 3937 3931 3065   cx="3.87697910e
+0000b740: 2b30 3122 2063 793d 2238 2e31 3832 3935  +01" cy="8.18295
+0000b750: 3434 3065 2b30 3122 2072 3d22 302e 3533  440e+01" r="0.53
+0000b760: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000b770: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000b780: 6520 6378 3d22 332e 3939 3334 3937 3630  e cx="3.99349760
+0000b790: 652b 3031 2220 6379 3d22 372e 3936 3134  e+01" cy="7.9614
+0000b7a0: 3832 3430 652b 3031 2220 723d 2230 2e35  8240e+01" r="0.5
+0000b7b0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000b7c0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000b7d0: 6c65 2063 783d 2232 2e30 3431 3031 3036  le cx="2.0410106
+0000b7e0: 3065 2b30 3122 2063 793d 2236 2e30 3033  0e+01" cy="6.003
+0000b7f0: 3339 3536 3065 2b30 3122 2072 3d22 302e  39560e+01" r="0.
+0000b800: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000b810: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000b820: 636c 6520 6378 3d22 362e 3136 3033 3637  cle cx="6.160367
+0000b830: 3330 652b 3031 2220 6379 3d22 362e 3136  30e+01" cy="6.16
+0000b840: 3131 3731 3030 652b 3031 2220 723d 2230  117100e+01" r="0
+0000b850: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000b860: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000b870: 7263 6c65 2063 783d 2236 2e33 3731 3535  rcle cx="6.37155
+0000b880: 3530 3065 2b30 3122 2063 793d 2236 2e33  500e+01" cy="6.3
+0000b890: 3733 3439 3138 3065 2b30 3122 2072 3d22  7349180e+01" r="
+0000b8a0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000b8b0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000b8c0: 6972 636c 6520 6378 3d22 352e 3730 3736  ircle cx="5.7076
+0000b8d0: 3834 3430 652b 3031 2220 6379 3d22 322e  8440e+01" cy="2.
+0000b8e0: 3039 3832 3834 3830 652b 3031 2220 723d  09828480e+01" r=
+0000b8f0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000b900: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000b910: 6369 7263 6c65 2063 783d 2235 2e35 3133  circle cx="5.513
+0000b920: 3730 3032 3065 2b30 3122 2063 793d 2231  70020e+01" cy="1
+0000b930: 2e39 3032 3739 3232 3065 2b30 3122 2072  .90279220e+01" r
+0000b940: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000b950: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000b960: 3c63 6972 636c 6520 6378 3d22 362e 3531  <circle cx="6.51
+0000b970: 3939 3234 3530 652b 3031 2220 6379 3d22  992450e+01" cy="
+0000b980: 372e 3838 3435 3038 3130 652b 3031 2220  7.88450810e+01" 
+0000b990: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000b9a0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000b9b0: 203c 6369 7263 6c65 2063 783d 2231 2e31   <circle cx="1.1
+0000b9c0: 3030 3030 3030 3365 2b30 3122 2063 793d  0000003e+01" cy=
+0000b9d0: 2231 2e31 3030 3030 3033 3065 2b30 3122  "1.10000030e+01"
+0000b9e0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000b9f0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000ba00: 2020 3c63 6972 636c 6520 6378 3d22 362e    <circle cx="6.
+0000ba10: 3730 3830 3636 3830 652b 3031 2220 6379  70806680e+01" cy
+0000ba20: 3d22 362e 3938 3831 3030 3930 652b 3031  ="6.98810090e+01
+0000ba30: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000ba40: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000ba50: 2020 203c 6369 7263 6c65 2063 783d 2234     <circle cx="4
+0000ba60: 2e30 3337 3033 3135 3065 2b30 3122 2063  .03703150e+01" c
+0000ba70: 793d 2232 2e30 3232 3137 3237 3065 2b30  y="2.02217270e+0
+0000ba80: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000ba90: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000baa0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000bab0: 382e 3030 3537 3634 3230 652b 3031 2220  8.00576420e+01" 
+0000bac0: 6379 3d22 362e 3131 3733 3533 3630 652b  cy="6.11735360e+
+0000bad0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000bae0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000baf0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000bb00: 2231 2e36 3136 3533 3931 3065 2b30 3122  "1.61653910e+01"
+0000bb10: 2063 793d 2235 2e39 3230 3031 3630 3065   cy="5.92001600e
+0000bb20: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000bb30: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000bb40: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000bb50: 3d22 362e 3335 3134 3137 3530 652b 3031  ="6.35141750e+01
+0000bb60: 2220 6379 3d22 372e 3431 3439 3732 3730  " cy="7.41497270
+0000bb70: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000bb80: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000bb90: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000bba0: 783d 2231 2e36 3633 3034 3834 3065 2b30  x="1.66304840e+0
+0000bbb0: 3122 2063 793d 2235 2e36 3231 3130 3335  1" cy="5.6211035
+0000bbc0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000bbd0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000bbe0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000bbf0: 6378 3d22 342e 3135 3638 3535 3730 652b  cx="4.15685570e+
+0000bc00: 3031 2220 6379 3d22 312e 3533 3135 3930  01" cy="1.531590
+0000bc10: 3830 652b 3031 2220 723d 2230 2e35 3336  80e+01" r="0.536
+0000bc20: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000bc30: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000bc40: 2063 783d 2234 2e34 3032 3631 3936 3065   cx="4.40261960e
+0000bc50: 2b30 3122 2063 793d 2231 2e35 3936 3636  +01" cy="1.59666
+0000bc60: 3335 3065 2b30 3122 2072 3d22 302e 3533  350e+01" r="0.53
+0000bc70: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000bc80: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000bc90: 6520 6378 3d22 312e 3838 3034 3636 3830  e cx="1.88046680
+0000bca0: 652b 3031 2220 6379 3d22 372e 3630 3637  e+01" cy="7.6067
+0000bcb0: 3531 3030 652b 3031 2220 723d 2230 2e35  5100e+01" r="0.5
+0000bcc0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000bcd0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000bce0: 6c65 2063 783d 2236 2e38 3133 3933 3734  le cx="6.8139374
+0000bcf0: 3065 2b30 3122 2063 793d 2237 2e33 3733  0e+01" cy="7.373
+0000bd00: 3138 3933 3065 2b30 3122 2072 3d22 302e  18930e+01" r="0.
+0000bd10: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000bd20: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000bd30: 636c 6520 6378 3d22 372e 3334 3439 3335  cle cx="7.344935
+0000bd40: 3630 652b 3031 2220 6379 3d22 372e 3930  60e+01" cy="7.90
+0000bd50: 3234 3131 3830 652b 3031 2220 723d 2230  241180e+01" r="0
+0000bd60: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000bd70: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000bd80: 7263 6c65 2063 783d 2231 2e37 3930 3431  rcle cx="1.79041
+0000bd90: 3238 3065 2b30 3122 2063 793d 2237 2e39  280e+01" cy="7.9
+0000bda0: 3532 3931 3839 3065 2b30 3122 2072 3d22  5291890e+01" r="
+0000bdb0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000bdc0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000bdd0: 6972 636c 6520 6378 3d22 372e 3437 3539  ircle cx="7.4759
+0000bde0: 3436 3830 652b 3031 2220 6379 3d22 372e  4680e+01" cy="7.
+0000bdf0: 3230 3131 3739 3530 652b 3031 2220 723d  20117950e+01" r=
+0000be00: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000be10: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000be20: 6369 7263 6c65 2063 783d 2237 2e31 3938  circle cx="7.198
+0000be30: 3431 3734 3065 2b30 3122 2063 793d 2237  41740e+01" cy="7
+0000be40: 2e34 3738 3730 3839 3065 2b30 3122 2072  .47870890e+01" r
+0000be50: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000be60: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000be70: 3c63 6972 636c 6520 6378 3d22 332e 3637  <circle cx="3.67
+0000be80: 3430 3631 3530 652b 3031 2220 6379 3d22  406150e+01" cy="
+0000be90: 312e 3734 3433 3435 3430 652b 3031 2220  1.74434540e+01" 
+0000bea0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000beb0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000bec0: 203c 6369 7263 6c65 2063 783d 2237 2e38   <circle cx="7.8
+0000bed0: 3832 3337 3036 3065 2b30 3122 2063 793d  8237060e+01" cy=
+0000bee0: 2236 2e35 3232 3037 3436 3065 2b30 3122  "6.52207460e+01"
+0000bef0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000bf00: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000bf10: 2020 3c63 6972 636c 6520 6378 3d22 372e    <circle cx="7.
+0000bf20: 3337 3034 3032 3030 652b 3031 2220 6379  37040200e+01" cy
+0000bf30: 3d22 362e 3831 3637 3234 3730 652b 3031  ="6.81672470e+01
+0000bf40: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000bf50: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000bf60: 2020 203c 6369 7263 6c65 2063 783d 2236     <circle cx="6
+0000bf70: 2e39 3835 3238 3834 3065 2b30 3122 2063  .98528840e+01" c
+0000bf80: 793d 2236 2e37 3130 3839 3031 3065 2b30  y="6.71089010e+0
+0000bf90: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000bfa0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000bfb0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000bfc0: 382e 3034 3635 3134 3430 652b 3031 2220  8.04651440e+01" 
+0000bfd0: 6379 3d22 372e 3737 3130 3535 3930 652b  cy="7.77105590e+
+0000bfe0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000bff0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000c000: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000c010: 2237 2e37 3638 3938 3530 3065 2b30 3122  "7.76898500e+01"
+0000c020: 2063 793d 2238 2e30 3438 3538 3533 3065   cy="8.04858530e
+0000c030: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000c040: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000c050: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000c060: 3d22 332e 3433 3730 3331 3230 652b 3031  ="3.43703120e+01
+0000c070: 2220 6379 3d22 322e 3032 3231 3732 3730  " cy="2.02217270
+0000c080: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000c090: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000c0a0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000c0b0: 783d 2237 2e35 3834 3533 3939 3065 2b30  x="7.58453990e+0
+0000c0c0: 3122 2063 793d 2236 2e36 3339 3137 3930  1" cy="6.6391790
+0000c0d0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000c0e0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000c0f0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000c100: 6378 3d22 372e 3839 3939 3935 3330 652b  cx="7.89999530e+
+0000c110: 3031 2220 6379 3d22 372e 3334 3733 3533  01" cy="7.347353
+0000c120: 3030 652b 3031 2220 723d 2230 2e35 3336  00e+01" r="0.536
+0000c130: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000c140: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000c150: 2063 783d 2233 2e39 3734 3036 3132 3065   cx="3.97406120e
+0000c160: 2b30 3122 2063 793d 2231 2e37 3434 3334  +01" cy="1.74434
+0000c170: 3534 3065 2b30 3122 2072 3d22 302e 3533  540e+01" r="0.53
+0000c180: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000c190: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000c1a0: 6520 6378 3d22 372e 3431 3236 3034 3830  e cx="7.41260480
+0000c1b0: 652b 3031 2220 6379 3d22 362e 3335 3337  e+01" cy="6.3537
+0000c1c0: 3932 3630 652b 3031 2220 723d 2230 2e35  9260e+01" r="0.5
+0000c1d0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000c1e0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000c1f0: 6c65 2063 783d 2236 2e36 3336 3631 3034  le cx="6.6366104
+0000c200: 3065 2b30 3122 2063 793d 2237 2e35 3837  0e+01" cy="7.587
+0000c210: 3130 3439 3065 2b30 3122 2072 3d22 302e  10490e+01" r="0.
+0000c220: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000c230: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000c240: 636c 6520 6378 3d22 372e 3630 3732 3832  cle cx="7.607282
+0000c250: 3930 652b 3031 2220 6379 3d22 312e 3838  90e+01" cy="1.88
+0000c260: 3039 3937 3830 652b 3031 2220 723d 2230  099780e+01" r="0
+0000c270: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000c280: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000c290: 7263 6c65 2063 783d 2238 2e33 3631 3338  rcle cx="8.36138
+0000c2a0: 3636 3065 2b30 3122 2063 793d 2234 2e30  660e+01" cy="4.0
+0000c2b0: 3635 3739 3535 3065 2b30 3122 2072 3d22  6579550e+01" r="
+0000c2c0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000c2d0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000c2e0: 6972 636c 6520 6378 3d22 342e 3837 3238  ircle cx="4.8728
+0000c2f0: 3131 3130 652b 3031 2220 6379 3d22 312e  1110e+01" cy="1.
+0000c300: 3637 3635 3933 3430 652b 3031 2220 723d  67659340e+01" r=
+0000c310: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000c320: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000c330: 6369 7263 6c65 2063 783d 2235 2e30 3937  circle cx="5.097
+0000c340: 3137 3231 3065 2b30 3122 2063 793d 2231  17210e+01" cy="1
+0000c350: 2e36 3931 3335 3838 3065 2b30 3122 2072  .69135880e+01" r
+0000c360: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000c370: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000c380: 3c63 6972 636c 6520 6378 3d22 342e 3736  <circle cx="4.76
+0000c390: 3535 3336 3530 652b 3031 2220 6379 3d22  553650e+01" cy="
+0000c3a0: 312e 3837 3433 3839 3130 652b 3031 2220  1.87438910e+01" 
+0000c3b0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000c3c0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000c3d0: 203c 6369 7263 6c65 2063 783d 2234 2e30   <circle cx="4.0
+0000c3e0: 3635 3634 3739 3065 2b30 3122 2063 793d  6564790e+01" cy=
+0000c3f0: 2238 2e33 3631 3335 3630 3065 2b30 3122  "8.36135600e+01"
+0000c400: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000c410: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000c420: 2020 3c63 6972 636c 6520 6378 3d22 312e    <circle cx="1.
+0000c430: 3637 3635 3933 3430 652b 3031 2220 6379  67659340e+01" cy
+0000c440: 3d22 342e 3837 3238 3039 3330 652b 3031  ="4.87280930e+01
+0000c450: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000c460: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000c470: 2020 203c 6369 7263 6c65 2063 783d 2232     <circle cx="2
+0000c480: 2e32 3235 3335 3736 3065 2b30 3122 2063  .22535760e+01" c
+0000c490: 793d 2237 2e35 3136 3532 3837 3065 2b30  y="7.51652870e+0
+0000c4a0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000c4b0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000c4c0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000c4d0: 382e 3131 3737 3234 3230 652b 3031 2220  8.11772420e+01" 
+0000c4e0: 6379 3d22 322e 3339 3139 3639 3230 652b  cy="2.39196920e+
+0000c4f0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000c500: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000c510: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000c520: 2234 2e33 3632 3036 3635 3065 2b30 3122  "4.36206650e+01"
+0000c530: 2063 793d 2238 2e33 3037 3935 3237 3065   cy="8.30795270e
+0000c540: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000c550: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000c560: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000c570: 3d22 342e 3838 3238 3932 3030 652b 3031  ="4.88289200e+01
+0000c580: 2220 6379 3d22 322e 3038 3730 3738 3030  " cy="2.08707800
+0000c590: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000c5a0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000c5b0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000c5c0: 783d 2231 2e36 3931 3335 3838 3065 2b30  x="1.69135880e+0
+0000c5d0: 3122 2063 793d 2235 2e30 3937 3137 3033  1" cy="5.0971703
+0000c5e0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000c5f0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000c600: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000c610: 6378 3d22 342e 3238 3237 3935 3430 652b  cx="4.28279540e+
+0000c620: 3031 2220 6379 3d22 322e 3038 3732 3435  01" cy="2.087245
+0000c630: 3430 652b 3031 2220 723d 2230 2e35 3336  40e+01" r="0.536
+0000c640: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000c650: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000c660: 2063 783d 2234 2e34 3635 3538 3930 3065   cx="4.46558900e
+0000c670: 2b30 3122 2063 793d 2231 2e38 3734 3439  +01" cy="1.87449
+0000c680: 3038 3065 2b30 3122 2072 3d22 302e 3533  080e+01" r="0.53
+0000c690: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000c6a0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000c6b0: 6520 6378 3d22 372e 3737 3234 3033 3230  e cx="7.77240320
+0000c6c0: 652b 3031 2220 6379 3d22 322e 3438 3135  e+01" cy="2.4815
+0000c6d0: 3739 3530 652b 3031 2220 723d 2230 2e35  7950e+01" r="0.5
+0000c6e0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000c6f0: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000c700: 6c65 2063 783d 2237 2e38 3733 3038 3938  le cx="7.8730898
+0000c710: 3065 2b30 3122 2063 793d 2233 2e35 3138  0e+01" cy="3.518
+0000c720: 3339 3339 3065 2b30 3122 2072 3d22 302e  39390e+01" r="0.
+0000c730: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000c740: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000c750: 636c 6520 6378 3d22 332e 3432 3431 3639  cle cx="3.424169
+0000c760: 3330 652b 3031 2220 6379 3d22 382e 3238  30e+01" cy="8.28
+0000c770: 3732 3933 3230 652b 3031 2220 723d 2230  729320e+01" r="0
+0000c780: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000c790: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000c7a0: 7263 6c65 2063 783d 2237 2e35 3137 3030  rcle cx="7.51700
+0000c7b0: 3330 3065 2b30 3122 2063 793d 2232 2e32  300e+01" cy="2.2
+0000c7c0: 3235 3833 3733 3065 2b30 3122 2072 3d22  2583730e+01" r="
+0000c7d0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000c7e0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000c7f0: 6972 636c 6520 6378 3d22 382e 3230 3834  ircle cx="8.2084
+0000c800: 3431 3530 652b 3031 2220 6379 3d22 322e  4150e+01" cy="2.
+0000c810: 3034 3632 3136 3230 652b 3031 2220 723d  04621620e+01" r=
+0000c820: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000c830: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000c840: 6369 7263 6c65 2063 783d 2233 2e30 3831  circle cx="3.081
+0000c850: 3831 3437 3065 2b30 3122 2063 793d 2238  81470e+01" cy="8
+0000c860: 2e31 3537 3433 3934 3065 2b30 3122 2072  .15743940e+01" r
+0000c870: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000c880: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000c890: 3c63 6972 636c 6520 6378 3d22 322e 3438  <circle cx="2.48
+0000c8a0: 3131 3034 3330 652b 3031 2220 6379 3d22  110430e+01" cy="
+0000c8b0: 372e 3737 3139 3233 3530 652b 3031 2220  7.77192350e+01" 
+0000c8c0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000c8d0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000c8e0: 203c 6369 7263 6c65 2063 783d 2237 2e39   <circle cx="7.9
+0000c8f0: 3533 3530 3537 3065 2b30 3122 2063 793d  5350570e+01" cy=
+0000c900: 2231 2e37 3930 3939 3837 3065 2b30 3122  "1.79099870e+01"
+0000c910: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000c920: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000c930: 2020 3c63 6972 636c 6520 6378 3d22 382e    <circle cx="8.
+0000c940: 3238 3735 3235 3430 652b 3031 2220 6379  28752540e+01" cy
+0000c950: 3d22 332e 3432 3434 3139 3530 652b 3031  ="3.42441950e+01
+0000c960: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000c970: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000c980: 2020 203c 6369 7263 6c65 2063 783d 2238     <circle cx="8
+0000c990: 2e31 3537 3738 3935 3065 2b30 3122 2063  .15778950e+01" c
+0000c9a0: 793d 2233 2e30 3832 3137 3932 3065 2b30  y="3.08217920e+0
+0000c9b0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000c9c0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000c9d0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000c9e0: 382e 3330 3739 3035 3930 652b 3031 2220  8.30790590e+01" 
+0000c9f0: 6379 3d22 342e 3336 3232 3235 3830 652b  cy="4.36222580e+
+0000ca00: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000ca10: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000ca20: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000ca30: 2238 2e31 3336 3635 3339 3065 2b30 3122  "8.13665390e+01"
+0000ca40: 2063 793d 2233 2e36 3531 3333 3734 3065   cy="3.65133740e
+0000ca50: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000ca60: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000ca70: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000ca80: 3d22 362e 3234 3538 3039 3730 652b 3031  ="6.24580970e+01
+0000ca90: 2220 6379 3d22 372e 3032 3831 3032 3330  " cy="7.02810230
+0000caa0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000cab0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000cac0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000cad0: 783d 2237 2e32 3332 3336 3237 3065 2b30  x="7.23236270e+0
+0000cae0: 3122 2063 793d 2232 2e32 3439 3437 3034  1" cy="2.2494704
+0000caf0: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000cb00: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000cb10: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000cb20: 6378 3d22 372e 3437 3336 3430 3130 652b  cx="7.47364010e+
+0000cb30: 3031 2220 6379 3d22 322e 3737 3732 3937  01" cy="2.777297
+0000cb40: 3930 652b 3031 2220 723d 2230 2e35 3336  90e+01" r="0.536
+0000cb50: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000cb60: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000cb70: 2063 783d 2237 2e38 3136 3035 3134 3065   cx="7.81605140e
+0000cb80: 2b30 3122 2063 793d 2235 2e35 3939 3833  +01" cy="5.59983
+0000cb90: 3536 3065 2b30 3122 2072 3d22 302e 3533  560e+01" r="0.53
+0000cba0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000cbb0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000cbc0: 6520 6378 3d22 312e 3833 3631 3338 3230  e cx="1.83613820
+0000cbd0: 652b 3031 2220 6379 3d22 362e 3931 3336  e+01" cy="6.9136
+0000cbe0: 3136 3030 652b 3031 2220 723d 2230 2e35  1600e+01" r="0.5
+0000cbf0: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000cc00: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000cc10: 6c65 2063 783d 2237 2e37 3439 3332 3831  le cx="7.7493281
+0000cc20: 3065 2b30 3122 2063 793d 2232 2e37 3636  0e+01" cy="2.766
+0000cc30: 3930 3131 3065 2b30 3122 2072 3d22 302e  90110e+01" r="0.
+0000cc40: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000cc50: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000cc60: 636c 6520 6378 3d22 362e 3931 3339 3735  cle cx="6.913975
+0000cc70: 3130 652b 3031 2220 6379 3d22 312e 3833  10e+01" cy="1.83
+0000cc80: 3634 3931 3930 652b 3031 2220 723d 2230  649190e+01" r="0
+0000cc90: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000cca0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000ccb0: 7263 6c65 2063 783d 2236 2e35 3638 3831  rcle cx="6.56881
+0000ccc0: 3631 3065 2b30 3122 2063 793d 2231 2e37  610e+01" cy="1.7
+0000ccd0: 3032 3933 3337 3065 2b30 3122 2072 3d22  0293370e+01" r="
+0000cce0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000ccf0: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000cd00: 6972 636c 6520 6378 3d22 352e 3932 3030  ircle cx="5.9200
+0000cd10: 3937 3030 652b 3031 2220 6379 3d22 312e  9700e+01" cy="1.
+0000cd20: 3631 3636 3138 3330 652b 3031 2220 723d  61661830e+01" r=
+0000cd30: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000cd40: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000cd50: 6369 7263 6c65 2063 783d 2237 2e32 3232  circle cx="7.222
+0000cd60: 3438 3433 3065 2b30 3122 2063 793d 2232  48430e+01" cy="2
+0000cd70: 2e35 3235 3731 3832 3065 2b30 3122 2072  .52571820e+01" r
+0000cd80: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000cd90: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000cda0: 3c63 6972 636c 6520 6378 3d22 312e 3730  <circle cx="1.70
+0000cdb0: 3236 3937 3030 652b 3031 2220 6379 3d22  269700e+01" cy="
+0000cdc0: 362e 3536 3835 3734 3930 652b 3031 2220  6.56857490e+01" 
+0000cdd0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000cde0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000cdf0: 203c 6369 7263 6c65 2063 783d 2237 2e30   <circle cx="7.0
+0000ce00: 3431 3038 3339 3065 2b30 3122 2063 793d  4108390e+01" cy=
+0000ce10: 2232 2e31 3230 3832 3038 3065 2b30 3122  "2.12082080e+01"
+0000ce20: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000ce30: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000ce40: 2020 3c63 6972 636c 6520 6378 3d22 362e    <circle cx="6.
+0000ce50: 3831 3730 3137 3230 652b 3031 2220 6379  81701720e+01" cy
+0000ce60: 3d22 322e 3235 3838 3433 3930 652b 3031  ="2.25884390e+01
+0000ce70: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000ce80: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000ce90: 2020 203c 6369 7263 6c65 2063 783d 2237     <circle cx="7
+0000cea0: 2e38 3334 3236 3131 3065 2b30 3122 2063  .83426110e+01" c
+0000ceb0: 793d 2235 2e38 3331 3436 3332 3065 2b30  y="5.83146320e+0
+0000cec0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000ced0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000cee0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000cef0: 372e 3533 3734 3334 3830 652b 3031 2220  7.53743480e+01" 
+0000cf00: 6379 3d22 352e 3934 3931 3831 3430 652b  cy="5.94918140e+
+0000cf10: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000cf20: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000cf30: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000cf40: 2237 2e37 3431 3130 3834 3065 2b30 3122  "7.74110840e+01"
+0000cf50: 2063 793d 2233 2e31 3832 3737 3637 3065   cy="3.18277670e
+0000cf60: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000cf70: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000cf80: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000cf90: 3d22 362e 3334 3230 3035 3330 652b 3031  ="6.34200530e+01
+0000cfa0: 2220 6379 3d22 312e 3835 3633 3636 3630  " cy="1.85636660
+0000cfb0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000cfc0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000cfd0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000cfe0: 783d 2231 2e35 3331 3539 3038 3065 2b30  x="1.53159080e+0
+0000cff0: 3122 2063 793d 2234 2e31 3536 3835 3339  1" cy="4.1568539
+0000d000: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000d010: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000d020: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000d030: 6378 3d22 382e 3231 3131 3936 3430 652b  cx="8.21119640e+
+0000d040: 3031 2220 6379 3d22 352e 3031 3135 3430  01" cy="5.011540
+0000d050: 3730 652b 3031 2220 723d 2230 2e35 3336  70e+01" r="0.536
+0000d060: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000d070: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000d080: 2063 783d 2231 2e35 3936 3636 3335 3065   cx="1.59666350e
+0000d090: 2b30 3122 2063 793d 2234 2e34 3032 3631  +01" cy="4.40261
+0000d0a0: 3738 3065 2b30 3122 2072 3d22 302e 3533  780e+01" r="0.53
+0000d0b0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000d0c0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000d0d0: 6520 6378 3d22 382e 3137 3137 3330 3530  e cx="8.17173050
+0000d0e0: 652b 3031 2220 6379 3d22 352e 3336 3235  e+01" cy="5.3625
+0000d0f0: 3232 3730 652b 3031 2220 723d 2230 2e35  2270e+01" r="0.5
+0000d100: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000d110: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000d120: 6c65 2063 783d 2237 2e35 3038 3730 3539  le cx="7.5087059
+0000d130: 3065 2b30 3122 2063 793d 2235 2e35 3034  0e+01" cy="5.504
+0000d140: 3436 3731 3065 2b30 3122 2072 3d22 302e  46710e+01" r="0.
+0000d150: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000d160: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000d170: 636c 6520 6378 3d22 372e 3837 3739 3732  cle cx="7.877972
+0000d180: 3330 652b 3031 2220 6379 3d22 322e 3935  30e+01" cy="2.95
+0000d190: 3831 3435 3730 652b 3031 2220 723d 2230  814570e+01" r="0
+0000d1a0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000d1b0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000d1c0: 7263 6c65 2063 783d 2237 2e39 3431 3938  rcle cx="7.94198
+0000d1d0: 3033 3065 2b30 3122 2063 793d 2235 2e34  030e+01" cy="5.4
+0000d1e0: 3038 3238 3935 3065 2b30 3122 2072 3d22  0828950e+01" r="
+0000d1f0: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000d200: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000d210: 6972 636c 6520 6378 3d22 372e 3738 3132  ircle cx="7.7812
+0000d220: 3836 3230 652b 3031 2220 6379 3d22 352e  8620e+01" cy="5.
+0000d230: 3130 3437 3436 3530 652b 3031 2220 723d  10474650e+01" r=
+0000d240: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000d250: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000d260: 6369 7263 6c65 2063 783d 2235 2e36 3231  circle cx="5.621
+0000d270: 3134 3538 3065 2b30 3122 2063 793d 2231  14580e+01" cy="1
+0000d280: 2e36 3633 3038 3938 3065 2b30 3122 2072  .66308980e+01" r
+0000d290: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000d2a0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000d2b0: 3c63 6972 636c 6520 6378 3d22 362e 3432  <circle cx="6.42
+0000d2c0: 3333 3232 3130 652b 3031 2220 6379 3d22  332210e+01" cy="
+0000d2d0: 362e 3831 3730 3230 3830 652b 3031 2220  6.81702080e+01" 
+0000d2e0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000d2f0: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000d300: 203c 6369 7263 6c65 2063 783d 2236 2e34   <circle cx="6.4
+0000d310: 3739 3239 3034 3065 2b30 3122 2063 793d  7929040e+01" cy=
+0000d320: 2232 2e31 3232 3237 3730 3065 2b30 3122  "2.12227700e+01"
+0000d330: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000d340: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000d350: 2020 3c63 6972 636c 6520 6378 3d22 362e    <circle cx="6.
+0000d360: 3831 3339 3139 3430 652b 3031 2220 6379  81391940e+01" cy
+0000d370: 3d22 352e 3839 3033 3538 3330 652b 3031  ="5.89035830e+01
+0000d380: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000d390: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000d3a0: 2020 203c 6369 7263 6c65 2063 783d 2236     <circle cx="6
+0000d3b0: 2e39 3130 3237 3037 3065 2b30 3122 2063  .91027070e+01" c
+0000d3c0: 793d 2231 2e33 3438 3539 3032 3065 2b30  y="1.34859020e+0
+0000d3d0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000d3e0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000d3f0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000d400: 372e 3232 3132 3739 3230 652b 3031 2220  7.22127920e+01" 
+0000d410: 6379 3d22 352e 3834 3337 3536 3330 652b  cy="5.84375630e+
+0000d420: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000d430: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000d440: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000d450: 2233 2e38 3837 3033 3231 3065 2b30 3122  "3.88703210e+01"
+0000d460: 2063 793d 2238 2e32 3231 3733 3030 3065   cy="8.22173000e
+0000d470: 2b30 3022 2072 3d22 302e 3533 3638 3130  +00" r="0.536810
+0000d480: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000d490: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000d4a0: 3d22 362e 3630 3631 3037 3630 652b 3031  ="6.60610760e+01
+0000d4b0: 2220 6379 3d22 362e 3036 3032 3633 3930  " cy="6.06026390
+0000d4c0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000d4d0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000d4e0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000d4f0: 783d 2237 2e32 3134 3038 3031 3065 2b30  x="7.21408010e+0
+0000d500: 3122 2063 793d 2235 2e36 3138 3537 3030  1" cy="5.6185700
+0000d510: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000d520: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000d530: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000d540: 6378 3d22 372e 3630 3232 3237 3630 652b  cx="7.60222760e+
+0000d550: 3031 2220 6379 3d22 312e 3338 3937 3932  01" cy="1.389792
+0000d560: 3230 652b 3031 2220 723d 2230 2e35 3336  20e+01" r="0.536
+0000d570: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000d580: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000d590: 2063 783d 2234 2e35 3139 3832 3537 3065   cx="4.51982570e
+0000d5a0: 2b30 3122 2063 793d 2231 2e32 3039 3431  +01" cy="1.20941
+0000d5b0: 3837 3065 2b30 3122 2072 3d22 302e 3533  870e+01" r="0.53
+0000d5c0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000d5d0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000d5e0: 6520 6378 3d22 352e 3130 3734 3235 3830  e cx="5.10742580
+0000d5f0: 652b 3031 2220 6379 3d22 322e 3130 3230  e+01" cy="2.1020
+0000d600: 3737 3430 652b 3031 2220 723d 2230 2e35  7740e+01" r="0.5
+0000d610: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000d620: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000d630: 6c65 2063 783d 2236 2e38 3134 3432 3739  le cx="6.8144279
+0000d640: 3065 2b30 3122 2063 793d 2236 2e34 3235  0e+01" cy="6.425
+0000d650: 3936 3030 3065 2b30 3122 2072 3d22 302e  96000e+01" r="0.
+0000d660: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000d670: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000d680: 636c 6520 6378 3d22 372e 3830 3938 3538  cle cx="7.809858
+0000d690: 3530 652b 3031 2220 6379 3d22 342e 3735  50e+01" cy="4.75
+0000d6a0: 3536 3034 3130 652b 3031 2220 723d 2230  560410e+01" r="0
+0000d6b0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000d6c0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000d6d0: 7263 6c65 2063 783d 2237 2e30 3235 3639  rcle cx="7.02569
+0000d6e0: 3438 3065 2b30 3122 2063 793d 2236 2e32  480e+01" cy="6.2
+0000d6f0: 3438 3138 3339 3065 2b30 3122 2072 3d22  4818390e+01" r="
+0000d700: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000d710: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000d720: 6972 636c 6520 6378 3d22 352e 3231 3434  ircle cx="5.2144
+0000d730: 3639 3130 652b 3031 2220 6379 3d22 312e  6910e+01" cy="1.
+0000d740: 3930 3339 3331 3630 652b 3031 2220 723d  90393160e+01" r=
+0000d750: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000d760: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000d770: 6369 7263 6c65 2063 783d 2236 2e31 3536  circle cx="6.156
+0000d780: 3237 3431 3065 2b30 3122 2063 793d 2238  27410e+01" cy="8
+0000d790: 2e35 3734 3432 3230 3065 2b30 3022 2072  .57442200e+00" r
+0000d7a0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000d7b0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000d7c0: 3c63 6972 636c 6520 6378 3d22 362e 3630  <circle cx="6.60
+0000d7d0: 3135 3834 3230 652b 3031 2220 6379 3d22  158420e+01" cy="
+0000d7e0: 362e 3332 3937 3431 3030 652b 3031 2220  6.32974100e+01" 
+0000d7f0: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000d800: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000d810: 203c 6369 7263 6c65 2063 783d 2237 2e30   <circle cx="7.0
+0000d820: 3239 3236 3936 3065 2b30 3122 2063 793d  2926960e+01" cy=
+0000d830: 2235 2e39 3731 3831 3130 3065 2b30 3122  "5.97181100e+01"
+0000d840: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000d850: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000d860: 2020 3c63 6972 636c 6520 6378 3d22 382e    <circle cx="8.
+0000d870: 3033 3031 3936 3530 652b 3031 2220 6379  03019650e+01" cy
+0000d880: 3d22 342e 3730 3339 3833 3730 652b 3031  ="4.70398370e+01
+0000d890: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000d8a0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000d8b0: 2020 203c 6369 7263 6c65 2063 783d 2238     <circle cx="8
+0000d8c0: 2e33 3439 3832 3739 3065 2b30 3122 2063  .34982790e+01" c
+0000d8d0: 793d 2239 2e30 3032 3335 3430 3065 2b30  y="9.00235400e+0
+0000d8e0: 3022 2072 3d22 302e 3533 3638 3130 3436  0" r="0.53681046
+0000d8f0: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000d900: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000d910: 352e 3734 3132 3736 3930 652b 3031 2220  5.74127690e+01" 
+0000d920: 6379 3d22 372e 3030 3635 3536 3330 652b  cy="7.00655630e+
+0000d930: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000d940: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000d950: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000d960: 2235 2e35 3133 3735 3531 3065 2b30 3122  "5.51375510e+01"
+0000d970: 2063 793d 2231 2e32 3632 3234 3531 3065   cy="1.26224510e
+0000d980: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000d990: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000d9a0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000d9b0: 3d22 352e 3035 3130 3231 3030 652b 3031  ="5.05102100e+01
+0000d9c0: 2220 6379 3d22 372e 3938 3239 3731 3730  " cy="7.98297170
+0000d9d0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000d9e0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000d9f0: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000da00: 783d 2236 2e31 3431 3832 3733 3065 2b30  x="6.14182730e+0
+0000da10: 3122 2063 793d 2236 2e38 3130 3938 3336  1" cy="6.8109836
+0000da20: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000da30: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000da40: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000da50: 6378 3d22 332e 3238 3730 3330 3930 652b  cx="3.28703090e+
+0000da60: 3031 2220 6379 3d22 312e 3432 3231 3732  01" cy="1.422172
+0000da70: 3430 652b 3031 2220 723d 2230 2e35 3336  40e+01" r="0.536
+0000da80: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000da90: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000daa0: 2063 783d 2235 2e32 3930 3130 3639 3065   cx="5.29010690e
+0000dab0: 2b30 3122 2063 793d 2237 2e36 3230 3234  +01" cy="7.62024
+0000dac0: 3734 3065 2b30 3122 2072 3d22 302e 3533  740e+01" r="0.53
+0000dad0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000dae0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000daf0: 6520 6378 3d22 312e 3835 3030 3030 3030  e cx="1.85000000
+0000db00: 652b 3031 2220 6379 3d22 312e 3130 3030  e+01" cy="1.1000
+0000db10: 3030 3330 652b 3031 2220 723d 2230 2e35  0030e+01" r="0.5
+0000db20: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000db30: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000db40: 6c65 2063 783d 2239 2e30 3433 3037 3930  le cx="9.0430790
+0000db50: 3065 2b30 3122 2063 793d 2235 2e39 3838  0e+01" cy="5.988
+0000db60: 3139 3733 3065 2b30 3122 2072 3d22 302e  19730e+01" r="0.
+0000db70: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000db80: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000db90: 636c 6520 6378 3d22 342e 3531 3838 3931  cle cx="4.518891
+0000dba0: 3530 652b 3031 2220 6379 3d22 372e 3834  50e+01" cy="7.84
+0000dbb0: 3535 3934 3830 652b 3031 2220 723d 2230  559480e+01" r="0
+0000dbc0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000dbd0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000dbe0: 7263 6c65 2063 783d 2236 2e30 3834 3531  rcle cx="6.08451
+0000dbf0: 3731 3065 2b30 3122 2063 793d 2236 2e33  710e+01" cy="6.3
+0000dc00: 3736 3439 3432 3065 2b30 3122 2072 3d22  7649420e+01" r="
+0000dc10: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000dc20: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000dc30: 6972 636c 6520 6378 3d22 352e 3731 3630  ircle cx="5.7160
+0000dc40: 3937 3630 652b 3031 2220 6379 3d22 372e  9760e+01" cy="7.
+0000dc50: 3531 3338 3333 3230 652b 3031 2220 723d  51383320e+01" r=
+0000dc60: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000dc70: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000dc80: 6369 7263 6c65 2063 783d 2234 2e39 3839  circle cx="4.989
+0000dc90: 3733 3337 3065 2b30 3122 2063 793d 2231  73370e+01" cy="1
+0000dca0: 2e32 3838 3937 3936 3065 2b30 3122 2072  .28897960e+01" r
+0000dcb0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000dcc0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000dcd0: 3c63 6972 636c 6520 6378 3d22 322e 3735  <circle cx="2.75
+0000dce0: 3030 3030 3930 652b 3031 2220 6379 3d22  000090e+01" cy="
+0000dcf0: 312e 3639 3939 3939 3730 652b 3031 2220  1.69999970e+01" 
+0000dd00: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000dd10: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000dd20: 203c 6369 7263 6c65 2063 783d 2232 2e31   <circle cx="2.1
+0000dd30: 3030 3538 3739 3065 2b30 3122 2063 793d  0058790e+01" cy=
+0000dd40: 2236 2e32 3338 3833 3536 3065 2b30 3122  "6.23883560e+01"
+0000dd50: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000dd60: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000dd70: 2020 3c63 6972 636c 6520 6378 3d22 312e    <circle cx="1.
+0000dd80: 3939 3438 3038 3230 652b 3031 2220 6379  99480820e+01" cy
+0000dd90: 3d22 362e 3639 3131 3637 3530 652b 3031  ="6.69116750e+01
+0000dda0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000ddb0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000ddc0: 2020 203c 6369 7263 6c65 2063 783d 2238     <circle cx="8
+0000ddd0: 2e36 3237 3734 3739 3065 2b30 3122 2063  .62774790e+01" c
+0000dde0: 793d 2235 2e31 3233 3530 3037 3065 2b30  y="5.12350070e+0
+0000ddf0: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000de00: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000de10: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000de20: 322e 3939 3030 3136 3530 652b 3031 2220  2.99001650e+01" 
+0000de30: 6379 3d22 372e 3539 3131 3139 3830 652b  cy="7.59111980e+
+0000de40: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000de50: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000de60: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000de70: 2232 2e35 3133 3234 3432 3065 2b30 3122  "2.51324420e+01"
+0000de80: 2063 793d 2237 2e34 3835 3134 3132 3065   cy="7.48514120e
+0000de90: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000dea0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000deb0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000dec0: 3d22 332e 3735 3930 3333 3230 652b 3031  ="3.75903320e+01
+0000ded0: 2220 6379 3d22 372e 3839 3533 3030 3930  " cy="7.89530090
+0000dee0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000def0: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000df00: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000df10: 783d 2233 2e33 3035 3333 3531 3065 2b30  x="3.30533510e+0
+0000df20: 3122 2063 793d 2237 2e39 3939 3630 3832  1" cy="7.9996082
+0000df30: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000df40: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000df50: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000df60: 6378 3d22 392e 3036 3433 3434 3230 652b  cx="9.06434420e+
+0000df70: 3031 2220 6379 3d22 382e 3331 3439 3139  01" cy="8.314919
+0000df80: 3630 652b 3031 2220 723d 2230 2e35 3336  60e+01" r="0.536
+0000df90: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000dfa0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000dfb0: 2063 783d 2238 2e34 3832 3137 3032 3065   cx="8.48217020e
+0000dfc0: 2b30 3122 2063 793d 2237 2e34 3536 3133  +01" cy="7.45613
+0000dfd0: 3630 3065 2b30 3122 2072 3d22 302e 3533  600e+01" r="0.53
+0000dfe0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000dff0: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000e000: 6520 6378 3d22 392e 3133 3837 3935 3830  e cx="9.13879580
+0000e010: 652b 3031 2220 6379 3d22 332e 3833 3930  e+01" cy="3.8390
+0000e020: 3537 3630 652b 3031 2220 723d 2230 2e35  5760e+01" r="0.5
+0000e030: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000e040: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000e050: 6c65 2063 783d 2238 2e36 3436 3930 3632  le cx="8.6469062
+0000e060: 3065 2b30 3122 2063 793d 2233 2e30 3835  0e+01" cy="3.085
+0000e070: 3735 3439 3065 2b30 3122 2072 3d22 302e  75490e+01" r="0.
+0000e080: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000e090: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000e0a0: 636c 6520 6378 3d22 382e 3630 3935 3832  cle cx="8.609582
+0000e0b0: 3330 652b 3031 2220 6379 3d22 322e 3339  30e+01" cy="2.39
+0000e0c0: 3733 3635 3630 652b 3031 2220 723d 2230  736560e+01" r="0
+0000e0d0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000e0e0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000e0f0: 7263 6c65 2063 783d 2238 2e37 3232 3036  rcle cx="8.72206
+0000e100: 3136 3065 2b30 3122 2063 793d 2234 2e34  160e+01" cy="4.4
+0000e110: 3737 3136 3330 3065 2b30 3122 2072 3d22  7716300e+01" r="
+0000e120: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000e130: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000e140: 6972 636c 6520 6378 3d22 322e 3430 3830  ircle cx="2.4080
+0000e150: 3630 3330 652b 3031 2220 6379 3d22 372e  6030e+01" cy="7.
+0000e160: 3030 3933 3832 3330 652b 3031 2220 723d  00938230e+01" r=
+0000e170: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000e180: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000e190: 6369 7263 6c65 2063 783d 2239 2e30 3939  circle cx="9.099
+0000e1a0: 3832 3835 3065 2b30 3122 2063 793d 2231  82850e+01" cy="1
+0000e1b0: 2e36 3530 3233 3630 3065 2b30 3122 2072  .65023600e+01" r
+0000e1c0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000e1d0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000e1e0: 3c63 6972 636c 6520 6378 3d22 382e 3436  <circle cx="8.46
+0000e1f0: 3031 3237 3430 652b 3031 2220 6379 3d22  012740e+01" cy="
+0000e200: 362e 3632 3739 3033 3830 652b 3031 2220  6.62790380e+01" 
+0000e210: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000e220: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000e230: 203c 6369 7263 6c65 2063 783d 2232 2e30   <circle cx="2.0
+0000e240: 3837 3330 3636 3065 2b30 3122 2063 793d  8730660e+01" cy=
+0000e250: 2234 2e35 3832 3833 3230 3065 2b30 3122  "4.58283200e+01"
+0000e260: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000e270: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000e280: 2020 3c63 6972 636c 6520 6378 3d22 312e    <circle cx="1.
+0000e290: 3830 3934 3138 3130 652b 3031 2220 6379  80941810e+01" cy
+0000e2a0: 3d22 342e 3231 3938 3233 3330 652b 3031  ="4.21982330e+01
+0000e2b0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000e2c0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000e2d0: 2020 203c 6369 7263 6c65 2063 783d 2232     <circle cx="2
+0000e2e0: 2e30 3232 3137 3237 3065 2b30 3122 2063  .02217270e+01" c
+0000e2f0: 793d 2233 2e37 3337 3033 3030 3065 2b30  y="3.73703000e+0
+0000e300: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000e310: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000e320: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000e330: 352e 3132 3331 3338 3030 652b 3031 2220  5.12313800e+01" 
+0000e340: 6379 3d22 382e 3632 3830 3838 3931 652b  cy="8.62808891e+
+0000e350: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000e360: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000e370: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000e380: 2235 2e39 3837 3839 3133 3065 2b30 3122  "5.98789130e+01"
+0000e390: 2063 793d 2239 2e30 3433 3337 3830 3765   cy="9.04337807e
+0000e3a0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000e3b0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000e3c0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000e3d0: 3d22 312e 3639 3939 3939 3730 652b 3031  ="1.69999970e+01
+0000e3e0: 2220 6379 3d22 322e 3735 3030 3030 3030  " cy="2.75000000
+0000e3f0: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000e400: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000e410: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000e420: 783d 2238 2e33 3134 3334 3435 3065 2b30  x="8.31434450e+0
+0000e430: 3122 2063 793d 2239 2e30 3634 3931 3935  1" cy="9.0649195
+0000e440: 3765 2b30 3122 2072 3d22 302e 3533 3638  7e+01" r="0.5368
+0000e450: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000e460: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000e470: 6378 3d22 322e 3130 3234 3036 3830 652b  cx="2.10240680e+
+0000e480: 3031 2220 6379 3d22 352e 3430 3738 3534  01" cy="5.407854
+0000e490: 3830 652b 3031 2220 723d 2230 2e35 3336  80e+01" r="0.536
+0000e4a0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000e4b0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000e4c0: 2063 783d 2234 2e34 3737 3035 3935 3065   cx="4.47705950e
+0000e4d0: 2b30 3122 2063 793d 2238 2e37 3232 3036  +01" cy="8.72206
+0000e4e0: 3733 3665 2b30 3122 2072 3d22 302e 3533  736e+01" r="0.53
+0000e4f0: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000e500: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000e510: 6520 6378 3d22 362e 3632 3636 3735 3330  e cx="6.62667530
+0000e520: 652b 3031 2220 6379 3d22 382e 3436 3133  e+01" cy="8.4613
+0000e530: 3337 3030 652b 3031 2220 723d 2230 2e35  3700e+01" r="0.5
+0000e540: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000e550: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000e560: 6c65 2063 783d 2237 2e34 3534 3634 3032  le cx="7.4546402
+0000e570: 3065 2b30 3122 2063 793d 2238 2e34 3833  0e+01" cy="8.483
+0000e580: 3636 3630 3065 2b30 3122 2072 3d22 302e  66600e+01" r="0.
+0000e590: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000e5a0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000e5b0: 636c 6520 6378 3d22 332e 3038 3535 3531  cle cx="3.085551
+0000e5c0: 3530 652b 3031 2220 6379 3d22 382e 3634  50e+01" cy="8.64
+0000e5d0: 3637 3132 3838 652b 3031 2220 723d 2230  671288e+01" r="0
+0000e5e0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000e5f0: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000e600: 7263 6c65 2063 783d 2232 2e33 3936 3939  rcle cx="2.39699
+0000e610: 3330 3065 2b30 3122 2063 793d 2238 2e36  300e+01" cy="8.6
+0000e620: 3039 3231 3137 3765 2b30 3122 2072 3d22  0921177e+01" r="
+0000e630: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000e640: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000e650: 6972 636c 6520 6378 3d22 312e 3635 3030  ircle cx="1.6500
+0000e660: 3231 3830 652b 3031 2220 6379 3d22 392e  2180e+01" cy="9.
+0000e670: 3039 3936 3134 3636 652b 3031 2220 723d  09961466e+01" r=
+0000e680: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000e690: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000e6a0: 6369 7263 6c65 2063 783d 2231 2e34 3232  circle cx="1.422
+0000e6b0: 3137 3234 3065 2b30 3122 2063 793d 2233  17240e+01" cy="3
+0000e6c0: 2e32 3837 3033 3030 3065 2b30 3122 2072  .28703000e+01" r
+0000e6d0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000e6e0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000e6f0: 3c63 6972 636c 6520 6378 3d22 332e 3833  <circle cx="3.83
+0000e700: 3930 3130 3830 652b 3031 2220 6379 3d22  901080e+01" cy="
+0000e710: 392e 3133 3837 3539 3137 652b 3031 2220  9.13875917e+01" 
+0000e720: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000e730: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000e740: 203c 6369 7263 6c65 2063 783d 2236 2e33   <circle cx="6.3
+0000e750: 3735 3539 3333 3065 2b30 3122 2063 793d  7559330e+01" cy=
+0000e760: 2236 2e30 3835 3430 3237 3065 2b30 3122  "6.08540270e+01"
+0000e770: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000e780: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000e790: 2020 3c63 6972 636c 6520 6378 3d22 312e    <circle cx="1.
+0000e7a0: 3130 3030 3030 3033 652b 3031 2220 6379  10000003e+01" cy
+0000e7b0: 3d22 312e 3835 3030 3030 3030 652b 3031  ="1.85000000e+01
+0000e7c0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000e7d0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000e7e0: 2020 203c 6369 7263 6c65 2063 783d 2238     <circle cx="8
+0000e7f0: 2e32 3231 3732 3634 3065 2b30 3022 2063  .22172640e+00" c
+0000e800: 793d 2233 2e38 3837 3032 3934 3065 2b30  y="3.88702940e+0
+0000e810: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000e820: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000e830: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000e840: 312e 3236 3232 3034 3234 652b 3031 2220  1.26220424e+01" 
+0000e850: 6379 3d22 352e 3531 3337 3132 3830 652b  cy="5.51371280e+
+0000e860: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000e870: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000e880: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000e890: 2231 2e32 3039 3431 3832 3565 2b30 3122  "1.20941825e+01"
+0000e8a0: 2063 793d 2234 2e35 3139 3832 3330 3065   cy="4.51982300e
+0000e8b0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000e8c0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000e8d0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000e8e0: 3d22 382e 3537 3430 3236 3930 652b 3030  ="8.57402690e+00
+0000e8f0: 2220 6379 3d22 362e 3135 3632 3331 3830  " cy="6.15623180
+0000e900: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000e910: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000e920: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000e930: 783d 2238 2e31 3231 3537 3839 3065 2b30  x="8.12157890e+0
+0000e940: 3122 2063 793d 2234 2e31 3735 3032 3934  1" cy="4.1750294
+0000e950: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000e960: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000e970: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000e980: 6378 3d22 342e 3137 3439 3238 3630 652b  cx="4.17492860e+
+0000e990: 3031 2220 6379 3d22 382e 3132 3135 3833  01" cy="8.121583
+0000e9a0: 3430 652b 3031 2220 723d 2230 2e35 3336  40e+01" r="0.536
+0000e9b0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000e9c0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000e9d0: 2063 783d 2231 2e38 3839 3231 3834 3065   cx="1.88921840e
+0000e9e0: 2b30 3122 2063 793d 2234 2e39 3839 3939  +01" cy="4.98999
+0000e9f0: 3635 3065 2b30 3122 2072 3d22 302e 3533  650e+01" r="0.53
+0000ea00: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000ea10: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000ea20: 6520 6378 3d22 372e 3834 3535 3631 3530  e cx="7.84556150
+0000ea30: 652b 3031 2220 6379 3d22 342e 3531 3839  e+01" cy="4.5189
+0000ea40: 3530 3030 652b 3031 2220 723d 2230 2e35  5000e+01" r="0.5
+0000ea50: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000ea60: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000ea70: 6c65 2063 783d 2231 2e32 3838 3937 3934  le cx="1.2889794
+0000ea80: 3265 2b30 3122 2063 793d 2234 2e39 3839  2e+01" cy="4.989
+0000ea90: 3733 3130 3065 2b30 3122 2072 3d22 302e  73100e+01" r="0.
+0000eaa0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000eab0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000eac0: 636c 6520 6378 3d22 372e 3839 3533 3334  cle cx="7.895334
+0000ead0: 3230 652b 3031 2220 6379 3d22 332e 3735  20e+01" cy="3.75
+0000eae0: 3930 3738 3230 652b 3031 2220 723d 2230  907820e+01" r="0
+0000eaf0: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000eb00: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000eb10: 7263 6c65 2063 783d 2231 2e38 3631 3638  rcle cx="1.86168
+0000eb20: 3734 3065 2b30 3122 2063 793d 2235 2e38  740e+01" cy="5.8
+0000eb30: 3132 3231 3034 3065 2b30 3122 2072 3d22  1221040e+01" r="
+0000eb40: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000eb50: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000eb60: 6972 636c 6520 6378 3d22 312e 3338 3934  ircle cx="1.3894
+0000eb70: 3231 3331 652b 3031 2220 6379 3d22 372e  2131e+01" cy="7.
+0000eb80: 3630 3138 3534 3130 652b 3031 2220 723d  60185410e+01" r=
+0000eb90: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000eba0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000ebb0: 6369 7263 6c65 2063 783d 2239 2e30 3030  circle cx="9.000
+0000ebc0: 3232 3130 3065 2b30 3022 2063 793d 2238  22100e+00" cy="8
+0000ebd0: 2e33 3439 3631 3436 3065 2b30 3122 2072  .34961460e+01" r
+0000ebe0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000ebf0: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000ec00: 3c63 6972 636c 6520 6378 3d22 312e 3334  <circle cx="1.34
+0000ec10: 3833 3933 3139 652b 3031 2220 6379 3d22  839319e+01" cy="
+0000ec20: 362e 3931 3030 3731 3830 652b 3031 2220  6.91007180e+01" 
+0000ec30: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000ec40: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000ec50: 203c 6369 7263 6c65 2063 783d 2234 2e39   <circle cx="4.9
+0000ec60: 3839 3939 3833 3065 2b30 3122 2063 793d  8999830e+01" cy=
+0000ec70: 2231 2e38 3839 3231 3834 3065 2b30 3122  "1.88921840e+01"
+0000ec80: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000ec90: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000eca0: 2020 3c63 6972 636c 6520 6378 3d22 372e    <circle cx="7.
+0000ecb0: 3632 3234 3635 3930 652b 3031 2220 6379  62246590e+01" cy
+0000ecc0: 3d22 372e 3632 3438 3832 3430 652b 3031  ="7.62488240e+01
+0000ecd0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000ece0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000ecf0: 2020 203c 6369 7263 6c65 2063 783d 2236     <circle cx="6
+0000ed00: 2e32 3338 3837 3631 3065 2b30 3122 2063  .23887610e+01" c
+0000ed10: 793d 2232 2e31 3030 3632 3438 3065 2b30  y="2.10062480e+0
+0000ed20: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000ed30: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000ed40: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000ed50: 322e 3133 3630 3230 3930 652b 3031 2220  2.13602090e+01" 
+0000ed60: 6379 3d22 372e 3836 3139 3531 3430 652b  cy="7.86195140e+
+0000ed70: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000ed80: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000ed90: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000eda0: 2234 2e32 3139 3832 3531 3065 2b30 3122  "4.21982510e+01"
+0000edb0: 2063 793d 2231 2e38 3039 3431 3831 3065   cy="1.80941810e
+0000edc0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000edd0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000ede0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000edf0: 3d22 352e 3831 3232 3530 3930 652b 3031  ="5.81225090e+01
+0000ee00: 2220 6379 3d22 312e 3836 3137 3238 3830  " cy="1.86172880
+0000ee10: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000ee20: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000ee30: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000ee40: 783d 2233 2e37 3337 3033 3039 3065 2b30  x="3.73703090e+0
+0000ee50: 3122 2063 793d 2232 2e30 3232 3137 3237  1" cy="2.0221727
+0000ee60: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000ee70: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000ee80: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000ee90: 6378 3d22 342e 3538 3238 3332 3930 652b  cx="4.58283290e+
+0000eea0: 3031 2220 6379 3d22 322e 3038 3733 3036  01" cy="2.087306
+0000eeb0: 3630 652b 3031 2220 723d 2230 2e35 3336  60e+01" r="0.536
+0000eec0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000eed0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000eee0: 2063 783d 2236 2e35 3239 3534 3436 3065   cx="6.52954460e
+0000eef0: 2b30 3122 2063 793d 2237 2e32 3031 3530  +01" cy="7.20150
+0000ef00: 3038 3065 2b30 3122 2072 3d22 302e 3533  080e+01" r="0.53
+0000ef10: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000ef20: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000ef30: 6520 6378 3d22 372e 3139 3839 3038 3830  e cx="7.19890880
+0000ef40: 652b 3031 2220 6379 3d22 362e 3533 3231  e+01" cy="6.5321
+0000ef50: 3333 3930 652b 3031 2220 723d 2230 2e35  3390e+01" r="0.5
+0000ef60: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000ef70: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000ef80: 6c65 2063 783d 2235 2e34 3037 3835 3537  le cx="5.4078557
+0000ef90: 3065 2b30 3122 2063 793d 2232 2e31 3032  0e+01" cy="2.102
+0000efa0: 3430 3638 3065 2b30 3122 2072 3d22 302e  40680e+01" r="0.
+0000efb0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000efc0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000efd0: 636c 6520 6378 3d22 372e 3039 3135 3930  cle cx="7.091590
+0000efe0: 3130 652b 3031 2220 6379 3d22 372e 3039  10e+01" cy="7.09
+0000eff0: 3433 3738 3330 652b 3031 2220 723d 2230  437830e+01" r="0
+0000f000: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000f010: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000f020: 7263 6c65 2063 783d 2236 2e32 3333 3436  rcle cx="6.23346
+0000f030: 3938 3065 2b30 3122 2063 793d 2237 2e37  980e+01" cy="7.7
+0000f040: 3130 3731 3237 3065 2b30 3122 2072 3d22  1071270e+01" r="
+0000f050: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000f060: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000f070: 6972 636c 6520 6378 3d22 372e 3730 3837  ircle cx="7.7087
+0000f080: 3733 3230 652b 3031 2220 6379 3d22 362e  7320e+01" cy="6.
+0000f090: 3233 3534 3236 3430 652b 3031 2220 723d  23542640e+01" r=
+0000f0a0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000f0b0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000f0c0: 6369 7263 6c65 2063 783d 2237 2e38 3632  circle cx="7.862
+0000f0d0: 3438 3135 3065 2b30 3122 2063 793d 2232  48150e+01" cy="2
+0000f0e0: 2e31 3336 3535 3139 3065 2b30 3122 2072  .13655190e+01" r
+0000f0f0: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000f100: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000f110: 3c63 6972 636c 6520 6378 3d22 372e 3939  <circle cx="7.99
+0000f120: 3938 3034 3430 652b 3031 2220 6379 3d22  980440e+01" cy="
+0000f130: 332e 3330 3535 3332 3230 652b 3031 2220  3.30553220e+01" 
+0000f140: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000f150: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000f160: 203c 6369 7263 6c65 2063 783d 2236 2e38   <circle cx="6.8
+0000f170: 3039 3336 3831 3065 2b30 3122 2063 793d  0936810e+01" cy=
+0000f180: 2236 2e31 3433 3436 3335 3065 2b30 3122  "6.14346350e+01"
+0000f190: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000f1a0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000f1b0: 2020 3c63 6972 636c 6520 6378 3d22 372e    <circle cx="7.
+0000f1c0: 3030 3537 3939 3430 652b 3031 2220 6379  00579940e+01" cy
+0000f1d0: 3d22 352e 3734 3139 3936 3030 652b 3031  ="5.74199600e+01
+0000f1e0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000f1f0: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000f200: 2020 203c 6369 7263 6c65 2063 783d 2236     <circle cx="6
+0000f210: 2e36 3931 3336 3130 3065 2b30 3122 2063  .69136100e+01" c
+0000f220: 793d 2231 2e39 3935 3030 3830 3065 2b30  y="1.99500800e+0
+0000f230: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000f240: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000f250: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000f260: 372e 3531 3238 3039 3030 652b 3031 2220  7.51280900e+01" 
+0000f270: 6379 3d22 352e 3731 3730 3834 3930 652b  cy="5.71708490e+
+0000f280: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000f290: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000f2a0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000f2b0: 2237 2e36 3139 3934 3638 3065 2b30 3122  "7.61994680e+01"
+0000f2c0: 2063 793d 2235 2e32 3930 3431 3734 3065   cy="5.29041740e
+0000f2d0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000f2e0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000f2f0: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000f300: 3d22 372e 3539 3132 3732 3830 652b 3031  ="7.59127280e+01
+0000f310: 2220 6379 3d22 322e 3939 3031 3833 3030  " cy="2.99018300
+0000f320: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000f330: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000f340: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000f350: 783d 2237 2e30 3039 3534 3739 3065 2b30  x="7.00954790e+0
+0000f360: 3122 2063 793d 2232 2e34 3038 3231 3432  1" cy="2.4082142
+0000f370: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000f380: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000f390: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000f3a0: 6378 3d22 372e 3938 3236 3339 3630 652b  cx="7.98263960e+
+0000f3b0: 3031 2220 6379 3d22 352e 3035 3133 3831  01" cy="5.051381
+0000f3c0: 3030 652b 3031 2220 723d 2230 2e35 3336  00e+01" r="0.536
+0000f3d0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000f3e0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000f3f0: 2063 783d 2237 2e34 3835 3435 3038 3065   cx="7.48545080e
+0000f400: 2b30 3122 2063 793d 2232 2e35 3133 3535  +01" cy="2.51355
+0000f410: 3437 3065 2b30 3122 2072 3d22 302e 3533  470e+01" r="0.53
+0000f420: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000f430: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000f440: 6520 6378 3d22 372e 3730 3030 3030 3030  e cx="7.70000000
+0000f450: 652b 3031 2220 6379 3d22 332e 3836 3736  e+01" cy="3.8676
+0000f460: 3835 3730 652b 3031 2220 723d 2230 2e35  8570e+01" r="0.5
+0000f470: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000f480: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000f490: 6c65 2063 783d 2237 2e36 3535 3534 3831  le cx="7.6555481
+0000f4a0: 3065 2b30 3122 2063 793d 2233 2e36 3334  0e+01" cy="3.634
+0000f4b0: 3634 3234 3065 2b30 3122 2072 3d22 302e  64240e+01" r="0.
+0000f4c0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000f4d0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000f4e0: 636c 6520 6378 3d22 372e 3536 3239 3833  cle cx="7.562983
+0000f4f0: 3130 652b 3031 2220 6379 3d22 332e 3431  10e+01" cy="3.41
+0000f500: 3131 3639 3730 652b 3031 2220 723d 2230  116970e+01" r="0
+0000f510: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000f520: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000f530: 7263 6c65 2063 783d 2237 2e34 3732 3832  rcle cx="7.47282
+0000f540: 3734 3065 2b30 3122 2063 793d 2233 2e31  740e+01" cy="3.1
+0000f550: 3933 3531 3535 3065 2b30 3122 2072 3d22  9351550e+01" r="
+0000f560: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000f570: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000f580: 6972 636c 6520 6378 3d22 372e 3334 3135  ircle cx="7.3415
+0000f590: 3735 3030 652b 3031 2220 6379 3d22 322e  7500e+01" cy="2.
+0000f5a0: 3939 3539 3930 3730 652b 3031 2220 723d  99599070e+01" r=
+0000f5b0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000f5c0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000f5d0: 6369 7263 6c65 2063 783d 2237 2e31 3732  circle cx="7.172
+0000f5e0: 3739 3236 3065 2b30 3122 2063 793d 2232  79260e+01" cy="2
+0000f5f0: 2e38 3237 3230 3833 3065 2b30 3122 2072  .82720830e+01" r
+0000f600: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000f610: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000f620: 3c63 6972 636c 6520 6378 3d22 372e 3030  <circle cx="7.00
+0000f630: 3430 3039 3330 652b 3031 2220 6379 3d22  400930e+01" cy="
+0000f640: 322e 3635 3834 3235 3030 652b 3031 2220  2.65842500e+01" 
+0000f650: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000f660: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000f670: 203c 6369 7263 6c65 2063 783d 2236 2e38   <circle cx="6.8
+0000f680: 3036 3438 3435 3065 2b30 3122 2063 793d  0648450e+01" cy=
+0000f690: 2232 2e35 3237 3137 3236 3065 2b30 3122  "2.52717260e+01"
+0000f6a0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000f6b0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000f6c0: 2020 3c63 6972 636c 6520 6378 3d22 362e    <circle cx="6.
+0000f6d0: 3538 3838 3330 3330 652b 3031 2220 6379  58883030e+01" cy
+0000f6e0: 3d22 322e 3433 3730 3136 3930 652b 3031  ="2.43701690e+01
+0000f6f0: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000f700: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000f710: 2020 203c 6369 7263 6c65 2063 783d 2236     <circle cx="6
+0000f720: 2e33 3635 3335 3736 3065 2b30 3122 2063  .36535760e+01" c
+0000f730: 793d 2232 2e33 3434 3435 3139 3065 2b30  y="2.34445190e+0
+0000f740: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000f750: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000f760: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000f770: 362e 3133 3233 3134 3330 652b 3031 2220  6.13231430e+01" 
+0000f780: 6379 3d22 322e 3330 3030 3030 3030 652b  cy="2.30000000e+
+0000f790: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000f7a0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000f7b0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000f7c0: 2235 2e36 3030 3030 3033 3065 2b30 3122  "5.60000030e+01"
+0000f7d0: 2063 793d 2232 2e33 3030 3030 3030 3065   cy="2.30000000e
+0000f7e0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000f7f0: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000f800: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000f810: 3d22 352e 3239 3939 3939 3730 652b 3031  ="5.29999970e+01
+0000f820: 2220 6379 3d22 322e 3330 3030 3030 3030  " cy="2.30000000
+0000f830: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000f840: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000f850: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000f860: 783d 2235 2e30 3030 3030 3030 3065 2b30  x="5.00000000e+0
+0000f870: 3122 2063 793d 2232 2e33 3030 3030 3030  1" cy="2.3000000
+0000f880: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000f890: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000f8a0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000f8b0: 6378 3d22 342e 3730 3030 3030 3330 652b  cx="4.70000030e+
+0000f8c0: 3031 2220 6379 3d22 322e 3330 3030 3030  01" cy="2.300000
+0000f8d0: 3030 652b 3031 2220 723d 2230 2e35 3336  00e+01" r="0.536
+0000f8e0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000f8f0: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000f900: 2063 783d 2234 2e34 3030 3030 3036 3065   cx="4.40000060e
+0000f910: 2b30 3122 2063 793d 2232 2e33 3030 3030  +01" cy="2.30000
+0000f920: 3030 3065 2b30 3122 2072 3d22 302e 3533  000e+01" r="0.53
+0000f930: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000f940: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000f950: 6520 6378 3d22 342e 3130 3030 3030 3930  e cx="4.10000090
+0000f960: 652b 3031 2220 6379 3d22 322e 3330 3030  e+01" cy="2.3000
+0000f970: 3030 3030 652b 3031 2220 723d 2230 2e35  0000e+01" r="0.5
+0000f980: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000f990: 202f 3e0d 0a20 2020 2020 203c 6369 7263   />..      <circ
+0000f9a0: 6c65 2063 783d 2233 2e38 3030 3030 3033  le cx="3.8000003
+0000f9b0: 3065 2b30 3122 2063 793d 2232 2e33 3030  0e+01" cy="2.300
+0000f9c0: 3030 3030 3065 2b30 3122 2072 3d22 302e  00000e+01" r="0.
+0000f9d0: 3533 3638 3130 3436 3533 3738 3131 3737  5368104653781177
+0000f9e0: 2220 2f3e 0d0a 2020 2020 2020 3c63 6972  " />..      <cir
+0000f9f0: 636c 6520 6378 3d22 332e 3530 3030 3030  cle cx="3.500000
+0000fa00: 3630 652b 3031 2220 6379 3d22 322e 3330  60e+01" cy="2.30
+0000fa10: 3030 3030 3030 652b 3031 2220 723d 2230  000000e+01" r="0
+0000fa20: 2e35 3336 3831 3034 3635 3337 3831 3137  .536810465378117
+0000fa30: 3722 202f 3e0d 0a20 2020 2020 203c 6369  7" />..      <ci
+0000fa40: 7263 6c65 2063 783d 2233 2e32 3030 3030  rcle cx="3.20000
+0000fa50: 3030 3065 2b30 3122 2063 793d 2232 2e33  000e+01" cy="2.3
+0000fa60: 3030 3030 3030 3065 2b30 3122 2072 3d22  0000000e+01" r="
+0000fa70: 302e 3533 3638 3130 3436 3533 3738 3131  0.53681046537811
+0000fa80: 3737 2220 2f3e 0d0a 2020 2020 2020 3c63  77" />..      <c
+0000fa90: 6972 636c 6520 6378 3d22 322e 3930 3030  ircle cx="2.9000
+0000faa0: 3030 3330 652b 3031 2220 6379 3d22 322e  0030e+01" cy="2.
+0000fab0: 3330 3030 3030 3030 652b 3031 2220 723d  30000000e+01" r=
+0000fac0: 2230 2e35 3336 3831 3034 3635 3337 3831  "0.5368104653781
+0000fad0: 3137 3722 202f 3e0d 0a20 2020 2020 203c  177" />..      <
+0000fae0: 6369 7263 6c65 2063 783d 2232 2e35 3939  circle cx="2.599
+0000faf0: 3939 3937 3065 2b30 3122 2063 793d 2232  99970e+01" cy="2
+0000fb00: 2e33 3030 3030 3030 3065 2b30 3122 2072  .30000000e+01" r
+0000fb10: 3d22 302e 3533 3638 3130 3436 3533 3738  ="0.536810465378
+0000fb20: 3131 3737 2220 2f3e 0d0a 2020 2020 2020  1177" />..      
+0000fb30: 3c63 6972 636c 6520 6378 3d22 362e 3133  <circle cx="6.13
+0000fb40: 3233 3134 3330 652b 3031 2220 6379 3d22  231430e+01" cy="
+0000fb50: 352e 3930 3030 3030 3030 652b 3031 2220  5.90000000e+01" 
+0000fb60: 723d 2230 2e35 3336 3831 3034 3635 3337  r="0.53681046537
+0000fb70: 3831 3137 3722 202f 3e0d 0a20 2020 2020  81177" />..     
+0000fb80: 203c 6369 7263 6c65 2063 783d 2236 2e33   <circle cx="6.3
+0000fb90: 3635 3335 3736 3065 2b30 3122 2063 793d  6535760e+01" cy=
+0000fba0: 2235 2e38 3535 3534 3831 3065 2b30 3122  "5.85554810e+01"
+0000fbb0: 2072 3d22 302e 3533 3638 3130 3436 3533   r="0.5368104653
+0000fbc0: 3738 3131 3737 2220 2f3e 0d0a 2020 2020  781177" />..    
+0000fbd0: 2020 3c63 6972 636c 6520 6378 3d22 362e    <circle cx="6.
+0000fbe0: 3538 3838 3330 3330 652b 3031 2220 6379  58883030e+01" cy
+0000fbf0: 3d22 352e 3736 3239 3833 3130 652b 3031  ="5.76298310e+01
+0000fc00: 2220 723d 2230 2e35 3336 3831 3034 3635  " r="0.536810465
+0000fc10: 3337 3831 3137 3722 202f 3e0d 0a20 2020  3781177" />..   
+0000fc20: 2020 203c 6369 7263 6c65 2063 783d 2236     <circle cx="6
+0000fc30: 2e38 3036 3438 3435 3065 2b30 3122 2063  .80648450e+01" c
+0000fc40: 793d 2235 2e36 3732 3832 3734 3065 2b30  y="5.67282740e+0
+0000fc50: 3122 2072 3d22 302e 3533 3638 3130 3436  1" r="0.53681046
+0000fc60: 3533 3738 3131 3737 2220 2f3e 0d0a 2020  53781177" />..  
+0000fc70: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+0000fc80: 372e 3030 3430 3039 3330 652b 3031 2220  7.00400930e+01" 
+0000fc90: 6379 3d22 352e 3534 3135 3735 3030 652b  cy="5.54157500e+
+0000fca0: 3031 2220 723d 2230 2e35 3336 3831 3034  01" r="0.5368104
+0000fcb0: 3635 3337 3831 3137 3722 202f 3e0d 0a20  653781177" />.. 
+0000fcc0: 2020 2020 203c 6369 7263 6c65 2063 783d       <circle cx=
+0000fcd0: 2237 2e31 3732 3739 3137 3065 2b30 3122  "7.17279170e+01"
+0000fce0: 2063 793d 2235 2e33 3732 3739 3236 3065   cy="5.37279260e
+0000fcf0: 2b30 3122 2072 3d22 302e 3533 3638 3130  +01" r="0.536810
+0000fd00: 3436 3533 3738 3131 3737 2220 2f3e 0d0a  4653781177" />..
+0000fd10: 2020 2020 2020 3c63 6972 636c 6520 6378        <circle cx
+0000fd20: 3d22 372e 3334 3135 3735 3030 652b 3031  ="7.34157500e+01
+0000fd30: 2220 6379 3d22 352e 3230 3430 3039 3330  " cy="5.20400930
+0000fd40: 652b 3031 2220 723d 2230 2e35 3336 3831  e+01" r="0.53681
+0000fd50: 3034 3635 3337 3831 3137 3722 202f 3e0d  04653781177" />.
+0000fd60: 0a20 2020 2020 203c 6369 7263 6c65 2063  .      <circle c
+0000fd70: 783d 2237 2e34 3732 3832 3734 3065 2b30  x="7.47282740e+0
+0000fd80: 3122 2063 793d 2235 2e30 3036 3438 3435  1" cy="5.0064845
+0000fd90: 3065 2b30 3122 2072 3d22 302e 3533 3638  0e+01" r="0.5368
+0000fda0: 3130 3436 3533 3738 3131 3737 2220 2f3e  104653781177" />
+0000fdb0: 0d0a 2020 2020 2020 3c63 6972 636c 6520  ..      <circle 
+0000fdc0: 6378 3d22 372e 3536 3239 3833 3130 652b  cx="7.56298310e+
+0000fdd0: 3031 2220 6379 3d22 342e 3738 3838 3330  01" cy="4.788830
+0000fde0: 3330 652b 3031 2220 723d 2230 2e35 3336  30e+01" r="0.536
+0000fdf0: 3831 3034 3635 3337 3831 3137 3722 202f  8104653781177" /
+0000fe00: 3e0d 0a20 2020 2020 203c 6369 7263 6c65  >..      <circle
+0000fe10: 2063 783d 2237 2e36 3535 3534 3831 3065   cx="7.65554810e
+0000fe20: 2b30 3122 2063 793d 2234 2e35 3635 3335  +01" cy="4.56535
+0000fe30: 3736 3065 2b30 3122 2072 3d22 302e 3533  760e+01" r="0.53
+0000fe40: 3638 3130 3436 3533 3738 3131 3737 2220  68104653781177" 
+0000fe50: 2f3e 0d0a 2020 2020 2020 3c63 6972 636c  />..      <circl
+0000fe60: 6520 6378 3d22 372e 3730 3030 3030 3030  e cx="7.70000000
+0000fe70: 652b 3031 2220 6379 3d22 342e 3333 3233  e+01" cy="4.3323
+0000fe80: 3134 3330 652b 3031 2220 723d 2230 2e35  1430e+01" r="0.5
+0000fe90: 3336 3831 3034 3635 3337 3831 3137 3722  368104653781177"
+0000fea0: 202f 3e0d 0a20 2020 3c2f 673e 0d0a 3c2f   />..   </g>..</
+0000feb0: 7376 673e                                svg>
```

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/HeartPlate_Q8_2x2.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/HeartPlate_Q8_2x2.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/dat_to_svg/HeartPlate_Q8_2x2_exp.svg` & `lmcv_tools-0.0.8/tests/benchmark/translate/dat_to_svg/HeartPlate_Q8_2x2_exp.svg`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Circle_S3_S4R_4x4.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Circle_S3_S4R_4x4.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Circle_S3_S4R_4x4_exp.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Circle_S3_S4R_4x4_exp.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/ComplexPart_C3D20R.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/ComplexPart_C3D20R.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/ComplexPart_C3D20R_exp.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/ComplexPart_C3D20R_exp.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/ComplexPart_S8R.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/ComplexPart_S8R.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/ComplexPart_S8R_exp.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/ComplexPart_S8R_exp.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D20_1x1x1.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D20_1x1x1.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D20_1x1x1_exp.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D20_1x1x1_exp.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D20_2x2x2.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D20_2x2x2.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D20_2x2x2_exp.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D20_2x2x2_exp.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D8_1x1x1.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D8_1x1x1.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D8_1x1x1_exp.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D8_1x1x1_exp.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D8_2x2x2.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D8_2x2x2.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Cube_C3D8_2x2x2_exp.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Cube_C3D8_2x2x2_exp.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S4_1x1.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S4_1x1.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S4_2x2.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S4_2x2.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S4_2x2_exp.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S4_2x2_exp.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S8R_1x1.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S8R_1x1.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S8R_1x1_exp.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S8R_1x1_exp.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S8R_2x2.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S8R_2x2.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Square_S8R_2x2_exp.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Square_S8R_2x2_exp.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_S3_1x1.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_S3_1x1.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_S3_2x2.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_S3_2x2.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_S3_2x2_exp.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_S3_2x2_exp.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_1x1.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_1x1.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_2x2.inp` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_2x2.inp`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_2x2_exp.dat` & `lmcv_tools-0.0.8/tests/benchmark/translate/inp_to_dat/Triangle_STRI65_2x2_exp.dat`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/LICENSE` & `lmcv_tools-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcv_tools-0.0.7/README.md` & `lmcv_tools-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -100,30 +100,35 @@
 $ lmcv_tools extract [atributes] from [path/to/.pos] to [path/to/.csv]
 $ lmcv_tools extract [atributes] from [path/to/.pos] where [condition]
 $ lmcv_tools extract [atributes] from [path/to/.pos] where [condition] to [path/to/.csv]
 ```
 
 **Attributes** are names that represent a piece of data from a .pos file. They follow a simple pattern: "[set name].[attribute name]". The supported attributes are:
 
-| Attribute       | Meaning                                                                 |
-| ---             | ---                                                                     |
-| step.id         | Integer that identify analisys step.                                    |
-| step.factor     | Float point factor of a step.                                           |
-| node.id         | Integer that identify a node.                                           |
-| node.x          | Float point coordinate on x-axis of a node.                             |
-| node.y          | Float point coordinate on y-axis of a node.                             |
-| node.z          | Float point coordinate on z-axis of a node.                             |
-| step.node.u     | Float point displacement on x-axis of a node in specific step.          |
-| step.node.v     | Float point displacement on y-axis of a node in specific step.          |
-| step.node.w     | Float point displacement on z-axis of a node in specific step.          |
-| buckling.id     | Integer that identify analisys buckling mode.                           |
-| buckling.factor | Float point factor of a buckling mode.                                  |
-| buckling.node.u | Float point displacement on x-axis of a node in specific buckling mode. |
-| buckling.node.v | Float point displacement on y-axis of a node in specific buckling mode. |
-| buckling.node.w | Float point displacement on w-axis of a node in specific buckling mode. |
+| Attribute        | Meaning                                                                  |
+| ---              | ---                                                                      |
+| step.id          | Integer that identify analisys step.                                     |
+| step.factor      | Float point factor of a step.                                            |
+| node.id          | Integer that identify a node.                                            |
+| node.x           | Float point coordinate on x-axis of a node.                              |
+| node.y           | Float point coordinate on y-axis of a node.                              |
+| node.z           | Float point coordinate on z-axis of a node.                              |
+| step.node.u      | Float point displacement on x-axis of a node in specific step.           |
+| step.node.v      | Float point displacement on y-axis of a node in specific step.           |
+| step.node.w      | Float point displacement on z-axis of a node in specific step.           |
+| buckling.id      | Integer that identify analisys buckling mode.                            |
+| buckling.factor  | Float point factor of a buckling mode.                                   |
+| buckling.node.u  | Float point displacement on x-axis of a node in specific buckling mode.  |
+| buckling.node.v  | Float point displacement on y-axis of a node in specific buckling mode.  |
+| buckling.node.w  | Float point displacement on w-axis of a node in specific buckling mode.  |
+| vibration.id     | Integer that identify analisys vibration mode.                           |
+| vibration.factor | Float point factor of a vibration mode.                                  |
+| vibration.node.u | Float point displacement on x-axis of a node in specific vibration mode. |
+| vibration.node.v | Float point displacement on y-axis of a node in specific vibration mode. |
+| vibration.node.w | Float point displacement on w-axis of a node in specific vibration mode. |
 
 All attributes that belong the same set can be related by "[set name].id" and extracted together. To do this, type them separeted by space before "from" keyword. The attributes will be related in order which they were typed. Example:
 
 ```text
 $ lmcv_tools extract step.id step.factor step.node.u from Example.pos
 ```
 
@@ -191,16 +196,22 @@
 ```
 
 | Parameters            | Description                                          |
 | ---                   | ---                                                  |
 | Laminas Count         | Total number of laminas.                             |
 | Laminas Thickness     | Thinkcness of laminas.                               |
 | Power Law Exponent    | Exponent of Power Law.                               |
-| Micromechanical Model | Supported: voight, mori_tanaka.                      |
+| Micromechanical Model | Model to calculate effective properties.             |
 | Element Type          | Supported: Solid, Shell.                             |
 | E1                    | Elastic Modulus of Material 1.                       |
 | E2                    | Elastic Modulus of Material 2.                       |
 | nu1                   | Poisson's Coefficient of Material 1.                 |
 | nu2                   | Poisson's Coefficient of Material 2.                 |
 | pho1                  | Density of Material 1.                               |
 | pho2                  | Density of Material 2.                               |
-| Smart Laminas         | If True, a new smart generation method will be used. |
+| Smart Laminas         | If True, a new smart generation method will be used. |
+
+**Supported Micromechanical Models:**
+- voigt
+- mori_tanaka
+- hashin_shtrikman_lower_bound
+- hashin_shtrikman_upper_bound
```

### Comparing `lmcv_tools-0.0.7/pyproject.toml` & `lmcv_tools-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lmcv_tools"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name = "Dev-Gabriel-Braga", email = "gabriel.braga.matos@gmail.com" },
 ]
 description = "Command line tool that provides useful functionalities to LMCV Members"
 readme = "README.md"
 license = "GPL-3.0"
 requires-python = ">=3.9"
```

### Comparing `lmcv_tools-0.0.7/PKG-INFO` & `lmcv_tools-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcv_tools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Command line tool that provides useful functionalities to LMCV Members
 Project-URL: repository, https://github.com/Dev-Gabriel-Braga/lmcv_tools
 Author-email: Dev-Gabriel-Braga <gabriel.braga.matos@gmail.com>
 License-Expression: GPL-3.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -119,30 +119,35 @@
 $ lmcv_tools extract [atributes] from [path/to/.pos] to [path/to/.csv]
 $ lmcv_tools extract [atributes] from [path/to/.pos] where [condition]
 $ lmcv_tools extract [atributes] from [path/to/.pos] where [condition] to [path/to/.csv]
 ```
 
 **Attributes** are names that represent a piece of data from a .pos file. They follow a simple pattern: "[set name].[attribute name]". The supported attributes are:
 
-| Attribute       | Meaning                                                                 |
-| ---             | ---                                                                     |
-| step.id         | Integer that identify analisys step.                                    |
-| step.factor     | Float point factor of a step.                                           |
-| node.id         | Integer that identify a node.                                           |
-| node.x          | Float point coordinate on x-axis of a node.                             |
-| node.y          | Float point coordinate on y-axis of a node.                             |
-| node.z          | Float point coordinate on z-axis of a node.                             |
-| step.node.u     | Float point displacement on x-axis of a node in specific step.          |
-| step.node.v     | Float point displacement on y-axis of a node in specific step.          |
-| step.node.w     | Float point displacement on z-axis of a node in specific step.          |
-| buckling.id     | Integer that identify analisys buckling mode.                           |
-| buckling.factor | Float point factor of a buckling mode.                                  |
-| buckling.node.u | Float point displacement on x-axis of a node in specific buckling mode. |
-| buckling.node.v | Float point displacement on y-axis of a node in specific buckling mode. |
-| buckling.node.w | Float point displacement on w-axis of a node in specific buckling mode. |
+| Attribute        | Meaning                                                                  |
+| ---              | ---                                                                      |
+| step.id          | Integer that identify analisys step.                                     |
+| step.factor      | Float point factor of a step.                                            |
+| node.id          | Integer that identify a node.                                            |
+| node.x           | Float point coordinate on x-axis of a node.                              |
+| node.y           | Float point coordinate on y-axis of a node.                              |
+| node.z           | Float point coordinate on z-axis of a node.                              |
+| step.node.u      | Float point displacement on x-axis of a node in specific step.           |
+| step.node.v      | Float point displacement on y-axis of a node in specific step.           |
+| step.node.w      | Float point displacement on z-axis of a node in specific step.           |
+| buckling.id      | Integer that identify analisys buckling mode.                            |
+| buckling.factor  | Float point factor of a buckling mode.                                   |
+| buckling.node.u  | Float point displacement on x-axis of a node in specific buckling mode.  |
+| buckling.node.v  | Float point displacement on y-axis of a node in specific buckling mode.  |
+| buckling.node.w  | Float point displacement on w-axis of a node in specific buckling mode.  |
+| vibration.id     | Integer that identify analisys vibration mode.                           |
+| vibration.factor | Float point factor of a vibration mode.                                  |
+| vibration.node.u | Float point displacement on x-axis of a node in specific vibration mode. |
+| vibration.node.v | Float point displacement on y-axis of a node in specific vibration mode. |
+| vibration.node.w | Float point displacement on w-axis of a node in specific vibration mode. |
 
 All attributes that belong the same set can be related by "[set name].id" and extracted together. To do this, type them separeted by space before "from" keyword. The attributes will be related in order which they were typed. Example:
 
 ```text
 $ lmcv_tools extract step.id step.factor step.node.u from Example.pos
 ```
 
@@ -210,16 +215,22 @@
 ```
 
 | Parameters            | Description                                          |
 | ---                   | ---                                                  |
 | Laminas Count         | Total number of laminas.                             |
 | Laminas Thickness     | Thinkcness of laminas.                               |
 | Power Law Exponent    | Exponent of Power Law.                               |
-| Micromechanical Model | Supported: voight, mori_tanaka.                      |
+| Micromechanical Model | Model to calculate effective properties.             |
 | Element Type          | Supported: Solid, Shell.                             |
 | E1                    | Elastic Modulus of Material 1.                       |
 | E2                    | Elastic Modulus of Material 2.                       |
 | nu1                   | Poisson's Coefficient of Material 1.                 |
 | nu2                   | Poisson's Coefficient of Material 2.                 |
 | pho1                  | Density of Material 1.                               |
 | pho2                  | Density of Material 2.                               |
-| Smart Laminas         | If True, a new smart generation method will be used. |
+| Smart Laminas         | If True, a new smart generation method will be used. |
+
+**Supported Micromechanical Models:**
+- voigt
+- mori_tanaka
+- hashin_shtrikman_lower_bound
+- hashin_shtrikman_upper_bound
```

