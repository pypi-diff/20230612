# Comparing `tmp/propeller_design_tools-0.3.2.tar.gz` & `tmp/propeller_design_tools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jake\Desktop\Python Projects\propeller_design_tools\dist\.tmp-79ztm9bx\propeller_design_tools-0.3.2.tar", last modified: Sun Jun 11 23:07:25 2023, max compression
+gzip compressed data, was "C:\Users\Jake\Desktop\Python Projects\propeller_design_tools\dist\.tmp-nosnmco7\propeller_design_tools-0.3.3.tar", last modified: Sun Jun 11 23:26:23 2023, max compression
```

## Comparing `propeller_design_tools-0.3.2.tar` & `propeller_design_tools-0.3.3.tar`

### file list

```diff
@@ -1,373 +1,373 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:25.000000 propeller_design_tools-0.3.2/
--rw-rw-rw-   0        0        0    35801 2021-08-21 05:57:07.000000 propeller_design_tools-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     1405 2022-04-23 18:14:56.000000 propeller_design_tools-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     9163 2023-06-11 23:07:25.000000 propeller_design_tools-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     8308 2023-06-11 22:57:31.000000 propeller_design_tools-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/
--rw-rw-rw-   0        0        0      479 2022-04-06 00:00:39.000000 propeller_design_tools-0.3.2/propeller_design_tools/__init__.py
--rw-rw-rw-   0        0        0    28820 2022-05-20 22:03:53.000000 propeller_design_tools-0.3.2/propeller_design_tools/airfoil.py
--rw-rw-rw-   0        0        0     4871 2022-04-17 06:33:40.000000 propeller_design_tools-0.3.2/propeller_design_tools/custom_opengl_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:13:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag35.dat
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:01.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag36.dat
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:08.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag37.dat
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:18.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag38.dat
--rw-rw-rw-   0        0        0     1132 2021-10-24 06:54:37.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/arad13.dat
--rw-rw-rw-   0        0        0      816 2022-04-21 23:31:48.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/boe103.dat
--rw-rw-rw-   0        0        0      794 2022-04-21 23:06:50.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/boe106.dat
--rw-rw-rw-   0        0        0     2730 2021-02-07 20:57:01.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/clarky.dat
--rw-rw-rw-   0        0        0     1520 2021-10-24 06:55:45.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/e855.dat
--rw-rw-rw-   0        0        0     2778 2022-03-17 04:23:04.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/hs1606.dat
--rw-rw-rw-   0        0        0     2768 2021-10-24 06:48:49.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/mrc-16.dat
--rwxrwxrwx   0        0        0  1002125 2021-01-30 20:37:44.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/xfoil.exe
--rw-rw-rw-   0        0        0    18378 2022-04-21 23:06:28.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_ui_classes.py
--rw-rw-rw-   0        0        0    50416 2023-04-27 19:31:58.000000 propeller_design_tools-0.3.2/propeller_design_tools/funcs.py
--rw-rw-rw-   0        0        0    17861 2022-04-25 18:38:28.000000 propeller_design_tools-0.3.2/propeller_design_tools/helper_ui_classes.py
--rw-rw-rw-   0        0        0    16315 2023-04-26 19:09:09.000000 propeller_design_tools-0.3.2/propeller_design_tools/helper_ui_subclasses.py
--rw-rw-rw-   0        0        0      401 2022-03-18 16:03:32.000000 propeller_design_tools-0.3.2/propeller_design_tools/opt_ui_classes.py
--rw-rw-rw-   0        0        0    11040 2022-04-07 18:47:57.000000 propeller_design_tools-0.3.2/propeller_design_tools/optimizations.py
--rw-rw-rw-   0        0        0    15622 2022-04-25 20:19:25.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_analysis_ui_classes.py
--rw-rw-rw-   0        0        0    36995 2022-06-12 01:05:11.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_creation_ui_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/
--rw-rw-rw-   0        0        0    25993 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta
--rw-rw-rw-   0        0        0     8599 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop
--rw-rw-rw-   0        0        0     6239 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:25.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/
--rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     3807 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt
--rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt
--rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt
--rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt
--rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt
--rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt
--rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt
--rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt
--rw-rw-rw-   0        0        0     3814 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt
--rw-rw-rw-   0        0        0     3815 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt
--rw-rw-rw-   0        0        0     3816 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt
--rw-rw-rw-   0        0        0     3817 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt
--rw-rw-rw-   0        0        0     3819 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt
--rw-rw-rw-   0        0        0     3821 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt
--rw-rw-rw-   0        0        0     3822 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:25.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/station_polars/
--rw-rw-rw-   0        0        0     4595 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/
--rw-rw-rw-   0        0        0    13191 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta
--rw-rw-rw-   0        0        0     4923 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop
--rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/station_polars/
--rw-rw-rw-   0        0        0     5160 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/
--rw-rw-rw-   0        0        0    13630 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta
--rw-rw-rw-   0        0        0     4875 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop
--rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/
--rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     3765 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     3770 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     3774 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     3775 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     3777 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     3778 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     3781 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     3784 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/station_polars/
--rw-rw-rw-   0        0        0     6152 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar
--rwxrwxrwx   0        0        0  1176521 2021-01-30 22:15:06.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/xrotor.exe
--rw-rw-rw-   0        0        0    53871 2022-06-12 00:41:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/propeller.py
--rw-rw-rw-   0        0        0    17617 2022-04-22 04:16:32.000000 propeller_design_tools-0.3.2/propeller_design_tools/radialstation.py
--rw-rw-rw-   0        0        0     1674 2022-03-17 22:38:26.000000 propeller_design_tools-0.3.2/propeller_design_tools/science_spinbox_class.py
--rw-rw-rw-   0        0        0     4111 2022-04-10 23:06:53.000000 propeller_design_tools-0.3.2/propeller_design_tools/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:25.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/
--rw-rw-rw-   0        0        0     1358 2022-03-17 07:01:27.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/crosshair_cursor.png
--rw-rw-rw-   0        0        0    10192 2022-03-18 16:44:10.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot1.wav
--rw-rw-rw-   0        0        0    18704 2022-03-18 16:44:09.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot2.wav
--rw-rw-rw-   0        0        0    23984 2022-03-18 16:44:09.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot3.wav
--rw-rw-rw-   0        0        0    24784 2022-03-18 16:44:11.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot4.wav
--rw-rw-rw-   0        0        0      236 2023-06-11 22:33:04.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/user-settings.txt
--rw-rw-rw-   0        0        0     5857 2022-04-22 04:28:14.000000 propeller_design_tools-0.3.2/propeller_design_tools/user_interface.py
--rw-rw-rw-   0        0        0     2839 2022-03-11 21:49:52.000000 propeller_design_tools-0.3.2/propeller_design_tools/user_io.py
-drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools.egg-info/
--rw-rw-rw-   0        0        0     9163 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    26612 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      274 2022-04-10 09:00:21.000000 propeller_design_tools-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0     1017 2023-06-11 23:07:25.000000 propeller_design_tools-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/
+-rw-rw-rw-   0        0        0    35801 2021-08-21 05:57:07.000000 propeller_design_tools-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     1405 2022-04-23 18:14:56.000000 propeller_design_tools-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    10276 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9421 2023-06-11 23:23:35.000000 propeller_design_tools-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools/
+-rw-rw-rw-   0        0        0      479 2022-04-06 00:00:39.000000 propeller_design_tools-0.3.3/propeller_design_tools/__init__.py
+-rw-rw-rw-   0        0        0    28820 2022-05-20 22:03:53.000000 propeller_design_tools-0.3.3/propeller_design_tools/airfoil.py
+-rw-rw-rw-   0        0        0     4871 2022-04-17 06:33:40.000000 propeller_design_tools-0.3.3/propeller_design_tools/custom_opengl_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_database/
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:13:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_database/ag35.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:01.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_database/ag36.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:08.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_database/ag37.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:18.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_database/ag38.dat
+-rw-rw-rw-   0        0        0     1132 2021-10-24 06:54:37.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_database/arad13.dat
+-rw-rw-rw-   0        0        0      816 2022-04-21 23:31:48.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_database/boe103.dat
+-rw-rw-rw-   0        0        0      794 2022-04-21 23:06:50.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_database/boe106.dat
+-rw-rw-rw-   0        0        0     2730 2021-02-07 20:57:01.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_database/clarky.dat
+-rw-rw-rw-   0        0        0     1520 2021-10-24 06:55:45.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_database/e855.dat
+-rw-rw-rw-   0        0        0     2778 2022-03-17 04:23:04.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_database/hs1606.dat
+-rw-rw-rw-   0        0        0     2768 2021-10-24 06:48:49.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_database/mrc-16.dat
+-rwxrwxrwx   0        0        0  1002125 2021-01-30 20:37:44.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_database/xfoil.exe
+-rw-rw-rw-   0        0        0    18378 2022-04-21 23:06:28.000000 propeller_design_tools-0.3.3/propeller_design_tools/foil_ui_classes.py
+-rw-rw-rw-   0        0        0    50416 2023-04-27 19:31:58.000000 propeller_design_tools-0.3.3/propeller_design_tools/funcs.py
+-rw-rw-rw-   0        0        0    17861 2022-04-25 18:38:28.000000 propeller_design_tools-0.3.3/propeller_design_tools/helper_ui_classes.py
+-rw-rw-rw-   0        0        0    16315 2023-04-26 19:09:09.000000 propeller_design_tools-0.3.3/propeller_design_tools/helper_ui_subclasses.py
+-rw-rw-rw-   0        0        0      401 2022-03-18 16:03:32.000000 propeller_design_tools-0.3.3/propeller_design_tools/opt_ui_classes.py
+-rw-rw-rw-   0        0        0    11040 2022-04-07 18:47:57.000000 propeller_design_tools-0.3.3/propeller_design_tools/optimizations.py
+-rw-rw-rw-   0        0        0    15622 2022-04-25 20:19:25.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_analysis_ui_classes.py
+-rw-rw-rw-   0        0        0    36995 2022-06-12 01:05:11.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_creation_ui_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/
+-rw-rw-rw-   0        0        0    25993 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta
+-rw-rw-rw-   0        0        0     8599 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop
+-rw-rw-rw-   0        0        0     6239 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/
+-rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3807 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt
+-rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt
+-rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt
+-rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt
+-rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt
+-rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt
+-rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt
+-rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt
+-rw-rw-rw-   0        0        0     3814 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt
+-rw-rw-rw-   0        0        0     3815 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt
+-rw-rw-rw-   0        0        0     3816 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt
+-rw-rw-rw-   0        0        0     3817 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt
+-rw-rw-rw-   0        0        0     3819 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt
+-rw-rw-rw-   0        0        0     3821 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt
+-rw-rw-rw-   0        0        0     3822 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/station_polars/
+-rw-rw-rw-   0        0        0     4595 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/
+-rw-rw-rw-   0        0        0    13191 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta
+-rw-rw-rw-   0        0        0     4923 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop
+-rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/station_polars/
+-rw-rw-rw-   0        0        0     5160 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/
+-rw-rw-rw-   0        0        0    13630 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta
+-rw-rw-rw-   0        0        0     4875 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop
+-rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/
+-rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3765 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3770 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3774 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3775 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3777 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3778 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3781 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3784 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/station_polars/
+-rw-rw-rw-   0        0        0     6152 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar
+-rwxrwxrwx   0        0        0  1176521 2021-01-30 22:15:06.000000 propeller_design_tools-0.3.3/propeller_design_tools/prop_database/xrotor.exe
+-rw-rw-rw-   0        0        0    53871 2022-06-12 00:41:00.000000 propeller_design_tools-0.3.3/propeller_design_tools/propeller.py
+-rw-rw-rw-   0        0        0    17617 2022-04-22 04:16:32.000000 propeller_design_tools-0.3.3/propeller_design_tools/radialstation.py
+-rw-rw-rw-   0        0        0     1674 2022-03-17 22:38:26.000000 propeller_design_tools-0.3.3/propeller_design_tools/science_spinbox_class.py
+-rw-rw-rw-   0        0        0     4111 2022-04-10 23:06:53.000000 propeller_design_tools-0.3.3/propeller_design_tools/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools/supporting_files/
+-rw-rw-rw-   0        0        0     1358 2022-03-17 07:01:27.000000 propeller_design_tools-0.3.3/propeller_design_tools/supporting_files/crosshair_cursor.png
+-rw-rw-rw-   0        0        0    10192 2022-03-18 16:44:10.000000 propeller_design_tools-0.3.3/propeller_design_tools/supporting_files/gunshot1.wav
+-rw-rw-rw-   0        0        0    18704 2022-03-18 16:44:09.000000 propeller_design_tools-0.3.3/propeller_design_tools/supporting_files/gunshot2.wav
+-rw-rw-rw-   0        0        0    23984 2022-03-18 16:44:09.000000 propeller_design_tools-0.3.3/propeller_design_tools/supporting_files/gunshot3.wav
+-rw-rw-rw-   0        0        0    24784 2022-03-18 16:44:11.000000 propeller_design_tools-0.3.3/propeller_design_tools/supporting_files/gunshot4.wav
+-rw-rw-rw-   0        0        0      236 2023-06-11 22:33:04.000000 propeller_design_tools-0.3.3/propeller_design_tools/supporting_files/user-settings.txt
+-rw-rw-rw-   0        0        0     5857 2022-04-22 04:28:14.000000 propeller_design_tools-0.3.3/propeller_design_tools/user_interface.py
+-rw-rw-rw-   0        0        0     2839 2022-03-11 21:49:52.000000 propeller_design_tools-0.3.3/propeller_design_tools/user_io.py
+drwxrwxrwx   0        0        0        0 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools.egg-info/
+-rw-rw-rw-   0        0        0    10276 2023-06-11 23:26:22.000000 propeller_design_tools-0.3.3/propeller_design_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    26612 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/propeller_design_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 23:26:22.000000 propeller_design_tools-0.3.3/propeller_design_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-11 23:26:22.000000 propeller_design_tools-0.3.3/propeller_design_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      274 2022-04-10 09:00:21.000000 propeller_design_tools-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1017 2023-06-11 23:26:23.000000 propeller_design_tools-0.3.3/setup.cfg
```

### Comparing `propeller_design_tools-0.3.2/LICENSE` & `propeller_design_tools-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/MANIFEST.in` & `propeller_design_tools-0.3.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/PKG-INFO` & `propeller_design_tools-0.3.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: propeller_design_tools
-Version: 0.3.2
-Summary: Tools, for propeller design (automates usage of XFOIL and XROTOR executables).
-Home-page: https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
-Author: Jacob Bronson
-Author-email: jakebronson89@gmail.com
-Project-URL: Bug Tracker, https://github.com/helloDestroyerOfWorlds/propeller_design_tools/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 propeller_design_tools (PDT)
 ============================
 ---
 **Work in progress / incomplete documentation**
 
 Note: The graphical user interface for this should be functional for Linux users as well very soon!!!
 
