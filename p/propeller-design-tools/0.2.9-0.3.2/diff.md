# Comparing `tmp/propeller_design_tools-0.2.9.tar.gz` & `tmp/propeller_design_tools-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jake\Desktop\Python Projects\propeller_design_tools\dist\tmp_sa74nkw\propeller_design_tools-0.2.9.tar", last modified: Mon Apr 25 20:26:39 2022, max compression
+gzip compressed data, was "C:\Users\Jake\Desktop\Python Projects\propeller_design_tools\dist\.tmp-79ztm9bx\propeller_design_tools-0.3.2.tar", last modified: Sun Jun 11 23:07:25 2023, max compression
```

## Comparing `propeller_design_tools-0.2.9.tar` & `propeller_design_tools-0.3.2.tar`

### file list

```diff
@@ -1,373 +1,373 @@
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:39.000000 propeller_design_tools-0.2.9/
--rw-rw-rw-   0        0        0    35801 2021-08-21 05:57:07.000000 propeller_design_tools-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     1405 2022-04-23 18:14:56.000000 propeller_design_tools-0.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     7509 2022-04-25 20:26:39.000000 propeller_design_tools-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     6611 2022-04-17 04:09:33.000000 propeller_design_tools-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/
--rw-rw-rw-   0        0        0      479 2022-04-06 00:00:39.000000 propeller_design_tools-0.2.9/propeller_design_tools/__init__.py
--rw-rw-rw-   0        0        0    28138 2022-04-15 17:59:25.000000 propeller_design_tools-0.2.9/propeller_design_tools/airfoil.py
--rw-rw-rw-   0        0        0     4871 2022-04-17 06:33:40.000000 propeller_design_tools-0.2.9/propeller_design_tools/custom_opengl_classes.py
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:13:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag35.dat
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:01.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag36.dat
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:08.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag37.dat
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:18.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag38.dat
--rw-rw-rw-   0        0        0     1132 2021-10-24 06:54:37.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/arad13.dat
--rw-rw-rw-   0        0        0      816 2022-04-21 23:31:48.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/boe103.dat
--rw-rw-rw-   0        0        0      794 2022-04-21 23:06:50.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/boe106.dat
--rw-rw-rw-   0        0        0     2730 2021-02-07 20:57:01.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/clarky.dat
--rw-rw-rw-   0        0        0     1520 2021-10-24 06:55:45.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/e855.dat
--rw-rw-rw-   0        0        0     2778 2022-03-17 04:23:04.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/hs1606.dat
--rw-rw-rw-   0        0        0     2768 2021-10-24 06:48:49.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/mrc-16.dat
--rwxrwxrwx   0        0        0  1002125 2021-01-30 20:37:44.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/xfoil.exe
--rw-rw-rw-   0        0        0    18378 2022-04-21 23:06:28.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_ui_classes.py
--rw-rw-rw-   0        0        0    49655 2022-04-22 04:19:36.000000 propeller_design_tools-0.2.9/propeller_design_tools/funcs.py
--rw-rw-rw-   0        0        0    17861 2022-04-25 18:38:28.000000 propeller_design_tools-0.2.9/propeller_design_tools/helper_ui_classes.py
--rw-rw-rw-   0        0        0    16262 2022-04-17 06:29:47.000000 propeller_design_tools-0.2.9/propeller_design_tools/helper_ui_subclasses.py
--rw-rw-rw-   0        0        0      401 2022-03-18 16:03:32.000000 propeller_design_tools-0.2.9/propeller_design_tools/opt_ui_classes.py
--rw-rw-rw-   0        0        0    11040 2022-04-07 18:47:57.000000 propeller_design_tools-0.2.9/propeller_design_tools/optimizations.py
--rw-rw-rw-   0        0        0    15622 2022-04-25 20:19:25.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_analysis_ui_classes.py
--rw-rw-rw-   0        0        0    36995 2022-04-22 17:46:35.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_creation_ui_classes.py
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/
--rw-rw-rw-   0        0        0    25993 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta
--rw-rw-rw-   0        0        0     8599 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop
--rw-rw-rw-   0        0        0     6239 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:39.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/
--rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     3807 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt
--rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt
--rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt
--rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt
--rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt
--rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt
--rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt
--rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt
--rw-rw-rw-   0        0        0     3814 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt
--rw-rw-rw-   0        0        0     3815 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt
--rw-rw-rw-   0        0        0     3816 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt
--rw-rw-rw-   0        0        0     3817 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt
--rw-rw-rw-   0        0        0     3819 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt
--rw-rw-rw-   0        0        0     3821 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt
--rw-rw-rw-   0        0        0     3822 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:39.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/station_polars/
--rw-rw-rw-   0        0        0     4595 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/
--rw-rw-rw-   0        0        0    13191 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta
--rw-rw-rw-   0        0        0     4923 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop
--rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/station_polars/
--rw-rw-rw-   0        0        0     5160 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/
--rw-rw-rw-   0        0        0    13630 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta
--rw-rw-rw-   0        0        0     4875 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop
--rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/
--rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     3765 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     3770 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     3774 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     3775 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     3777 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     3778 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     3781 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     3784 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/station_polars/
--rw-rw-rw-   0        0        0     6152 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar
--rwxrwxrwx   0        0        0  1176521 2021-01-30 22:15:06.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/xrotor.exe
--rw-rw-rw-   0        0        0    53754 2022-04-25 20:17:44.000000 propeller_design_tools-0.2.9/propeller_design_tools/propeller.py
--rw-rw-rw-   0        0        0    17617 2022-04-22 04:16:32.000000 propeller_design_tools-0.2.9/propeller_design_tools/radialstation.py
--rw-rw-rw-   0        0        0     1674 2022-03-17 22:38:26.000000 propeller_design_tools-0.2.9/propeller_design_tools/science_spinbox_class.py
--rw-rw-rw-   0        0        0     4111 2022-04-10 23:06:53.000000 propeller_design_tools-0.2.9/propeller_design_tools/settings.py
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:39.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/
--rw-rw-rw-   0        0        0     1358 2022-03-17 07:01:27.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/crosshair_cursor.png
--rw-rw-rw-   0        0        0    10192 2022-03-18 16:44:10.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot1.wav
--rw-rw-rw-   0        0        0    18704 2022-03-18 16:44:09.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot2.wav
--rw-rw-rw-   0        0        0    23984 2022-03-18 16:44:09.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot3.wav
--rw-rw-rw-   0        0        0    24784 2022-03-18 16:44:11.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot4.wav
--rw-rw-rw-   0        0        0      236 2022-04-25 20:19:27.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/user-settings.txt
--rw-rw-rw-   0        0        0     5857 2022-04-22 04:28:14.000000 propeller_design_tools-0.2.9/propeller_design_tools/user_interface.py
--rw-rw-rw-   0        0        0     2839 2022-03-11 21:49:52.000000 propeller_design_tools-0.2.9/propeller_design_tools/user_io.py
-drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools.egg-info/
--rw-rw-rw-   0        0        0     7509 2022-04-25 20:26:36.000000 propeller_design_tools-0.2.9/propeller_design_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    26612 2022-04-25 20:26:37.000000 propeller_design_tools-0.2.9/propeller_design_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-25 20:26:36.000000 propeller_design_tools-0.2.9/propeller_design_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-04-25 20:26:36.000000 propeller_design_tools-0.2.9/propeller_design_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      274 2022-04-10 09:00:21.000000 propeller_design_tools-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0     1021 2022-04-25 20:26:39.000000 propeller_design_tools-0.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:25.000000 propeller_design_tools-0.3.2/
+-rw-rw-rw-   0        0        0    35801 2021-08-21 05:57:07.000000 propeller_design_tools-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     1405 2022-04-23 18:14:56.000000 propeller_design_tools-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9163 2023-06-11 23:07:25.000000 propeller_design_tools-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8308 2023-06-11 22:57:31.000000 propeller_design_tools-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/
+-rw-rw-rw-   0        0        0      479 2022-04-06 00:00:39.000000 propeller_design_tools-0.3.2/propeller_design_tools/__init__.py
+-rw-rw-rw-   0        0        0    28820 2022-05-20 22:03:53.000000 propeller_design_tools-0.3.2/propeller_design_tools/airfoil.py
+-rw-rw-rw-   0        0        0     4871 2022-04-17 06:33:40.000000 propeller_design_tools-0.3.2/propeller_design_tools/custom_opengl_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:13:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag35.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:01.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag36.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:08.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag37.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:18.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag38.dat
+-rw-rw-rw-   0        0        0     1132 2021-10-24 06:54:37.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/arad13.dat
+-rw-rw-rw-   0        0        0      816 2022-04-21 23:31:48.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/boe103.dat
+-rw-rw-rw-   0        0        0      794 2022-04-21 23:06:50.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/boe106.dat
+-rw-rw-rw-   0        0        0     2730 2021-02-07 20:57:01.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/clarky.dat
+-rw-rw-rw-   0        0        0     1520 2021-10-24 06:55:45.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/e855.dat
+-rw-rw-rw-   0        0        0     2778 2022-03-17 04:23:04.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/hs1606.dat
+-rw-rw-rw-   0        0        0     2768 2021-10-24 06:48:49.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/mrc-16.dat
+-rwxrwxrwx   0        0        0  1002125 2021-01-30 20:37:44.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_database/xfoil.exe
+-rw-rw-rw-   0        0        0    18378 2022-04-21 23:06:28.000000 propeller_design_tools-0.3.2/propeller_design_tools/foil_ui_classes.py
+-rw-rw-rw-   0        0        0    50416 2023-04-27 19:31:58.000000 propeller_design_tools-0.3.2/propeller_design_tools/funcs.py
+-rw-rw-rw-   0        0        0    17861 2022-04-25 18:38:28.000000 propeller_design_tools-0.3.2/propeller_design_tools/helper_ui_classes.py
+-rw-rw-rw-   0        0        0    16315 2023-04-26 19:09:09.000000 propeller_design_tools-0.3.2/propeller_design_tools/helper_ui_subclasses.py
+-rw-rw-rw-   0        0        0      401 2022-03-18 16:03:32.000000 propeller_design_tools-0.3.2/propeller_design_tools/opt_ui_classes.py
+-rw-rw-rw-   0        0        0    11040 2022-04-07 18:47:57.000000 propeller_design_tools-0.3.2/propeller_design_tools/optimizations.py
+-rw-rw-rw-   0        0        0    15622 2022-04-25 20:19:25.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_analysis_ui_classes.py
+-rw-rw-rw-   0        0        0    36995 2022-06-12 01:05:11.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_creation_ui_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/
+-rw-rw-rw-   0        0        0    25993 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta
+-rw-rw-rw-   0        0        0     8599 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop
+-rw-rw-rw-   0        0        0     6239 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:25.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/
+-rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3807 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt
+-rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt
+-rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt
+-rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt
+-rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt
+-rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt
+-rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt
+-rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt
+-rw-rw-rw-   0        0        0     3814 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt
+-rw-rw-rw-   0        0        0     3815 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt
+-rw-rw-rw-   0        0        0     3816 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt
+-rw-rw-rw-   0        0        0     3817 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt
+-rw-rw-rw-   0        0        0     3819 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt
+-rw-rw-rw-   0        0        0     3821 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt
+-rw-rw-rw-   0        0        0     3822 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:25.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/station_polars/
+-rw-rw-rw-   0        0        0     4595 2022-04-22 17:47:43.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/
+-rw-rw-rw-   0        0        0    13191 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta
+-rw-rw-rw-   0        0        0     4923 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop
+-rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/station_polars/
+-rw-rw-rw-   0        0        0     5160 2022-04-22 04:32:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/
+-rw-rw-rw-   0        0        0    13630 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta
+-rw-rw-rw-   0        0        0     4875 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop
+-rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/
+-rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3765 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3770 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3774 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3775 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3777 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3778 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3781 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3784 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/station_polars/
+-rw-rw-rw-   0        0        0     6152 2022-04-22 04:32:46.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar
+-rwxrwxrwx   0        0        0  1176521 2021-01-30 22:15:06.000000 propeller_design_tools-0.3.2/propeller_design_tools/prop_database/xrotor.exe
+-rw-rw-rw-   0        0        0    53871 2022-06-12 00:41:00.000000 propeller_design_tools-0.3.2/propeller_design_tools/propeller.py
+-rw-rw-rw-   0        0        0    17617 2022-04-22 04:16:32.000000 propeller_design_tools-0.3.2/propeller_design_tools/radialstation.py
+-rw-rw-rw-   0        0        0     1674 2022-03-17 22:38:26.000000 propeller_design_tools-0.3.2/propeller_design_tools/science_spinbox_class.py
+-rw-rw-rw-   0        0        0     4111 2022-04-10 23:06:53.000000 propeller_design_tools-0.3.2/propeller_design_tools/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:25.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/
+-rw-rw-rw-   0        0        0     1358 2022-03-17 07:01:27.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/crosshair_cursor.png
+-rw-rw-rw-   0        0        0    10192 2022-03-18 16:44:10.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot1.wav
+-rw-rw-rw-   0        0        0    18704 2022-03-18 16:44:09.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot2.wav
+-rw-rw-rw-   0        0        0    23984 2022-03-18 16:44:09.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot3.wav
+-rw-rw-rw-   0        0        0    24784 2022-03-18 16:44:11.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot4.wav
+-rw-rw-rw-   0        0        0      236 2023-06-11 22:33:04.000000 propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/user-settings.txt
+-rw-rw-rw-   0        0        0     5857 2022-04-22 04:28:14.000000 propeller_design_tools-0.3.2/propeller_design_tools/user_interface.py
+-rw-rw-rw-   0        0        0     2839 2022-03-11 21:49:52.000000 propeller_design_tools-0.3.2/propeller_design_tools/user_io.py
+drwxrwxrwx   0        0        0        0 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools.egg-info/
+-rw-rw-rw-   0        0        0     9163 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    26612 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-11 23:07:24.000000 propeller_design_tools-0.3.2/propeller_design_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      274 2022-04-10 09:00:21.000000 propeller_design_tools-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1017 2023-06-11 23:07:25.000000 propeller_design_tools-0.3.2/setup.cfg
```

### Comparing `propeller_design_tools-0.2.9/LICENSE` & `propeller_design_tools-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/MANIFEST.in` & `propeller_design_tools-0.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/PKG-INFO` & `propeller_design_tools-0.3.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,37 @@
-Metadata-Version: 2.1
-Name: propeller_design_tools
-Version: 0.2.9
-Summary: Tools, for propeller design (automates usage of XFOIL and XROTOR executables).
-Home-page: https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
-Author: Jacob Bronson
-Author-email: jakebronson89@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/helloDestroyerOfWorlds/propeller_design_tools/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
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
 