@@ -41,15 +22,26 @@
 IMPORTANT NOTE: to potentially aid in realizing errors are coming from XFOIL or XROTOR rather than this source code ->
 currently this source code implements these as executables installed when pip installing this package -> this means if
 you are having pip install errors and are on Linux it might be caused by that.  Actually, if you are having any errors,
 even in the GUI, and you are on Linux it might be caused by me not understanding until now much about Linux.  If this 
 is the case and you think you know what is causing the error, please feel free to reach out to me to let me know.
 
 CONTINUED: additionally, very soon I will be implementing a fix to automatically install all dependencies, which should
-fix many issues for Linux users, if not all of the current ones.
+fix many issues for Linux users, if not all of the current ones.  I also HIGHLY RECOMMEND to use only the "constant" 
+blade cl distribution target option for the first time you ever use this code, and then only venture into other options
+once you are familiar with the code more and can explain to me even what exactly Mark Drela means by this parameter.  I
+think it's just his way of saying the parameter that controls what you want each target section's operating AoA to be,
+which in all honestly I have personally found to not really affect the outputs all that much with the exception
+(obviously) of what each section's chord length will end up being.  It doesn't seem to impact overall realized efficiency
+of the design very much (< ~5-10 percent in all my experiences).
+
+For this same exact reason, it is also HIGHLY RECOMMENDED to use only the 'grad' or 'pot' solver options until you know
+you have the code at least generating an output without failing.  My personal favorite solver is obviously the 'vrtx'
+option, but XROTOR seems to be much less stable and take much, much longer to arrive at solutions when using 'vrtx'.
+Thank you all that is my TED talk.
 
 Purpose
 =======
 PDT seeks to provide the user a set of python3 utilities
 that can be used for arbitrary scripting efforts to automate
 usage of both XFOIL and XROTOR while implementing its own 
 unique python3.7-native algorithms to maintain local
@@ -186,8 +178,8 @@
 
 
 6. **WIP** Prop optimization (grid-search style generic optimizer for "optimal"
 prop design generation by means of maximizing or minimizing a given output / 
 calculated metric based on outputs, optionally taking into account different
 propeller operating points via the ability to define the propeller's "duty-cycle"
 -> coming soon! This should elimiate the user's need to even input a value for the
-desired blade cl distribution altogether.)
+desired blade cl distribution altogether.)
```

### Comparing `propeller_design_tools-0.3.2/README.md` & `propeller_design_tools-0.3.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: propeller_design_tools
+Version: 0.3.3
+Summary: Tools, for propeller design (automates usage of XFOIL and XROTOR executables).
+Home-page: https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
+Author: Jacob Bronson
+Author-email: jakebronson89@gmail.com
+Project-URL: Bug Tracker, https://github.com/helloDestroyerOfWorlds/propeller_design_tools/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 propeller_design_tools (PDT)
 ============================
 ---
 **Work in progress / incomplete documentation**
 
 Note: The graphical user interface for this should be functional for Linux users as well very soon!!!
 
@@ -22,15 +41,26 @@
 IMPORTANT NOTE: to potentially aid in realizing errors are coming from XFOIL or XROTOR rather than this source code ->
 currently this source code implements these as executables installed when pip installing this package -> this means if
 you are having pip install errors and are on Linux it might be caused by that.  Actually, if you are having any errors,
 even in the GUI, and you are on Linux it might be caused by me not understanding until now much about Linux.  If this 
 is the case and you think you know what is causing the error, please feel free to reach out to me to let me know.
 
 CONTINUED: additionally, very soon I will be implementing a fix to automatically install all dependencies, which should