+Note: The graphical user interface for this should be functional for Linux users as well very soon!!!
+
+Eventually I do plan to create better docs, but for now it's just what you see below and the source code itself.
+
 ---
 
 Description
 ===========
 Python 3.7 package that provides exactly what it sounds 
 like by automating usage of the GPL-licensed 
 CLI-utilities XFOIL and XROTOR.
 
 Both utilities are published by professor Mark Drela (MIT).
 - XFOIL: for arbitrary 2D airfoil analysis
 - XROTOR: for arbitrary propeller design schemes
 
+IMPORTANT NOTE: to potentially aid in realizing errors are coming from XFOIL or XROTOR rather than this source code ->
+currently this source code implements these as executables installed when pip installing this package -> this means if
+you are having pip install errors and are on Linux it might be caused by that.  Actually, if you are having any errors,
+even in the GUI, and you are on Linux it might be caused by me not understanding until now much about Linux.  If this 
+is the case and you think you know what is causing the error, please feel free to reach out to me to let me know.
+
+CONTINUED: additionally, very soon I will be implementing a fix to automatically install all dependencies, which should
+fix many issues for Linux users, if not all of the current ones.
+
 Purpose
 =======
 PDT seeks to provide the user a set of python3 utilities
 that can be used for arbitrary scripting efforts to automate
 usage of both XFOIL and XROTOR while implementing its own 
 unique python3.7-native algorithms to maintain local
 input files, meta files, databases, and results files and