-fix many issues for Linux users, if not all of the current ones.
+fix many issues for Linux users, if not all of the current ones.  I also HIGHLY RECOMMEND to use only the "constant" 
+blade cl distribution target option for the first time you ever use this code, and then only venture into other options
+once you are familiar with the code more and can explain to me even what exactly Mark Drela means by this parameter.  I
+think it's just his way of saying the parameter that controls what you want each target section's operating AoA to be,
+which in all honestly I have personally found to not really affect the outputs all that much with the exception
+(obviously) of what each section's chord length will end up being.  It doesn't seem to impact overall realized efficiency
+of the design very much (< ~5-10 percent in all my experiences).
+
+For this same exact reason, it is also HIGHLY RECOMMENDED to use only the 'grad' or 'pot' solver options until you know
+you have the code at least generating an output without failing.  My personal favorite solver is obviously the 'vrtx'
+option, but XROTOR seems to be much less stable and take much, much longer to arrive at solutions when using 'vrtx'.
+Thank you all that is my TED talk.
 
 Purpose
 =======
 PDT seeks to provide the user a set of python3 utilities
 that can be used for arbitrary scripting efforts to automate
 usage of both XFOIL and XROTOR while implementing its own 
 unique python3.7-native algorithms to maintain local
@@ -167,8 +197,8 @@
 
 
 6. **WIP** Prop optimization (grid-search style generic optimizer for "optimal"
 prop design generation by means of maximizing or minimizing a given output / 
 calculated metric based on outputs, optionally taking into account different
 propeller operating points via the ability to define the propeller's "duty-cycle"
 -> coming soon! This should elimiate the user's need to even input a value for the
-desired blade cl distribution altogether.)
+desired blade cl distribution altogether.)
```

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/airfoil.py` & `propeller_design_tools-0.3.3/propeller_design_tools/airfoil.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/custom_opengl_classes.py` & `propeller_design_tools-0.3.3/propeller_design_tools/custom_opengl_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag35.dat` & `propeller_design_tools-0.3.3/propeller_design_tools/foil_database/ag35.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag36.dat` & `propeller_design_tools-0.3.3/propeller_design_tools/foil_database/ag36.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag37.dat` & `propeller_design_tools-0.3.3/propeller_design_tools/foil_database/ag37.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag38.dat` & `propeller_design_tools-0.3.3/propeller_design_tools/foil_database/ag38.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/arad13.dat` & `propeller_design_tools-0.3.3/propeller_design_tools/foil_database/arad13.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/boe103.dat` & `propeller_design_tools-0.3.3/propeller_design_tools/foil_database/boe103.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/boe106.dat` & `propeller_design_tools-0.3.3/propeller_design_tools/foil_database/boe106.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/clarky.dat` & `propeller_design_tools-0.3.3/propeller_design_tools/foil_database/clarky.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/e855.dat` & `propeller_design_tools-0.3.3/propeller_design_tools/foil_database/e855.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/hs1606.dat` & `propeller_design_tools-0.3.3/propeller_design_tools/foil_database/hs1606.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/mrc-16.dat` & `propeller_design_tools-0.3.3/propeller_design_tools/foil_database/mrc-16.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/xfoil.exe` & `propeller_design_tools-0.3.3/propeller_design_tools/foil_database/xfoil.exe`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/foil_ui_classes.py` & `propeller_design_tools-0.3.3/propeller_design_tools/foil_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/funcs.py` & `propeller_design_tools-0.3.3/propeller_design_tools/funcs.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/helper_ui_classes.py` & `propeller_design_tools-0.3.3/propeller_design_tools/helper_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/helper_ui_subclasses.py` & `propeller_design_tools-0.3.3/propeller_design_tools/helper_ui_subclasses.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/optimizations.py` & `propeller_design_tools-0.3.3/propeller_design_tools/optimizations.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_analysis_ui_classes.py` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_analysis_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_creation_ui_classes.py` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_creation_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/xrotor.exe` & `propeller_design_tools-0.3.3/propeller_design_tools/prop_database/xrotor.exe`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/propeller.py` & `propeller_design_tools-0.3.3/propeller_design_tools/propeller.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/radialstation.py` & `propeller_design_tools-0.3.3/propeller_design_tools/radialstation.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/science_spinbox_class.py` & `propeller_design_tools-0.3.3/propeller_design_tools/science_spinbox_class.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/settings.py` & `propeller_design_tools-0.3.3/propeller_design_tools/settings.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/crosshair_cursor.png` & `propeller_design_tools-0.3.3/propeller_design_tools/supporting_files/crosshair_cursor.png`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot1.wav` & `propeller_design_tools-0.3.3/propeller_design_tools/supporting_files/gunshot1.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot2.wav` & `propeller_design_tools-0.3.3/propeller_design_tools/supporting_files/gunshot2.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot3.wav` & `propeller_design_tools-0.3.3/propeller_design_tools/supporting_files/gunshot3.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot4.wav` & `propeller_design_tools-0.3.3/propeller_design_tools/supporting_files/gunshot4.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/user_interface.py` & `propeller_design_tools-0.3.3/propeller_design_tools/user_interface.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools/user_io.py` & `propeller_design_tools-0.3.3/propeller_design_tools/user_io.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools.egg-info/PKG-INFO` & `propeller_design_tools-0.3.3/propeller_design_tools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propeller-design-tools
-Version: 0.3.2
+Version: 0.3.3
 Summary: Tools, for propeller design (automates usage of XFOIL and XROTOR executables).
 Home-page: https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
 Author: Jacob Bronson
 Author-email: jakebronson89@gmail.com
 Project-URL: Bug Tracker, https://github.com/helloDestroyerOfWorlds/propeller_design_tools/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -41,15 +41,26 @@
 IMPORTANT NOTE: to potentially aid in realizing errors are coming from XFOIL or XROTOR rather than this source code ->
 currently this source code implements these as executables installed when pip installing this package -> this means if
 you are having pip install errors and are on Linux it might be caused by that.  Actually, if you are having any errors,
 even in the GUI, and you are on Linux it might be caused by me not understanding until now much about Linux.  If this 
 is the case and you think you know what is causing the error, please feel free to reach out to me to let me know.
 
 CONTINUED: additionally, very soon I will be implementing a fix to automatically install all dependencies, which should