@@ -67,16 +59,19 @@
 of every script right after the imports**
 
 *The airfoil directory will be used to store any foil / 
 XFOIL- related support files, and the propeller directory
 will be used similarly to store any propeller / XROTOR - 
 related support files.*
 
-Requisite: XFOIL and XROTOR Executables
+Pre-Requisite: XFOIL and XROTOR Executables
 -------------------------------------------
+(soon this section will be obsolete as I plan to implement a pure-python
+version of both XFOIL and XROTOR in the source code)
+
 In order to utilize any PDT functionality that depends on 
 running XFOIL, the "xfoil.exe" executable file needs to be
 in the user-set "airfoil_database" location. *Current pip 
 installations include the xfoil.exe file in the foil_database,
 there should theoretically be no need to download it manually.*
 
 [XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
@@ -84,18 +79,19 @@
 Likewise, in order to utilize any PDT functionality that
 depends on running XROTOR, the "xrotor.exe" executable file
 needs to be in the user-set "propeller_database" location.
 *Current pip installations include the xrotor.exe file in the 
 default prop_database, there should theoretically be no need to 
 download it manually.*
 
-[XROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
+[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
 *(this is actually a link to "CROTOR", which I find is
-actually the easiest way to obtain a windows-executable
-of XROTOR)*
+the easiest way to obtain a windows-executable of XROTOR)*
+
+[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
 
 Example Scripts / Workflow
 --------------------------
 At a high-level, the current concept for PDT workflow is as 
 follows (after obtaining the required executables and pip-installing 
 the PDT package):
 
@@ -154,21 +150,25 @@
 including profle xyz coordinate listings, and .stl 3D geometry files -> see
 [example4_stl_generation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example4_stl_generation.py
    )
 
    ![ex4-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex4-1.png)
 
+Note: It is known that currently there is an issue with these .stl files opening in SolidWorks -> try converting them
+using anything (first idea is MS Paint, I think the new version can save STL files as well).  As far as I can tell this 
+is only an issue for SolidWorks users on Windows, these files open and display fine in every other application.
 
 5. Analyze a given Propeller() instance across a sweep of operating points -> see 
 [example5_prop_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example5_prop_analysis.py
    )
 
    ![ex5-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex5-1.png)
 
 
 6. **WIP** Prop optimization (grid-search style generic optimizer for "optimal"
 prop design generation by means of maximizing or minimizing a given output / 
 calculated metric based on outputs, optionally taking into account different
-propeller operating points via the ability to define the propeller's "duty-cycle")
-
+propeller operating points via the ability to define the propeller's "duty-cycle"
+-> coming soon! This should elimiate the user's need to even input a value for the
+desired blade cl distribution altogether.)
```

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/airfoil.py` & `propeller_design_tools-0.3.2/propeller_design_tools/airfoil.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,21 @@
         # get the airfoil filename, filepath
         fname = funcs.get_airfoil_file_from_db(self.name, exact_namematch=exact_namematch)
         if verbose:
             Info('Found airfoil coordinate file: {}'.format(fname))
         self.coord_fpath = os.path.join(get_foil_db(), fname)
 
         name, x_coords, y_coords = funcs.read_airfoil_coordinate_file(fpath=self.coord_fpath, verbose=verbose)
+        _, xc_closed_te, yc_closed_te = funcs.read_airfoil_coordinate_file(fpath=self.coord_fpath, verbose=False,
+                                                                           te_gap_set=0.0)
         self.filename = os.path.basename(self.coord_fpath)
         self.x_coords = np.array(x_coords)
         self.y_coords = np.array(y_coords)
+        self.xc_closed_te = xc_closed_te
+        self.yc_closed_te = yc_closed_te
 
         self.xfoil_coord_fpath = self.write_xfoil_coord_file()
         self.polar_data = {}      # dictionary of dictionaries, keys are floats of Re
         self.rectified_polar_data = {}
 
         if os.path.exists(self.get_database_savepath()):
             self.load_polar_data(verbose=verbose)
@@ -65,21 +69,26 @@
         savepath = os.path.join(xfoil_folder, '{}.txt'.format(savename))
         with open(savepath, 'w') as f:
             f.write('{}\n\n'.format(self.name))
             for coord in zip(self.x_coords, self.y_coords):
                 f.write('{x:.7f} {y:.7f}\n'.format(x=coord[0], y=coord[1]))
         return savepath
 
-    def plot_geometry(self, fig=None):
+    def plot_geometry(self, fig=None, closed_te: bool = False):
         if fig is None:
             fig = plt.figure()
             ax = fig.add_subplot(111)
         else:
             ax = fig.axes[0]
-        ax.plot(self.x_coords, self.y_coords)
+
+        if closed_te:
+            ax.plot(self.xc_closed_te, self.yc_closed_te)
+        else:
+            ax.plot(self.x_coords, self.y_coords)
+
         ax.set_aspect('equal')
         ax.grid(True)
         left, right = ax.get_xlim()
         ax.set_ylim((left - right / 2), -(left - right / 2))
         ax.set_title(self.filename)
 
         return fig
@@ -569,14 +578,20 @@
 
     def get_coords(self, n_interp: int = None):
         if n_interp is None:
             return np.vstack([self.x_coords, self.y_coords])
         else:
             raise Error('Code to interpolate more profile points is incomplete...')
 
+    def get_coords_closed_te(self, n_interp: int = None):
+        if n_interp is None:
+            return np.vstack([self.xc_closed_te, self.yc_closed_te])
+        else:
+            raise Error('Code to interpolate more profile points is incomplete...')
+
     def plot_2D_trimesh(self):
         fig = self.plot_geometry()
         ax = fig.axes[0]
 
         vectors = funcs.compute_profile_trimesh(profile_coords=self.get_coords())
         for vector in vectors:
             pt1, pt2, pt3 = vector
```

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/custom_opengl_classes.py` & `propeller_design_tools-0.3.2/propeller_design_tools/custom_opengl_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag35.dat` & `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag35.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag36.dat` & `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag36.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag37.dat` & `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag37.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag38.dat` & `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/ag38.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/arad13.dat` & `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/arad13.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/boe103.dat` & `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/boe103.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/boe106.dat` & `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/boe106.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/clarky.dat` & `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/clarky.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/e855.dat` & `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/e855.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/hs1606.dat` & `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/hs1606.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/mrc-16.dat` & `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/mrc-16.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/xfoil.exe` & `propeller_design_tools-0.3.2/propeller_design_tools/foil_database/xfoil.exe`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/foil_ui_classes.py` & `propeller_design_tools-0.3.2/propeller_design_tools/foil_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/funcs.py` & `propeller_design_tools-0.3.2/propeller_design_tools/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         else:   # otherwise, just stuff it back in to the new dictionary un-altered
             new_d[key] = val
 
     return new_d
 
 
 # =============== FILE READING / WRITING FUNCTIONS ===============
-def read_airfoil_coordinate_file(fpath: str, verbose: bool = True):
+def read_airfoil_coordinate_file(fpath: str, verbose: bool = True, te_gap_set: float = 0.004):
     """
     Function to read an airfoil coordinate listing file in .dat or .txt format, assumes foil name is on
     1st line, then reads in the list of coordinates following (ignoring any lines with numbers > 1.0, and
     assuming the coordinates are single-space delimited) -> this is the file format as downloaded from
 
     https://m-selig.ae.illinois.edu/ads/coord_database.html
 
@@ -286,18 +286,17 @@
 
     # flip lower if needed such that it is always increasing in x
     if not x_directions[-1] == 1:
         lower_coords = np.array(list(reversed(lower_coords)))
 
     # check TE gap
     te_gap = upper_coords[0][1] - lower_coords[-1][1]
-    te_gap_lim = 0.004
     blend_start = 0.7
-    if te_gap < te_gap_lim:
-        total_dy = (te_gap_lim - te_gap) / 2
+    if te_gap != te_gap_set:
+        total_dy = (te_gap_set - te_gap) / 2
 
         upper_idxs = np.where(upper_coords[:, 0] > blend_start)[0]
         for i in upper_idxs:
             xc, yc = upper_coords[i]
             dy = total_dy * (xc - blend_start) / (1 - blend_start)
             yc += dy
             upper_coords[i] = [xc, yc]
@@ -305,16 +304,16 @@
         lower_idxs = np.where(lower_coords[:, 0] > 0.8)[0]
         for i in lower_idxs:
             xc, yc = lower_coords[i]
             dy = total_dy * (xc - blend_start) / (1 - blend_start)
             yc -= dy
             lower_coords[i] = [xc, yc]
         if verbose:
-            Info('Detected airfoil ({}) with TE thinner than hardcoded limit\n-> artificially adjusted TE gap to {} '
-                     '(normalized)'.format(name, te_gap_lim))
+            Info('Detected airfoil ({}) with TE not equal to the requested value\n-> artificially adjusted TE gap to {} '
+                     '(normalized)'.format(name, te_gap_set))
 
     # re-combine upper and lower coords and split back into x, y arrays
     if upper_coords[-1][0] == lower_coords[0][0] and upper_coords[-1][1] == lower_coords[0][1]:  # check for double 0, 0
         coords = np.append(upper_coords, lower_coords[1:], axis=0)
     else:
         coords = np.append(upper_coords, lower_coords, axis=0)
 
@@ -367,26 +366,36 @@
                 f.write('cl{}\n'.format(cl))
         f.write('!\n{}'.format(' ' * 100) * keypress_iternum)
         f.write('pwrt\n')
         f.write('{}\n\n\n'.format(output_fpath))
         f.write('quit\n')
 
     # now open it again and send it as the xfoil commands
+    # CREATE_NO_WINDOW = 0x08000000   # flag to create no window, should work on both Windows and Linux??
     with open(xfoil_cmnd_file, 'r') as f:
+        # if hide_windows:
+        #     create_kw = {'creationflags': subprocess.CREATE_NO_WINDOW}
+        # else:
+        #     create_kw = {}
+
         sui = subprocess.STARTUPINFO()
         if hide_windows:
             sui.dwFlags |= subprocess.STARTF_USESHOWWINDOW
 
         if verbose:
             out, err = None, None
         else:
             out, err = subprocess.DEVNULL, subprocess.DEVNULL
 
         subprocess.run([xfoil_fpath], startupinfo=sui, stdin=f, stdout=out, stderr=err,
                        timeout=tmout, cwd=xfoil_dir)
+        # subprocess.run([xfoil_fpath], stdin=f, stdout=out, stderr=err, timeout=tmout, cwd=xfoil_dir,
+        #                **create_kw)
+        # p = subprocess.Popen([xfoil_fpath], stdin=f, stdout=out, stderr=err, cwd=xfoil_dir, **create_kw)
+        # p.wait(timeout=tmout)
 
     # delete the temp command file
     os.remove(xfoil_cmnd_file)
 
 
 def read_xfoil_pacc_file(fpath: str = None, delete_after: bool = False):
     # if not given, default fpath is this
@@ -1152,14 +1161,16 @@
     """
     v1_u = unit_vector(v1)
     v2_u = unit_vector(v2)
     return np.arccos(np.clip(np.dot(v1_u, v2_u), -1.0, 1.0))
 
 
 def compute_polygon_angles(exterior_coords: list):
+    if exterior_coords[0] == exterior_coords[-1]:
+        removed = exterior_coords.pop(-1)
     angles = []
     for i in range(len(exterior_coords)):
         pt = exterior_coords[i]
         last_pt = exterior_coords[i - 1]
         if i == len(exterior_coords) - 1:
             next_pt = exterior_coords[0]
         else:
@@ -1168,15 +1179,15 @@
         v1 = [next_pt[0] - pt[0], next_pt[1] - pt[1], next_pt[2] - pt[2]]
         v2 = [last_pt[0] - pt[0], last_pt[1] - pt[1], last_pt[2] - pt[2]]
         ang = angle_between(v1, v2)
         angles.append(ang)
     return angles
 
 
-def compute_profile_trimesh(profile_coords):
+def compute_profile_trimesh(profile_coords, reverse_order: bool = False):
     if len(profile_coords) == 3:
         xc, yc, zc = profile_coords
     elif len(profile_coords) == 2:
         xc, yc = profile_coords
         zc = np.zeros(len(xc))
     else:
         raise ValueError('len of profile_coords must be either 2 or 3')
@@ -1196,15 +1207,18 @@
         min_idx = np.argmin(angles)
         prev_idx = min_idx - 1
         if min_idx == len(angles) - 1:
             next_idx = 0
         else:
             next_idx = min_idx + 1
         pt1, pt2, pt3 = points[prev_idx], points[min_idx], points[next_idx]
-        vector = [pt1, pt2, pt3]
+        if not reverse_order:
+            vector = [pt1, pt2, pt3]
+        else:
+            vector = [pt3, pt2, pt1]
         vectors.append(vector)
         _ = points.pop(min_idx)
 
     return vectors
 
 
 # ===== USER INTERFACE STUFF =====
```

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/helper_ui_classes.py` & `propeller_design_tools-0.3.2/propeller_design_tools/helper_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/helper_ui_subclasses.py` & `propeller_design_tools-0.3.2/propeller_design_tools/helper_ui_subclasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,14 +342,15 @@
 
     def set_default_str(self, default_str: str):
         if default_str is not None:
             self.setValue(self.valueFromText(default_str))
 
     def set_box_range(self, box_range):
         if box_range is not None:
+            box_range = [int(v) for v in box_range]
             self.setRange(*box_range)   # the * unpacks this from tuple or list into 2 values min, max
 
     def set_box_single_step(self, box_single_step):
         if box_single_step is not None:
             self.setSingleStep(box_single_step)
```

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/optimizations.py` & `propeller_design_tools-0.3.2/propeller_design_tools/optimizations.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_analysis_ui_classes.py` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_analysis_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_creation_ui_classes.py` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_creation_ui_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         form_lay2c.addRow(PDT_Label('Atmosphere\nProperties->', font_size=12), self.atmo_props_widg)
         self.station_params_widg = StationParamsWidget()
         form_lay2c.addRow(PDT_Label('Control\nStations->', font_size=12), self.station_params_widg)
 
         # extra geo params
         form_lay2c.addRow(PDT_Label('Extra Geometry Output Parameters', font_size=14, bold=True))
         self.skew_sb = PDT_DoubleSpinBox(font_size=12, width=80)
-        self.skew_sb.setMaximum(45)
+        self.skew_sb.setMaximum(70)
         form_lay2c.addRow(PDT_Label('Skew:', font_size=12), self.skew_sb)
         self.n_prof_pts_sb = PDT_SpinBox(font_size=12, width=80)
         self.n_prof_pts_sb.setSpecialValueText('None')
         form_lay2c.addRow(PDT_Label('# Profile Pts:', font_size=12), self.n_prof_pts_sb)
         self.n_profs_sb = PDT_SpinBox(font_size=12, width=80, box_range=[0, 500])
         form_lay2c.addRow(PDT_Label('# Radial Profiles:', font_size=12), self.n_profs_sb)
```

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/xrotor.exe` & `propeller_design_tools-0.3.2/propeller_design_tools/prop_database/xrotor.exe`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/propeller.py` & `propeller_design_tools-0.3.2/propeller_design_tools/propeller.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,14 @@
                                     val[key] = float(entry)
                                 except:     # otherwise store as string
                                     val[key] = entry
                         elif tipe is list:
                             val = []
                     setattr(self, attr, val)
         self.set_blade_data(blade_dict=blade_data)
-        self.set_bld_profiles(point_dict=point_cloud)
 
     def read_xrotor_restart(self):
         with open(self.xrr_file, 'r') as f:
             txt = f.read().strip()
         lines = txt.split('\n')
 
         def read_line_pair(kw_idx):
@@ -327,28 +326,14 @@
         for st in self.stations:
             fig = st.plot_xrotor_fit_params()
 
     def set_blade_data(self, blade_dict: dict):
         self.blade_data = blade_dict
         return
 
-    def set_bld_profiles(self, point_dict: dict):
-        pc = {}
-        for key, val in point_dict.items():
-            fkey, axkey = key.strip(')').split('(', 1)
-            r = float(fkey)
-            if r not in pc:
-                pc[r] = {}
-            pc[r][axkey] = val
-
-        for key, val in pc.items():
-            pc[key] = np.vstack([val[ak] for ak in ['x', 'y']])
-        self.blade_xyz_profiles = pc
-        return
-
     def save_meta_file(self):
         attrs_2_ignore = ['blade_xyz_profiles', 'meta_file', 'xrr_file', 'xrop_file', 'station_polars']   # ignore the files so that prop_dirs can be switched
 
         if os.path.exists(self.meta_file):
             os.remove(self.meta_file)
 
         with open(self.meta_file, 'w') as f:
@@ -426,15 +411,16 @@
             Info('Blade "skew" is not implemented in XROTOR, and therefore not reflected in XROTOR results.\n'
                  '  > Skew effects are considered negligible for PDT purposes for small enough skew angles.')
 
         # clear out the existing xyz profiles
         funcs.delete_files_from_folder(self.bld_prof_folder)
 
         station = self.stations[0]
-        nondim_coords = station.foil.get_coords(n_interp=n_prof_pts)
+        # nondim_coords = station.foil.get_coords(n_interp=n_prof_pts)
+        nondim_coords = station.foil.get_coords_closed_te(n_interp=n_prof_pts)
 
         self.blade_xyz_profiles = {}
         for i, roR in enumerate(np.linspace(self.blade_data['r/R'][0], self.blade_data['r/R'][-1], n_profs)):
             chord = np.interp(x=roR, xp=self.blade_data['r/R'], fp=self.blade_data['CH']) * self.radius
             beta = np.rad2deg(np.interp(x=roR, xp=self.blade_data['r/R'], fp=self.blade_data['BE']))
             skew = tot_skew * roR
             r = roR * self.radius
@@ -866,52 +852,59 @@
                     vector = Custom3DArrow(view=view, tip_root=[vector_tip, vector_root], width=3, color=(.92, .84, .2, 1))
 
         return view
 
     def generate_stl_geometry(self, plot_after: bool = True, verbose: bool = True):
         n_prof = len(self.blade_xyz_profiles)
         n_pts = np.max(np.shape(self.blade_xyz_profiles[0]))
-        n_tri = n_pts * 2 * n_prof
+        n_main_surf = (n_prof - 1) * 2 * (n_pts - 1)
+        n_root = n_pts - 3
+        n_tip = n_pts - 3
+        n_tri = n_main_surf + n_root + n_tip
 
         mdata = np.zeros(n_tri, dtype=mesh.Mesh.dtype)
 
         tri_idx = 0
 
+        # root profile
+        vectors = funcs.compute_profile_trimesh(profile_coords=self.blade_xyz_profiles[0])  # outwards
+        # vectors = funcs.compute_profile_trimesh(profile_coords=self.blade_xyz_profiles[0], reverse_order=True)  # inwards
+        for vec in vectors:
+            mdata['vectors'][tri_idx] = np.array(vec)
+            tri_idx += 1
+
+        # tip profile
+        vectors = funcs.compute_profile_trimesh(profile_coords=self.blade_xyz_profiles[n_prof - 1], reverse_order=True)    # outwards
+        # vectors = funcs.compute_profile_trimesh(profile_coords=self.blade_xyz_profiles[n_prof - 1])    # inwards
+        for vec in vectors:
+            mdata['vectors'][tri_idx] = np.array(vec)
+            tri_idx += 1
+
         # iterate over the profiles
         for k in range(n_prof - 1):
             xyz_prof = self.blade_xyz_profiles[k]
             nxt_prof = self.blade_xyz_profiles[k + 1]
 
-            # root profile
-            if k == 0:
-                vectors = funcs.compute_profile_trimesh(profile_coords=xyz_prof)
-                for vec in vectors:
-                    mdata['vectors'][tri_idx] = np.array(vec)
-                    tri_idx += 1
-
-            # tip profile
-            if k == n_prof - 2:
-                vectors = funcs.compute_profile_trimesh(profile_coords=nxt_prof)
-                for vec in vectors:
-                    mdata['vectors'][tri_idx] = np.array(vec)
-                    tri_idx += 1
-
             # inter-profile surfaces
-            for i in range(n_pts):  # right hand rule to get normal direction correct
-                if i == n_pts - 1:     # TE gap
-                    i = -1
+            for i in range(n_pts - 1):  # right hand rule to get normal direction correct
                 a = xyz_prof[:, i]  # a is a point-coordinate in (x, y, z) format
                 b = nxt_prof[:, i]  # same for b-f
                 c = nxt_prof[:, i + 1]
                 d = a.copy()
                 e = c.copy()
                 f = xyz_prof[:, i + 1]
 
+                # outwards
                 mdata['vectors'][tri_idx] = np.array([a, b, c])      # populate the array of triangle vectors
                 mdata['vectors'][tri_idx + 1] = np.array([d, e, f])  # going in order, 2 triangles per iteration
+
+                # inwards
+                # mdata['vectors'][tri_idx] = np.array([c, b, a])      # populate the array of triangle vectors
+                # mdata['vectors'][tri_idx + 1] = np.array([f, e, d])  # going in order, 2 triangles per iteration
+
                 tri_idx += 2
 
         m = mesh.Mesh(mdata)
 
         if os.path.exists(self.stl_fpath):
             os.remove(self.stl_fpath)
         m.save(filename=self.stl_fpath)
```

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/radialstation.py` & `propeller_design_tools-0.3.2/propeller_design_tools/radialstation.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/science_spinbox_class.py` & `propeller_design_tools-0.3.2/propeller_design_tools/science_spinbox_class.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/settings.py` & `propeller_design_tools-0.3.2/propeller_design_tools/settings.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/crosshair_cursor.png` & `propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/crosshair_cursor.png`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot1.wav` & `propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot1.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot2.wav` & `propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot2.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot3.wav` & `propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot3.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot4.wav` & `propeller_design_tools-0.3.2/propeller_design_tools/supporting_files/gunshot4.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/user_interface.py` & `propeller_design_tools-0.3.2/propeller_design_tools/user_interface.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools/user_io.py` & `propeller_design_tools-0.3.2/propeller_design_tools/user_io.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/propeller_design_tools.egg-info/SOURCES.txt` & `propeller_design_tools-0.3.2/propeller_design_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.9/setup.cfg` & `propeller_design_tools-0.3.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 726f 7065 6c6c 6572 5f64 6573   = propeller_des
 00000020: 6967 6e5f 746f 6f6c 730d 0a76 6572 7369  ign_tools..versi
-00000030: 6f6e 203d 2030 2e32 2e39 0d0a 6175 7468  on = 0.2.9..auth
+00000030: 6f6e 203d 2030 2e33 2e32 0d0a 6175 7468  on = 0.3.2..auth
 00000040: 6f72 203d 204a 6163 6f62 2042 726f 6e73  or = Jacob Brons
 00000050: 6f6e 0d0a 6175 7468 6f72 5f65 6d61 696c  on..author_email
 00000060: 203d 206a 616b 6562 726f 6e73 6f6e 3839   = jakebronson89
 00000070: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000080: 7269 7074 696f 6e20 3d20 546f 6f6c 732c  ription = Tools,
 00000090: 2066 6f72 2070 726f 7065 6c6c 6572 2064   for propeller d
 000000a0: 6573 6967 6e20 2861 7574 6f6d 6174 6573  esign (automates
@@ -26,39 +26,39 @@
 00000190: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
 000001a0: 2f67 6974 6875 622e 636f 6d2f 6865 6c6c  /github.com/hell
 000001b0: 6f44 6573 7472 6f79 6572 4f66 576f 726c  oDestroyerOfWorl
 000001c0: 6473 2f70 726f 7065 6c6c 6572 5f64 6573  ds/propeller_des
 000001d0: 6967 6e5f 746f 6f6c 732f 6973 7375 6573  ign_tools/issues
 000001e0: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
 000001f0: 0d0a 0944 6576 656c 6f70 6d65 6e74 2053  ...Development S
-00000200: 7461 7475 7320 3a3a 2032 202d 2050 7265  tatus :: 2 - Pre
-00000210: 2d41 6c70 6861 0d0a 0949 6e74 656e 6465  -Alpha...Intende
-00000220: 6420 4175 6469 656e 6365 203a 3a20 5363  d Audience :: Sc
-00000230: 6965 6e63 652f 5265 7365 6172 6368 0d0a  ience/Research..
-00000240: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-00000250: 4170 7072 6f76 6564 203a 3a20 474e 5520  Approved :: GNU 
-00000260: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
-00000270: 6963 656e 7365 2076 3320 2847 504c 7633  icense v3 (GPLv3
-00000280: 290d 0a09 4e61 7475 7261 6c20 4c61 6e67  )...Natural Lang
-00000290: 7561 6765 203a 3a20 456e 676c 6973 680d  uage :: English.
-000002a0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000002b0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002c0: 203a 3a20 330d 0a09 4f70 6572 6174 696e   :: 3...Operatin
-000002d0: 6720 5379 7374 656d 203a 3a20 4d69 6372  g System :: Micr
-000002e0: 6f73 6f66 7420 3a3a 2057 696e 646f 7773  osoft :: Windows
-000002f0: 0d0a 0954 6f70 6963 203a 3a20 5363 6965  ...Topic :: Scie
-00000300: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
-00000310: 6e67 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  ng....[options].
-00000320: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-00000330: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
-00000340: 6573 203d 203e 3d33 2e36 0d0a 696e 636c  es = >=3.6..incl
-00000350: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-00000360: 203d 2074 7275 650d 0a0d 0a5b 6f70 7469   = true....[opti
-00000370: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
-00000380: 5d0d 0a2a 203d 2070 726f 7065 6c6c 6572  ]..* = propeller
-00000390: 5f64 6573 6967 6e5f 746f 6f6c 732f 7375  _design_tools/su
-000003a0: 7070 6f72 7469 6e67 5f66 696c 6573 2f2a  pporting_files/*
-000003b0: 2e70 6e67 0d0a 0d0a 5b6f 7074 696f 6e73  .png....[options
-000003c0: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-000003d0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-000003e0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-000003f0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000200: 7461 7475 7320 3a3a 2033 202d 2041 6c70  tatus :: 3 - Alp
+00000210: 6861 0d0a 0949 6e74 656e 6465 6420 4175  ha...Intended Au
+00000220: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
+00000230: 652f 5265 7365 6172 6368 0d0a 094c 6963  e/Research...Lic
+00000240: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000250: 6f76 6564 203a 3a20 474e 5520 4765 6e65  oved :: GNU Gene
+00000260: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+00000270: 7365 2076 3320 2847 504c 7633 290d 0a09  se v3 (GPLv3)...
+00000280: 4e61 7475 7261 6c20 4c61 6e67 7561 6765  Natural Language
+00000290: 203a 3a20 456e 676c 6973 680d 0a09 5072   :: English...Pr
+000002a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000002b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000002c0: 330d 0a09 4f70 6572 6174 696e 6720 5379  3...Operating Sy
+000002d0: 7374 656d 203a 3a20 4d69 6372 6f73 6f66  stem :: Microsof
+000002e0: 7420 3a3a 2057 696e 646f 7773 0d0a 0954  t :: Windows...T
+000002f0: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
+00000300: 6963 2f45 6e67 696e 6565 7269 6e67 0d0a  ic/Engineering..
+00000310: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
+00000320: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
+00000330: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+00000340: 203e 3d33 2e36 0d0a 696e 636c 7564 655f   >=3.6..include_
+00000350: 7061 636b 6167 655f 6461 7461 203d 2074  package_data = t
+00000360: 7275 650d 0a0d 0a5b 6f70 7469 6f6e 732e  rue....[options.
+00000370: 7061 636b 6167 655f 6461 7461 5d0d 0a2a  package_data]..*
+00000380: 203d 2070 726f 7065 6c6c 6572 5f64 6573   = propeller_des
+00000390: 6967 6e5f 746f 6f6c 732f 7375 7070 6f72  ign_tools/suppor
+000003a0: 7469 6e67 5f66 696c 6573 2f2a 2e70 6e67  ting_files/*.png
+000003b0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+000003c0: 6b61 6765 732e 6669 6e64 5d0d 0a0d 0a5b  kages.find]....[
+000003d0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000003e0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+000003f0: 6520 3d20 300d 0a0d 0a                   e = 0....
```