-fix many issues for Linux users, if not all of the current ones.
+fix many issues for Linux users, if not all of the current ones.  I also HIGHLY RECOMMEND to use only the "constant" 
+blade cl distribution target option for the first time you ever use this code, and then only venture into other options
+once you are familiar with the code more and can explain to me even what exactly Mark Drela means by this parameter.  I
+think it's just his way of saying the parameter that controls what you want each target section's operating AoA to be,
+which in all honestly I have personally found to not really affect the outputs all that much with the exception
+(obviously) of what each section's chord length will end up being.  It doesn't seem to impact overall realized efficiency
+of the design very much (< ~5-10 percent in all my experiences).
+
+For this same exact reason, it is also HIGHLY RECOMMENDED to use only the 'grad' or 'pot' solver options until you know
+you have the code at least generating an output without failing.  My personal favorite solver is obviously the 'vrtx'
+option, but XROTOR seems to be much less stable and take much, much longer to arrive at solutions when using 'vrtx'.
+Thank you all that is my TED talk.
 
 Purpose
 =======
 PDT seeks to provide the user a set of python3 utilities
 that can be used for arbitrary scripting efforts to automate
 usage of both XFOIL and XROTOR while implementing its own 
 unique python3.7-native algorithms to maintain local
```

### Comparing `propeller_design_tools-0.3.2/propeller_design_tools.egg-info/SOURCES.txt` & `propeller_design_tools-0.3.3/propeller_design_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.2/setup.cfg` & `propeller_design_tools-0.3.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 726f 7065 6c6c 6572 5f64 6573   = propeller_des
 00000020: 6967 6e5f 746f 6f6c 730d 0a76 6572 7369  ign_tools..versi
-00000030: 6f6e 203d 2030 2e33 2e32 0d0a 6175 7468  on = 0.3.2..auth
+00000030: 6f6e 203d 2030 2e33 2e33 0d0a 6175 7468  on = 0.3.3..auth
 00000040: 6f72 203d 204a 6163 6f62 2042 726f 6e73  or = Jacob Brons
 00000050: 6f6e 0d0a 6175 7468 6f72 5f65 6d61 696c  on..author_email
 00000060: 203d 206a 616b 6562 726f 6e73 6f6e 3839   = jakebronson89
 00000070: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000080: 7269 7074 696f 6e20 3d20 546f 6f6c 732c  ription = Tools,
 00000090: 2066 6f72 2070 726f 7065 6c6c 6572 2064   for propeller d
 000000a0: 6573 6967 6e20 2861 7574 6f6d 6174 6573  esign (automates
```

