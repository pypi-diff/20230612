# Comparing `tmp/nanoqnt-0.2.0.tar.gz` & `tmp/nanoqnt-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoqnt-0.2.0.tar", max compression
+gzip compressed data, was "nanoqnt-0.2.0rc1.tar", max compression
```

## Comparing `nanoqnt-0.2.0.tar` & `nanoqnt-0.2.0rc1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0        0 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/__init__.py
--rw-r--r--   0        0        0     4154 2023-03-24 15:14:25.767476 nanoqnt-0.2.0/nanoqnt/dispertech-logo.ico
--rw-r--r--   0        0        0      851 2023-05-10 11:53:19.425596 nanoqnt-0.2.0/nanoqnt/main.py
--rw-r--r--   0        0        0        0 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/model/__init__.py
--rw-r--r--   0        0        0    13028 2023-05-10 07:36:10.399369 nanoqnt-0.2.0/nanoqnt/model/analyze_nanoqnt.py
--rw-r--r--   0        0        0      289 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/model/decorators.py
--rw-r--r--   0        0        0       34 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/model/exceptions.py
--rw-r--r--   0        0        0     1541 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/model/stage_control.py
--rw-r--r--   0        0        0      401 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/stage_main.py
--rw-r--r--   0        0        0      335 2023-04-18 06:49:12.570624 nanoqnt-0.2.0/nanoqnt/util/__init__.py
--rw-r--r--   0        0        0       63 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/__init__.py
--rw-r--r--   0        0        0      870 2023-05-10 07:36:10.414717 nanoqnt-0.2.0/nanoqnt/view/channel_selector.py
--rw-r--r--   0        0        0     2282 2023-05-10 07:36:10.405463 nanoqnt-0.2.0/nanoqnt/view/GUI/channel_selector.ui
--rw-r--r--   0        0        0    15341 2023-05-10 07:36:10.411641 nanoqnt-0.2.0/nanoqnt/view/GUI/data_exploration.ui
--rw-r--r--   0        0        0     3759 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg
--rw-r--r--   0        0        0     4715 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11814 - Atom.svg
--rw-r--r--   0        0        0     3727 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11815 - Battery.svg
--rw-r--r--   0        0        0     5275 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11816 - Orbit.svg
--rw-r--r--   0        0        0     2802 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11817 - Beaker.svg
--rw-r--r--   0        0        0     4637 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg
--rw-r--r--   0        0        0     1936 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11819 - Bounce.svg
--rw-r--r--   0        0        0     2442 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11820 - Caliper.svg
--rw-r--r--   0        0        0     2191 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11821 - Catapult.svg
--rw-r--r--   0        0        0     2594 2023-03-23 13:26:26.889455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11822 - Collision.svg
--rw-r--r--   0        0        0     2347 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg
--rw-r--r--   0        0        0     2347 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg
--rw-r--r--   0        0        0     2710 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg
--rw-r--r--   0        0        0     3426 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg
--rw-r--r--   0        0        0     3508 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg
--rw-r--r--   0        0        0     3527 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11828 - Energy.svg
--rw-r--r--   0        0        0     1821 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11829 - Flask.svg
--rw-r--r--   0        0        0     4901 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11830 - Float.svg
--rw-r--r--   0        0        0     1522 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg
--rw-r--r--   0        0        0     8697 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11832 - Force.svg
--rw-r--r--   0        0        0     3310 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11833 - Formula.svg
--rw-r--r--   0        0        0     2416 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11834 - Gears.svg
--rw-r--r--   0        0        0     4479 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11835 - Gravity.svg
--rw-r--r--   0        0        0     4165 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg
--rw-r--r--   0        0        0     3653 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11837 - Histogram.svg
--rw-r--r--   0        0        0     2013 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg
--rw-r--r--   0        0        0     2576 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11839 - Magnet.svg
--rw-r--r--   0        0        0     5579 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg
--rw-r--r--   0        0        0     3646 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11841 - Metronome.svg
--rw-r--r--   0        0        0     1706 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg
--rw-r--r--   0        0        0     3307 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11843 - Molecule.svg
--rw-r--r--   0        0        0     2707 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11844 - Motion.svg
--rw-r--r--   0        0        0     1163 2023-03-23 13:26:26.899455 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg
--rw-r--r--   0        0        0     5179 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg
--rw-r--r--   0        0        0     2264 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg
--rw-r--r--   0        0        0     4868 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11848 - Planet.svg
--rw-r--r--   0        0        0     9381 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg
--rw-r--r--   0        0        0      806 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11850 - Power.svg
--rw-r--r--   0        0        0     2581 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11851 - Press.svg
--rw-r--r--   0        0        0     3090 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11852 - Proton.svg
--rw-r--r--   0        0        0     2528 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11853 - Pulley.svg
--rw-r--r--   0        0        0     4144 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11854 - Reflection.svg
--rw-r--r--   0        0        0     3109 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11855 - Resistor.svg
--rw-r--r--   0        0        0     2481 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11856 - Rolling.svg
--rw-r--r--   0        0        0     3390 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11857 - Rotate.svg
--rw-r--r--   0        0        0     2463 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg
--rw-r--r--   0        0        0     2156 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11859 - Temperature.svg
--rw-r--r--   0        0        0     2552 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg
--rw-r--r--   0        0        0     2816 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11861 - Waves.svg
--rw-r--r--   0        0        0     3799 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg
--rw-r--r--   0        0        0       46 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/Icons.qrc
--rw-r--r--   0        0        0      342 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/Open Folder.svg
--rw-r--r--   0        0        0      215 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/open.svg
--rw-r--r--   0        0        0      559 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/Save.svg
--rw-r--r--   0        0        0     5754 2023-05-10 07:36:10.411641 nanoqnt-0.2.0/nanoqnt/view/GUI/particles_widget.ui
--rw-r--r--   0        0        0     3497 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/GUI/scan_control.ui
--rw-r--r--   0        0        0    11492 2023-05-10 07:36:10.414717 nanoqnt-0.2.0/nanoqnt/view/main_window.py
--rw-r--r--   0        0        0     2002 2023-05-10 07:36:10.414717 nanoqnt-0.2.0/nanoqnt/view/particle_widget.py
--rw-r--r--   0        0        0     1390 2023-03-23 13:26:26.909458 nanoqnt-0.2.0/nanoqnt/view/stage_control.py
--rw-r--r--   0        0        0      538 2023-05-10 11:36:40.385695 nanoqnt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-10 09:53:29.080137 nanoqnt-0.2.0/README.md
--rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 nanoqnt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-06-12 12:02:24.897116 nanoqnt-0.2.0rc1/README.md
+-rw-r--r--   0        0        0        0 2023-01-02 14:34:22.063965 nanoqnt-0.2.0rc1/nanoqnt/__init__.py
+-rw-r--r--   0        0        0     4154 2023-06-12 12:02:24.898367 nanoqnt-0.2.0rc1/nanoqnt/dispertech-logo.ico
+-rw-r--r--   0        0        0      820 2023-06-12 12:02:24.899141 nanoqnt-0.2.0rc1/nanoqnt/main.py
+-rw-r--r--   0        0        0        0 2022-12-20 12:52:00.514018 nanoqnt-0.2.0rc1/nanoqnt/model/__init__.py
+-rw-r--r--   0        0        0    13247 2023-06-12 12:02:24.899813 nanoqnt-0.2.0rc1/nanoqnt/model/analyze_nanoqnt.py
+-rw-r--r--   0        0        0      280 2023-06-12 12:02:24.900270 nanoqnt-0.2.0rc1/nanoqnt/model/decorators.py
+-rw-r--r--   0        0        0       34 2023-06-12 12:02:24.900680 nanoqnt-0.2.0rc1/nanoqnt/model/exceptions.py
+-rw-r--r--   0        0        0      385 2023-06-12 12:02:24.901046 nanoqnt-0.2.0rc1/nanoqnt/stage_main.py
+-rw-r--r--   0        0        0      351 2023-06-12 12:02:24.901498 nanoqnt-0.2.0rc1/nanoqnt/util/__init__.py
+-rw-r--r--   0        0        0     1202 2023-06-12 12:02:24.901860 nanoqnt-0.2.0rc1/nanoqnt/util/make_hdf5.py
+-rw-r--r--   0        0        0     3759 2022-03-16 14:59:30.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg
+-rw-r--r--   0        0        0     4715 2022-03-16 14:59:22.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11814 - Atom.svg
+-rw-r--r--   0        0        0     3727 2022-03-16 14:59:14.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11815 - Battery.svg
+-rw-r--r--   0        0        0     5275 2022-03-16 14:59:06.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11816 - Orbit.svg
+-rw-r--r--   0        0        0     2802 2022-03-16 14:58:58.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11817 - Beaker.svg
+-rw-r--r--   0        0        0     4637 2022-03-16 14:58:50.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg
+-rw-r--r--   0        0        0     1936 2022-03-16 14:58:44.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11819 - Bounce.svg
+-rw-r--r--   0        0        0     2442 2022-03-16 14:58:36.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11820 - Caliper.svg
+-rw-r--r--   0        0        0     2191 2022-03-16 14:58:28.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11821 - Catapult.svg
+-rw-r--r--   0        0        0     2594 2022-03-16 14:58:22.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11822 - Collision.svg
+-rw-r--r--   0        0        0     2347 2022-03-16 14:58:14.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg
+-rw-r--r--   0        0        0     2347 2022-03-16 14:58:04.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg
+-rw-r--r--   0        0        0     2710 2022-03-16 14:57:56.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg
+-rw-r--r--   0        0        0     3426 2022-03-16 15:19:36.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg
+-rw-r--r--   0        0        0     3508 2022-03-16 14:57:38.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg
+-rw-r--r--   0        0        0     3527 2022-03-16 14:57:30.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11828 - Energy.svg
+-rw-r--r--   0        0        0     1821 2022-03-16 14:57:22.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11829 - Flask.svg
+-rw-r--r--   0        0        0     4901 2022-03-16 14:57:14.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11830 - Float.svg
+-rw-r--r--   0        0        0     1522 2022-03-16 14:57:06.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg
+-rw-r--r--   0        0        0     8697 2022-03-16 14:56:58.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11832 - Force.svg
+-rw-r--r--   0        0        0     3310 2022-03-16 14:56:48.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11833 - Formula.svg
+-rw-r--r--   0        0        0     2416 2022-03-16 14:56:40.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11834 - Gears.svg
+-rw-r--r--   0        0        0     4479 2022-03-16 14:56:32.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11835 - Gravity.svg
+-rw-r--r--   0        0        0     4165 2022-03-16 14:56:24.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg
+-rw-r--r--   0        0        0     3653 2022-03-16 14:56:16.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11837 - Histogram.svg
+-rw-r--r--   0        0        0     2013 2022-03-16 14:56:08.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg
+-rw-r--r--   0        0        0     2576 2022-03-16 14:56:00.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11839 - Magnet.svg
+-rw-r--r--   0        0        0     5579 2022-03-16 14:55:54.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg
+-rw-r--r--   0        0        0     3646 2022-03-16 14:55:46.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11841 - Metronome.svg
+-rw-r--r--   0        0        0     1706 2022-03-16 14:55:38.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg
+-rw-r--r--   0        0        0     3307 2022-03-16 14:55:32.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11843 - Molecule.svg
+-rw-r--r--   0        0        0     2707 2022-03-16 14:55:24.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11844 - Motion.svg
+-rw-r--r--   0        0        0     1163 2022-03-16 14:55:18.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg
+-rw-r--r--   0        0        0     5179 2022-03-16 14:55:10.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg
+-rw-r--r--   0        0        0     2264 2022-03-16 14:55:02.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg
+-rw-r--r--   0        0        0     4868 2022-03-16 14:54:54.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11848 - Planet.svg
+-rw-r--r--   0        0        0     9381 2022-03-16 14:54:44.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg
+-rw-r--r--   0        0        0      806 2022-03-16 14:54:36.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11850 - Power.svg
+-rw-r--r--   0        0        0     2581 2022-03-16 14:54:28.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11851 - Press.svg
+-rw-r--r--   0        0        0     3090 2022-03-16 14:54:20.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11852 - Proton.svg
+-rw-r--r--   0        0        0     2528 2022-03-16 14:54:12.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11853 - Pulley.svg
+-rw-r--r--   0        0        0     4144 2022-03-16 14:54:04.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11854 - Reflection.svg
+-rw-r--r--   0        0        0     3109 2022-03-16 14:53:56.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11855 - Resistor.svg
+-rw-r--r--   0        0        0     2481 2022-03-16 14:53:54.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11856 - Rolling.svg
+-rw-r--r--   0        0        0     3390 2022-03-16 14:53:52.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11857 - Rotate.svg
+-rw-r--r--   0        0        0     2463 2022-03-16 14:53:50.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg
+-rw-r--r--   0        0        0     2156 2022-03-16 14:53:48.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11859 - Temperature.svg
+-rw-r--r--   0        0        0     2552 2022-03-16 14:53:48.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg
+-rw-r--r--   0        0        0     2816 2022-03-16 15:41:46.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11861 - Waves.svg
+-rw-r--r--   0        0        0     3799 2022-03-16 14:53:44.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg
+-rw-r--r--   0        0        0       43 2022-12-20 12:57:18.786580 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/Icons.qrc
+-rw-r--r--   0        0        0      342 2022-11-15 12:55:54.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/Open Folder.svg
+-rw-r--r--   0        0        0      559 2022-11-15 12:55:54.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/Save.svg
+-rw-r--r--   0        0        0      215 2020-07-27 20:54:42.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/open.svg
+-rw-r--r--   0        0        0     2193 2023-06-12 12:02:24.902373 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/channel_selector.ui
+-rw-r--r--   0        0        0    14859 2023-06-12 12:02:24.902919 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/data_exploration.ui
+-rw-r--r--   0        0        0     5564 2023-06-12 12:02:24.903391 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/particles_widget.ui
+-rw-r--r--   0        0        0     3367 2023-01-26 21:32:32.021169 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/scan_control.ui
+-rw-r--r--   0        0        0       62 2023-06-12 12:02:24.903693 nanoqnt-0.2.0rc1/nanoqnt/view/__init__.py
+-rw-r--r--   0        0        0      848 2023-06-12 12:02:24.903942 nanoqnt-0.2.0rc1/nanoqnt/view/channel_selector.py
+-rw-r--r--   0        0        0    11311 2023-06-12 12:02:24.904324 nanoqnt-0.2.0rc1/nanoqnt/view/main_window.py
+-rw-r--r--   0        0        0     1947 2023-06-12 12:02:24.904552 nanoqnt-0.2.0rc1/nanoqnt/view/particle_widget.py
+-rw-r--r--   0        0        0     1359 2023-06-12 12:02:24.904821 nanoqnt-0.2.0rc1/nanoqnt/view/stage_control.py
+-rw-r--r--   0        0        0      516 2023-06-12 12:17:21.653416 nanoqnt-0.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nanoqnt-0.2.0rc1/PKG-INFO
```

### Comparing `nanoqnt-0.2.0/nanoqnt/dispertech-logo.ico` & `nanoqnt-0.2.0rc1/nanoqnt/dispertech-logo.ico`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/main.py` & `nanoqnt-0.2.0rc1/nanoqnt/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-import os
-from multiprocessing import freeze_support
-
-import sys
-
-from PyQt5 import QtGui
-from PyQt5.QtWidgets import QApplication
-
-from nanoqnt.model.analyze_nanoqnt import AnalyzeNanoQNT
-from nanoqnt.view.main_window import NanoQNTMainWindow
-
-try:
-    from ctypes import windll  # Only exists on Windows.
-    myappid = 'Dispertech.NanoQNT.Analysis.0.2.0'
-    windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
-except ImportError:
-    pass
-
-def start_nanoqnt():
-    basedir = os.path.dirname(__file__)
-    model = AnalyzeNanoQNT()
-    app = QApplication([])
-    app.setWindowIcon(QtGui.QIcon(os.path.join(basedir, 'dispertech-logo.ico')))
-    main_window = NanoQNTMainWindow(model)
-    main_window.show()
-    app.exec()
-    sys.exit()
-
-
-if __name__ == '__main__':
-    freeze_support()
-    start_nanoqnt()
+import os
+import sys
+from multiprocessing import freeze_support
+
+from PyQt5 import QtGui
+from PyQt5.QtWidgets import QApplication
+
+from nanoqnt.model.analyze_nanoqnt import AnalyzeNanoQNT
+from nanoqnt.view.main_window import NanoQNTMainWindow
+
+try:
+    from ctypes import windll  # Only exists on Windows.
+
+    myappid = 'Dispertech.NanoQNT.Analysis.0.2.0'
+    windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
+except ImportError:
+    pass
+
+
+def start_nanoqnt():
+    basedir = os.path.dirname(__file__)
+    model = AnalyzeNanoQNT()
+    app = QApplication([])
+    app.setWindowIcon(QtGui.QIcon(os.path.join(basedir, 'dispertech-logo.ico')))
+    main_window = NanoQNTMainWindow(model)
+    main_window.show()
+    app.exec()
+    sys.exit()
+
+
+if __name__ == '__main__':
+    freeze_support()
+    start_nanoqnt()
```

### Comparing `nanoqnt-0.2.0/nanoqnt/model/analyze_nanoqnt.py` & `nanoqnt-0.2.0rc1/nanoqnt/model/analyze_nanoqnt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,277 +1,289 @@
-import numpy as np
-import skimage
-import yaml
-from pathlib import Path
-
-import pandas as pd
-import pims as pims
-import trackpy as tp
-from scipy.spatial import KDTree
-from skimage import morphology
-from skimage.measure import label, regionprops, regionprops_table
-from trackpy.find import where_close
-from trackpy.utils import pandas_concat
-import scipy.optimize as opt
-
-from nanoqnt.util import twoD_Gaussian
-
-
-class AnalyzeNanoQNT:
-    def __init__(self):
-        self.filename = None
-        self.data = None
-        self.metadata = {}
-        self.particle_df = []
-        self.particles = pd.DataFrame()
-        self.num_frames = 0
-        self.find_settings = {}
-        self.filename = Path.home()
-        self.concentration = 0  # pcles/ml
-        self.linked_particles = None
-        self.total_num_particles = 0
-        self.summarized_particles = None
-
-        self.ignore_edge_pixels = 8
-
-        self.num_channels = 1
-        self.channels_data = {}
-        self.bkg = None
-
-    def open(self, filename):
-        """ Opens the file with the data. Normally a multi-tiff file, but it can be adapted to other formats.
-
-        :param filename:
-        """
-        self.filename = Path(filename)
-        self.metadata['filename'] = filename
-        self.metadata['last_dir'] = self.filename.parent
-        self.data = pims.open(filename)
-        self.num_frames = len(self.data)  # This is really the number of frames in the data, not the number of
-        # multi-channel frames
-
-        self.particle_df = [pd.DataFrame() for _ in range(len(self.data))]
-        self.particles = pd.DataFrame()
-        self.find_settings = {}
-        self.linked_particles = None
-        self.summarized_particles = None
-        self.total_num_particles = 0
-        self.channels_data = {}
-
-    def find_particles(self, frame_num, diameter, minmass, method='mask'):
-        """ Finds particles in a given frame and stores the data frame in a list indexed by the frame number.
-
-        :param int frame_num: The number of the frame (0-indexed) to analyze
-        :param int diameter: The expected diameter of the particles. Must be an odd number and is passed directly to
-        Trackpy
-        :param int minmass: Filter to select bright enough spots. The parameter is passed directly to Trackpy.
-        :param str method: Either select trackpy or mask. Default is mask.
-        """
-        if method == 'python' or method == 'numba':
-            if frame_num in self.find_settings:
-                settings = self.find_settings[frame_num]
-                if diameter == settings['diameter'] and minmass == settings['minmass']:
-                    return self.particle_df[frame_num]
-            self.find_settings[frame_num] = {
-                'diameter': diameter,
-                'minmass': minmass,
-                }
-            df = tp.locate(self.data[frame_num], diameter, minmass=minmass, characterize=False)
-            df = df.loc[df['y'] >= self.ignore_edge_pixels]
-            self.particle_df[frame_num] = df
-            return df
-
-        elif method == 'mask':
-            mask = self.data[frame_num] > minmass
-            mask = morphology.remove_small_objects(mask, diameter)
-            label_img = label(mask)
-            props = regionprops_table(label_img, intensity_image=np.array(self.data[frame_num]), properties=('centroid',
-                                                                                                             'intensity_mean',))
-            df = pd.DataFrame(props).rename(columns={'centroid-0': 'y', 'centroid-1': 'x', 'intensity_mean': 'mass'})
-            to_drop = where_close(df[['x', 'y']], separation=diameter * 2, intensity=df['mass'])
-            df = df.drop(to_drop)
-            df = df.loc[df['y'] >= self.ignore_edge_pixels]
-            self.particle_df[frame_num] = df
-            return df
-
-    def find_all_particles(self, frames_no, diameter, minmass, method='python'):
-        """ Finds all the particles in a given range of frames. If the data has multiple channels, then it can handle
-        different settings for each one. In that case, diameter and minmass must be iterables and in the appropriate
-        order, i.e., the first setting will be for the first channel, etc.
-
-        The data is structured as a dictionary, where each channel is a different key, and then the localizations are
-        stored as a pandas dataframe.
-
-        :param list frames_no:
-        :param tuple diameter:
-        :param tuple minmass:
-        :param str method:
-        :return dict: dictionary of particles found in each channel
-        """
-        try:
-            if len(diameter) != self.num_channels:
-                diameter = self.num_channels * [diameter]
-        except TypeError:
-            diameter = self.num_channels * [diameter]
-        try:
-            if len(minmass) != self.num_channels:
-                minmass = self.num_channels * [minmass]
-        except TypeError:
-            minmass = self.num_channels * [minmass]
-
-        if len(frames_no) == 1:
-            frames_no = (0, self.num_frames)
-
-        self.particles = {}
-
-        self.metadata.update({
-            'frames': frames_no,
-            'diameter': diameter,
-            'minmass': minmass,
-            'engine': method,
-            })
-
-        if method == 'mask':
-            for channel in range(self.num_channels):
-                all_features = []
-                for frame in range(frames_no[0], frames_no[1]):
-                    real_frame = frame*self.num_channels + channel
-                    df = self.find_particles(real_frame, diameter[channel], minmass[channel], method='mask')
-                    df['frame'] = frame
-                    all_features.append(df)
-                self.particles[channel] = pandas_concat(all_features).reset_index(drop=True)
-            return self.particles
-
-        ## For the python or numba methods, only 1-channel data is available
-        if self.num_channels > 1:
-            raise Exception("Trackpy-based methods only work with 1-channel data for the time being")
-
-        self.particles[0] = tp.batch(self.data[frames_no[0]:frames_no[1]],
-                                               diameter[0],
-                                               minmass=minmass[0],
-                                               characterize=False,
-                                               preprocess=False,
-                                               processes='auto',
-                                               engine=method)
-        self.particles[0]['intensity'] = np.nan
-
-        return self.particles
-
-    def link_particles(self, search_radius, memory=0, min_frames=0):
-        self.linked_particles = {}
-        for channel in range(self.num_channels):
-            self.linked_particles[channel] = tp.link(self.particles[channel], search_radius, memory=memory)
-            self.linked_particles[channel] = tp.filter_stubs(self.linked_particles[channel], min_frames)
-
-        self.metadata.update({
-                                 'search_radius': search_radius,
-                                 'min_frames': min_frames,
-                                 'memory': memory
-                                 })
-
-    def calculate_intensities(self):
-        """Calculates the intensities of the linked particles assuming they were the product of the mask method.
-        The methods that rely on the trackpy algorithm already include the intensity.
-        """
-        fit_size = 10
-        x_fit = np.linspace(0, 2 * fit_size, 2 * fit_size + 1)
-        y_fit = np.linspace(0, 2 * fit_size, 2 * fit_size + 1)
-        x_fit, y_fit = np.meshgrid(x_fit, y_fit)
-        initial_guess = (200, fit_size, fit_size, 2, 2, 200)
-
-        self.summary_data = {}
-        intensity_columns = [f'i_{channel}' for channel in range(self.num_channels)]
-        for channel in range(self.num_channels):
-            self.summary_data[channel] = pd.DataFrame(columns=['particle', 'frame', 'x', 'y'] + intensity_columns)
-
-            for p in self.linked_particles[channel]['particle'].unique():
-                pcle = self.linked_particles[channel].loc[self.linked_particles[channel]['particle'] == p]
-                ix = pcle['mass'].idxmax()
-                x = int(pcle.loc[ix]['y'])
-                y = int(pcle.loc[ix]['x'])
-                frame = int(pcle.loc[ix]['frame'])
-                # TODO: This is hardcoded and dangerous. The margin used to drop particles must be properly considered
-                if x < 20 or x > 2048 - 20 or y < 20 or y > 2048 - 20:
-                    continue
-
-                # try:
-                #     f = frame*self.num_channels + channel
-                #     popt, pcov = opt.curve_fit(twoD_Gaussian, (x_fit, y_fit),
-                #                                np.array(self.data[f][x - fit_size:x + fit_size + 1,
-                #                                         y - fit_size:y + fit_size + 1]).reshape(-1),
-                #                                p0=initial_guess)
-                # except Exception as e:
-                #     print(e)
-                #     continue
-
-                df = pd.DataFrame.from_dict({
-                    'particle': [p],
-                    'frame': [pcle.loc[ix]['frame']],
-                    'x': [pcle.loc[ix]['x']],
-                    'y': [pcle.loc[ix]['y']],
-                    f'i_{channel}': [pcle['mass'].max()]})
-                self.summary_data[channel] = pd.concat((self.summary_data[channel], df), ignore_index=True)
-            self.summary_data[channel] = self.summary_data[channel].reset_index(drop=True)
-
-    def multi_color_link(self):
-        """ Find the same particles in every channel and add the intensity information on each """
-        kd_trees = {}
-        for channel in range(self.num_channels):
-            kd_trees[channel] = KDTree(np.array(self.summary_data[channel][['x', 'y']]))
-
-        for channel in range(self.num_channels):
-            for channel_2 in range(channel+1, self.num_channels):
-                for ix, p in self.summary_data[channel].iterrows():
-                    dist, ind = kd_trees[channel_2].query((p['x'], p['y']), p=2, distance_upper_bound=15)
-                    if ind == kd_trees[channel_2].n:
-                        continue
-                    if abs(self.summary_data[channel_2].loc[ind]['frame'] - p['frame']) > 5:
-                        print('Frames too far apart with ', ix, p['x'], p['y'], p['frame'])
-                        continue
-                    self.summary_data[channel].loc[ix, f'i_{channel_2}'] = \
-                        self.summary_data[channel_2].loc[ind][f'i_{channel_2}']
-                    self.summary_data[channel_2].loc[ind, f'i_{channel}'] = p[f'i_{channel}']
-    def save_all_data(self, filename):
-        self.linked_particles.to_csv(str(filename))
-
-    def save_data(self, filename):
-        """ Saves only the most important information to the file: particle and intensity information.
-        """
-        if not type(filename) is Path:
-            filename = Path(filename)
-
-        for i in range(self.num_channels):
-            stem = filename.stem
-            file_name = filename.with_stem(f'{stem}_{i}')
-            self.summary_data[i].to_csv(str(file_name))
-
-        with open(filename.with_suffix('.yml'), 'w') as f:
-            yaml.dump(self.metadata, f)
-
-    def sub_pix_bias(self, index):
-        f = self.particle_df[index]
-        return f[['x', 'y']].applymap(lambda x: x % 1)
-
-    def calculate_concentration(self, step_size=5):
-        self.total_num_particles = {}
-        self.concentration = {}
-        if self.linked_particles is None:
-            return
-        fraction_sensor_used = (2048 - self.ignore_edge_pixels) / 2048
-        field_of_view = fraction_sensor_used * (13.3 / 20) ** 2  # (Sensor size/magnification) # mm2
-        for channel in range(self.num_channels):
-            frames = self.linked_particles[channel]['frame'].max() - self.linked_particles[channel]['frame'].min() + 1
-            volume = field_of_view * frames * step_size / 1000  # In mm3 (step_size in microns)
-            volume = volume / 1000  # in ml
-            num_particles = len(self.linked_particles[channel].groupby('particle').sum())
-
-            self.total_num_particles[channel] = num_particles
-            self.concentration[channel] = num_particles / volume
-
-        self.metadata.update({'concentration': self.concentration})
-
-    def calculate_background(self, frames_no=None, num_frames=10, sigma=200):
-        if frames_no is None:
-            average = np.mean(self.data[:num_frames], 0)
-        else:
-            average = np.mean(self.data[frames_no[0]:frames_no[1]], 0)
-        self.bkg = skimage.filters.gaussian(average, sigma=sigma)
+import json
+from pathlib import Path
+
+import numpy as np
+import pandas as pd
+import pims as pims
+import skimage
+import trackpy as tp
+import yaml
+from scipy.spatial import KDTree
+from skimage import morphology
+from skimage.measure import label, regionprops_table
+from trackpy.find import where_close
+from trackpy.utils import pandas_concat
+
+
+class AnalyzeNanoQNT:
+    def __init__(self):
+        self.filename = None
+        self.data = None
+        self.metadata = {}
+        self.particle_df = []
+        self.particles = pd.DataFrame()
+        self.num_frames = 0
+        self.find_settings = {}
+        self.filename = Path.home()
+        self.concentration = 0  # pcles/ml
+        self.linked_particles = None
+        self.total_num_particles = 0
+        self.summarized_particles = None
+
+        self.ignore_edge_pixels = 8
+
+        self.num_channels = 1
+        self.channels_data = {}
+        self.bkg = None
+
+    def open(self, filename):
+        """ Opens the file with the data. Normally a multi-tiff file, but it can be adapted to other formats.
+        It also looks for the comments.txt file (create by uManager) in order to load some metadata
+
+        :param filename: The full-path to the file to be opened
+        """
+        self.filename = Path(filename)
+        self.metadata['filename'] = str(filename)
+        self.metadata['last_dir'] = str(self.filename.parent)
+        self.data = pims.open(filename)
+        self.num_frames = len(self.data)  # This is really the number of frames in the data, not the number of
+        # multi-channel frames
+
+        self.particle_df = [pd.DataFrame() for _ in range(len(self.data))]
+        self.particles = pd.DataFrame()
+        self.find_settings = {}
+        self.linked_particles = None
+        self.summarized_particles = None
+        self.total_num_particles = 0
+        self.channels_data = {}
+
+        comments_file = self.filename.parent / 'comments.txt'
+        try:
+            with open(comments_file, 'r') as f:
+                self.metadata['uManager'] = json.load(f)
+        except FileNotFoundError:
+            self.metadata['uManager'] = {'comments': 'file not found'}
+
+        try:
+            comment = self.metadata['uManager']['map']['General annotation']['scalar']['comments']['scalar']
+            start = comment.index('(') + 1
+            end = comment.index(')')
+            self.num_channels = len(comment[start:end].split(' '))
+        except:
+            pass
+
+    def find_particles(self, frame_num, diameter, minmass, method='mask'):
+        """ Finds particles in a given frame and stores the data frame in a list indexed by the frame number.
+
+        :param int frame_num: The number of the frame (0-indexed) to analyze
+        :param int diameter: The expected diameter of the particles. Must be an odd number and is passed directly to
+        Trackpy
+        :param int minmass: Filter to select bright enough spots. The parameter is passed directly to Trackpy.
+        :param str method: Either select trackpy or mask. Default is mask.
+        """
+        if method == 'python' or method == 'numba':
+            if frame_num in self.find_settings:
+                settings = self.find_settings[frame_num]
+                if diameter == settings['diameter'] and minmass == settings['minmass']:
+                    return self.particle_df[frame_num]
+            self.find_settings[frame_num] = {
+                'diameter': diameter,
+                'minmass': minmass,
+                }
+            df = tp.locate(self.data[frame_num], diameter, minmass=minmass, characterize=False)
+            df = df.loc[df['y'] >= self.ignore_edge_pixels]
+            self.particle_df[frame_num] = df
+            return df
+
+        elif method == 'mask':
+            mask = self.data[frame_num] > minmass
+            mask = morphology.remove_small_objects(mask, diameter)
+            label_img = label(mask)
+            props = regionprops_table(label_img, intensity_image=np.array(self.data[frame_num]), properties=('centroid',
+                                                                                                             'intensity_mean',))
+            df = pd.DataFrame(props).rename(columns={'centroid-0': 'y', 'centroid-1': 'x', 'intensity_mean': 'mass'})
+            to_drop = where_close(df[['x', 'y']], separation=diameter * 2, intensity=df['mass'])
+            df = df.drop(to_drop)
+            df = df.loc[df['y'] >= self.ignore_edge_pixels]
+            self.particle_df[frame_num] = df
+            return df
+
+    def find_all_particles(self, frames_no, diameter, minmass, method='python'):
+        """ Finds all the particles in a given range of frames. If the data has multiple channels, then it can handle
+        different settings for each one. In that case, diameter and minmass must be iterables and in the appropriate
+        order, i.e., the first setting will be for the first channel, etc.
+
+        The data is structured as a dictionary, where each channel is a different key, and then the localizations are
+        stored as a pandas dataframe.
+
+        :param list frames_no:
+        :param tuple diameter:
+        :param tuple minmass:
+        :param str method:
+        :return dict: dictionary of particles found in each channel
+        """
+        try:
+            if len(diameter) != self.num_channels:
+                diameter = self.num_channels * [diameter]
+        except TypeError:
+            diameter = self.num_channels * [diameter]
+        try:
+            if len(minmass) != self.num_channels:
+                minmass = self.num_channels * [minmass]
+        except TypeError:
+            minmass = self.num_channels * [minmass]
+
+        if len(frames_no) == 1:
+            frames_no = (0, self.num_frames)
+
+        self.particles = {}
+
+        self.metadata.update({
+            'frames': frames_no,
+            'diameter': diameter,
+            'minmass': minmass,
+            'engine': method,
+            })
+
+        if method == 'mask':
+            for channel in range(self.num_channels):
+                all_features = []
+                for frame in range(frames_no[0], frames_no[1]):
+                    real_frame = frame * self.num_channels + channel
+                    df = self.find_particles(real_frame, diameter[channel], minmass[channel], method='mask')
+                    df['frame'] = frame
+                    all_features.append(df)
+                self.particles[channel] = pandas_concat(all_features).reset_index(drop=True)
+            return self.particles
+
+        ## For the python or numba methods, only 1-channel data is available
+        if self.num_channels > 1:
+            raise Exception("Trackpy-based methods only work with 1-channel data for the time being")
+
+        self.particles[0] = tp.batch(self.data[frames_no[0]:frames_no[1]],
+                                     diameter[0],
+                                     minmass=minmass[0],
+                                     characterize=False,
+                                     preprocess=False,
+                                     processes='auto',
+                                     engine=method)
+        self.particles[0]['intensity'] = np.nan
+
+        return self.particles
+
+    def link_particles(self, search_radius, memory=0, min_frames=0):
+        self.linked_particles = {}
+        for channel in range(self.num_channels):
+            self.linked_particles[channel] = tp.link(self.particles[channel], search_radius, memory=memory)
+            self.linked_particles[channel] = tp.filter_stubs(self.linked_particles[channel], min_frames)
+
+        self.metadata.update({
+            'search_radius': search_radius,
+            'min_frames': min_frames,
+            'memory': memory
+            })
+
+    def calculate_intensities(self):
+        """Calculates the intensities of the linked particles assuming they were the product of the mask method.
+        The methods that rely on the trackpy algorithm already include the intensity.
+        """
+        fit_size = 10
+        x_fit = np.linspace(0, 2 * fit_size, 2 * fit_size + 1)
+        y_fit = np.linspace(0, 2 * fit_size, 2 * fit_size + 1)
+        x_fit, y_fit = np.meshgrid(x_fit, y_fit)
+        initial_guess = (200, fit_size, fit_size, 2, 2, 200)
+
+        self.summary_data = {}
+        intensity_columns = [f'i_{channel}' for channel in range(self.num_channels)]
+        for channel in range(self.num_channels):
+            self.summary_data[channel] = pd.DataFrame(columns=['particle', 'frame', 'x', 'y'] + intensity_columns)
+
+            for p in self.linked_particles[channel]['particle'].unique():
+                pcle = self.linked_particles[channel].loc[self.linked_particles[channel]['particle'] == p]
+                ix = pcle['mass'].idxmax()
+                x = int(pcle.loc[ix]['y'])
+                y = int(pcle.loc[ix]['x'])
+                frame = int(pcle.loc[ix]['frame'])
+                # TODO: This is hardcoded and dangerous. The margin used to drop particles must be properly considered
+                if x < 20 or x > 2048 - 20 or y < 20 or y > 2048 - 20:
+                    continue
+
+                # try:
+                #     f = frame*self.num_channels + channel
+                #     popt, pcov = opt.curve_fit(twoD_Gaussian, (x_fit, y_fit),
+                #                                np.array(self.data[f][x - fit_size:x + fit_size + 1,
+                #                                         y - fit_size:y + fit_size + 1]).reshape(-1),
+                #                                p0=initial_guess)
+                # except Exception as e:
+                #     print(e)
+                #     continue
+
+                df = pd.DataFrame.from_dict({
+                    'particle': [p],
+                    'frame': [pcle.loc[ix]['frame']],
+                    'x': [pcle.loc[ix]['x']],
+                    'y': [pcle.loc[ix]['y']],
+                    f'i_{channel}': [pcle['mass'].max()]
+                    })
+                self.summary_data[channel] = pd.concat((self.summary_data[channel], df), ignore_index=True)
+            self.summary_data[channel] = self.summary_data[channel].reset_index(drop=True)
+
+    def multi_color_link(self):  # TODO: Add max frame distance as a parameter instead of fixing it to 5
+        """ Find the same particles in every channel and add the intensity information on each """
+        kd_trees = {}
+        for channel in range(self.num_channels):
+            kd_trees[channel] = KDTree(np.array(self.summary_data[channel][['x', 'y']]))
+
+        for channel in range(self.num_channels):
+            for channel_2 in range(channel + 1, self.num_channels):
+                for ix, p in self.summary_data[channel].iterrows():
+                    dist, ind = kd_trees[channel_2].query((p['x'], p['y']), p=2, distance_upper_bound=15)
+                    if ind == kd_trees[channel_2].n:
+                        continue
+                    if abs(self.summary_data[channel_2].loc[ind]['frame'] - p['frame']) > 5:
+                        print('Frames too far apart with ', ix, p['x'], p['y'], p['frame'])
+                        continue
+                    self.summary_data[channel].loc[ix, f'i_{channel_2}'] = \
+                        self.summary_data[channel_2].loc[ind][f'i_{channel_2}']
+                    self.summary_data[channel_2].loc[ind, f'i_{channel}'] = p[f'i_{channel}']
+
+    def save_all_data(self, filename):
+        self.linked_particles.to_csv(str(filename))
+
+    def save_data(self, filename):
+        """ Saves only the most important information to the file: particle and intensity information.
+        """
+        if not type(filename) is Path:
+            filename = Path(filename)
+
+        for i in range(self.num_channels):
+            stem = filename.stem
+            file_name = filename.with_stem(f'{stem}_{i}')
+            self.summary_data[i].to_csv(str(file_name))
+
+        with open(filename.with_suffix('.yml'), 'w') as f:
+            yaml.dump(self.metadata, f)
+
+    def calculate_concentration(self, step_size=5):
+        self.total_num_particles = {}
+        self.concentration = {}
+        if self.linked_particles is None:
+            return
+        fraction_sensor_used = (2048 - self.ignore_edge_pixels) / 2048
+        field_of_view = fraction_sensor_used * (13.3 / 20) ** 2  # (Sensor size/magnification) # mm2
+        for channel in range(self.num_channels):
+            frames = self.linked_particles[channel]['frame'].max() - self.linked_particles[channel]['frame'].min() + 1
+            volume = field_of_view * frames * step_size / 1000  # In mm3 (step_size in microns)
+            volume = volume / 1000  # in ml
+            num_particles = len(self.linked_particles[channel].groupby('particle').sum())
+
+            self.total_num_particles[channel] = num_particles
+            self.concentration[channel] = num_particles / volume
+
+        self.metadata.update({'concentration': self.concentration})
+
+    def calculate_background(self, frames_no=None, num_frames=10, sigma=200):
+        if frames_no is None:
+            average = np.mean(self.data[:num_frames], 0)
+        else:
+            average = np.mean(self.data[frames_no[0]:frames_no[1]], 0)
+        self.bkg = skimage.filters.gaussian(average, sigma=sigma)
```

### Comparing `nanoqnt-0.2.0/nanoqnt/view/channel_selector.py` & `nanoqnt-0.2.0rc1/nanoqnt/view/channel_selector.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from PyQt5 import uic
-from PyQt5.QtWidgets import QLabel, QLineEdit, QWidget
-
-from nanoqnt.view import VIEW_FOLDER
-
-
-class ChannelSelector(QWidget):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        uic.loadUi(str(VIEW_FOLDER / 'GUI' / 'channel_selector.ui'), self)
-        self.update_channels(0)
-        self.channel_box.currentIndexChanged.connect(self.update_channels)
-        self.channels = []
-        self.accept_button.clicked.connect(self.close)
-
-    def update_channels(self, number):
-        self.channels = []
-        layout = self.channels_widget.layout()
-        for i in range(layout.rowCount()):
-            layout.removeRow(0)
-
-        for i in range(number+1):
-            self.channels.append(QLineEdit(f"Name {i}"))
-            layout.addRow(QLabel(f"Channel {i}"), self.channels[-1])
+from PyQt5 import uic
+from PyQt5.QtWidgets import QLabel, QLineEdit, QWidget
+
+from nanoqnt.view import VIEW_FOLDER
+
+
+class ChannelSelector(QWidget):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        uic.loadUi(str(VIEW_FOLDER / 'GUI' / 'channel_selector.ui'), self)
+        self.update_channels(0)
+        self.channel_box.currentIndexChanged.connect(self.update_channels)
+        self.channels = []
+        self.accept_button.clicked.connect(self.close)
+
+    def update_channels(self, number):
+        self.channels = []
+        layout = self.channels_widget.layout()
+        for i in range(layout.rowCount()):
+            layout.removeRow(0)
+
+        for i in range(number + 1):
+            self.channels.append(QLineEdit(f"Name {i}"))
+            layout.addRow(QLabel(f"Channel {i}"), self.channels[-1])
```

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/channel_selector.ui` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/channel_selector.ui`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with CRLF line terminators*

 * *Files 23% similar despite different names*

```diff
@@ -1,143 +1,138 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0d0a 3c75 6920 7665 7273  F-8"?>..<ui vers
-00000030: 696f 6e3d 2234 2e30 223e 0d0a 203c 636c  ion="4.0">.. <cl
-00000040: 6173 733e 466f 726d 3c2f 636c 6173 733e  ass>Form</class>
-00000050: 0d0a 203c 7769 6467 6574 2063 6c61 7373  .. <widget class
-00000060: 3d22 5157 6964 6765 7422 206e 616d 653d  ="QWidget" name=
-00000070: 2246 6f72 6d22 3e0d 0a20 203c 7072 6f70  "Form">..  <prop
-00000080: 6572 7479 206e 616d 653d 2267 656f 6d65  erty name="geome
-00000090: 7472 7922 3e0d 0a20 2020 3c72 6563 743e  try">..   <rect>
-000000a0: 0d0a 2020 2020 3c78 3e30 3c2f 783e 0d0a  ..    <x>0</x>..
-000000b0: 2020 2020 3c79 3e30 3c2f 793e 0d0a 2020      <y>0</y>..  
-000000c0: 2020 3c77 6964 7468 3e33 3836 3c2f 7769    <width>386</wi
-000000d0: 6474 683e 0d0a 2020 2020 3c68 6569 6768  dth>..    <heigh
-000000e0: 743e 3233 343c 2f68 6569 6768 743e 0d0a  t>234</height>..
-000000f0: 2020 203c 2f72 6563 743e 0d0a 2020 3c2f     </rect>..  </
-00000100: 7072 6f70 6572 7479 3e0d 0a20 203c 7072  property>..  <pr
-00000110: 6f70 6572 7479 206e 616d 653d 2277 696e  operty name="win
-00000120: 646f 7754 6974 6c65 223e 0d0a 2020 203c  dowTitle">..   <
-00000130: 7374 7269 6e67 3e43 6861 6e6e 656c 2053  string>Channel S
-00000140: 656c 6563 746f 723c 2f73 7472 696e 673e  elector</string>
-00000150: 0d0a 2020 3c2f 7072 6f70 6572 7479 3e0d  ..  </property>.
-00000160: 0a20 203c 6c61 796f 7574 2063 6c61 7373  .  <layout class
-00000170: 3d22 5156 426f 784c 6179 6f75 7422 206e  ="QVBoxLayout" n
-00000180: 616d 653d 2276 6572 7469 6361 6c4c 6179  ame="verticalLay
-00000190: 6f75 7422 3e0d 0a20 2020 3c69 7465 6d3e  out">..   <item>
-000001a0: 0d0a 2020 2020 3c77 6964 6765 7420 636c  ..    <widget cl
-000001b0: 6173 733d 2251 5769 6467 6574 2220 6e61  ass="QWidget" na
-000001c0: 6d65 3d22 7769 6467 6574 2220 6e61 7469  me="widget" nati
-000001d0: 7665 3d22 7472 7565 223e 0d0a 2020 2020  ve="true">..    
-000001e0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-000001f0: 2273 697a 6550 6f6c 6963 7922 3e0d 0a20  "sizePolicy">.. 
-00000200: 2020 2020 203c 7369 7a65 706f 6c69 6379       <sizepolicy
-00000210: 2068 7369 7a65 7479 7065 3d22 5072 6566   hsizetype="Pref
-00000220: 6572 7265 6422 2076 7369 7a65 7479 7065  erred" vsizetype
-00000230: 3d22 4d69 6e69 6d75 6d22 3e0d 0a20 2020  ="Minimum">..   
-00000240: 2020 2020 3c68 6f72 7374 7265 7463 683e      <horstretch>
-00000250: 303c 2f68 6f72 7374 7265 7463 683e 0d0a  0</horstretch>..
-00000260: 2020 2020 2020 203c 7665 7273 7472 6574         <verstret
-00000270: 6368 3e30 3c2f 7665 7273 7472 6574 6368  ch>0</verstretch
-00000280: 3e0d 0a20 2020 2020 203c 2f73 697a 6570  >..      </sizep
-00000290: 6f6c 6963 793e 0d0a 2020 2020 203c 2f70  olicy>..     </p
-000002a0: 726f 7065 7274 793e 0d0a 2020 2020 203c  roperty>..     <
-000002b0: 6c61 796f 7574 2063 6c61 7373 3d22 5146  layout class="QF
-000002c0: 6f72 6d4c 6179 6f75 7422 206e 616d 653d  ormLayout" name=
-000002d0: 2266 6f72 6d4c 6179 6f75 7422 3e0d 0a20  "formLayout">.. 
-000002e0: 2020 2020 203c 6974 656d 2072 6f77 3d22       <item row="
-000002f0: 3122 2063 6f6c 756d 6e3d 2231 223e 0d0a  1" column="1">..
-00000300: 2020 2020 2020 203c 7769 6467 6574 2063         <widget c
-00000310: 6c61 7373 3d22 5143 6f6d 626f 426f 7822  lass="QComboBox"
-00000320: 206e 616d 653d 2263 6861 6e6e 656c 5f62   name="channel_b
-00000330: 6f78 223e 0d0a 2020 2020 2020 2020 3c69  ox">..        <i
-00000340: 7465 6d3e 0d0a 2020 2020 2020 2020 203c  tem>..         <
-00000350: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
-00000360: 6578 7422 3e0d 0a20 2020 2020 2020 2020  ext">..         
-00000370: 203c 7374 7269 6e67 3e31 3c2f 7374 7269   <string>1</stri
-00000380: 6e67 3e0d 0a20 2020 2020 2020 2020 3c2f  ng>..         </
-00000390: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
-000003a0: 2020 203c 2f69 7465 6d3e 0d0a 2020 2020     </item>..    
-000003b0: 2020 2020 3c69 7465 6d3e 0d0a 2020 2020      <item>..    
-000003c0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-000003d0: 616d 653d 2274 6578 7422 3e0d 0a20 2020  ame="text">..   
-000003e0: 2020 2020 2020 203c 7374 7269 6e67 3e32         <string>2
-000003f0: 3c2f 7374 7269 6e67 3e0d 0a20 2020 2020  </string>..     
-00000400: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
-00000410: 0a20 2020 2020 2020 203c 2f69 7465 6d3e  .        </item>
-00000420: 0d0a 2020 2020 2020 2020 3c69 7465 6d3e  ..        <item>
-00000430: 0d0a 2020 2020 2020 2020 203c 7072 6f70  ..         <prop
-00000440: 6572 7479 206e 616d 653d 2274 6578 7422  erty name="text"
-00000450: 3e0d 0a20 2020 2020 2020 2020 203c 7374  >..          <st
-00000460: 7269 6e67 3e33 3c2f 7374 7269 6e67 3e0d  ring>3</string>.
-00000470: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
-00000480: 6572 7479 3e0d 0a20 2020 2020 2020 203c  erty>..        <
-00000490: 2f69 7465 6d3e 0d0a 2020 2020 2020 2020  /item>..        
-000004a0: 3c69 7465 6d3e 0d0a 2020 2020 2020 2020  <item>..        
-000004b0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-000004c0: 2274 6578 7422 3e0d 0a20 2020 2020 2020  "text">..       
-000004d0: 2020 203c 7374 7269 6e67 3e34 3c2f 7374     <string>4</st
-000004e0: 7269 6e67 3e0d 0a20 2020 2020 2020 2020  ring>..         
-000004f0: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
-00000500: 2020 2020 203c 2f69 7465 6d3e 0d0a 2020       </item>..  
-00000510: 2020 2020 203c 2f77 6964 6765 743e 0d0a       </widget>..
-00000520: 2020 2020 2020 3c2f 6974 656d 3e0d 0a20        </item>.. 
-00000530: 2020 2020 203c 6974 656d 2072 6f77 3d22       <item row="
-00000540: 3122 2063 6f6c 756d 6e3d 2230 223e 0d0a  1" column="0">..
-00000550: 2020 2020 2020 203c 7769 6467 6574 2063         <widget c
-00000560: 6c61 7373 3d22 514c 6162 656c 2220 6e61  lass="QLabel" na
-00000570: 6d65 3d22 6c61 6265 6c22 3e0d 0a20 2020  me="label">..   
-00000580: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00000590: 616d 653d 2274 6578 7422 3e0d 0a20 2020  ame="text">..   
-000005a0: 2020 2020 2020 3c73 7472 696e 673e 4e75        <string>Nu
-000005b0: 6d62 6572 206f 6620 6368 616e 6e65 6c73  mber of channels
-000005c0: 3c2f 7374 7269 6e67 3e0d 0a20 2020 2020  </string>..     
-000005d0: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-000005e0: 2020 2020 2020 203c 2f77 6964 6765 743e         </widget>
-000005f0: 0d0a 2020 2020 2020 3c2f 6974 656d 3e0d  ..      </item>.
-00000600: 0a20 2020 2020 3c2f 6c61 796f 7574 3e0d  .     </layout>.
-00000610: 0a20 2020 203c 2f77 6964 6765 743e 0d0a  .    </widget>..
-00000620: 2020 203c 2f69 7465 6d3e 0d0a 2020 203c     </item>..   <
-00000630: 6974 656d 3e0d 0a20 2020 203c 7769 6467  item>..    <widg
-00000640: 6574 2063 6c61 7373 3d22 5157 6964 6765  et class="QWidge
-00000650: 7422 206e 616d 653d 2263 6861 6e6e 656c  t" name="channel
-00000660: 735f 7769 6467 6574 2220 6e61 7469 7665  s_widget" native
-00000670: 3d22 7472 7565 223e 0d0a 2020 2020 203c  ="true">..     <
-00000680: 6c61 796f 7574 2063 6c61 7373 3d22 5146  layout class="QF
-00000690: 6f72 6d4c 6179 6f75 7422 206e 616d 653d  ormLayout" name=
-000006a0: 2266 6f72 6d4c 6179 6f75 745f 3222 2f3e  "formLayout_2"/>
-000006b0: 0d0a 2020 2020 3c2f 7769 6467 6574 3e0d  ..    </widget>.
-000006c0: 0a20 2020 3c2f 6974 656d 3e0d 0a20 2020  .   </item>..   
-000006d0: 3c69 7465 6d3e 0d0a 2020 2020 3c73 7061  <item>..    <spa
-000006e0: 6365 7220 6e61 6d65 3d22 7665 7274 6963  cer name="vertic
-000006f0: 616c 5370 6163 6572 223e 0d0a 2020 2020  alSpacer">..    
-00000700: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00000710: 226f 7269 656e 7461 7469 6f6e 223e 0d0a  "orientation">..
-00000720: 2020 2020 2020 3c65 6e75 6d3e 5174 3a3a        <enum>Qt::
-00000730: 5665 7274 6963 616c 3c2f 656e 756d 3e0d  Vertical</enum>.
-00000740: 0a20 2020 2020 3c2f 7072 6f70 6572 7479  .     </property
-00000750: 3e0d 0a20 2020 2020 3c70 726f 7065 7274  >..     <propert
-00000760: 7920 6e61 6d65 3d22 7369 7a65 4869 6e74  y name="sizeHint
-00000770: 2220 7374 6473 6574 3d22 3022 3e0d 0a20  " stdset="0">.. 
-00000780: 2020 2020 203c 7369 7a65 3e0d 0a20 2020       <size>..   
-00000790: 2020 2020 3c77 6964 7468 3e32 303c 2f77      <width>20</w
-000007a0: 6964 7468 3e0d 0a20 2020 2020 2020 3c68  idth>..       <h
-000007b0: 6569 6768 743e 3430 3c2f 6865 6967 6874  eight>40</height
-000007c0: 3e0d 0a20 2020 2020 203c 2f73 697a 653e  >..      </size>
-000007d0: 0d0a 2020 2020 203c 2f70 726f 7065 7274  ..     </propert
-000007e0: 793e 0d0a 2020 2020 3c2f 7370 6163 6572  y>..    </spacer
-000007f0: 3e0d 0a20 2020 3c2f 6974 656d 3e0d 0a20  >..   </item>.. 
-00000800: 2020 3c69 7465 6d3e 0d0a 2020 2020 3c77    <item>..    <w
-00000810: 6964 6765 7420 636c 6173 733d 2251 5075  idget class="QPu
-00000820: 7368 4275 7474 6f6e 2220 6e61 6d65 3d22  shButton" name="
-00000830: 6163 6365 7074 5f62 7574 746f 6e22 3e0d  accept_button">.
-00000840: 0a20 2020 2020 3c70 726f 7065 7274 7920  .     <property 
-00000850: 6e61 6d65 3d22 7465 7874 223e 0d0a 2020  name="text">..  
-00000860: 2020 2020 3c73 7472 696e 673e 4163 6365      <string>Acce
-00000870: 7074 3c2f 7374 7269 6e67 3e0d 0a20 2020  pt</string>..   
-00000880: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
-00000890: 2020 203c 2f77 6964 6765 743e 0d0a 2020     </widget>..  
-000008a0: 203c 2f69 7465 6d3e 0d0a 2020 3c2f 6c61   </item>..  </la
-000008b0: 796f 7574 3e0d 0a20 3c2f 7769 6467 6574  yout>.. </widget
-000008c0: 3e0d 0a20 3c72 6573 6f75 7263 6573 2f3e  >.. <resources/>
-000008d0: 0d0a 203c 636f 6e6e 6563 7469 6f6e 732f  .. <connections/
-000008e0: 3e0d 0a3c 2f75 693e 0d0a                 >..</ui>..
+00000020: 462d 3822 3f3e 0a3c 7569 2076 6572 7369  F-8"?>.<ui versi
+00000030: 6f6e 3d22 342e 3022 3e0a 203c 636c 6173  on="4.0">. <clas
+00000040: 733e 466f 726d 3c2f 636c 6173 733e 0a20  s>Form</class>. 
+00000050: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
+00000060: 5769 6467 6574 2220 6e61 6d65 3d22 466f  Widget" name="Fo
+00000070: 726d 223e 0a20 203c 7072 6f70 6572 7479  rm">.  <property
+00000080: 206e 616d 653d 2267 656f 6d65 7472 7922   name="geometry"
+00000090: 3e0a 2020 203c 7265 6374 3e0a 2020 2020  >.   <rect>.    
+000000a0: 3c78 3e30 3c2f 783e 0a20 2020 203c 793e  <x>0</x>.    <y>
+000000b0: 303c 2f79 3e0a 2020 2020 3c77 6964 7468  0</y>.    <width
+000000c0: 3e33 3836 3c2f 7769 6474 683e 0a20 2020  >386</width>.   
+000000d0: 203c 6865 6967 6874 3e32 3334 3c2f 6865   <height>234</he
+000000e0: 6967 6874 3e0a 2020 203c 2f72 6563 743e  ight>.   </rect>
+000000f0: 0a20 203c 2f70 726f 7065 7274 793e 0a20  .  </property>. 
+00000100: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000110: 2277 696e 646f 7754 6974 6c65 223e 0a20  "windowTitle">. 
+00000120: 2020 3c73 7472 696e 673e 4368 616e 6e65    <string>Channe
+00000130: 6c20 5365 6c65 6374 6f72 3c2f 7374 7269  l Selector</stri
+00000140: 6e67 3e0a 2020 3c2f 7072 6f70 6572 7479  ng>.  </property
+00000150: 3e0a 2020 3c6c 6179 6f75 7420 636c 6173  >.  <layout clas
+00000160: 733d 2251 5642 6f78 4c61 796f 7574 2220  s="QVBoxLayout" 
+00000170: 6e61 6d65 3d22 7665 7274 6963 616c 4c61  name="verticalLa
+00000180: 796f 7574 223e 0a20 2020 3c69 7465 6d3e  yout">.   <item>
+00000190: 0a20 2020 203c 7769 6467 6574 2063 6c61  .    <widget cla
+000001a0: 7373 3d22 5157 6964 6765 7422 206e 616d  ss="QWidget" nam
+000001b0: 653d 2277 6964 6765 7422 206e 6174 6976  e="widget" nativ
+000001c0: 653d 2274 7275 6522 3e0a 2020 2020 203c  e="true">.     <
+000001d0: 7072 6f70 6572 7479 206e 616d 653d 2273  property name="s
+000001e0: 697a 6550 6f6c 6963 7922 3e0a 2020 2020  izePolicy">.    
+000001f0: 2020 3c73 697a 6570 6f6c 6963 7920 6873    <sizepolicy hs
+00000200: 697a 6574 7970 653d 2250 7265 6665 7272  izetype="Preferr
+00000210: 6564 2220 7673 697a 6574 7970 653d 224d  ed" vsizetype="M
+00000220: 696e 696d 756d 223e 0a20 2020 2020 2020  inimum">.       
+00000230: 3c68 6f72 7374 7265 7463 683e 303c 2f68  <horstretch>0</h
+00000240: 6f72 7374 7265 7463 683e 0a20 2020 2020  orstretch>.     
+00000250: 2020 3c76 6572 7374 7265 7463 683e 303c    <verstretch>0<
+00000260: 2f76 6572 7374 7265 7463 683e 0a20 2020  /verstretch>.   
+00000270: 2020 203c 2f73 697a 6570 6f6c 6963 793e     </sizepolicy>
+00000280: 0a20 2020 2020 3c2f 7072 6f70 6572 7479  .     </property
+00000290: 3e0a 2020 2020 203c 6c61 796f 7574 2063  >.     <layout c
+000002a0: 6c61 7373 3d22 5146 6f72 6d4c 6179 6f75  lass="QFormLayou
+000002b0: 7422 206e 616d 653d 2266 6f72 6d4c 6179  t" name="formLay
+000002c0: 6f75 7422 3e0a 2020 2020 2020 3c69 7465  out">.      <ite
+000002d0: 6d20 726f 773d 2231 2220 636f 6c75 6d6e  m row="1" column
+000002e0: 3d22 3122 3e0a 2020 2020 2020 203c 7769  ="1">.       <wi
+000002f0: 6467 6574 2063 6c61 7373 3d22 5143 6f6d  dget class="QCom
+00000300: 626f 426f 7822 206e 616d 653d 2263 6861  boBox" name="cha
+00000310: 6e6e 656c 5f62 6f78 223e 0a20 2020 2020  nnel_box">.     
+00000320: 2020 203c 6974 656d 3e0a 2020 2020 2020     <item>.      
+00000330: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00000340: 653d 2274 6578 7422 3e0a 2020 2020 2020  e="text">.      
+00000350: 2020 2020 3c73 7472 696e 673e 313c 2f73      <string>1</s
+00000360: 7472 696e 673e 0a20 2020 2020 2020 2020  tring>.         
+00000370: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00000380: 2020 2020 3c2f 6974 656d 3e0a 2020 2020      </item>.    
+00000390: 2020 2020 3c69 7465 6d3e 0a20 2020 2020      <item>.     
+000003a0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+000003b0: 6d65 3d22 7465 7874 223e 0a20 2020 2020  me="text">.     
+000003c0: 2020 2020 203c 7374 7269 6e67 3e32 3c2f       <string>2</
+000003d0: 7374 7269 6e67 3e0a 2020 2020 2020 2020  string>.        
+000003e0: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+000003f0: 2020 2020 203c 2f69 7465 6d3e 0a20 2020       </item>.   
+00000400: 2020 2020 203c 6974 656d 3e0a 2020 2020       <item>.    
+00000410: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00000420: 616d 653d 2274 6578 7422 3e0a 2020 2020  ame="text">.    
+00000430: 2020 2020 2020 3c73 7472 696e 673e 333c        <string>3<
+00000440: 2f73 7472 696e 673e 0a20 2020 2020 2020  /string>.       
+00000450: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+00000460: 2020 2020 2020 3c2f 6974 656d 3e0a 2020        </item>.  
+00000470: 2020 2020 2020 3c69 7465 6d3e 0a20 2020        <item>.   
+00000480: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00000490: 6e61 6d65 3d22 7465 7874 223e 0a20 2020  name="text">.   
+000004a0: 2020 2020 2020 203c 7374 7269 6e67 3e34         <string>4
+000004b0: 3c2f 7374 7269 6e67 3e0a 2020 2020 2020  </string>.      
+000004c0: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
+000004d0: 2020 2020 2020 203c 2f69 7465 6d3e 0a20         </item>. 
+000004e0: 2020 2020 2020 3c2f 7769 6467 6574 3e0a        </widget>.
+000004f0: 2020 2020 2020 3c2f 6974 656d 3e0a 2020        </item>.  
+00000500: 2020 2020 3c69 7465 6d20 726f 773d 2231      <item row="1
+00000510: 2220 636f 6c75 6d6e 3d22 3022 3e0a 2020  " column="0">.  
+00000520: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
+00000530: 7373 3d22 514c 6162 656c 2220 6e61 6d65  ss="QLabel" name
+00000540: 3d22 6c61 6265 6c22 3e0a 2020 2020 2020  ="label">.      
+00000550: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00000560: 3d22 7465 7874 223e 0a20 2020 2020 2020  ="text">.       
+00000570: 2020 3c73 7472 696e 673e 4e75 6d62 6572    <string>Number
+00000580: 206f 6620 6368 616e 6e65 6c73 3c2f 7374   of channels</st
+00000590: 7269 6e67 3e0a 2020 2020 2020 2020 3c2f  ring>.        </
+000005a0: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+000005b0: 203c 2f77 6964 6765 743e 0a20 2020 2020   </widget>.     
+000005c0: 203c 2f69 7465 6d3e 0a20 2020 2020 3c2f   </item>.     </
+000005d0: 6c61 796f 7574 3e0a 2020 2020 3c2f 7769  layout>.    </wi
+000005e0: 6467 6574 3e0a 2020 203c 2f69 7465 6d3e  dget>.   </item>
+000005f0: 0a20 2020 3c69 7465 6d3e 0a20 2020 203c  .   <item>.    <
+00000600: 7769 6467 6574 2063 6c61 7373 3d22 5157  widget class="QW
+00000610: 6964 6765 7422 206e 616d 653d 2263 6861  idget" name="cha
+00000620: 6e6e 656c 735f 7769 6467 6574 2220 6e61  nnels_widget" na
+00000630: 7469 7665 3d22 7472 7565 223e 0a20 2020  tive="true">.   
+00000640: 2020 3c6c 6179 6f75 7420 636c 6173 733d    <layout class=
+00000650: 2251 466f 726d 4c61 796f 7574 2220 6e61  "QFormLayout" na
+00000660: 6d65 3d22 666f 726d 4c61 796f 7574 5f32  me="formLayout_2
+00000670: 222f 3e0a 2020 2020 3c2f 7769 6467 6574  "/>.    </widget
+00000680: 3e0a 2020 203c 2f69 7465 6d3e 0a20 2020  >.   </item>.   
+00000690: 3c69 7465 6d3e 0a20 2020 203c 7370 6163  <item>.    <spac
+000006a0: 6572 206e 616d 653d 2276 6572 7469 6361  er name="vertica
+000006b0: 6c53 7061 6365 7222 3e0a 2020 2020 203c  lSpacer">.     <
+000006c0: 7072 6f70 6572 7479 206e 616d 653d 226f  property name="o
+000006d0: 7269 656e 7461 7469 6f6e 223e 0a20 2020  rientation">.   
+000006e0: 2020 203c 656e 756d 3e51 743a 3a56 6572     <enum>Qt::Ver
+000006f0: 7469 6361 6c3c 2f65 6e75 6d3e 0a20 2020  tical</enum>.   
+00000700: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+00000710: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00000720: 653d 2273 697a 6548 696e 7422 2073 7464  e="sizeHint" std
+00000730: 7365 743d 2230 223e 0a20 2020 2020 203c  set="0">.      <
+00000740: 7369 7a65 3e0a 2020 2020 2020 203c 7769  size>.       <wi
+00000750: 6474 683e 3230 3c2f 7769 6474 683e 0a20  dth>20</width>. 
+00000760: 2020 2020 2020 3c68 6569 6768 743e 3430        <height>40
+00000770: 3c2f 6865 6967 6874 3e0a 2020 2020 2020  </height>.      
+00000780: 3c2f 7369 7a65 3e0a 2020 2020 203c 2f70  </size>.     </p
+00000790: 726f 7065 7274 793e 0a20 2020 203c 2f73  roperty>.    </s
+000007a0: 7061 6365 723e 0a20 2020 3c2f 6974 656d  pacer>.   </item
+000007b0: 3e0a 2020 203c 6974 656d 3e0a 2020 2020  >.   <item>.    
+000007c0: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
+000007d0: 5075 7368 4275 7474 6f6e 2220 6e61 6d65  PushButton" name
+000007e0: 3d22 6163 6365 7074 5f62 7574 746f 6e22  ="accept_button"
+000007f0: 3e0a 2020 2020 203c 7072 6f70 6572 7479  >.     <property
+00000800: 206e 616d 653d 2274 6578 7422 3e0a 2020   name="text">.  
+00000810: 2020 2020 3c73 7472 696e 673e 4163 6365      <string>Acce
+00000820: 7074 3c2f 7374 7269 6e67 3e0a 2020 2020  pt</string>.    
+00000830: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+00000840: 203c 2f77 6964 6765 743e 0a20 2020 3c2f   </widget>.   </
+00000850: 6974 656d 3e0a 2020 3c2f 6c61 796f 7574  item>.  </layout
+00000860: 3e0a 203c 2f77 6964 6765 743e 0a20 3c72  >. </widget>. <r
+00000870: 6573 6f75 7263 6573 2f3e 0a20 3c63 6f6e  esources/>. <con
+00000880: 6e65 6374 696f 6e73 2f3e 0a3c 2f75 693e  nections/>.</ui>
+00000890: 0a                                       .
```

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/data_exploration.ui` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/data_exploration.ui`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, Unicode text, UTF-8 text, with CRLF line terminators*

 * *Files 25% similar despite different names*

```diff
@@ -1,959 +1,929 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0d0a 3c75 6920 7665 7273  F-8"?>..<ui vers
-00000030: 696f 6e3d 2234 2e30 223e 0d0a 203c 636c  ion="4.0">.. <cl
-00000040: 6173 733e 4d61 696e 5769 6e64 6f77 3c2f  ass>MainWindow</
-00000050: 636c 6173 733e 0d0a 203c 7769 6467 6574  class>.. <widget
-00000060: 2063 6c61 7373 3d22 514d 6169 6e57 696e   class="QMainWin
-00000070: 646f 7722 206e 616d 653d 224d 6169 6e57  dow" name="MainW
-00000080: 696e 646f 7722 3e0d 0a20 203c 7072 6f70  indow">..  <prop
-00000090: 6572 7479 206e 616d 653d 2267 656f 6d65  erty name="geome
-000000a0: 7472 7922 3e0d 0a20 2020 3c72 6563 743e  try">..   <rect>
-000000b0: 0d0a 2020 2020 3c78 3e30 3c2f 783e 0d0a  ..    <x>0</x>..
-000000c0: 2020 2020 3c79 3e30 3c2f 793e 0d0a 2020      <y>0</y>..  
-000000d0: 2020 3c77 6964 7468 3e37 3638 3c2f 7769    <width>768</wi
-000000e0: 6474 683e 0d0a 2020 2020 3c68 6569 6768  dth>..    <heigh
-000000f0: 743e 3634 313c 2f68 6569 6768 743e 0d0a  t>641</height>..
-00000100: 2020 203c 2f72 6563 743e 0d0a 2020 3c2f     </rect>..  </
-00000110: 7072 6f70 6572 7479 3e0d 0a20 203c 7072  property>..  <pr
-00000120: 6f70 6572 7479 206e 616d 653d 2277 696e  operty name="win
-00000130: 646f 7754 6974 6c65 223e 0d0a 2020 203c  dowTitle">..   <
-00000140: 7374 7269 6e67 3e4e 616e 6f51 4e54 2044  string>NanoQNT D
-00000150: 6174 6120 416e 616c 7973 6973 3c2f 7374  ata Analysis</st
-00000160: 7269 6e67 3e0d 0a20 203c 2f70 726f 7065  ring>..  </prope
-00000170: 7274 793e 0d0a 2020 3c70 726f 7065 7274  rty>..  <propert
-00000180: 7920 6e61 6d65 3d22 756e 6966 6965 6454  y name="unifiedT
-00000190: 6974 6c65 416e 6454 6f6f 6c42 6172 4f6e  itleAndToolBarOn
-000001a0: 4d61 6322 3e0d 0a20 2020 3c62 6f6f 6c3e  Mac">..   <bool>
-000001b0: 7472 7565 3c2f 626f 6f6c 3e0d 0a20 203c  true</bool>..  <
-000001c0: 2f70 726f 7065 7274 793e 0d0a 2020 3c77  /property>..  <w
-000001d0: 6964 6765 7420 636c 6173 733d 2251 5769  idget class="QWi
-000001e0: 6467 6574 2220 6e61 6d65 3d22 6365 6e74  dget" name="cent
-000001f0: 7261 6c77 6964 6765 7422 3e0d 0a20 2020  ralwidget">..   
-00000200: 3c6c 6179 6f75 7420 636c 6173 733d 2251  <layout class="Q
-00000210: 4842 6f78 4c61 796f 7574 2220 6e61 6d65  HBoxLayout" name
-00000220: 3d22 686f 7269 7a6f 6e74 616c 4c61 796f  ="horizontalLayo
-00000230: 7574 223e 0d0a 2020 2020 3c69 7465 6d3e  ut">..    <item>
-00000240: 0d0a 2020 2020 203c 7769 6467 6574 2063  ..     <widget c
-00000250: 6c61 7373 3d22 5157 6964 6765 7422 206e  lass="QWidget" n
-00000260: 616d 653d 2273 6574 7469 6e67 735f 7769  ame="settings_wi
-00000270: 6467 6574 2220 6e61 7469 7665 3d22 7472  dget" native="tr
-00000280: 7565 223e 0d0a 2020 2020 2020 3c70 726f  ue">..      <pro
-00000290: 7065 7274 7920 6e61 6d65 3d22 7369 7a65  perty name="size
-000002a0: 506f 6c69 6379 223e 0d0a 2020 2020 2020  Policy">..      
-000002b0: 203c 7369 7a65 706f 6c69 6379 2068 7369   <sizepolicy hsi
-000002c0: 7a65 7479 7065 3d22 4d69 6e69 6d75 6d22  zetype="Minimum"
-000002d0: 2076 7369 7a65 7479 7065 3d22 5072 6566   vsizetype="Pref
-000002e0: 6572 7265 6422 3e0d 0a20 2020 2020 2020  erred">..       
-000002f0: 203c 686f 7273 7472 6574 6368 3e30 3c2f   <horstretch>0</
-00000300: 686f 7273 7472 6574 6368 3e0d 0a20 2020  horstretch>..   
-00000310: 2020 2020 203c 7665 7273 7472 6574 6368       <verstretch
-00000320: 3e30 3c2f 7665 7273 7472 6574 6368 3e0d  >0</verstretch>.
-00000330: 0a20 2020 2020 2020 3c2f 7369 7a65 706f  .       </sizepo
-00000340: 6c69 6379 3e0d 0a20 2020 2020 203c 2f70  licy>..      </p
-00000350: 726f 7065 7274 793e 0d0a 2020 2020 2020  roperty>..      
-00000360: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00000370: 6d61 7869 6d75 6d53 697a 6522 3e0d 0a20  maximumSize">.. 
-00000380: 2020 2020 2020 3c73 697a 653e 0d0a 2020        <size>..  
-00000390: 2020 2020 2020 3c77 6964 7468 3e32 3235        <width>225
-000003a0: 3c2f 7769 6474 683e 0d0a 2020 2020 2020  </width>..      
-000003b0: 2020 3c68 6569 6768 743e 3136 3737 3732    <height>167772
-000003c0: 3135 3c2f 6865 6967 6874 3e0d 0a20 2020  15</height>..   
-000003d0: 2020 2020 3c2f 7369 7a65 3e0d 0a20 2020      </size>..   
-000003e0: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-000003f0: 2020 2020 2020 3c6c 6179 6f75 7420 636c        <layout cl
-00000400: 6173 733d 2251 466f 726d 4c61 796f 7574  ass="QFormLayout
-00000410: 2220 6e61 6d65 3d22 666f 726d 4c61 796f  " name="formLayo
-00000420: 7574 223e 0d0a 2020 2020 2020 203c 7072  ut">..       <pr
-00000430: 6f70 6572 7479 206e 616d 653d 226c 6566  operty name="lef
-00000440: 744d 6172 6769 6e22 3e0d 0a20 2020 2020  tMargin">..     
-00000450: 2020 203c 6e75 6d62 6572 3e30 3c2f 6e75     <number>0</nu
-00000460: 6d62 6572 3e0d 0a20 2020 2020 2020 3c2f  mber>..       </
-00000470: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
-00000480: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00000490: 3d22 746f 704d 6172 6769 6e22 3e0d 0a20  ="topMargin">.. 
-000004a0: 2020 2020 2020 203c 6e75 6d62 6572 3e30         <number>0
-000004b0: 3c2f 6e75 6d62 6572 3e0d 0a20 2020 2020  </number>..     
-000004c0: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
-000004d0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-000004e0: 6e61 6d65 3d22 7269 6768 744d 6172 6769  name="rightMargi
-000004f0: 6e22 3e0d 0a20 2020 2020 2020 203c 6e75  n">..        <nu
-00000500: 6d62 6572 3e30 3c2f 6e75 6d62 6572 3e0d  mber>0</number>.
-00000510: 0a20 2020 2020 2020 3c2f 7072 6f70 6572  .       </proper
-00000520: 7479 3e0d 0a20 2020 2020 2020 3c70 726f  ty>..       <pro
-00000530: 7065 7274 7920 6e61 6d65 3d22 626f 7474  perty name="bott
-00000540: 6f6d 4d61 7267 696e 223e 0d0a 2020 2020  omMargin">..    
-00000550: 2020 2020 3c6e 756d 6265 723e 303c 2f6e      <number>0</n
-00000560: 756d 6265 723e 0d0a 2020 2020 2020 203c  umber>..       <
-00000570: 2f70 726f 7065 7274 793e 0d0a 2020 2020  /property>..    
-00000580: 2020 203c 6974 656d 2072 6f77 3d22 3022     <item row="0"
-00000590: 2063 6f6c 756d 6e3d 2230 2220 636f 6c73   column="0" cols
-000005a0: 7061 6e3d 2232 223e 0d0a 2020 2020 2020  pan="2">..      
-000005b0: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
-000005c0: 2251 4368 6563 6b42 6f78 2220 6e61 6d65  "QCheckBox" name
-000005d0: 3d22 6669 6e64 5f70 6172 7469 636c 6573  ="find_particles
-000005e0: 5f63 6865 636b 223e 0d0a 2020 2020 2020  _check">..      
-000005f0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00000600: 653d 2274 6f6f 6c54 6970 223e 0d0a 2020  e="toolTip">..  
-00000610: 2020 2020 2020 2020 3c73 7472 696e 673e          <string>
-00000620: 266c 743b 6874 6d6c 2667 743b 266c 743b  &lt;html&gt;&lt;
-00000630: 6865 6164 2f26 6774 3b26 6c74 3b62 6f64  head/&gt;&lt;bod
-00000640: 7926 6774 3b26 6c74 3b70 2667 743b 5768  y&gt;&lt;p&gt;Wh
-00000650: 6574 6865 7220 746f 206d 6172 6b20 7468  ether to mark th
-00000660: 6520 7061 7274 6963 6c65 7320 6f6e 2074  e particles on t
-00000670: 6865 2069 6d61 6765 7326 6c74 3b2f 7026  he images&lt;/p&
-00000680: 6774 3b26 6c74 3b2f 626f 6479 2667 743b  gt;&lt;/body&gt;
-00000690: 266c 743b 2f68 746d 6c26 6774 3b3c 2f73  &lt;/html&gt;</s
-000006a0: 7472 696e 673e 0d0a 2020 2020 2020 2020  tring>..        
-000006b0: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
-000006c0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-000006d0: 206e 616d 653d 2274 6578 7422 3e0d 0a20   name="text">.. 
-000006e0: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-000006f0: 3e46 696e 6420 5061 7274 6963 6c65 733c  >Find Particles<
-00000700: 2f73 7472 696e 673e 0d0a 2020 2020 2020  /string>..      
-00000710: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-00000720: 2020 2020 2020 2020 3c2f 7769 6467 6574          </widget
-00000730: 3e0d 0a20 2020 2020 2020 3c2f 6974 656d  >..       </item
-00000740: 3e0d 0a20 2020 2020 2020 3c69 7465 6d20  >..       <item 
-00000750: 726f 773d 2231 2220 636f 6c75 6d6e 3d22  row="1" column="
-00000760: 3022 3e0d 0a20 2020 2020 2020 203c 7769  0">..        <wi
-00000770: 6467 6574 2063 6c61 7373 3d22 514c 6162  dget class="QLab
-00000780: 656c 2220 6e61 6d65 3d22 6c61 6265 6c5f  el" name="label_
-00000790: 3922 3e0d 0a20 2020 2020 2020 2020 3c70  9">..         <p
-000007a0: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
-000007b0: 7874 223e 0d0a 2020 2020 2020 2020 2020  xt">..          
-000007c0: 3c73 7472 696e 673e 4672 616d 6520 5261  <string>Frame Ra
-000007d0: 6e67 653c 2f73 7472 696e 673e 0d0a 2020  nge</string>..  
-000007e0: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
-000007f0: 793e 0d0a 2020 2020 2020 2020 203c 7072  y>..         <pr
-00000800: 6f70 6572 7479 206e 616d 653d 2262 7564  operty name="bud
-00000810: 6479 223e 0d0a 2020 2020 2020 2020 2020  dy">..          
-00000820: 3c63 7374 7269 6e67 3e73 7461 7274 5f66  <cstring>start_f
-00000830: 7261 6d65 5f6c 696e 653c 2f63 7374 7269  rame_line</cstri
-00000840: 6e67 3e0d 0a20 2020 2020 2020 2020 3c2f  ng>..         </
-00000850: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
-00000860: 2020 203c 2f77 6964 6765 743e 0d0a 2020     </widget>..  
-00000870: 2020 2020 203c 2f69 7465 6d3e 0d0a 2020       </item>..  
-00000880: 2020 2020 203c 6974 656d 2072 6f77 3d22       <item row="
-00000890: 3122 2063 6f6c 756d 6e3d 2231 223e 0d0a  1" column="1">..
-000008a0: 2020 2020 2020 2020 3c77 6964 6765 7420          <widget 
-000008b0: 636c 6173 733d 2251 4c69 6e65 4564 6974  class="QLineEdit
-000008c0: 2220 6e61 6d65 3d22 7374 6172 745f 6672  " name="start_fr
-000008d0: 616d 655f 6c69 6e65 223e 0d0a 2020 2020  ame_line">..    
-000008e0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-000008f0: 616d 653d 2274 6f6f 6c54 6970 223e 0d0a  ame="toolTip">..
-00000900: 2020 2020 2020 2020 2020 3c73 7472 696e            <strin
-00000910: 673e 5374 6172 7420 4672 616d 653c 2f73  g>Start Frame</s
-00000920: 7472 696e 673e 0d0a 2020 2020 2020 2020  tring>..        
-00000930: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
-00000940: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00000950: 206e 616d 653d 2274 6578 7422 3e0d 0a20   name="text">.. 
-00000960: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-00000970: 3e30 3c2f 7374 7269 6e67 3e0d 0a20 2020  >0</string>..   
-00000980: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
-00000990: 3e0d 0a20 2020 2020 2020 203c 2f77 6964  >..        </wid
-000009a0: 6765 743e 0d0a 2020 2020 2020 203c 2f69  get>..       </i
-000009b0: 7465 6d3e 0d0a 2020 2020 2020 203c 6974  tem>..       <it
-000009c0: 656d 2072 6f77 3d22 3222 2063 6f6c 756d  em row="2" colum
-000009d0: 6e3d 2231 223e 0d0a 2020 2020 2020 2020  n="1">..        
-000009e0: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
-000009f0: 4c69 6e65 4564 6974 2220 6e61 6d65 3d22  LineEdit" name="
-00000a00: 656e 645f 6672 616d 655f 6c69 6e65 223e  end_frame_line">
-00000a10: 0d0a 2020 2020 2020 2020 203c 7072 6f70  ..         <prop
-00000a20: 6572 7479 206e 616d 653d 2274 6f6f 6c54  erty name="toolT
-00000a30: 6970 223e 0d0a 2020 2020 2020 2020 2020  ip">..          
-00000a40: 3c73 7472 696e 673e 456e 6420 4672 616d  <string>End Fram
-00000a50: 653c 2f73 7472 696e 673e 0d0a 2020 2020  e</string>..    
-00000a60: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00000a70: 0d0a 2020 2020 2020 2020 203c 7072 6f70  ..         <prop
-00000a80: 6572 7479 206e 616d 653d 2274 6578 7422  erty name="text"
-00000a90: 3e0d 0a20 2020 2020 2020 2020 203c 7374  >..          <st
-00000aa0: 7269 6e67 3e2d 313c 2f73 7472 696e 673e  ring>-1</string>
-00000ab0: 0d0a 2020 2020 2020 2020 203c 2f70 726f  ..         </pro
-00000ac0: 7065 7274 793e 0d0a 2020 2020 2020 2020  perty>..        
-00000ad0: 3c2f 7769 6467 6574 3e0d 0a20 2020 2020  </widget>..     
-00000ae0: 2020 3c2f 6974 656d 3e0d 0a20 2020 2020    </item>..     
-00000af0: 2020 3c69 7465 6d20 726f 773d 2233 2220    <item row="3" 
-00000b00: 636f 6c75 6d6e 3d22 3022 3e0d 0a20 2020  column="0">..   
-00000b10: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
-00000b20: 7373 3d22 514c 6162 656c 2220 6e61 6d65  ss="QLabel" name
-00000b30: 3d22 6c61 6265 6c5f 3322 3e0d 0a20 2020  ="label_3">..   
-00000b40: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00000b50: 6e61 6d65 3d22 7465 7874 223e 0d0a 2020  name="text">..  
-00000b60: 2020 2020 2020 2020 3c73 7472 696e 673e          <string>
-00000b70: 456e 6769 6e65 3c2f 7374 7269 6e67 3e0d  Engine</string>.
-00000b80: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
-00000b90: 6572 7479 3e0d 0a20 2020 2020 2020 2020  erty>..         
-00000ba0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00000bb0: 6275 6464 7922 3e0d 0a20 2020 2020 2020  buddy">..       
-00000bc0: 2020 203c 6373 7472 696e 673e 656e 6769     <cstring>engi
-00000bd0: 6e65 5f62 6f78 3c2f 6373 7472 696e 673e  ne_box</cstring>
-00000be0: 0d0a 2020 2020 2020 2020 203c 2f70 726f  ..         </pro
-00000bf0: 7065 7274 793e 0d0a 2020 2020 2020 2020  perty>..        
-00000c00: 3c2f 7769 6467 6574 3e0d 0a20 2020 2020  </widget>..     
-00000c10: 2020 3c2f 6974 656d 3e0d 0a20 2020 2020    </item>..     
-00000c20: 2020 3c69 7465 6d20 726f 773d 2233 2220    <item row="3" 
-00000c30: 636f 6c75 6d6e 3d22 3122 3e0d 0a20 2020  column="1">..   
-00000c40: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
-00000c50: 7373 3d22 5143 6f6d 626f 426f 7822 206e  ss="QComboBox" n
-00000c60: 616d 653d 2265 6e67 696e 655f 626f 7822  ame="engine_box"
-00000c70: 3e0d 0a20 2020 2020 2020 2020 3c70 726f  >..         <pro
-00000c80: 7065 7274 7920 6e61 6d65 3d22 746f 6f6c  perty name="tool
-00000c90: 5469 7022 3e0d 0a20 2020 2020 2020 2020  Tip">..         
-00000ca0: 203c 7374 7269 6e67 3e26 6c74 3b68 746d   <string>&lt;htm
-00000cb0: 6c26 6774 3b26 6c74 3b68 6561 642f 2667  l&gt;&lt;head/&g
-00000cc0: 743b 266c 743b 626f 6479 2667 743b 266c  t;&lt;body&gt;&l
-00000cd0: 743b 7026 6774 3b49 6620 696e 7374 616c  t;p&gt;If instal
-00000ce0: 6c65 642c 206e 756d 6261 2069 7320 7072  led, numba is pr
-00000cf0: 6566 6572 7265 6426 6c74 3b2f 7026 6774  eferred&lt;/p&gt
-00000d00: 3b26 6c74 3b2f 626f 6479 2667 743b 266c  ;&lt;/body&gt;&l
-00000d10: 743b 2f68 746d 6c26 6774 3b3c 2f73 7472  t;/html&gt;</str
-00000d20: 696e 673e 0d0a 2020 2020 2020 2020 203c  ing>..         <
-00000d30: 2f70 726f 7065 7274 793e 0d0a 2020 2020  /property>..    
-00000d40: 2020 2020 203c 6974 656d 3e0d 0a20 2020       <item>..   
-00000d50: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00000d60: 206e 616d 653d 2274 6578 7422 3e0d 0a20   name="text">.. 
-00000d70: 2020 2020 2020 2020 2020 3c73 7472 696e            <strin
-00000d80: 673e 6d61 736b 3c2f 7374 7269 6e67 3e0d  g>mask</string>.
-00000d90: 0a20 2020 2020 2020 2020 203c 2f70 726f  .          </pro
-00000da0: 7065 7274 793e 0d0a 2020 2020 2020 2020  perty>..        
-00000db0: 203c 2f69 7465 6d3e 0d0a 2020 2020 2020   </item>..      
-00000dc0: 2020 203c 6974 656d 3e0d 0a20 2020 2020     <item>..     
-00000dd0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00000de0: 616d 653d 2274 6578 7422 3e0d 0a20 2020  ame="text">..   
-00000df0: 2020 2020 2020 2020 3c73 7472 696e 673e          <string>
-00000e00: 6e75 6d62 613c 2f73 7472 696e 673e 0d0a  numba</string>..
-00000e10: 2020 2020 2020 2020 2020 3c2f 7072 6f70            </prop
-00000e20: 6572 7479 3e0d 0a20 2020 2020 2020 2020  erty>..         
-00000e30: 3c2f 6974 656d 3e0d 0a20 2020 2020 2020  </item>..       
-00000e40: 2020 3c69 7465 6d3e 0d0a 2020 2020 2020    <item>..      
-00000e50: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00000e60: 6d65 3d22 7465 7874 223e 0d0a 2020 2020  me="text">..    
-00000e70: 2020 2020 2020 203c 7374 7269 6e67 3e70         <string>p
-00000e80: 7974 686f 6e3c 2f73 7472 696e 673e 0d0a  ython</string>..
-00000e90: 2020 2020 2020 2020 2020 3c2f 7072 6f70            </prop
-00000ea0: 6572 7479 3e0d 0a20 2020 2020 2020 2020  erty>..         
-00000eb0: 3c2f 6974 656d 3e0d 0a20 2020 2020 2020  </item>..       
-00000ec0: 203c 2f77 6964 6765 743e 0d0a 2020 2020   </widget>..    
-00000ed0: 2020 203c 2f69 7465 6d3e 0d0a 2020 2020     </item>..    
-00000ee0: 2020 203c 6974 656d 2072 6f77 3d22 3522     <item row="5"
-00000ef0: 2063 6f6c 756d 6e3d 2230 223e 0d0a 2020   column="0">..  
-00000f00: 2020 2020 2020 3c77 6964 6765 7420 636c        <widget cl
-00000f10: 6173 733d 2251 4c61 6265 6c22 206e 616d  ass="QLabel" nam
-00000f20: 653d 226c 6162 656c 5f34 223e 0d0a 2020  e="label_4">..  
-00000f30: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00000f40: 206e 616d 653d 2274 6578 7422 3e0d 0a20   name="text">.. 
-00000f50: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-00000f60: 3e53 6561 7263 6820 7261 6469 7573 3c2f  >Search radius</
-00000f70: 7374 7269 6e67 3e0d 0a20 2020 2020 2020  string>..       
-00000f80: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
-00000f90: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00000fa0: 7920 6e61 6d65 3d22 6275 6464 7922 3e0d  y name="buddy">.
-00000fb0: 0a20 2020 2020 2020 2020 203c 6373 7472  .          <cstr
-00000fc0: 696e 673e 7365 6172 6368 5f72 6164 6975  ing>search_radiu
-00000fd0: 735f 6c69 6e65 3c2f 6373 7472 696e 673e  s_line</cstring>
-00000fe0: 0d0a 2020 2020 2020 2020 203c 2f70 726f  ..         </pro
-00000ff0: 7065 7274 793e 0d0a 2020 2020 2020 2020  perty>..        
-00001000: 3c2f 7769 6467 6574 3e0d 0a20 2020 2020  </widget>..     
-00001010: 2020 3c2f 6974 656d 3e0d 0a20 2020 2020    </item>..     
-00001020: 2020 3c69 7465 6d20 726f 773d 2235 2220    <item row="5" 
-00001030: 636f 6c75 6d6e 3d22 3122 3e0d 0a20 2020  column="1">..   
-00001040: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
-00001050: 7373 3d22 514c 696e 6545 6469 7422 206e  ss="QLineEdit" n
-00001060: 616d 653d 2273 6561 7263 685f 7261 6469  ame="search_radi
-00001070: 7573 5f6c 696e 6522 3e0d 0a20 2020 2020  us_line">..     
-00001080: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00001090: 6d65 3d22 746f 6f6c 5469 7022 3e0d 0a20  me="toolTip">.. 
-000010a0: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-000010b0: 3e26 6c74 3b68 746d 6c26 6774 3b26 6c74  >&lt;html&gt;&lt
-000010c0: 3b68 6561 642f 2667 743b 266c 743b 626f  ;head/&gt;&lt;bo
-000010d0: 6479 2667 743b 266c 743b 7026 6774 3b53  dy&gt;&lt;p&gt;S
-000010e0: 6561 7263 6820 7261 6469 7573 2066 6f72  earch radius for
-000010f0: 2074 6865 206c 696e 6b69 6e67 2070 726f   the linking pro
-00001100: 6365 6475 7265 266c 743b 2f70 2667 743b  cedure&lt;/p&gt;
-00001110: 266c 743b 2f62 6f64 7926 6774 3b26 6c74  &lt;/body&gt;&lt
-00001120: 3b2f 6874 6d6c 2667 743b 3c2f 7374 7269  ;/html&gt;</stri
-00001130: 6e67 3e0d 0a20 2020 2020 2020 2020 3c2f  ng>..         </
-00001140: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
-00001150: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00001160: 6d65 3d22 7465 7874 223e 0d0a 2020 2020  me="text">..    
-00001170: 2020 2020 2020 3c73 7472 696e 673e 353c        <string>5<
-00001180: 2f73 7472 696e 673e 0d0a 2020 2020 2020  /string>..      
-00001190: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-000011a0: 2020 2020 2020 2020 3c2f 7769 6467 6574          </widget
-000011b0: 3e0d 0a20 2020 2020 2020 3c2f 6974 656d  >..       </item
-000011c0: 3e0d 0a20 2020 2020 2020 3c69 7465 6d20  >..       <item 
-000011d0: 726f 773d 2236 2220 636f 6c75 6d6e 3d22  row="6" column="
-000011e0: 3022 3e0d 0a20 2020 2020 2020 203c 7769  0">..        <wi
-000011f0: 6467 6574 2063 6c61 7373 3d22 514c 6162  dget class="QLab
-00001200: 656c 2220 6e61 6d65 3d22 6c61 6265 6c5f  el" name="label_
-00001210: 3622 3e0d 0a20 2020 2020 2020 2020 3c70  6">..         <p
-00001220: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
-00001230: 7874 223e 0d0a 2020 2020 2020 2020 2020  xt">..          
-00001240: 3c73 7472 696e 673e 4d69 6e20 4672 616d  <string>Min Fram
-00001250: 6573 3c2f 7374 7269 6e67 3e0d 0a20 2020  es</string>..   
-00001260: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
-00001270: 3e0d 0a20 2020 2020 2020 2020 3c70 726f  >..         <pro
-00001280: 7065 7274 7920 6e61 6d65 3d22 6275 6464  perty name="budd
-00001290: 7922 3e0d 0a20 2020 2020 2020 2020 203c  y">..          <
-000012a0: 6373 7472 696e 673e 6d69 6e5f 6672 616d  cstring>min_fram
-000012b0: 6573 5f6c 696e 653c 2f63 7374 7269 6e67  es_line</cstring
-000012c0: 3e0d 0a20 2020 2020 2020 2020 3c2f 7072  >..         </pr
-000012d0: 6f70 6572 7479 3e0d 0a20 2020 2020 2020  operty>..       
-000012e0: 203c 2f77 6964 6765 743e 0d0a 2020 2020   </widget>..    
-000012f0: 2020 203c 2f69 7465 6d3e 0d0a 2020 2020     </item>..    
-00001300: 2020 203c 6974 656d 2072 6f77 3d22 3622     <item row="6"
-00001310: 2063 6f6c 756d 6e3d 2231 223e 0d0a 2020   column="1">..  
-00001320: 2020 2020 2020 3c77 6964 6765 7420 636c        <widget cl
-00001330: 6173 733d 2251 4c69 6e65 4564 6974 2220  ass="QLineEdit" 
-00001340: 6e61 6d65 3d22 6d69 6e5f 6672 616d 6573  name="min_frames
-00001350: 5f6c 696e 6522 3e0d 0a20 2020 2020 2020  _line">..       
-00001360: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00001370: 3d22 746f 6f6c 5469 7022 3e0d 0a20 2020  ="toolTip">..   
-00001380: 2020 2020 2020 203c 7374 7269 6e67 3e26         <string>&
-00001390: 6c74 3b68 746d 6c26 6774 3b26 6c74 3b68  lt;html&gt;&lt;h
-000013a0: 6561 642f 2667 743b 266c 743b 626f 6479  ead/&gt;&lt;body
-000013b0: 2667 743b 266c 743b 7026 6774 3b4d 696e  &gt;&lt;p&gt;Min
-000013c0: 696d 756d 206e 756d 6265 7220 6f66 2066  imum number of f
-000013d0: 7261 6d65 7320 746f 2063 6f6e 7369 6465  rames to conside
-000013e0: 7220 6974 2061 2070 6172 7469 636c 6526  r it a particle&
-000013f0: 6c74 3b2f 7026 6774 3b26 6c74 3b2f 626f  lt;/p&gt;&lt;/bo
-00001400: 6479 2667 743b 266c 743b 2f68 746d 6c26  dy&gt;&lt;/html&
-00001410: 6774 3b3c 2f73 7472 696e 673e 0d0a 2020  gt;</string>..  
-00001420: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
-00001430: 793e 0d0a 2020 2020 2020 2020 203c 7072  y>..         <pr
-00001440: 6f70 6572 7479 206e 616d 653d 2274 6578  operty name="tex
-00001450: 7422 3e0d 0a20 2020 2020 2020 2020 203c  t">..          <
-00001460: 7374 7269 6e67 3e33 3c2f 7374 7269 6e67  string>3</string
-00001470: 3e0d 0a20 2020 2020 2020 2020 3c2f 7072  >..         </pr
-00001480: 6f70 6572 7479 3e0d 0a20 2020 2020 2020  operty>..       
-00001490: 203c 2f77 6964 6765 743e 0d0a 2020 2020   </widget>..    
-000014a0: 2020 203c 2f69 7465 6d3e 0d0a 2020 2020     </item>..    
-000014b0: 2020 203c 6974 656d 2072 6f77 3d22 3722     <item row="7"
-000014c0: 2063 6f6c 756d 6e3d 2231 223e 0d0a 2020   column="1">..  
-000014d0: 2020 2020 2020 3c77 6964 6765 7420 636c        <widget cl
-000014e0: 6173 733d 2251 5075 7368 4275 7474 6f6e  ass="QPushButton
-000014f0: 2220 6e61 6d65 3d22 6361 6c63 756c 6174  " name="calculat
-00001500: 655f 6275 7474 6f6e 223e 0d0a 2020 2020  e_button">..    
-00001510: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00001520: 616d 653d 2274 6f6f 6c54 6970 223e 0d0a  ame="toolTip">..
-00001530: 2020 2020 2020 2020 2020 3c73 7472 696e            <strin
-00001540: 673e 266c 743b 6874 6d6c 2667 743b 266c  g>&lt;html&gt;&l
-00001550: 743b 6865 6164 2f26 6774 3b26 6c74 3b62  t;head/&gt;&lt;b
-00001560: 6f64 7926 6774 3b26 6c74 3b70 2667 743b  ody&gt;&lt;p&gt;
-00001570: 4669 6e64 2074 6865 206c 6f63 6174 696f  Find the locatio
-00001580: 6e73 206f 6620 616c 6c20 7468 6520 7061  ns of all the pa
-00001590: 7274 6963 6c65 7320 696e 2074 6865 2072  rticles in the r
-000015a0: 616e 6765 206f 6620 6672 616d 6573 266c  ange of frames&l
-000015b0: 743b 2f70 2667 743b 266c 743b 2f62 6f64  t;/p&gt;&lt;/bod
-000015c0: 7926 6774 3b26 6c74 3b2f 6874 6d6c 2667  y&gt;&lt;/html&g
-000015d0: 743b 3c2f 7374 7269 6e67 3e0d 0a20 2020  t;</string>..   
-000015e0: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
-000015f0: 3e0d 0a20 2020 2020 2020 2020 3c70 726f  >..         <pro
-00001600: 7065 7274 7920 6e61 6d65 3d22 7465 7874  perty name="text
-00001610: 223e 0d0a 2020 2020 2020 2020 2020 3c73  ">..          <s
-00001620: 7472 696e 673e 4361 6c63 756c 6174 6520  tring>Calculate 
-00001630: 616c 6c3c 2f73 7472 696e 673e 0d0a 2020  all</string>..  
-00001640: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
-00001650: 793e 0d0a 2020 2020 2020 2020 3c2f 7769  y>..        </wi
-00001660: 6467 6574 3e0d 0a20 2020 2020 2020 3c2f  dget>..       </
-00001670: 6974 656d 3e0d 0a20 2020 2020 2020 3c69  item>..       <i
-00001680: 7465 6d20 726f 773d 2239 2220 636f 6c75  tem row="9" colu
-00001690: 6d6e 3d22 3022 2063 6f6c 7370 616e 3d22  mn="0" colspan="
-000016a0: 3222 3e0d 0a20 2020 2020 2020 203c 7769  2">..        <wi
-000016b0: 6467 6574 2063 6c61 7373 3d22 4c69 6e65  dget class="Line
-000016c0: 2220 6e61 6d65 3d22 6c69 6e65 223e 0d0a  " name="line">..
-000016d0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-000016e0: 7479 206e 616d 653d 226f 7269 656e 7461  ty name="orienta
-000016f0: 7469 6f6e 223e 0d0a 2020 2020 2020 2020  tion">..        
-00001700: 2020 3c65 6e75 6d3e 5174 3a3a 486f 7269    <enum>Qt::Hori
-00001710: 7a6f 6e74 616c 3c2f 656e 756d 3e0d 0a20  zontal</enum>.. 
-00001720: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
-00001730: 7479 3e0d 0a20 2020 2020 2020 203c 2f77  ty>..        </w
-00001740: 6964 6765 743e 0d0a 2020 2020 2020 203c  idget>..       <
-00001750: 2f69 7465 6d3e 0d0a 2020 2020 2020 203c  /item>..       <
-00001760: 6974 656d 2072 6f77 3d22 3130 2220 636f  item row="10" co
-00001770: 6c75 6d6e 3d22 3022 3e0d 0a20 2020 2020  lumn="0">..     
-00001780: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
-00001790: 3d22 514c 6162 656c 2220 6e61 6d65 3d22  ="QLabel" name="
-000017a0: 6c61 6265 6c5f 3822 3e0d 0a20 2020 2020  label_8">..     
-000017b0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-000017c0: 6d65 3d22 7465 7874 223e 0d0a 2020 2020  me="text">..    
-000017d0: 2020 2020 2020 3c73 7472 696e 673e 5374        <string>St
-000017e0: 6570 2053 697a 6520 28c2 b56d 293c 2f73  ep Size (..m)</s
-000017f0: 7472 696e 673e 0d0a 2020 2020 2020 2020  tring>..        
-00001800: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
-00001810: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00001820: 206e 616d 653d 2262 7564 6479 223e 0d0a   name="buddy">..
-00001830: 2020 2020 2020 2020 2020 3c63 7374 7269            <cstri
-00001840: 6e67 3e73 7465 705f 7369 7a65 5f6c 696e  ng>step_size_lin
-00001850: 653c 2f63 7374 7269 6e67 3e0d 0a20 2020  e</cstring>..   
-00001860: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
-00001870: 3e0d 0a20 2020 2020 2020 203c 2f77 6964  >..        </wid
-00001880: 6765 743e 0d0a 2020 2020 2020 203c 2f69  get>..       </i
-00001890: 7465 6d3e 0d0a 2020 2020 2020 203c 6974  tem>..       <it
-000018a0: 656d 2072 6f77 3d22 3130 2220 636f 6c75  em row="10" colu
-000018b0: 6d6e 3d22 3122 3e0d 0a20 2020 2020 2020  mn="1">..       
-000018c0: 203c 7769 6467 6574 2063 6c61 7373 3d22   <widget class="
-000018d0: 514c 696e 6545 6469 7422 206e 616d 653d  QLineEdit" name=
-000018e0: 2273 7465 705f 7369 7a65 5f6c 696e 6522  "step_size_line"
-000018f0: 3e0d 0a20 2020 2020 2020 2020 3c70 726f  >..         <pro
-00001900: 7065 7274 7920 6e61 6d65 3d22 746f 6f6c  perty name="tool
-00001910: 5469 7022 3e0d 0a20 2020 2020 2020 2020  Tip">..         
-00001920: 203c 7374 7269 6e67 3e26 6c74 3b68 746d   <string>&lt;htm
-00001930: 6c26 6774 3b26 6c74 3b68 6561 642f 2667  l&gt;&lt;head/&g
-00001940: 743b 266c 743b 626f 6479 2667 743b 266c  t;&lt;body&gt;&l
-00001950: 743b 7026 6774 3b53 7465 7020 7369 7a65  t;p&gt;Step size
-00001960: 2064 7572 696e 6720 7468 6520 7363 616e   during the scan
-00001970: 266c 743b 2f70 2667 743b 266c 743b 2f62  &lt;/p&gt;&lt;/b
-00001980: 6f64 7926 6774 3b26 6c74 3b2f 6874 6d6c  ody&gt;&lt;/html
-00001990: 2667 743b 3c2f 7374 7269 6e67 3e0d 0a20  &gt;</string>.. 
-000019a0: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
-000019b0: 7479 3e0d 0a20 2020 2020 2020 2020 3c70  ty>..         <p
-000019c0: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
-000019d0: 7874 223e 0d0a 2020 2020 2020 2020 2020  xt">..          
-000019e0: 3c73 7472 696e 673e 353c 2f73 7472 696e  <string>5</strin
-000019f0: 673e 0d0a 2020 2020 2020 2020 203c 2f70  g>..         </p
-00001a00: 726f 7065 7274 793e 0d0a 2020 2020 2020  roperty>..      
-00001a10: 2020 3c2f 7769 6467 6574 3e0d 0a20 2020    </widget>..   
-00001a20: 2020 2020 3c2f 6974 656d 3e0d 0a20 2020      </item>..   
-00001a30: 2020 2020 3c69 7465 6d20 726f 773d 2231      <item row="1
-00001a40: 3122 2063 6f6c 756d 6e3d 2231 223e 0d0a  1" column="1">..
-00001a50: 2020 2020 2020 2020 3c73 7061 6365 7220          <spacer 
-00001a60: 6e61 6d65 3d22 7665 7274 6963 616c 5370  name="verticalSp
-00001a70: 6163 6572 223e 0d0a 2020 2020 2020 2020  acer">..        
-00001a80: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00001a90: 226f 7269 656e 7461 7469 6f6e 223e 0d0a  "orientation">..
-00001aa0: 2020 2020 2020 2020 2020 3c65 6e75 6d3e            <enum>
-00001ab0: 5174 3a3a 5665 7274 6963 616c 3c2f 656e  Qt::Vertical</en
-00001ac0: 756d 3e0d 0a20 2020 2020 2020 2020 3c2f  um>..         </
-00001ad0: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
-00001ae0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00001af0: 6d65 3d22 7369 7a65 4869 6e74 2220 7374  me="sizeHint" st
-00001b00: 6473 6574 3d22 3022 3e0d 0a20 2020 2020  dset="0">..     
-00001b10: 2020 2020 203c 7369 7a65 3e0d 0a20 2020       <size>..   
-00001b20: 2020 2020 2020 2020 3c77 6964 7468 3e32          <width>2
-00001b30: 303c 2f77 6964 7468 3e0d 0a20 2020 2020  0</width>..     
-00001b40: 2020 2020 2020 3c68 6569 6768 743e 3430        <height>40
-00001b50: 3c2f 6865 6967 6874 3e0d 0a20 2020 2020  </height>..     
-00001b60: 2020 2020 203c 2f73 697a 653e 0d0a 2020       </size>..  
-00001b70: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
-00001b80: 793e 0d0a 2020 2020 2020 2020 3c2f 7370  y>..        </sp
-00001b90: 6163 6572 3e0d 0a20 2020 2020 2020 3c2f  acer>..       </
-00001ba0: 6974 656d 3e0d 0a20 2020 2020 203c 2f6c  item>..      </l
-00001bb0: 6179 6f75 743e 0d0a 2020 2020 203c 2f77  ayout>..     </w
-00001bc0: 6964 6765 743e 0d0a 2020 2020 3c2f 6974  idget>..    </it
-00001bd0: 656d 3e0d 0a20 2020 203c 6974 656d 3e0d  em>..    <item>.
-00001be0: 0a20 2020 2020 3c77 6964 6765 7420 636c  .     <widget cl
-00001bf0: 6173 733d 2251 5769 6467 6574 2220 6e61  ass="QWidget" na
-00001c00: 6d65 3d22 7769 6467 6574 2220 6e61 7469  me="widget" nati
-00001c10: 7665 3d22 7472 7565 223e 0d0a 2020 2020  ve="true">..    
-00001c20: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00001c30: 3d22 7369 7a65 506f 6c69 6379 223e 0d0a  ="sizePolicy">..
-00001c40: 2020 2020 2020 203c 7369 7a65 706f 6c69         <sizepoli
-00001c50: 6379 2068 7369 7a65 7479 7065 3d22 4578  cy hsizetype="Ex
-00001c60: 7061 6e64 696e 6722 2076 7369 7a65 7479  panding" vsizety
-00001c70: 7065 3d22 5072 6566 6572 7265 6422 3e0d  pe="Preferred">.
-00001c80: 0a20 2020 2020 2020 203c 686f 7273 7472  .        <horstr
-00001c90: 6574 6368 3e30 3c2f 686f 7273 7472 6574  etch>0</horstret
-00001ca0: 6368 3e0d 0a20 2020 2020 2020 203c 7665  ch>..        <ve
-00001cb0: 7273 7472 6574 6368 3e30 3c2f 7665 7273  rstretch>0</vers
-00001cc0: 7472 6574 6368 3e0d 0a20 2020 2020 2020  tretch>..       
-00001cd0: 3c2f 7369 7a65 706f 6c69 6379 3e0d 0a20  </sizepolicy>.. 
-00001ce0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00001cf0: 0d0a 2020 2020 2020 3c6c 6179 6f75 7420  ..      <layout 
-00001d00: 636c 6173 733d 2251 5642 6f78 4c61 796f  class="QVBoxLayo
-00001d10: 7574 2220 6e61 6d65 3d22 7665 7274 6963  ut" name="vertic
-00001d20: 616c 4c61 796f 7574 223e 0d0a 2020 2020  alLayout">..    
-00001d30: 2020 203c 6974 656d 3e0d 0a20 2020 2020     <item>..     
-00001d40: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
-00001d50: 3d22 5157 6964 6765 7422 206e 616d 653d  ="QWidget" name=
-00001d60: 2273 6c69 6465 725f 7769 6467 6574 2220  "slider_widget" 
-00001d70: 6e61 7469 7665 3d22 7472 7565 223e 0d0a  native="true">..
-00001d80: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00001d90: 7479 206e 616d 653d 2273 697a 6550 6f6c  ty name="sizePol
-00001da0: 6963 7922 3e0d 0a20 2020 2020 2020 2020  icy">..         
-00001db0: 203c 7369 7a65 706f 6c69 6379 2068 7369   <sizepolicy hsi
-00001dc0: 7a65 7479 7065 3d22 5072 6566 6572 7265  zetype="Preferre
-00001dd0: 6422 2076 7369 7a65 7479 7065 3d22 4d69  d" vsizetype="Mi
-00001de0: 6e69 6d75 6d22 3e0d 0a20 2020 2020 2020  nimum">..       
-00001df0: 2020 2020 3c68 6f72 7374 7265 7463 683e      <horstretch>
-00001e00: 303c 2f68 6f72 7374 7265 7463 683e 0d0a  0</horstretch>..
-00001e10: 2020 2020 2020 2020 2020 203c 7665 7273             <vers
-00001e20: 7472 6574 6368 3e30 3c2f 7665 7273 7472  tretch>0</verstr
-00001e30: 6574 6368 3e0d 0a20 2020 2020 2020 2020  etch>..         
-00001e40: 203c 2f73 697a 6570 6f6c 6963 793e 0d0a   </sizepolicy>..
-00001e50: 2020 2020 2020 2020 203c 2f70 726f 7065           </prope
-00001e60: 7274 793e 0d0a 2020 2020 2020 2020 203c  rty>..         <
-00001e70: 7072 6f70 6572 7479 206e 616d 653d 226d  property name="m
-00001e80: 6178 696d 756d 5369 7a65 223e 0d0a 2020  aximumSize">..  
-00001e90: 2020 2020 2020 2020 3c73 697a 653e 0d0a          <size>..
-00001ea0: 2020 2020 2020 2020 2020 203c 7769 6474             <widt
-00001eb0: 683e 3136 3737 3732 3135 3c2f 7769 6474  h>16777215</widt
-00001ec0: 683e 0d0a 2020 2020 2020 2020 2020 203c  h>..           <
-00001ed0: 6865 6967 6874 3e35 303c 2f68 6569 6768  height>50</heigh
-00001ee0: 743e 0d0a 2020 2020 2020 2020 2020 3c2f  t>..          </
-00001ef0: 7369 7a65 3e0d 0a20 2020 2020 2020 2020  size>..         
-00001f00: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
-00001f10: 2020 2020 2020 3c6c 6179 6f75 7420 636c        <layout cl
-00001f20: 6173 733d 2251 4842 6f78 4c61 796f 7574  ass="QHBoxLayout
-00001f30: 2220 6e61 6d65 3d22 686f 7269 7a6f 6e74  " name="horizont
-00001f40: 616c 4c61 796f 7574 5f33 223e 0d0a 2020  alLayout_3">..  
-00001f50: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00001f60: 7920 6e61 6d65 3d22 746f 704d 6172 6769  y name="topMargi
-00001f70: 6e22 3e0d 0a20 2020 2020 2020 2020 2020  n">..           
-00001f80: 3c6e 756d 6265 723e 303c 2f6e 756d 6265  <number>0</numbe
-00001f90: 723e 0d0a 2020 2020 2020 2020 2020 3c2f  r>..          </
-00001fa0: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
-00001fb0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00001fc0: 616d 653d 2262 6f74 746f 6d4d 6172 6769  ame="bottomMargi
-00001fd0: 6e22 3e0d 0a20 2020 2020 2020 2020 2020  n">..           
-00001fe0: 3c6e 756d 6265 723e 303c 2f6e 756d 6265  <number>0</numbe
-00001ff0: 723e 0d0a 2020 2020 2020 2020 2020 3c2f  r>..          </
-00002000: 7072 6f70 6572 7479 3e0d 0a20 2020 2020  property>..     
-00002010: 2020 2020 203c 6974 656d 3e0d 0a20 2020       <item>..   
-00002020: 2020 2020 2020 2020 3c77 6964 6765 7420          <widget 
-00002030: 636c 6173 733d 2251 4c61 6265 6c22 206e  class="QLabel" n
-00002040: 616d 653d 2266 7261 6d65 5f6e 756d 223e  ame="frame_num">
-00002050: 0d0a 2020 2020 2020 2020 2020 2020 3c70  ..            <p
-00002060: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
-00002070: 7874 223e 0d0a 2020 2020 2020 2020 2020  xt">..          
-00002080: 2020 203c 7374 7269 6e67 3e30 3c2f 7374     <string>0</st
-00002090: 7269 6e67 3e0d 0a20 2020 2020 2020 2020  ring>..         
-000020a0: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-000020b0: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-000020c0: 7065 7274 7920 6e61 6d65 3d22 6275 6464  perty name="budd
-000020d0: 7922 3e0d 0a20 2020 2020 2020 2020 2020  y">..           
-000020e0: 2020 3c63 7374 7269 6e67 3e66 7261 6d65    <cstring>frame
-000020f0: 5f73 6c69 6465 723c 2f63 7374 7269 6e67  _slider</cstring
-00002100: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-00002110: 2f70 726f 7065 7274 793e 0d0a 2020 2020  /property>..    
-00002120: 2020 2020 2020 203c 2f77 6964 6765 743e         </widget>
-00002130: 0d0a 2020 2020 2020 2020 2020 3c2f 6974  ..          </it
-00002140: 656d 3e0d 0a20 2020 2020 2020 2020 203c  em>..          <
-00002150: 6974 656d 3e0d 0a20 2020 2020 2020 2020  item>..         
-00002160: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
-00002170: 2251 536c 6964 6572 2220 6e61 6d65 3d22  "QSlider" name="
-00002180: 6672 616d 655f 736c 6964 6572 223e 0d0a  frame_slider">..
-00002190: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-000021a0: 7065 7274 7920 6e61 6d65 3d22 656e 6162  perty name="enab
-000021b0: 6c65 6422 3e0d 0a20 2020 2020 2020 2020  led">..         
-000021c0: 2020 2020 3c62 6f6f 6c3e 6661 6c73 653c      <bool>false<
-000021d0: 2f62 6f6f 6c3e 0d0a 2020 2020 2020 2020  /bool>..        
-000021e0: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
-000021f0: 0a20 2020 2020 2020 2020 2020 203c 7072  .            <pr
-00002200: 6f70 6572 7479 206e 616d 653d 226d 6f75  operty name="mou
-00002210: 7365 5472 6163 6b69 6e67 223e 0d0a 2020  seTracking">..  
-00002220: 2020 2020 2020 2020 2020 203c 626f 6f6c             <bool
-00002230: 3e74 7275 653c 2f62 6f6f 6c3e 0d0a 2020  >true</bool>..  
-00002240: 2020 2020 2020 2020 2020 3c2f 7072 6f70            </prop
-00002250: 6572 7479 3e0d 0a20 2020 2020 2020 2020  erty>..         
-00002260: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00002270: 653d 2266 6f63 7573 506f 6c69 6379 223e  e="focusPolicy">
-00002280: 0d0a 2020 2020 2020 2020 2020 2020 203c  ..             <
-00002290: 656e 756d 3e51 743a 3a57 6865 656c 466f  enum>Qt::WheelFo
-000022a0: 6375 733c 2f65 6e75 6d3e 0d0a 2020 2020  cus</enum>..    
-000022b0: 2020 2020 2020 2020 3c2f 7072 6f70 6572          </proper
-000022c0: 7479 3e0d 0a20 2020 2020 2020 2020 2020  ty>..           
-000022d0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-000022e0: 2273 7461 7475 7354 6970 223e 0d0a 2020  "statusTip">..  
-000022f0: 2020 2020 2020 2020 2020 203c 7374 7269             <stri
-00002300: 6e67 3e53 7461 7475 7320 7469 703c 2f73  ng>Status tip</s
-00002310: 7472 696e 673e 0d0a 2020 2020 2020 2020  tring>..        
-00002320: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
-00002330: 0a20 2020 2020 2020 2020 2020 203c 7072  .            <pr
-00002340: 6f70 6572 7479 206e 616d 653d 226f 7269  operty name="ori
-00002350: 656e 7461 7469 6f6e 223e 0d0a 2020 2020  entation">..    
-00002360: 2020 2020 2020 2020 203c 656e 756d 3e51           <enum>Q
-00002370: 743a 3a48 6f72 697a 6f6e 7461 6c3c 2f65  t::Horizontal</e
-00002380: 6e75 6d3e 0d0a 2020 2020 2020 2020 2020  num>..          
-00002390: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
-000023a0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-000023b0: 6572 7479 206e 616d 653d 2274 6963 6b50  erty name="tickP
-000023c0: 6f73 6974 696f 6e22 3e0d 0a20 2020 2020  osition">..     
-000023d0: 2020 2020 2020 2020 3c65 6e75 6d3e 5153          <enum>QS
-000023e0: 6c69 6465 723a 3a54 6963 6b73 4162 6f76  lider::TicksAbov
-000023f0: 653c 2f65 6e75 6d3e 0d0a 2020 2020 2020  e</enum>..      
-00002400: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
-00002410: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-00002420: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
-00002430: 6963 6b49 6e74 6572 7661 6c22 3e0d 0a20  ickInterval">.. 
-00002440: 2020 2020 2020 2020 2020 2020 3c6e 756d              <num
-00002450: 6265 723e 3230 3c2f 6e75 6d62 6572 3e0d  ber>20</number>.
-00002460: 0a20 2020 2020 2020 2020 2020 203c 2f70  .            </p
-00002470: 726f 7065 7274 793e 0d0a 2020 2020 2020  roperty>..      
-00002480: 2020 2020 203c 2f77 6964 6765 743e 0d0a       </widget>..
-00002490: 2020 2020 2020 2020 2020 3c2f 6974 656d            </item
-000024a0: 3e0d 0a20 2020 2020 2020 2020 3c2f 6c61  >..         </la
-000024b0: 796f 7574 3e0d 0a20 2020 2020 2020 203c  yout>..        <
-000024c0: 2f77 6964 6765 743e 0d0a 2020 2020 2020  /widget>..      
-000024d0: 203c 2f69 7465 6d3e 0d0a 2020 2020 2020   </item>..      
-000024e0: 203c 6974 656d 3e0d 0a20 2020 2020 2020   <item>..       
-000024f0: 203c 7769 6467 6574 2063 6c61 7373 3d22   <widget class="
-00002500: 5157 6964 6765 7422 206e 616d 653d 2276  QWidget" name="v
-00002510: 6964 656f 5f77 6964 6765 7422 206e 6174  ideo_widget" nat
-00002520: 6976 653d 2274 7275 6522 3e0d 0a20 2020  ive="true">..   
-00002530: 2020 2020 2020 3c6c 6179 6f75 7420 636c        <layout cl
-00002540: 6173 733d 2251 4772 6964 4c61 796f 7574  ass="QGridLayout
-00002550: 2220 6e61 6d65 3d22 6772 6964 4c61 796f  " name="gridLayo
-00002560: 7574 223e 0d0a 2020 2020 2020 2020 2020  ut">..          
-00002570: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00002580: 6c65 6674 4d61 7267 696e 223e 0d0a 2020  leftMargin">..  
-00002590: 2020 2020 2020 2020 203c 6e75 6d62 6572           <number
-000025a0: 3e30 3c2f 6e75 6d62 6572 3e0d 0a20 2020  >0</number>..   
-000025b0: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
-000025c0: 793e 0d0a 2020 2020 2020 2020 2020 3c70  y>..          <p
-000025d0: 726f 7065 7274 7920 6e61 6d65 3d22 746f  roperty name="to
-000025e0: 704d 6172 6769 6e22 3e0d 0a20 2020 2020  pMargin">..     
-000025f0: 2020 2020 2020 3c6e 756d 6265 723e 303c        <number>0<
-00002600: 2f6e 756d 6265 723e 0d0a 2020 2020 2020  /number>..      
-00002610: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
-00002620: 0a20 2020 2020 2020 2020 203c 7072 6f70  .          <prop
-00002630: 6572 7479 206e 616d 653d 2272 6967 6874  erty name="right
-00002640: 4d61 7267 696e 223e 0d0a 2020 2020 2020  Margin">..      
-00002650: 2020 2020 203c 6e75 6d62 6572 3e30 3c2f       <number>0</
-00002660: 6e75 6d62 6572 3e0d 0a20 2020 2020 2020  number>..       
-00002670: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-00002680: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00002690: 7274 7920 6e61 6d65 3d22 626f 7474 6f6d  rty name="bottom
-000026a0: 4d61 7267 696e 223e 0d0a 2020 2020 2020  Margin">..      
-000026b0: 2020 2020 203c 6e75 6d62 6572 3e30 3c2f       <number>0</
-000026c0: 6e75 6d62 6572 3e0d 0a20 2020 2020 2020  number>..       
-000026d0: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-000026e0: 2020 2020 2020 2020 203c 2f6c 6179 6f75           </layou
-000026f0: 743e 0d0a 2020 2020 2020 2020 3c2f 7769  t>..        </wi
-00002700: 6467 6574 3e0d 0a20 2020 2020 2020 3c2f  dget>..       </
-00002710: 6974 656d 3e0d 0a20 2020 2020 203c 2f6c  item>..      </l
-00002720: 6179 6f75 743e 0d0a 2020 2020 203c 2f77  ayout>..     </w
-00002730: 6964 6765 743e 0d0a 2020 2020 3c2f 6974  idget>..    </it
-00002740: 656d 3e0d 0a20 2020 3c2f 6c61 796f 7574  em>..   </layout
-00002750: 3e0d 0a20 203c 2f77 6964 6765 743e 0d0a  >..  </widget>..
-00002760: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
-00002770: 2251 5374 6174 7573 4261 7222 206e 616d  "QStatusBar" nam
-00002780: 653d 2273 7461 7475 7362 6172 222f 3e0d  e="statusbar"/>.
-00002790: 0a20 203c 7769 6467 6574 2063 6c61 7373  .  <widget class
-000027a0: 3d22 5154 6f6f 6c42 6172 2220 6e61 6d65  ="QToolBar" name
-000027b0: 3d22 746f 6f6c 4261 7222 3e0d 0a20 2020  ="toolBar">..   
-000027c0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-000027d0: 7769 6e64 6f77 5469 746c 6522 3e0d 0a20  windowTitle">.. 
-000027e0: 2020 203c 7374 7269 6e67 3e74 6f6f 6c42     <string>toolB
-000027f0: 6172 3c2f 7374 7269 6e67 3e0d 0a20 2020  ar</string>..   
-00002800: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
-00002810: 3c61 7474 7269 6275 7465 206e 616d 653d  <attribute name=
-00002820: 2274 6f6f 6c42 6172 4172 6561 223e 0d0a  "toolBarArea">..
-00002830: 2020 2020 3c65 6e75 6d3e 546f 7054 6f6f      <enum>TopToo
-00002840: 6c42 6172 4172 6561 3c2f 656e 756d 3e0d  lBarArea</enum>.
-00002850: 0a20 2020 3c2f 6174 7472 6962 7574 653e  .   </attribute>
-00002860: 0d0a 2020 203c 6174 7472 6962 7574 6520  ..   <attribute 
-00002870: 6e61 6d65 3d22 746f 6f6c 4261 7242 7265  name="toolBarBre
-00002880: 616b 223e 0d0a 2020 2020 3c62 6f6f 6c3e  ak">..    <bool>
-00002890: 6661 6c73 653c 2f62 6f6f 6c3e 0d0a 2020  false</bool>..  
-000028a0: 203c 2f61 7474 7269 6275 7465 3e0d 0a20   </attribute>.. 
-000028b0: 2020 3c61 6464 6163 7469 6f6e 206e 616d    <addaction nam
-000028c0: 653d 2261 6374 696f 6e5f 6f70 656e 222f  e="action_open"/
-000028d0: 3e0d 0a20 2020 3c61 6464 6163 7469 6f6e  >..   <addaction
-000028e0: 206e 616d 653d 2261 6374 696f 6e5f 6d61   name="action_ma
-000028f0: 7373 5f68 6973 746f 6772 616d 222f 3e0d  ss_histogram"/>.
-00002900: 0a20 2020 3c61 6464 6163 7469 6f6e 206e  .   <addaction n
-00002910: 616d 653d 2261 6374 696f 6e5f 6461 7461  ame="action_data
-00002920: 5f70 6c6f 7473 222f 3e0d 0a20 2020 3c61  _plots"/>..   <a
-00002930: 6464 6163 7469 6f6e 206e 616d 653d 2261  ddaction name="a
-00002940: 6374 696f 6e5f 7361 7665 5f64 6174 6122  ction_save_data"
-00002950: 2f3e 0d0a 2020 3c2f 7769 6467 6574 3e0d  />..  </widget>.
-00002960: 0a20 203c 7769 6467 6574 2063 6c61 7373  .  <widget class
-00002970: 3d22 514d 656e 7542 6172 2220 6e61 6d65  ="QMenuBar" name
-00002980: 3d22 6d65 6e75 4261 7222 3e0d 0a20 2020  ="menuBar">..   
-00002990: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-000029a0: 6765 6f6d 6574 7279 223e 0d0a 2020 2020  geometry">..    
-000029b0: 3c72 6563 743e 0d0a 2020 2020 203c 783e  <rect>..     <x>
-000029c0: 303c 2f78 3e0d 0a20 2020 2020 3c79 3e30  0</x>..     <y>0
-000029d0: 3c2f 793e 0d0a 2020 2020 203c 7769 6474  </y>..     <widt
-000029e0: 683e 3736 383c 2f77 6964 7468 3e0d 0a20  h>768</width>.. 
-000029f0: 2020 2020 3c68 6569 6768 743e 3234 3c2f      <height>24</
-00002a00: 6865 6967 6874 3e0d 0a20 2020 203c 2f72  height>..    </r
-00002a10: 6563 743e 0d0a 2020 203c 2f70 726f 7065  ect>..   </prope
-00002a20: 7274 793e 0d0a 2020 203c 7769 6467 6574  rty>..   <widget
-00002a30: 2063 6c61 7373 3d22 514d 656e 7522 206e   class="QMenu" n
-00002a40: 616d 653d 226d 656e 7546 696c 6522 3e0d  ame="menuFile">.
-00002a50: 0a20 2020 203c 7072 6f70 6572 7479 206e  .    <property n
-00002a60: 616d 653d 2274 6974 6c65 223e 0d0a 2020  ame="title">..  
-00002a70: 2020 203c 7374 7269 6e67 3e46 696c 653c     <string>File<
-00002a80: 2f73 7472 696e 673e 0d0a 2020 2020 3c2f  /string>..    </
-00002a90: 7072 6f70 6572 7479 3e0d 0a20 2020 203c  property>..    <
-00002aa0: 6164 6461 6374 696f 6e20 6e61 6d65 3d22  addaction name="
-00002ab0: 6163 7469 6f6e 5f6f 7065 6e22 2f3e 0d0a  action_open"/>..
-00002ac0: 2020 2020 3c61 6464 6163 7469 6f6e 206e      <addaction n
-00002ad0: 616d 653d 2261 6374 696f 6e5f 7361 7665  ame="action_save
-00002ae0: 5f64 6174 6122 2f3e 0d0a 2020 2020 3c61  _data"/>..    <a
-00002af0: 6464 6163 7469 6f6e 206e 616d 653d 2261  ddaction name="a
-00002b00: 6374 696f 6e5f 6578 706f 7274 5f61 6c6c  ction_export_all
-00002b10: 5f64 6174 6122 2f3e 0d0a 2020 203c 2f77  _data"/>..   </w
-00002b20: 6964 6765 743e 0d0a 2020 203c 7769 6467  idget>..   <widg
-00002b30: 6574 2063 6c61 7373 3d22 514d 656e 7522  et class="QMenu"
-00002b40: 206e 616d 653d 226d 656e 7541 6e61 7973   name="menuAnays
-00002b50: 6973 223e 0d0a 2020 2020 3c70 726f 7065  is">..    <prope
-00002b60: 7274 7920 6e61 6d65 3d22 7469 746c 6522  rty name="title"
-00002b70: 3e0d 0a20 2020 2020 3c73 7472 696e 673e  >..     <string>
-00002b80: 416e 6179 7369 733c 2f73 7472 696e 673e  Anaysis</string>
-00002b90: 0d0a 2020 2020 3c2f 7072 6f70 6572 7479  ..    </property
-00002ba0: 3e0d 0a20 2020 203c 6164 6461 6374 696f  >..    <addactio
-00002bb0: 6e20 6e61 6d65 3d22 6163 7469 6f6e 5f63  n name="action_c
-00002bc0: 616c 6375 6c61 7465 5f62 6b67 222f 3e0d  alculate_bkg"/>.
-00002bd0: 0a20 2020 203c 6164 6461 6374 696f 6e20  .    <addaction 
-00002be0: 6e61 6d65 3d22 6163 7469 6f6e 5f73 686f  name="action_sho
-00002bf0: 775f 626b 6722 2f3e 0d0a 2020 2020 3c61  w_bkg"/>..    <a
-00002c00: 6464 6163 7469 6f6e 206e 616d 653d 2261  ddaction name="a
-00002c10: 6374 696f 6e5f 6461 7461 5f66 7261 6d65  ction_data_frame
-00002c20: 222f 3e0d 0a20 2020 3c2f 7769 6467 6574  "/>..   </widget
-00002c30: 3e0d 0a20 2020 3c77 6964 6765 7420 636c  >..   <widget cl
-00002c40: 6173 733d 2251 4d65 6e75 2220 6e61 6d65  ass="QMenu" name
-00002c50: 3d22 6d65 6e75 4865 6c70 223e 0d0a 2020  ="menuHelp">..  
-00002c60: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00002c70: 3d22 7469 746c 6522 3e0d 0a20 2020 2020  ="title">..     
-00002c80: 3c73 7472 696e 673e 4865 6c70 3c2f 7374  <string>Help</st
-00002c90: 7269 6e67 3e0d 0a20 2020 203c 2f70 726f  ring>..    </pro
-00002ca0: 7065 7274 793e 0d0a 2020 2020 3c61 6464  perty>..    <add
-00002cb0: 6163 7469 6f6e 206e 616d 653d 2261 6374  action name="act
-00002cc0: 696f 6e5f 6162 6f75 7422 2f3e 0d0a 2020  ion_about"/>..  
-00002cd0: 2020 3c61 6464 6163 7469 6f6e 206e 616d    <addaction nam
-00002ce0: 653d 2261 6374 696f 6e47 6f5f 746f 5f64  e="actionGo_to_d
-00002cf0: 6f63 756d 656e 7461 7469 6f6e 222f 3e0d  ocumentation"/>.
-00002d00: 0a20 2020 3c2f 7769 6467 6574 3e0d 0a20  .   </widget>.. 
-00002d10: 2020 3c61 6464 6163 7469 6f6e 206e 616d    <addaction nam
-00002d20: 653d 226d 656e 7546 696c 6522 2f3e 0d0a  e="menuFile"/>..
-00002d30: 2020 203c 6164 6461 6374 696f 6e20 6e61     <addaction na
-00002d40: 6d65 3d22 6d65 6e75 416e 6179 7369 7322  me="menuAnaysis"
-00002d50: 2f3e 0d0a 2020 203c 6164 6461 6374 696f  />..   <addactio
-00002d60: 6e20 6e61 6d65 3d22 6d65 6e75 4865 6c70  n name="menuHelp
-00002d70: 222f 3e0d 0a20 203c 2f77 6964 6765 743e  "/>..  </widget>
-00002d80: 0d0a 2020 3c61 6374 696f 6e20 6e61 6d65  ..  <action name
-00002d90: 3d22 6163 7469 6f6e 5f6f 7065 6e22 3e0d  ="action_open">.
-00002da0: 0a20 2020 3c70 726f 7065 7274 7920 6e61  .   <property na
-00002db0: 6d65 3d22 6963 6f6e 223e 0d0a 2020 2020  me="icon">..    
-00002dc0: 3c69 636f 6e73 6574 3e0d 0a20 2020 2020  <iconset>..     
-00002dd0: 3c6e 6f72 6d61 6c6f 6666 3e49 636f 6e73  <normaloff>Icons
-00002de0: 2f4f 7065 6e20 466f 6c64 6572 2e73 7667  /Open Folder.svg
-00002df0: 3c2f 6e6f 726d 616c 6f66 663e 4963 6f6e  </normaloff>Icon
-00002e00: 732f 4f70 656e 2046 6f6c 6465 722e 7376  s/Open Folder.sv
-00002e10: 673c 2f69 636f 6e73 6574 3e0d 0a20 2020  g</iconset>..   
-00002e20: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
-00002e30: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00002e40: 7465 7874 223e 0d0a 2020 2020 3c73 7472  text">..    <str
-00002e50: 696e 673e 4f70 656e 3c2f 7374 7269 6e67  ing>Open</string
-00002e60: 3e0d 0a20 2020 3c2f 7072 6f70 6572 7479  >..   </property
-00002e70: 3e0d 0a20 2020 3c70 726f 7065 7274 7920  >..   <property 
-00002e80: 6e61 6d65 3d22 746f 6f6c 5469 7022 3e0d  name="toolTip">.
-00002e90: 0a20 2020 203c 7374 7269 6e67 3e4f 7065  .    <string>Ope
-00002ea0: 6e20 6461 7461 2066 696c 653c 2f73 7472  n data file</str
-00002eb0: 696e 673e 0d0a 2020 203c 2f70 726f 7065  ing>..   </prope
-00002ec0: 7274 793e 0d0a 2020 203c 7072 6f70 6572  rty>..   <proper
-00002ed0: 7479 206e 616d 653d 2273 686f 7274 6375  ty name="shortcu
-00002ee0: 7422 3e0d 0a20 2020 203c 7374 7269 6e67  t">..    <string
-00002ef0: 3e43 7472 6c2b 4f3c 2f73 7472 696e 673e  >Ctrl+O</string>
-00002f00: 0d0a 2020 203c 2f70 726f 7065 7274 793e  ..   </property>
-00002f10: 0d0a 2020 3c2f 6163 7469 6f6e 3e0d 0a20  ..  </action>.. 
-00002f20: 203c 6163 7469 6f6e 206e 616d 653d 2261   <action name="a
-00002f30: 6374 696f 6e5f 6d61 7373 5f68 6973 746f  ction_mass_histo
-00002f40: 6772 616d 223e 0d0a 2020 203c 7072 6f70  gram">..   <prop
-00002f50: 6572 7479 206e 616d 653d 2269 636f 6e22  erty name="icon"
-00002f60: 3e0d 0a20 2020 203c 6963 6f6e 7365 743e  >..    <iconset>
-00002f70: 0d0a 2020 2020 203c 6e6f 726d 616c 6f66  ..     <normalof
-00002f80: 663e 4963 6f6e 732f 3131 3833 3720 2d20  f>Icons/11837 - 
-00002f90: 4869 7374 6f67 7261 6d2e 7376 673c 2f6e  Histogram.svg</n
-00002fa0: 6f72 6d61 6c6f 6666 3e49 636f 6e73 2f31  ormaloff>Icons/1
-00002fb0: 3138 3337 202d 2048 6973 746f 6772 616d  1837 - Histogram
-00002fc0: 2e73 7667 3c2f 6963 6f6e 7365 743e 0d0a  .svg</iconset>..
-00002fd0: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-00002fe0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00002ff0: 653d 2274 6578 7422 3e0d 0a20 2020 203c  e="text">..    <
-00003000: 7374 7269 6e67 3e4d 6173 7320 4869 7374  string>Mass Hist
-00003010: 6f67 7261 6d3c 2f73 7472 696e 673e 0d0a  ogram</string>..
-00003020: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-00003030: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00003040: 653d 2274 6f6f 6c54 6970 223e 0d0a 2020  e="toolTip">..  
-00003050: 2020 3c73 7472 696e 673e 4869 7374 6f67    <string>Histog
-00003060: 7261 6d20 6f66 2049 6e74 656e 7369 7469  ram of Intensiti
-00003070: 6573 2066 6f72 2074 6865 2063 7572 7265  es for the curre
-00003080: 6e74 2066 7261 6d65 3c2f 7374 7269 6e67  nt frame</string
-00003090: 3e0d 0a20 2020 3c2f 7072 6f70 6572 7479  >..   </property
-000030a0: 3e0d 0a20 203c 2f61 6374 696f 6e3e 0d0a  >..  </action>..
-000030b0: 2020 3c61 6374 696f 6e20 6e61 6d65 3d22    <action name="
-000030c0: 6163 7469 6f6e 5f64 6174 615f 6672 616d  action_data_fram
-000030d0: 6522 3e0d 0a20 2020 3c70 726f 7065 7274  e">..   <propert
-000030e0: 7920 6e61 6d65 3d22 6963 6f6e 223e 0d0a  y name="icon">..
-000030f0: 2020 2020 3c69 636f 6e73 6574 3e0d 0a20      <iconset>.. 
-00003100: 2020 2020 3c6e 6f72 6d61 6c6f 6666 3e49      <normaloff>I
-00003110: 636f 6e73 2f31 3138 3331 202d 2046 6c75  cons/11831 - Flu
-00003120: 6964 204d 6563 6861 6e69 6373 2e73 7667  id Mechanics.svg
-00003130: 3c2f 6e6f 726d 616c 6f66 663e 4963 6f6e  </normaloff>Icon
-00003140: 732f 3131 3833 3120 2d20 466c 7569 6420  s/11831 - Fluid 
-00003150: 4d65 6368 616e 6963 732e 7376 673c 2f69  Mechanics.svg</i
-00003160: 636f 6e73 6574 3e0d 0a20 2020 3c2f 7072  conset>..   </pr
-00003170: 6f70 6572 7479 3e0d 0a20 2020 3c70 726f  operty>..   <pro
-00003180: 7065 7274 7920 6e61 6d65 3d22 7465 7874  perty name="text
-00003190: 223e 0d0a 2020 2020 3c73 7472 696e 673e  ">..    <string>
-000031a0: 5472 656e 6473 3c2f 7374 7269 6e67 3e0d  Trends</string>.
-000031b0: 0a20 2020 3c2f 7072 6f70 6572 7479 3e0d  .   </property>.
-000031c0: 0a20 2020 3c70 726f 7065 7274 7920 6e61  .   <property na
-000031d0: 6d65 3d22 746f 6f6c 5469 7022 3e0d 0a20  me="toolTip">.. 
-000031e0: 2020 203c 7374 7269 6e67 3e53 686f 7720     <string>Show 
-000031f0: 7472 656e 6473 206f 7665 7220 6672 616d  trends over fram
-00003200: 6573 3c2f 7374 7269 6e67 3e0d 0a20 2020  es</string>..   
-00003210: 3c2f 7072 6f70 6572 7479 3e0d 0a20 203c  </property>..  <
-00003220: 2f61 6374 696f 6e3e 0d0a 2020 3c61 6374  /action>..  <act
-00003230: 696f 6e20 6e61 6d65 3d22 6163 7469 6f6e  ion name="action
-00003240: 5f64 6174 615f 706c 6f74 7322 3e0d 0a20  _data_plots">.. 
-00003250: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00003260: 3d22 6963 6f6e 223e 0d0a 2020 2020 3c69  ="icon">..    <i
-00003270: 636f 6e73 6574 3e0d 0a20 2020 2020 3c6e  conset>..     <n
-00003280: 6f72 6d61 6c6f 6666 3e49 636f 6e73 2f31  ormaloff>Icons/1
-00003290: 3138 3632 202d 2057 6569 6768 7420 5363  1862 - Weight Sc
-000032a0: 616c 652e 7376 673c 2f6e 6f72 6d61 6c6f  ale.svg</normalo
-000032b0: 6666 3e49 636f 6e73 2f31 3138 3632 202d  ff>Icons/11862 -
-000032c0: 2057 6569 6768 7420 5363 616c 652e 7376   Weight Scale.sv
-000032d0: 673c 2f69 636f 6e73 6574 3e0d 0a20 2020  g</iconset>..   
-000032e0: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
-000032f0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00003300: 7465 7874 223e 0d0a 2020 2020 3c73 7472  text">..    <str
-00003310: 696e 673e 4d61 7373 3c2f 7374 7269 6e67  ing>Mass</string
-00003320: 3e0d 0a20 2020 3c2f 7072 6f70 6572 7479  >..   </property
-00003330: 3e0d 0a20 2020 3c70 726f 7065 7274 7920  >..   <property 
-00003340: 6e61 6d65 3d22 746f 6f6c 5469 7022 3e0d  name="toolTip">.
-00003350: 0a20 2020 203c 7374 7269 6e67 3e53 686f  .    <string>Sho
-00003360: 7720 696e 7465 6e73 6974 6965 7320 6f66  w intensities of
-00003370: 2061 6c6c 2074 6865 2063 616c 6375 6c61   all the calcula
-00003380: 7465 6420 7061 7274 6963 6c65 733c 2f73  ted particles</s
-00003390: 7472 696e 673e 0d0a 2020 203c 2f70 726f  tring>..   </pro
-000033a0: 7065 7274 793e 0d0a 2020 3c2f 6163 7469  perty>..  </acti
-000033b0: 6f6e 3e0d 0a20 203c 6163 7469 6f6e 206e  on>..  <action n
-000033c0: 616d 653d 2261 6374 696f 6e5f 7361 7665  ame="action_save
-000033d0: 5f64 6174 6122 3e0d 0a20 2020 3c70 726f  _data">..   <pro
-000033e0: 7065 7274 7920 6e61 6d65 3d22 6963 6f6e  perty name="icon
-000033f0: 223e 0d0a 2020 2020 3c69 636f 6e73 6574  ">..    <iconset
-00003400: 3e0d 0a20 2020 2020 3c6e 6f72 6d61 6c6f  >..     <normalo
-00003410: 6666 3e49 636f 6e73 2f53 6176 652e 7376  ff>Icons/Save.sv
-00003420: 673c 2f6e 6f72 6d61 6c6f 6666 3e49 636f  g</normaloff>Ico
-00003430: 6e73 2f53 6176 652e 7376 673c 2f69 636f  ns/Save.svg</ico
-00003440: 6e73 6574 3e0d 0a20 2020 3c2f 7072 6f70  nset>..   </prop
-00003450: 6572 7479 3e0d 0a20 2020 3c70 726f 7065  erty>..   <prope
-00003460: 7274 7920 6e61 6d65 3d22 7465 7874 223e  rty name="text">
-00003470: 0d0a 2020 2020 3c73 7472 696e 673e 4578  ..    <string>Ex
-00003480: 706f 7274 3c2f 7374 7269 6e67 3e0d 0a20  port</string>.. 
-00003490: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
-000034a0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-000034b0: 3d22 746f 6f6c 5469 7022 3e0d 0a20 2020  ="toolTip">..   
-000034c0: 203c 7374 7269 6e67 3e45 7870 6f72 7420   <string>Export 
-000034d0: 6461 7461 2074 6f20 4353 563c 2f73 7472  data to CSV</str
-000034e0: 696e 673e 0d0a 2020 203c 2f70 726f 7065  ing>..   </prope
-000034f0: 7274 793e 0d0a 2020 3c2f 6163 7469 6f6e  rty>..  </action
-00003500: 3e0d 0a20 203c 6163 7469 6f6e 206e 616d  >..  <action nam
-00003510: 653d 2261 6374 696f 6e41 6476 616e 6365  e="actionAdvance
-00003520: 5f46 7261 6d65 223e 0d0a 2020 203c 7072  _Frame">..   <pr
-00003530: 6f70 6572 7479 206e 616d 653d 2274 6578  operty name="tex
-00003540: 7422 3e0d 0a20 2020 203c 7374 7269 6e67  t">..    <string
-00003550: 3e49 6e63 7265 6173 6520 4672 616d 653c  >Increase Frame<
-00003560: 2f73 7472 696e 673e 0d0a 2020 203c 2f70  /string>..   </p
-00003570: 726f 7065 7274 793e 0d0a 2020 203c 7072  roperty>..   <pr
-00003580: 6f70 6572 7479 206e 616d 653d 2273 686f  operty name="sho
-00003590: 7274 6375 7422 3e0d 0a20 2020 203c 7374  rtcut">..    <st
-000035a0: 7269 6e67 3e4d 6574 612b 416c 742b 5269  ring>Meta+Alt+Ri
-000035b0: 6768 743c 2f73 7472 696e 673e 0d0a 2020  ght</string>..  
-000035c0: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
-000035d0: 3c2f 6163 7469 6f6e 3e0d 0a20 203c 6163  </action>..  <ac
-000035e0: 7469 6f6e 206e 616d 653d 2261 6374 696f  tion name="actio
-000035f0: 6e44 6563 7265 6173 655f 4672 616d 6522  nDecrease_Frame"
-00003600: 3e0d 0a20 2020 3c70 726f 7065 7274 7920  >..   <property 
-00003610: 6e61 6d65 3d22 7465 7874 223e 0d0a 2020  name="text">..  
-00003620: 2020 3c73 7472 696e 673e 4465 6372 6561    <string>Decrea
-00003630: 7365 2046 7261 6d65 3c2f 7374 7269 6e67  se Frame</string
-00003640: 3e0d 0a20 2020 3c2f 7072 6f70 6572 7479  >..   </property
-00003650: 3e0d 0a20 2020 3c70 726f 7065 7274 7920  >..   <property 
-00003660: 6e61 6d65 3d22 7368 6f72 7463 7574 223e  name="shortcut">
-00003670: 0d0a 2020 2020 3c73 7472 696e 673e 4d65  ..    <string>Me
-00003680: 7461 2b41 6c74 2b4c 6566 743c 2f73 7472  ta+Alt+Left</str
-00003690: 696e 673e 0d0a 2020 203c 2f70 726f 7065  ing>..   </prope
-000036a0: 7274 793e 0d0a 2020 3c2f 6163 7469 6f6e  rty>..  </action
-000036b0: 3e0d 0a20 203c 6163 7469 6f6e 206e 616d  >..  <action nam
-000036c0: 653d 2261 6374 696f 6e47 6f5f 746f 5f64  e="actionGo_to_d
-000036d0: 6f63 756d 656e 7461 7469 6f6e 223e 0d0a  ocumentation">..
-000036e0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000036f0: 653d 2274 6578 7422 3e0d 0a20 2020 203c  e="text">..    <
-00003700: 7374 7269 6e67 3e4f 7065 6e20 446f 6375  string>Open Docu
-00003710: 6d65 6e74 6174 696f 6e3c 2f73 7472 696e  mentation</strin
-00003720: 673e 0d0a 2020 203c 2f70 726f 7065 7274  g>..   </propert
-00003730: 793e 0d0a 2020 3c2f 6163 7469 6f6e 3e0d  y>..  </action>.
-00003740: 0a20 203c 6163 7469 6f6e 206e 616d 653d  .  <action name=
-00003750: 2261 6374 696f 6e5f 6578 706f 7274 5f61  "action_export_a
-00003760: 6c6c 5f64 6174 6122 3e0d 0a20 2020 3c70  ll_data">..   <p
-00003770: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
-00003780: 7874 223e 0d0a 2020 2020 3c73 7472 696e  xt">..    <strin
-00003790: 673e 4578 706f 7274 2041 6c6c 2044 6174  g>Export All Dat
-000037a0: 613c 2f73 7472 696e 673e 0d0a 2020 203c  a</string>..   <
-000037b0: 2f70 726f 7065 7274 793e 0d0a 2020 203c  /property>..   <
-000037c0: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
-000037d0: 6f6f 6c54 6970 223e 0d0a 2020 2020 3c73  oolTip">..    <s
-000037e0: 7472 696e 673e 4578 706f 7274 2061 6c6c  tring>Export all
-000037f0: 2074 6865 2069 6e66 6f72 6d61 7469 6f6e   the information
-00003800: 2067 6174 6865 7265 6420 6f6e 2070 6172   gathered on par
-00003810: 7469 636c 6573 3c2f 7374 7269 6e67 3e0d  ticles</string>.
-00003820: 0a20 2020 3c2f 7072 6f70 6572 7479 3e0d  .   </property>.
-00003830: 0a20 203c 2f61 6374 696f 6e3e 0d0a 2020  .  </action>..  
-00003840: 3c61 6374 696f 6e20 6e61 6d65 3d22 6163  <action name="ac
-00003850: 7469 6f6e 5f61 626f 7574 223e 0d0a 2020  tion_about">..  
-00003860: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00003870: 2274 6578 7422 3e0d 0a20 2020 203c 7374  "text">..    <st
-00003880: 7269 6e67 3e41 626f 7574 3c2f 7374 7269  ring>About</stri
-00003890: 6e67 3e0d 0a20 2020 3c2f 7072 6f70 6572  ng>..   </proper
-000038a0: 7479 3e0d 0a20 2020 3c70 726f 7065 7274  ty>..   <propert
-000038b0: 7920 6e61 6d65 3d22 746f 6f6c 5469 7022  y name="toolTip"
-000038c0: 3e0d 0a20 2020 203c 7374 7269 6e67 3e41  >..    <string>A
-000038d0: 626f 7574 204e 616e 6f51 4e54 5079 3c2f  bout NanoQNTPy</
-000038e0: 7374 7269 6e67 3e0d 0a20 2020 3c2f 7072  string>..   </pr
-000038f0: 6f70 6572 7479 3e0d 0a20 203c 2f61 6374  operty>..  </act
-00003900: 696f 6e3e 0d0a 2020 3c61 6374 696f 6e20  ion>..  <action 
-00003910: 6e61 6d65 3d22 6163 7469 6f6e 5f63 616c  name="action_cal
-00003920: 6375 6c61 7465 5f62 6b67 223e 0d0a 2020  culate_bkg">..  
-00003930: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00003940: 2274 6578 7422 3e0d 0a20 2020 203c 7374  "text">..    <st
-00003950: 7269 6e67 3e43 616c 6375 6c61 7465 2042  ring>Calculate B
-00003960: 6163 6b67 726f 756e 643c 2f73 7472 696e  ackground</strin
-00003970: 673e 0d0a 2020 203c 2f70 726f 7065 7274  g>..   </propert
-00003980: 793e 0d0a 2020 3c2f 6163 7469 6f6e 3e0d  y>..  </action>.
-00003990: 0a20 203c 6163 7469 6f6e 206e 616d 653d  .  <action name=
-000039a0: 2261 6374 696f 6e5f 7368 6f77 5f62 6b67  "action_show_bkg
-000039b0: 223e 0d0a 2020 203c 7072 6f70 6572 7479  ">..   <property
-000039c0: 206e 616d 653d 2274 6578 7422 3e0d 0a20   name="text">.. 
-000039d0: 2020 203c 7374 7269 6e67 3e53 686f 7720     <string>Show 
-000039e0: 4261 636b 6772 6f75 6e64 3c2f 7374 7269  Background</stri
-000039f0: 6e67 3e0d 0a20 2020 3c2f 7072 6f70 6572  ng>..   </proper
-00003a00: 7479 3e0d 0a20 203c 2f61 6374 696f 6e3e  ty>..  </action>
-00003a10: 0d0a 203c 2f77 6964 6765 743e 0d0a 203c  .. </widget>.. <
-00003a20: 7461 6273 746f 7073 3e0d 0a20 203c 7461  tabstops>..  <ta
-00003a30: 6273 746f 703e 6669 6e64 5f70 6172 7469  bstop>find_parti
-00003a40: 636c 6573 5f63 6865 636b 3c2f 7461 6273  cles_check</tabs
-00003a50: 746f 703e 0d0a 2020 3c74 6162 7374 6f70  top>..  <tabstop
-00003a60: 3e73 7461 7274 5f66 7261 6d65 5f6c 696e  >start_frame_lin
-00003a70: 653c 2f74 6162 7374 6f70 3e0d 0a20 203c  e</tabstop>..  <
-00003a80: 7461 6273 746f 703e 656e 645f 6672 616d  tabstop>end_fram
-00003a90: 655f 6c69 6e65 3c2f 7461 6273 746f 703e  e_line</tabstop>
-00003aa0: 0d0a 2020 3c74 6162 7374 6f70 3e65 6e67  ..  <tabstop>eng
-00003ab0: 696e 655f 626f 783c 2f74 6162 7374 6f70  ine_box</tabstop
-00003ac0: 3e0d 0a20 203c 7461 6273 746f 703e 7365  >..  <tabstop>se
-00003ad0: 6172 6368 5f72 6164 6975 735f 6c69 6e65  arch_radius_line
-00003ae0: 3c2f 7461 6273 746f 703e 0d0a 2020 3c74  </tabstop>..  <t
-00003af0: 6162 7374 6f70 3e6d 696e 5f66 7261 6d65  abstop>min_frame
-00003b00: 735f 6c69 6e65 3c2f 7461 6273 746f 703e  s_line</tabstop>
-00003b10: 0d0a 2020 3c74 6162 7374 6f70 3e63 616c  ..  <tabstop>cal
-00003b20: 6375 6c61 7465 5f62 7574 746f 6e3c 2f74  culate_button</t
-00003b30: 6162 7374 6f70 3e0d 0a20 203c 7461 6273  abstop>..  <tabs
-00003b40: 746f 703e 7374 6570 5f73 697a 655f 6c69  top>step_size_li
-00003b50: 6e65 3c2f 7461 6273 746f 703e 0d0a 2020  ne</tabstop>..  
-00003b60: 3c74 6162 7374 6f70 3e66 7261 6d65 5f73  <tabstop>frame_s
-00003b70: 6c69 6465 723c 2f74 6162 7374 6f70 3e0d  lider</tabstop>.
-00003b80: 0a20 3c2f 7461 6273 746f 7073 3e0d 0a20  . </tabstops>.. 
-00003b90: 3c72 6573 6f75 7263 6573 3e0d 0a20 203c  <resources>..  <
-00003ba0: 696e 636c 7564 6520 6c6f 6361 7469 6f6e  include location
-00003bb0: 3d22 4963 6f6e 732f 4963 6f6e 732e 7172  ="Icons/Icons.qr
-00003bc0: 6322 2f3e 0d0a 203c 2f72 6573 6f75 7263  c"/>.. </resourc
-00003bd0: 6573 3e0d 0a20 3c63 6f6e 6e65 6374 696f  es>.. <connectio
-00003be0: 6e73 2f3e 0d0a 3c2f 7569 3e0d 0a         ns/>..</ui>..
+00000020: 462d 3822 3f3e 0a3c 7569 2076 6572 7369  F-8"?>.<ui versi
+00000030: 6f6e 3d22 342e 3022 3e0a 203c 636c 6173  on="4.0">. <clas
+00000040: 733e 4d61 696e 5769 6e64 6f77 3c2f 636c  s>MainWindow</cl
+00000050: 6173 733e 0a20 3c77 6964 6765 7420 636c  ass>. <widget cl
+00000060: 6173 733d 2251 4d61 696e 5769 6e64 6f77  ass="QMainWindow
+00000070: 2220 6e61 6d65 3d22 4d61 696e 5769 6e64  " name="MainWind
+00000080: 6f77 223e 0a20 203c 7072 6f70 6572 7479  ow">.  <property
+00000090: 206e 616d 653d 2267 656f 6d65 7472 7922   name="geometry"
+000000a0: 3e0a 2020 203c 7265 6374 3e0a 2020 2020  >.   <rect>.    
+000000b0: 3c78 3e30 3c2f 783e 0a20 2020 203c 793e  <x>0</x>.    <y>
+000000c0: 303c 2f79 3e0a 2020 2020 3c77 6964 7468  0</y>.    <width
+000000d0: 3e37 3638 3c2f 7769 6474 683e 0a20 2020  >768</width>.   
+000000e0: 203c 6865 6967 6874 3e36 3431 3c2f 6865   <height>641</he
+000000f0: 6967 6874 3e0a 2020 203c 2f72 6563 743e  ight>.   </rect>
+00000100: 0a20 203c 2f70 726f 7065 7274 793e 0a20  .  </property>. 
+00000110: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000120: 2277 696e 646f 7754 6974 6c65 223e 0a20  "windowTitle">. 
+00000130: 2020 3c73 7472 696e 673e 4e61 6e6f 514e    <string>NanoQN
+00000140: 5420 4461 7461 2041 6e61 6c79 7369 733c  T Data Analysis<
+00000150: 2f73 7472 696e 673e 0a20 203c 2f70 726f  /string>.  </pro
+00000160: 7065 7274 793e 0a20 203c 7072 6f70 6572  perty>.  <proper
+00000170: 7479 206e 616d 653d 2275 6e69 6669 6564  ty name="unified
+00000180: 5469 746c 6541 6e64 546f 6f6c 4261 724f  TitleAndToolBarO
+00000190: 6e4d 6163 223e 0a20 2020 3c62 6f6f 6c3e  nMac">.   <bool>
+000001a0: 7472 7565 3c2f 626f 6f6c 3e0a 2020 3c2f  true</bool>.  </
+000001b0: 7072 6f70 6572 7479 3e0a 2020 3c77 6964  property>.  <wid
+000001c0: 6765 7420 636c 6173 733d 2251 5769 6467  get class="QWidg
+000001d0: 6574 2220 6e61 6d65 3d22 6365 6e74 7261  et" name="centra
+000001e0: 6c77 6964 6765 7422 3e0a 2020 203c 6c61  lwidget">.   <la
+000001f0: 796f 7574 2063 6c61 7373 3d22 5148 426f  yout class="QHBo
+00000200: 784c 6179 6f75 7422 206e 616d 653d 2268  xLayout" name="h
+00000210: 6f72 697a 6f6e 7461 6c4c 6179 6f75 7422  orizontalLayout"
+00000220: 3e0a 2020 2020 3c69 7465 6d3e 0a20 2020  >.    <item>.   
+00000230: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
+00000240: 2251 5769 6467 6574 2220 6e61 6d65 3d22  "QWidget" name="
+00000250: 7365 7474 696e 6773 5f77 6964 6765 7422  settings_widget"
+00000260: 206e 6174 6976 653d 2274 7275 6522 3e0a   native="true">.
+00000270: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00000280: 6e61 6d65 3d22 7369 7a65 506f 6c69 6379  name="sizePolicy
+00000290: 223e 0a20 2020 2020 2020 3c73 697a 6570  ">.       <sizep
+000002a0: 6f6c 6963 7920 6873 697a 6574 7970 653d  olicy hsizetype=
+000002b0: 224d 696e 696d 756d 2220 7673 697a 6574  "Minimum" vsizet
+000002c0: 7970 653d 2250 7265 6665 7272 6564 223e  ype="Preferred">
+000002d0: 0a20 2020 2020 2020 203c 686f 7273 7472  .        <horstr
+000002e0: 6574 6368 3e30 3c2f 686f 7273 7472 6574  etch>0</horstret
+000002f0: 6368 3e0a 2020 2020 2020 2020 3c76 6572  ch>.        <ver
+00000300: 7374 7265 7463 683e 303c 2f76 6572 7374  stretch>0</verst
+00000310: 7265 7463 683e 0a20 2020 2020 2020 3c2f  retch>.       </
+00000320: 7369 7a65 706f 6c69 6379 3e0a 2020 2020  sizepolicy>.    
+00000330: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+00000340: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00000350: 6d65 3d22 6d61 7869 6d75 6d53 697a 6522  me="maximumSize"
+00000360: 3e0a 2020 2020 2020 203c 7369 7a65 3e0a  >.       <size>.
+00000370: 2020 2020 2020 2020 3c77 6964 7468 3e32          <width>2
+00000380: 3235 3c2f 7769 6474 683e 0a20 2020 2020  25</width>.     
+00000390: 2020 203c 6865 6967 6874 3e31 3637 3737     <height>16777
+000003a0: 3231 353c 2f68 6569 6768 743e 0a20 2020  215</height>.   
+000003b0: 2020 2020 3c2f 7369 7a65 3e0a 2020 2020      </size>.    
+000003c0: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+000003d0: 2020 2020 3c6c 6179 6f75 7420 636c 6173      <layout clas
+000003e0: 733d 2251 466f 726d 4c61 796f 7574 2220  s="QFormLayout" 
+000003f0: 6e61 6d65 3d22 666f 726d 4c61 796f 7574  name="formLayout
+00000400: 223e 0a20 2020 2020 2020 3c70 726f 7065  ">.       <prope
+00000410: 7274 7920 6e61 6d65 3d22 6c65 6674 4d61  rty name="leftMa
+00000420: 7267 696e 223e 0a20 2020 2020 2020 203c  rgin">.        <
+00000430: 6e75 6d62 6572 3e30 3c2f 6e75 6d62 6572  number>0</number
+00000440: 3e0a 2020 2020 2020 203c 2f70 726f 7065  >.       </prope
+00000450: 7274 793e 0a20 2020 2020 2020 3c70 726f  rty>.       <pro
+00000460: 7065 7274 7920 6e61 6d65 3d22 746f 704d  perty name="topM
+00000470: 6172 6769 6e22 3e0a 2020 2020 2020 2020  argin">.        
+00000480: 3c6e 756d 6265 723e 303c 2f6e 756d 6265  <number>0</numbe
+00000490: 723e 0a20 2020 2020 2020 3c2f 7072 6f70  r>.       </prop
+000004a0: 6572 7479 3e0a 2020 2020 2020 203c 7072  erty>.       <pr
+000004b0: 6f70 6572 7479 206e 616d 653d 2272 6967  operty name="rig
+000004c0: 6874 4d61 7267 696e 223e 0a20 2020 2020  htMargin">.     
+000004d0: 2020 203c 6e75 6d62 6572 3e30 3c2f 6e75     <number>0</nu
+000004e0: 6d62 6572 3e0a 2020 2020 2020 203c 2f70  mber>.       </p
+000004f0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00000500: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00000510: 626f 7474 6f6d 4d61 7267 696e 223e 0a20  bottomMargin">. 
+00000520: 2020 2020 2020 203c 6e75 6d62 6572 3e30         <number>0
+00000530: 3c2f 6e75 6d62 6572 3e0a 2020 2020 2020  </number>.      
+00000540: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+00000550: 2020 2020 3c69 7465 6d20 726f 773d 2230      <item row="0
+00000560: 2220 636f 6c75 6d6e 3d22 3022 2063 6f6c  " column="0" col
+00000570: 7370 616e 3d22 3222 3e0a 2020 2020 2020  span="2">.      
+00000580: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
+00000590: 2251 4368 6563 6b42 6f78 2220 6e61 6d65  "QCheckBox" name
+000005a0: 3d22 6669 6e64 5f70 6172 7469 636c 6573  ="find_particles
+000005b0: 5f63 6865 636b 223e 0a20 2020 2020 2020  _check">.       
+000005c0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+000005d0: 3d22 746f 6f6c 5469 7022 3e0a 2020 2020  ="toolTip">.    
+000005e0: 2020 2020 2020 3c73 7472 696e 673e 266c        <string>&l
+000005f0: 743b 6874 6d6c 2667 743b 266c 743b 6865  t;html&gt;&lt;he
+00000600: 6164 2f26 6774 3b26 6c74 3b62 6f64 7926  ad/&gt;&lt;body&
+00000610: 6774 3b26 6c74 3b70 2667 743b 5768 6574  gt;&lt;p&gt;Whet
+00000620: 6865 7220 746f 206d 6172 6b20 7468 6520  her to mark the 
+00000630: 7061 7274 6963 6c65 7320 6f6e 2074 6865  particles on the
+00000640: 2069 6d61 6765 7326 6c74 3b2f 7026 6774   images&lt;/p&gt
+00000650: 3b26 6c74 3b2f 626f 6479 2667 743b 266c  ;&lt;/body&gt;&l
+00000660: 743b 2f68 746d 6c26 6774 3b3c 2f73 7472  t;/html&gt;</str
+00000670: 696e 673e 0a20 2020 2020 2020 2020 3c2f  ing>.         </
+00000680: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00000690: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+000006a0: 653d 2274 6578 7422 3e0a 2020 2020 2020  e="text">.      
+000006b0: 2020 2020 3c73 7472 696e 673e 4669 6e64      <string>Find
+000006c0: 2050 6172 7469 636c 6573 3c2f 7374 7269   Particles</stri
+000006d0: 6e67 3e0a 2020 2020 2020 2020 203c 2f70  ng>.         </p
+000006e0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+000006f0: 203c 2f77 6964 6765 743e 0a20 2020 2020   </widget>.     
+00000700: 2020 3c2f 6974 656d 3e0a 2020 2020 2020    </item>.      
+00000710: 203c 6974 656d 2072 6f77 3d22 3122 2063   <item row="1" c
+00000720: 6f6c 756d 6e3d 2230 223e 0a20 2020 2020  olumn="0">.     
+00000730: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
+00000740: 3d22 514c 6162 656c 2220 6e61 6d65 3d22  ="QLabel" name="
+00000750: 6c61 6265 6c5f 3922 3e0a 2020 2020 2020  label_9">.      
+00000760: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00000770: 653d 2274 6578 7422 3e0a 2020 2020 2020  e="text">.      
+00000780: 2020 2020 3c73 7472 696e 673e 4672 616d      <string>Fram
+00000790: 6520 5261 6e67 653c 2f73 7472 696e 673e  e Range</string>
+000007a0: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
+000007b0: 6572 7479 3e0a 2020 2020 2020 2020 203c  erty>.         <
+000007c0: 7072 6f70 6572 7479 206e 616d 653d 2262  property name="b
+000007d0: 7564 6479 223e 0a20 2020 2020 2020 2020  uddy">.         
+000007e0: 203c 6373 7472 696e 673e 7374 6172 745f   <cstring>start_
+000007f0: 6672 616d 655f 6c69 6e65 3c2f 6373 7472  frame_line</cstr
+00000800: 696e 673e 0a20 2020 2020 2020 2020 3c2f  ing>.         </
+00000810: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00000820: 2020 3c2f 7769 6467 6574 3e0a 2020 2020    </widget>.    
+00000830: 2020 203c 2f69 7465 6d3e 0a20 2020 2020     </item>.     
+00000840: 2020 3c69 7465 6d20 726f 773d 2231 2220    <item row="1" 
+00000850: 636f 6c75 6d6e 3d22 3122 3e0a 2020 2020  column="1">.    
+00000860: 2020 2020 3c77 6964 6765 7420 636c 6173      <widget clas
+00000870: 733d 2251 4c69 6e65 4564 6974 2220 6e61  s="QLineEdit" na
+00000880: 6d65 3d22 7374 6172 745f 6672 616d 655f  me="start_frame_
+00000890: 6c69 6e65 223e 0a20 2020 2020 2020 2020  line">.         
+000008a0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+000008b0: 746f 6f6c 5469 7022 3e0a 2020 2020 2020  toolTip">.      
+000008c0: 2020 2020 3c73 7472 696e 673e 5374 6172      <string>Star
+000008d0: 7420 4672 616d 653c 2f73 7472 696e 673e  t Frame</string>
+000008e0: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
+000008f0: 6572 7479 3e0a 2020 2020 2020 2020 203c  erty>.         <
+00000900: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
+00000910: 6578 7422 3e0a 2020 2020 2020 2020 2020  ext">.          
+00000920: 3c73 7472 696e 673e 303c 2f73 7472 696e  <string>0</strin
+00000930: 673e 0a20 2020 2020 2020 2020 3c2f 7072  g>.         </pr
+00000940: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00000950: 3c2f 7769 6467 6574 3e0a 2020 2020 2020  </widget>.      
+00000960: 203c 2f69 7465 6d3e 0a20 2020 2020 2020   </item>.       
+00000970: 3c69 7465 6d20 726f 773d 2232 2220 636f  <item row="2" co
+00000980: 6c75 6d6e 3d22 3122 3e0a 2020 2020 2020  lumn="1">.      
+00000990: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
+000009a0: 2251 4c69 6e65 4564 6974 2220 6e61 6d65  "QLineEdit" name
+000009b0: 3d22 656e 645f 6672 616d 655f 6c69 6e65  ="end_frame_line
+000009c0: 223e 0a20 2020 2020 2020 2020 3c70 726f  ">.         <pro
+000009d0: 7065 7274 7920 6e61 6d65 3d22 746f 6f6c  perty name="tool
+000009e0: 5469 7022 3e0a 2020 2020 2020 2020 2020  Tip">.          
+000009f0: 3c73 7472 696e 673e 456e 6420 4672 616d  <string>End Fram
+00000a00: 653c 2f73 7472 696e 673e 0a20 2020 2020  e</string>.     
+00000a10: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
+00000a20: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00000a30: 7479 206e 616d 653d 2274 6578 7422 3e0a  ty name="text">.
+00000a40: 2020 2020 2020 2020 2020 3c73 7472 696e            <strin
+00000a50: 673e 2d31 3c2f 7374 7269 6e67 3e0a 2020  g>-1</string>.  
+00000a60: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+00000a70: 793e 0a20 2020 2020 2020 203c 2f77 6964  y>.        </wid
+00000a80: 6765 743e 0a20 2020 2020 2020 3c2f 6974  get>.       </it
+00000a90: 656d 3e0a 2020 2020 2020 203c 6974 656d  em>.       <item
+00000aa0: 2072 6f77 3d22 3322 2063 6f6c 756d 6e3d   row="3" column=
+00000ab0: 2230 223e 0a20 2020 2020 2020 203c 7769  "0">.        <wi
+00000ac0: 6467 6574 2063 6c61 7373 3d22 514c 6162  dget class="QLab
+00000ad0: 656c 2220 6e61 6d65 3d22 6c61 6265 6c5f  el" name="label_
+00000ae0: 3322 3e0a 2020 2020 2020 2020 203c 7072  3">.         <pr
+00000af0: 6f70 6572 7479 206e 616d 653d 2274 6578  operty name="tex
+00000b00: 7422 3e0a 2020 2020 2020 2020 2020 3c73  t">.          <s
+00000b10: 7472 696e 673e 456e 6769 6e65 3c2f 7374  tring>Engine</st
+00000b20: 7269 6e67 3e0a 2020 2020 2020 2020 203c  ring>.         <
+00000b30: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+00000b40: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00000b50: 6d65 3d22 6275 6464 7922 3e0a 2020 2020  me="buddy">.    
+00000b60: 2020 2020 2020 3c63 7374 7269 6e67 3e65        <cstring>e
+00000b70: 6e67 696e 655f 626f 783c 2f63 7374 7269  ngine_box</cstri
+00000b80: 6e67 3e0a 2020 2020 2020 2020 203c 2f70  ng>.         </p
+00000b90: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00000ba0: 203c 2f77 6964 6765 743e 0a20 2020 2020   </widget>.     
+00000bb0: 2020 3c2f 6974 656d 3e0a 2020 2020 2020    </item>.      
+00000bc0: 203c 6974 656d 2072 6f77 3d22 3322 2063   <item row="3" c
+00000bd0: 6f6c 756d 6e3d 2231 223e 0a20 2020 2020  olumn="1">.     
+00000be0: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
+00000bf0: 3d22 5143 6f6d 626f 426f 7822 206e 616d  ="QComboBox" nam
+00000c00: 653d 2265 6e67 696e 655f 626f 7822 3e0a  e="engine_box">.
+00000c10: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00000c20: 7479 206e 616d 653d 2274 6f6f 6c54 6970  ty name="toolTip
+00000c30: 223e 0a20 2020 2020 2020 2020 203c 7374  ">.          <st
+00000c40: 7269 6e67 3e26 6c74 3b68 746d 6c26 6774  ring>&lt;html&gt
+00000c50: 3b26 6c74 3b68 6561 642f 2667 743b 266c  ;&lt;head/&gt;&l
+00000c60: 743b 626f 6479 2667 743b 266c 743b 7026  t;body&gt;&lt;p&
+00000c70: 6774 3b49 6620 696e 7374 616c 6c65 642c  gt;If installed,
+00000c80: 206e 756d 6261 2069 7320 7072 6566 6572   numba is prefer
+00000c90: 7265 6426 6c74 3b2f 7026 6774 3b26 6c74  red&lt;/p&gt;&lt
+00000ca0: 3b2f 626f 6479 2667 743b 266c 743b 2f68  ;/body&gt;&lt;/h
+00000cb0: 746d 6c26 6774 3b3c 2f73 7472 696e 673e  tml&gt;</string>
+00000cc0: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
+00000cd0: 6572 7479 3e0a 2020 2020 2020 2020 203c  erty>.         <
+00000ce0: 6974 656d 3e0a 2020 2020 2020 2020 2020  item>.          
+00000cf0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00000d00: 7465 7874 223e 0a20 2020 2020 2020 2020  text">.         
+00000d10: 2020 3c73 7472 696e 673e 6d61 736b 3c2f    <string>mask</
+00000d20: 7374 7269 6e67 3e0a 2020 2020 2020 2020  string>.        
+00000d30: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+00000d40: 2020 2020 2020 203c 2f69 7465 6d3e 0a20         </item>. 
+00000d50: 2020 2020 2020 2020 3c69 7465 6d3e 0a20          <item>. 
+00000d60: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00000d70: 7479 206e 616d 653d 2274 6578 7422 3e0a  ty name="text">.
+00000d80: 2020 2020 2020 2020 2020 203c 7374 7269             <stri
+00000d90: 6e67 3e6e 756d 6261 3c2f 7374 7269 6e67  ng>numba</string
+00000da0: 3e0a 2020 2020 2020 2020 2020 3c2f 7072  >.          </pr
+00000db0: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00000dc0: 203c 2f69 7465 6d3e 0a20 2020 2020 2020   </item>.       
+00000dd0: 2020 3c69 7465 6d3e 0a20 2020 2020 2020    <item>.       
+00000de0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00000df0: 653d 2274 6578 7422 3e0a 2020 2020 2020  e="text">.      
+00000e00: 2020 2020 203c 7374 7269 6e67 3e70 7974       <string>pyt
+00000e10: 686f 6e3c 2f73 7472 696e 673e 0a20 2020  hon</string>.   
+00000e20: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+00000e30: 793e 0a20 2020 2020 2020 2020 3c2f 6974  y>.         </it
+00000e40: 656d 3e0a 2020 2020 2020 2020 3c2f 7769  em>.        </wi
+00000e50: 6467 6574 3e0a 2020 2020 2020 203c 2f69  dget>.       </i
+00000e60: 7465 6d3e 0a20 2020 2020 2020 3c69 7465  tem>.       <ite
+00000e70: 6d20 726f 773d 2235 2220 636f 6c75 6d6e  m row="5" column
+00000e80: 3d22 3022 3e0a 2020 2020 2020 2020 3c77  ="0">.        <w
+00000e90: 6964 6765 7420 636c 6173 733d 2251 4c61  idget class="QLa
+00000ea0: 6265 6c22 206e 616d 653d 226c 6162 656c  bel" name="label
+00000eb0: 5f34 223e 0a20 2020 2020 2020 2020 3c70  _4">.         <p
+00000ec0: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
+00000ed0: 7874 223e 0a20 2020 2020 2020 2020 203c  xt">.          <
+00000ee0: 7374 7269 6e67 3e53 6561 7263 6820 7261  string>Search ra
+00000ef0: 6469 7573 3c2f 7374 7269 6e67 3e0a 2020  dius</string>.  
+00000f00: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+00000f10: 793e 0a20 2020 2020 2020 2020 3c70 726f  y>.         <pro
+00000f20: 7065 7274 7920 6e61 6d65 3d22 6275 6464  perty name="budd
+00000f30: 7922 3e0a 2020 2020 2020 2020 2020 3c63  y">.          <c
+00000f40: 7374 7269 6e67 3e73 6561 7263 685f 7261  string>search_ra
+00000f50: 6469 7573 5f6c 696e 653c 2f63 7374 7269  dius_line</cstri
+00000f60: 6e67 3e0a 2020 2020 2020 2020 203c 2f70  ng>.         </p
+00000f70: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00000f80: 203c 2f77 6964 6765 743e 0a20 2020 2020   </widget>.     
+00000f90: 2020 3c2f 6974 656d 3e0a 2020 2020 2020    </item>.      
+00000fa0: 203c 6974 656d 2072 6f77 3d22 3522 2063   <item row="5" c
+00000fb0: 6f6c 756d 6e3d 2231 223e 0a20 2020 2020  olumn="1">.     
+00000fc0: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
+00000fd0: 3d22 514c 696e 6545 6469 7422 206e 616d  ="QLineEdit" nam
+00000fe0: 653d 2273 6561 7263 685f 7261 6469 7573  e="search_radius
+00000ff0: 5f6c 696e 6522 3e0a 2020 2020 2020 2020  _line">.        
+00001000: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00001010: 2274 6f6f 6c54 6970 223e 0a20 2020 2020  "toolTip">.     
+00001020: 2020 2020 203c 7374 7269 6e67 3e26 6c74       <string>&lt
+00001030: 3b68 746d 6c26 6774 3b26 6c74 3b68 6561  ;html&gt;&lt;hea
+00001040: 642f 2667 743b 266c 743b 626f 6479 2667  d/&gt;&lt;body&g
+00001050: 743b 266c 743b 7026 6774 3b53 6561 7263  t;&lt;p&gt;Searc
+00001060: 6820 7261 6469 7573 2066 6f72 2074 6865  h radius for the
+00001070: 206c 696e 6b69 6e67 2070 726f 6365 6475   linking procedu
+00001080: 7265 266c 743b 2f70 2667 743b 266c 743b  re&lt;/p&gt;&lt;
+00001090: 2f62 6f64 7926 6774 3b26 6c74 3b2f 6874  /body&gt;&lt;/ht
+000010a0: 6d6c 2667 743b 3c2f 7374 7269 6e67 3e0a  ml&gt;</string>.
+000010b0: 2020 2020 2020 2020 203c 2f70 726f 7065           </prope
+000010c0: 7274 793e 0a20 2020 2020 2020 2020 3c70  rty>.         <p
+000010d0: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
+000010e0: 7874 223e 0a20 2020 2020 2020 2020 203c  xt">.          <
+000010f0: 7374 7269 6e67 3e35 3c2f 7374 7269 6e67  string>5</string
+00001100: 3e0a 2020 2020 2020 2020 203c 2f70 726f  >.         </pro
+00001110: 7065 7274 793e 0a20 2020 2020 2020 203c  perty>.        <
+00001120: 2f77 6964 6765 743e 0a20 2020 2020 2020  /widget>.       
+00001130: 3c2f 6974 656d 3e0a 2020 2020 2020 203c  </item>.       <
+00001140: 6974 656d 2072 6f77 3d22 3622 2063 6f6c  item row="6" col
+00001150: 756d 6e3d 2230 223e 0a20 2020 2020 2020  umn="0">.       
+00001160: 203c 7769 6467 6574 2063 6c61 7373 3d22   <widget class="
+00001170: 514c 6162 656c 2220 6e61 6d65 3d22 6c61  QLabel" name="la
+00001180: 6265 6c5f 3622 3e0a 2020 2020 2020 2020  bel_6">.        
+00001190: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+000011a0: 2274 6578 7422 3e0a 2020 2020 2020 2020  "text">.        
+000011b0: 2020 3c73 7472 696e 673e 4d69 6e20 4672    <string>Min Fr
+000011c0: 616d 6573 3c2f 7374 7269 6e67 3e0a 2020  ames</string>.  
+000011d0: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+000011e0: 793e 0a20 2020 2020 2020 2020 3c70 726f  y>.         <pro
+000011f0: 7065 7274 7920 6e61 6d65 3d22 6275 6464  perty name="budd
+00001200: 7922 3e0a 2020 2020 2020 2020 2020 3c63  y">.          <c
+00001210: 7374 7269 6e67 3e6d 696e 5f66 7261 6d65  string>min_frame
+00001220: 735f 6c69 6e65 3c2f 6373 7472 696e 673e  s_line</cstring>
+00001230: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
+00001240: 6572 7479 3e0a 2020 2020 2020 2020 3c2f  erty>.        </
+00001250: 7769 6467 6574 3e0a 2020 2020 2020 203c  widget>.       <
+00001260: 2f69 7465 6d3e 0a20 2020 2020 2020 3c69  /item>.       <i
+00001270: 7465 6d20 726f 773d 2236 2220 636f 6c75  tem row="6" colu
+00001280: 6d6e 3d22 3122 3e0a 2020 2020 2020 2020  mn="1">.        
+00001290: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
+000012a0: 4c69 6e65 4564 6974 2220 6e61 6d65 3d22  LineEdit" name="
+000012b0: 6d69 6e5f 6672 616d 6573 5f6c 696e 6522  min_frames_line"
+000012c0: 3e0a 2020 2020 2020 2020 203c 7072 6f70  >.         <prop
+000012d0: 6572 7479 206e 616d 653d 2274 6f6f 6c54  erty name="toolT
+000012e0: 6970 223e 0a20 2020 2020 2020 2020 203c  ip">.          <
+000012f0: 7374 7269 6e67 3e26 6c74 3b68 746d 6c26  string>&lt;html&
+00001300: 6774 3b26 6c74 3b68 6561 642f 2667 743b  gt;&lt;head/&gt;
+00001310: 266c 743b 626f 6479 2667 743b 266c 743b  &lt;body&gt;&lt;
+00001320: 7026 6774 3b4d 696e 696d 756d 206e 756d  p&gt;Minimum num
+00001330: 6265 7220 6f66 2066 7261 6d65 7320 746f  ber of frames to
+00001340: 2063 6f6e 7369 6465 7220 6974 2061 2070   consider it a p
+00001350: 6172 7469 636c 6526 6c74 3b2f 7026 6774  article&lt;/p&gt
+00001360: 3b26 6c74 3b2f 626f 6479 2667 743b 266c  ;&lt;/body&gt;&l
+00001370: 743b 2f68 746d 6c26 6774 3b3c 2f73 7472  t;/html&gt;</str
+00001380: 696e 673e 0a20 2020 2020 2020 2020 3c2f  ing>.         </
+00001390: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+000013a0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+000013b0: 653d 2274 6578 7422 3e0a 2020 2020 2020  e="text">.      
+000013c0: 2020 2020 3c73 7472 696e 673e 333c 2f73      <string>3</s
+000013d0: 7472 696e 673e 0a20 2020 2020 2020 2020  tring>.         
+000013e0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+000013f0: 2020 2020 3c2f 7769 6467 6574 3e0a 2020      </widget>.  
+00001400: 2020 2020 203c 2f69 7465 6d3e 0a20 2020       </item>.   
+00001410: 2020 2020 3c69 7465 6d20 726f 773d 2237      <item row="7
+00001420: 2220 636f 6c75 6d6e 3d22 3122 3e0a 2020  " column="1">.  
+00001430: 2020 2020 2020 3c77 6964 6765 7420 636c        <widget cl
+00001440: 6173 733d 2251 5075 7368 4275 7474 6f6e  ass="QPushButton
+00001450: 2220 6e61 6d65 3d22 6361 6c63 756c 6174  " name="calculat
+00001460: 655f 6275 7474 6f6e 223e 0a20 2020 2020  e_button">.     
+00001470: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00001480: 6d65 3d22 746f 6f6c 5469 7022 3e0a 2020  me="toolTip">.  
+00001490: 2020 2020 2020 2020 3c73 7472 696e 673e          <string>
+000014a0: 266c 743b 6874 6d6c 2667 743b 266c 743b  &lt;html&gt;&lt;
+000014b0: 6865 6164 2f26 6774 3b26 6c74 3b62 6f64  head/&gt;&lt;bod
+000014c0: 7926 6774 3b26 6c74 3b70 2667 743b 4669  y&gt;&lt;p&gt;Fi
+000014d0: 6e64 2074 6865 206c 6f63 6174 696f 6e73  nd the locations
+000014e0: 206f 6620 616c 6c20 7468 6520 7061 7274   of all the part
+000014f0: 6963 6c65 7320 696e 2074 6865 2072 616e  icles in the ran
+00001500: 6765 206f 6620 6672 616d 6573 266c 743b  ge of frames&lt;
+00001510: 2f70 2667 743b 266c 743b 2f62 6f64 7926  /p&gt;&lt;/body&
+00001520: 6774 3b26 6c74 3b2f 6874 6d6c 2667 743b  gt;&lt;/html&gt;
+00001530: 3c2f 7374 7269 6e67 3e0a 2020 2020 2020  </string>.      
+00001540: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
+00001550: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00001560: 7920 6e61 6d65 3d22 7465 7874 223e 0a20  y name="text">. 
+00001570: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
+00001580: 3e43 616c 6375 6c61 7465 2061 6c6c 3c2f  >Calculate all</
+00001590: 7374 7269 6e67 3e0a 2020 2020 2020 2020  string>.        
+000015a0: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+000015b0: 2020 2020 203c 2f77 6964 6765 743e 0a20       </widget>. 
+000015c0: 2020 2020 2020 3c2f 6974 656d 3e0a 2020        </item>.  
+000015d0: 2020 2020 203c 6974 656d 2072 6f77 3d22       <item row="
+000015e0: 3922 2063 6f6c 756d 6e3d 2230 2220 636f  9" column="0" co
+000015f0: 6c73 7061 6e3d 2232 223e 0a20 2020 2020  lspan="2">.     
+00001600: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
+00001610: 3d22 4c69 6e65 2220 6e61 6d65 3d22 6c69  ="Line" name="li
+00001620: 6e65 223e 0a20 2020 2020 2020 2020 3c70  ne">.         <p
+00001630: 726f 7065 7274 7920 6e61 6d65 3d22 6f72  roperty name="or
+00001640: 6965 6e74 6174 696f 6e22 3e0a 2020 2020  ientation">.    
+00001650: 2020 2020 2020 3c65 6e75 6d3e 5174 3a3a        <enum>Qt::
+00001660: 486f 7269 7a6f 6e74 616c 3c2f 656e 756d  Horizontal</enum
+00001670: 3e0a 2020 2020 2020 2020 203c 2f70 726f  >.         </pro
+00001680: 7065 7274 793e 0a20 2020 2020 2020 203c  perty>.        <
+00001690: 2f77 6964 6765 743e 0a20 2020 2020 2020  /widget>.       
+000016a0: 3c2f 6974 656d 3e0a 2020 2020 2020 203c  </item>.       <
+000016b0: 6974 656d 2072 6f77 3d22 3130 2220 636f  item row="10" co
+000016c0: 6c75 6d6e 3d22 3022 3e0a 2020 2020 2020  lumn="0">.      
+000016d0: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
+000016e0: 2251 4c61 6265 6c22 206e 616d 653d 226c  "QLabel" name="l
+000016f0: 6162 656c 5f38 223e 0a20 2020 2020 2020  abel_8">.       
+00001700: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00001710: 3d22 7465 7874 223e 0a20 2020 2020 2020  ="text">.       
+00001720: 2020 203c 7374 7269 6e67 3e53 7465 7020     <string>Step 
+00001730: 5369 7a65 2028 c2b5 6d29 3c2f 7374 7269  Size (..m)</stri
+00001740: 6e67 3e0a 2020 2020 2020 2020 203c 2f70  ng>.         </p
+00001750: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00001760: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00001770: 3d22 6275 6464 7922 3e0a 2020 2020 2020  ="buddy">.      
+00001780: 2020 2020 3c63 7374 7269 6e67 3e73 7465      <cstring>ste
+00001790: 705f 7369 7a65 5f6c 696e 653c 2f63 7374  p_size_line</cst
+000017a0: 7269 6e67 3e0a 2020 2020 2020 2020 203c  ring>.         <
+000017b0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+000017c0: 2020 203c 2f77 6964 6765 743e 0a20 2020     </widget>.   
+000017d0: 2020 2020 3c2f 6974 656d 3e0a 2020 2020      </item>.    
+000017e0: 2020 203c 6974 656d 2072 6f77 3d22 3130     <item row="10
+000017f0: 2220 636f 6c75 6d6e 3d22 3122 3e0a 2020  " column="1">.  
+00001800: 2020 2020 2020 3c77 6964 6765 7420 636c        <widget cl
+00001810: 6173 733d 2251 4c69 6e65 4564 6974 2220  ass="QLineEdit" 
+00001820: 6e61 6d65 3d22 7374 6570 5f73 697a 655f  name="step_size_
+00001830: 6c69 6e65 223e 0a20 2020 2020 2020 2020  line">.         
+00001840: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00001850: 746f 6f6c 5469 7022 3e0a 2020 2020 2020  toolTip">.      
+00001860: 2020 2020 3c73 7472 696e 673e 266c 743b      <string>&lt;
+00001870: 6874 6d6c 2667 743b 266c 743b 6865 6164  html&gt;&lt;head
+00001880: 2f26 6774 3b26 6c74 3b62 6f64 7926 6774  /&gt;&lt;body&gt
+00001890: 3b26 6c74 3b70 2667 743b 5374 6570 2073  ;&lt;p&gt;Step s
+000018a0: 697a 6520 6475 7269 6e67 2074 6865 2073  ize during the s
+000018b0: 6361 6e26 6c74 3b2f 7026 6774 3b26 6c74  can&lt;/p&gt;&lt
+000018c0: 3b2f 626f 6479 2667 743b 266c 743b 2f68  ;/body&gt;&lt;/h
+000018d0: 746d 6c26 6774 3b3c 2f73 7472 696e 673e  tml&gt;</string>
+000018e0: 0a20 2020 2020 2020 2020 3c2f 7072 6f70  .         </prop
+000018f0: 6572 7479 3e0a 2020 2020 2020 2020 203c  erty>.         <
+00001900: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
+00001910: 6578 7422 3e0a 2020 2020 2020 2020 2020  ext">.          
+00001920: 3c73 7472 696e 673e 353c 2f73 7472 696e  <string>5</strin
+00001930: 673e 0a20 2020 2020 2020 2020 3c2f 7072  g>.         </pr
+00001940: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00001950: 3c2f 7769 6467 6574 3e0a 2020 2020 2020  </widget>.      
+00001960: 203c 2f69 7465 6d3e 0a20 2020 2020 2020   </item>.       
+00001970: 3c69 7465 6d20 726f 773d 2231 3122 2063  <item row="11" c
+00001980: 6f6c 756d 6e3d 2231 223e 0a20 2020 2020  olumn="1">.     
+00001990: 2020 203c 7370 6163 6572 206e 616d 653d     <spacer name=
+000019a0: 2276 6572 7469 6361 6c53 7061 6365 7222  "verticalSpacer"
+000019b0: 3e0a 2020 2020 2020 2020 203c 7072 6f70  >.         <prop
+000019c0: 6572 7479 206e 616d 653d 226f 7269 656e  erty name="orien
+000019d0: 7461 7469 6f6e 223e 0a20 2020 2020 2020  tation">.       
+000019e0: 2020 203c 656e 756d 3e51 743a 3a56 6572     <enum>Qt::Ver
+000019f0: 7469 6361 6c3c 2f65 6e75 6d3e 0a20 2020  tical</enum>.   
+00001a00: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
+00001a10: 3e0a 2020 2020 2020 2020 203c 7072 6f70  >.         <prop
+00001a20: 6572 7479 206e 616d 653d 2273 697a 6548  erty name="sizeH
+00001a30: 696e 7422 2073 7464 7365 743d 2230 223e  int" stdset="0">
+00001a40: 0a20 2020 2020 2020 2020 203c 7369 7a65  .          <size
+00001a50: 3e0a 2020 2020 2020 2020 2020 203c 7769  >.           <wi
+00001a60: 6474 683e 3230 3c2f 7769 6474 683e 0a20  dth>20</width>. 
+00001a70: 2020 2020 2020 2020 2020 3c68 6569 6768            <heigh
+00001a80: 743e 3430 3c2f 6865 6967 6874 3e0a 2020  t>40</height>.  
+00001a90: 2020 2020 2020 2020 3c2f 7369 7a65 3e0a          </size>.
+00001aa0: 2020 2020 2020 2020 203c 2f70 726f 7065           </prope
+00001ab0: 7274 793e 0a20 2020 2020 2020 203c 2f73  rty>.        </s
+00001ac0: 7061 6365 723e 0a20 2020 2020 2020 3c2f  pacer>.       </
+00001ad0: 6974 656d 3e0a 2020 2020 2020 3c2f 6c61  item>.      </la
+00001ae0: 796f 7574 3e0a 2020 2020 203c 2f77 6964  yout>.     </wid
+00001af0: 6765 743e 0a20 2020 203c 2f69 7465 6d3e  get>.    </item>
+00001b00: 0a20 2020 203c 6974 656d 3e0a 2020 2020  .    <item>.    
+00001b10: 203c 7769 6467 6574 2063 6c61 7373 3d22   <widget class="
+00001b20: 5157 6964 6765 7422 206e 616d 653d 2277  QWidget" name="w
+00001b30: 6964 6765 7422 206e 6174 6976 653d 2274  idget" native="t
+00001b40: 7275 6522 3e0a 2020 2020 2020 3c70 726f  rue">.      <pro
+00001b50: 7065 7274 7920 6e61 6d65 3d22 7369 7a65  perty name="size
+00001b60: 506f 6c69 6379 223e 0a20 2020 2020 2020  Policy">.       
+00001b70: 3c73 697a 6570 6f6c 6963 7920 6873 697a  <sizepolicy hsiz
+00001b80: 6574 7970 653d 2245 7870 616e 6469 6e67  etype="Expanding
+00001b90: 2220 7673 697a 6574 7970 653d 2250 7265  " vsizetype="Pre
+00001ba0: 6665 7272 6564 223e 0a20 2020 2020 2020  ferred">.       
+00001bb0: 203c 686f 7273 7472 6574 6368 3e30 3c2f   <horstretch>0</
+00001bc0: 686f 7273 7472 6574 6368 3e0a 2020 2020  horstretch>.    
+00001bd0: 2020 2020 3c76 6572 7374 7265 7463 683e      <verstretch>
+00001be0: 303c 2f76 6572 7374 7265 7463 683e 0a20  0</verstretch>. 
+00001bf0: 2020 2020 2020 3c2f 7369 7a65 706f 6c69        </sizepoli
+00001c00: 6379 3e0a 2020 2020 2020 3c2f 7072 6f70  cy>.      </prop
+00001c10: 6572 7479 3e0a 2020 2020 2020 3c6c 6179  erty>.      <lay
+00001c20: 6f75 7420 636c 6173 733d 2251 5642 6f78  out class="QVBox
+00001c30: 4c61 796f 7574 2220 6e61 6d65 3d22 7665  Layout" name="ve
+00001c40: 7274 6963 616c 4c61 796f 7574 223e 0a20  rticalLayout">. 
+00001c50: 2020 2020 2020 3c69 7465 6d3e 0a20 2020        <item>.   
+00001c60: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
+00001c70: 7373 3d22 5157 6964 6765 7422 206e 616d  ss="QWidget" nam
+00001c80: 653d 2273 6c69 6465 725f 7769 6467 6574  e="slider_widget
+00001c90: 2220 6e61 7469 7665 3d22 7472 7565 223e  " native="true">
+00001ca0: 0a20 2020 2020 2020 2020 3c70 726f 7065  .         <prope
+00001cb0: 7274 7920 6e61 6d65 3d22 7369 7a65 506f  rty name="sizePo
+00001cc0: 6c69 6379 223e 0a20 2020 2020 2020 2020  licy">.         
+00001cd0: 203c 7369 7a65 706f 6c69 6379 2068 7369   <sizepolicy hsi
+00001ce0: 7a65 7479 7065 3d22 5072 6566 6572 7265  zetype="Preferre
+00001cf0: 6422 2076 7369 7a65 7479 7065 3d22 4d69  d" vsizetype="Mi
+00001d00: 6e69 6d75 6d22 3e0a 2020 2020 2020 2020  nimum">.        
+00001d10: 2020 203c 686f 7273 7472 6574 6368 3e30     <horstretch>0
+00001d20: 3c2f 686f 7273 7472 6574 6368 3e0a 2020  </horstretch>.  
+00001d30: 2020 2020 2020 2020 203c 7665 7273 7472           <verstr
+00001d40: 6574 6368 3e30 3c2f 7665 7273 7472 6574  etch>0</verstret
+00001d50: 6368 3e0a 2020 2020 2020 2020 2020 3c2f  ch>.          </
+00001d60: 7369 7a65 706f 6c69 6379 3e0a 2020 2020  sizepolicy>.    
+00001d70: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
+00001d80: 0a20 2020 2020 2020 2020 3c70 726f 7065  .         <prope
+00001d90: 7274 7920 6e61 6d65 3d22 6d61 7869 6d75  rty name="maximu
+00001da0: 6d53 697a 6522 3e0a 2020 2020 2020 2020  mSize">.        
+00001db0: 2020 3c73 697a 653e 0a20 2020 2020 2020    <size>.       
+00001dc0: 2020 2020 3c77 6964 7468 3e31 3637 3737      <width>16777
+00001dd0: 3231 353c 2f77 6964 7468 3e0a 2020 2020  215</width>.    
+00001de0: 2020 2020 2020 203c 6865 6967 6874 3e35         <height>5
+00001df0: 303c 2f68 6569 6768 743e 0a20 2020 2020  0</height>.     
+00001e00: 2020 2020 203c 2f73 697a 653e 0a20 2020       </size>.   
+00001e10: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
+00001e20: 3e0a 2020 2020 2020 2020 203c 6c61 796f  >.         <layo
+00001e30: 7574 2063 6c61 7373 3d22 5148 426f 784c  ut class="QHBoxL
+00001e40: 6179 6f75 7422 206e 616d 653d 2268 6f72  ayout" name="hor
+00001e50: 697a 6f6e 7461 6c4c 6179 6f75 745f 3322  izontalLayout_3"
+00001e60: 3e0a 2020 2020 2020 2020 2020 3c70 726f  >.          <pro
+00001e70: 7065 7274 7920 6e61 6d65 3d22 746f 704d  perty name="topM
+00001e80: 6172 6769 6e22 3e0a 2020 2020 2020 2020  argin">.        
+00001e90: 2020 203c 6e75 6d62 6572 3e30 3c2f 6e75     <number>0</nu
+00001ea0: 6d62 6572 3e0a 2020 2020 2020 2020 2020  mber>.          
+00001eb0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00001ec0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00001ed0: 6e61 6d65 3d22 626f 7474 6f6d 4d61 7267  name="bottomMarg
+00001ee0: 696e 223e 0a20 2020 2020 2020 2020 2020  in">.           
+00001ef0: 3c6e 756d 6265 723e 303c 2f6e 756d 6265  <number>0</numbe
+00001f00: 723e 0a20 2020 2020 2020 2020 203c 2f70  r>.          </p
+00001f10: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00001f20: 2020 203c 6974 656d 3e0a 2020 2020 2020     <item>.      
+00001f30: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
+00001f40: 7373 3d22 514c 6162 656c 2220 6e61 6d65  ss="QLabel" name
+00001f50: 3d22 6672 616d 655f 6e75 6d22 3e0a 2020  ="frame_num">.  
+00001f60: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00001f70: 7274 7920 6e61 6d65 3d22 7465 7874 223e  rty name="text">
+00001f80: 0a20 2020 2020 2020 2020 2020 2020 3c73  .             <s
+00001f90: 7472 696e 673e 303c 2f73 7472 696e 673e  tring>0</string>
+00001fa0: 0a20 2020 2020 2020 2020 2020 203c 2f70  .            </p
+00001fb0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00001fc0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00001fd0: 616d 653d 2262 7564 6479 223e 0a20 2020  ame="buddy">.   
+00001fe0: 2020 2020 2020 2020 2020 3c63 7374 7269            <cstri
+00001ff0: 6e67 3e66 7261 6d65 5f73 6c69 6465 723c  ng>frame_slider<
+00002000: 2f63 7374 7269 6e67 3e0a 2020 2020 2020  /cstring>.      
+00002010: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
+00002020: 3e0a 2020 2020 2020 2020 2020 203c 2f77  >.           </w
+00002030: 6964 6765 743e 0a20 2020 2020 2020 2020  idget>.         
+00002040: 203c 2f69 7465 6d3e 0a20 2020 2020 2020   </item>.       
+00002050: 2020 203c 6974 656d 3e0a 2020 2020 2020     <item>.      
+00002060: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
+00002070: 7373 3d22 5153 6c69 6465 7222 206e 616d  ss="QSlider" nam
+00002080: 653d 2266 7261 6d65 5f73 6c69 6465 7222  e="frame_slider"
+00002090: 3e0a 2020 2020 2020 2020 2020 2020 3c70  >.            <p
+000020a0: 726f 7065 7274 7920 6e61 6d65 3d22 656e  roperty name="en
+000020b0: 6162 6c65 6422 3e0a 2020 2020 2020 2020  abled">.        
+000020c0: 2020 2020 203c 626f 6f6c 3e66 616c 7365       <bool>false
+000020d0: 3c2f 626f 6f6c 3e0a 2020 2020 2020 2020  </bool>.        
+000020e0: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
+000020f0: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+00002100: 7065 7274 7920 6e61 6d65 3d22 6d6f 7573  perty name="mous
+00002110: 6554 7261 636b 696e 6722 3e0a 2020 2020  eTracking">.    
+00002120: 2020 2020 2020 2020 203c 626f 6f6c 3e74           <bool>t
+00002130: 7275 653c 2f62 6f6f 6c3e 0a20 2020 2020  rue</bool>.     
+00002140: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+00002150: 793e 0a20 2020 2020 2020 2020 2020 203c  y>.            <
+00002160: 7072 6f70 6572 7479 206e 616d 653d 2266  property name="f
+00002170: 6f63 7573 506f 6c69 6379 223e 0a20 2020  ocusPolicy">.   
+00002180: 2020 2020 2020 2020 2020 3c65 6e75 6d3e            <enum>
+00002190: 5174 3a3a 5768 6565 6c46 6f63 7573 3c2f  Qt::WheelFocus</
+000021a0: 656e 756d 3e0a 2020 2020 2020 2020 2020  enum>.          
+000021b0: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+000021c0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+000021d0: 7274 7920 6e61 6d65 3d22 7374 6174 7573  rty name="status
+000021e0: 5469 7022 3e0a 2020 2020 2020 2020 2020  Tip">.          
+000021f0: 2020 203c 7374 7269 6e67 3e53 7461 7475     <string>Statu
+00002200: 7320 7469 703c 2f73 7472 696e 673e 0a20  s tip</string>. 
+00002210: 2020 2020 2020 2020 2020 203c 2f70 726f             </pro
+00002220: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00002230: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00002240: 653d 226f 7269 656e 7461 7469 6f6e 223e  e="orientation">
+00002250: 0a20 2020 2020 2020 2020 2020 2020 3c65  .             <e
+00002260: 6e75 6d3e 5174 3a3a 486f 7269 7a6f 6e74  num>Qt::Horizont
+00002270: 616c 3c2f 656e 756d 3e0a 2020 2020 2020  al</enum>.      
+00002280: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
+00002290: 3e0a 2020 2020 2020 2020 2020 2020 3c70  >.            <p
+000022a0: 726f 7065 7274 7920 6e61 6d65 3d22 7469  roperty name="ti
+000022b0: 636b 506f 7369 7469 6f6e 223e 0a20 2020  ckPosition">.   
+000022c0: 2020 2020 2020 2020 2020 3c65 6e75 6d3e            <enum>
+000022d0: 5153 6c69 6465 723a 3a54 6963 6b73 4162  QSlider::TicksAb
+000022e0: 6f76 653c 2f65 6e75 6d3e 0a20 2020 2020  ove</enum>.     
+000022f0: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+00002300: 793e 0a20 2020 2020 2020 2020 2020 203c  y>.            <
+00002310: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
+00002320: 6963 6b49 6e74 6572 7661 6c22 3e0a 2020  ickInterval">.  
+00002330: 2020 2020 2020 2020 2020 203c 6e75 6d62             <numb
+00002340: 6572 3e32 303c 2f6e 756d 6265 723e 0a20  er>20</number>. 
+00002350: 2020 2020 2020 2020 2020 203c 2f70 726f             </pro
+00002360: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00002370: 2020 3c2f 7769 6467 6574 3e0a 2020 2020    </widget>.    
+00002380: 2020 2020 2020 3c2f 6974 656d 3e0a 2020        </item>.  
+00002390: 2020 2020 2020 203c 2f6c 6179 6f75 743e         </layout>
+000023a0: 0a20 2020 2020 2020 203c 2f77 6964 6765  .        </widge
+000023b0: 743e 0a20 2020 2020 2020 3c2f 6974 656d  t>.       </item
+000023c0: 3e0a 2020 2020 2020 203c 6974 656d 3e0a  >.       <item>.
+000023d0: 2020 2020 2020 2020 3c77 6964 6765 7420          <widget 
+000023e0: 636c 6173 733d 2251 5769 6467 6574 2220  class="QWidget" 
+000023f0: 6e61 6d65 3d22 7669 6465 6f5f 7769 6467  name="video_widg
+00002400: 6574 2220 6e61 7469 7665 3d22 7472 7565  et" native="true
+00002410: 223e 0a20 2020 2020 2020 2020 3c6c 6179  ">.         <lay
+00002420: 6f75 7420 636c 6173 733d 2251 4772 6964  out class="QGrid
+00002430: 4c61 796f 7574 2220 6e61 6d65 3d22 6772  Layout" name="gr
+00002440: 6964 4c61 796f 7574 223e 0a20 2020 2020  idLayout">.     
+00002450: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00002460: 616d 653d 226c 6566 744d 6172 6769 6e22  ame="leftMargin"
+00002470: 3e0a 2020 2020 2020 2020 2020 203c 6e75  >.           <nu
+00002480: 6d62 6572 3e30 3c2f 6e75 6d62 6572 3e0a  mber>0</number>.
+00002490: 2020 2020 2020 2020 2020 3c2f 7072 6f70            </prop
+000024a0: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+000024b0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+000024c0: 746f 704d 6172 6769 6e22 3e0a 2020 2020  topMargin">.    
+000024d0: 2020 2020 2020 203c 6e75 6d62 6572 3e30         <number>0
+000024e0: 3c2f 6e75 6d62 6572 3e0a 2020 2020 2020  </number>.      
+000024f0: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
+00002500: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00002510: 7274 7920 6e61 6d65 3d22 7269 6768 744d  rty name="rightM
+00002520: 6172 6769 6e22 3e0a 2020 2020 2020 2020  argin">.        
+00002530: 2020 203c 6e75 6d62 6572 3e30 3c2f 6e75     <number>0</nu
+00002540: 6d62 6572 3e0a 2020 2020 2020 2020 2020  mber>.          
+00002550: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00002560: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00002570: 6e61 6d65 3d22 626f 7474 6f6d 4d61 7267  name="bottomMarg
+00002580: 696e 223e 0a20 2020 2020 2020 2020 2020  in">.           
+00002590: 3c6e 756d 6265 723e 303c 2f6e 756d 6265  <number>0</numbe
+000025a0: 723e 0a20 2020 2020 2020 2020 203c 2f70  r>.          </p
+000025b0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+000025c0: 2020 3c2f 6c61 796f 7574 3e0a 2020 2020    </layout>.    
+000025d0: 2020 2020 3c2f 7769 6467 6574 3e0a 2020      </widget>.  
+000025e0: 2020 2020 203c 2f69 7465 6d3e 0a20 2020       </item>.   
+000025f0: 2020 203c 2f6c 6179 6f75 743e 0a20 2020     </layout>.   
+00002600: 2020 3c2f 7769 6467 6574 3e0a 2020 2020    </widget>.    
+00002610: 3c2f 6974 656d 3e0a 2020 203c 2f6c 6179  </item>.   </lay
+00002620: 6f75 743e 0a20 203c 2f77 6964 6765 743e  out>.  </widget>
+00002630: 0a20 203c 7769 6467 6574 2063 6c61 7373  .  <widget class
+00002640: 3d22 5153 7461 7475 7342 6172 2220 6e61  ="QStatusBar" na
+00002650: 6d65 3d22 7374 6174 7573 6261 7222 2f3e  me="statusbar"/>
+00002660: 0a20 203c 7769 6467 6574 2063 6c61 7373  .  <widget class
+00002670: 3d22 5154 6f6f 6c42 6172 2220 6e61 6d65  ="QToolBar" name
+00002680: 3d22 746f 6f6c 4261 7222 3e0a 2020 203c  ="toolBar">.   <
+00002690: 7072 6f70 6572 7479 206e 616d 653d 2277  property name="w
+000026a0: 696e 646f 7754 6974 6c65 223e 0a20 2020  indowTitle">.   
+000026b0: 203c 7374 7269 6e67 3e74 6f6f 6c42 6172   <string>toolBar
+000026c0: 3c2f 7374 7269 6e67 3e0a 2020 203c 2f70  </string>.   </p
+000026d0: 726f 7065 7274 793e 0a20 2020 3c61 7474  roperty>.   <att
+000026e0: 7269 6275 7465 206e 616d 653d 2274 6f6f  ribute name="too
+000026f0: 6c42 6172 4172 6561 223e 0a20 2020 203c  lBarArea">.    <
+00002700: 656e 756d 3e54 6f70 546f 6f6c 4261 7241  enum>TopToolBarA
+00002710: 7265 613c 2f65 6e75 6d3e 0a20 2020 3c2f  rea</enum>.   </
+00002720: 6174 7472 6962 7574 653e 0a20 2020 3c61  attribute>.   <a
+00002730: 7474 7269 6275 7465 206e 616d 653d 2274  ttribute name="t
+00002740: 6f6f 6c42 6172 4272 6561 6b22 3e0a 2020  oolBarBreak">.  
+00002750: 2020 3c62 6f6f 6c3e 6661 6c73 653c 2f62    <bool>false</b
+00002760: 6f6f 6c3e 0a20 2020 3c2f 6174 7472 6962  ool>.   </attrib
+00002770: 7574 653e 0a20 2020 3c61 6464 6163 7469  ute>.   <addacti
+00002780: 6f6e 206e 616d 653d 2261 6374 696f 6e5f  on name="action_
+00002790: 6f70 656e 222f 3e0a 2020 203c 6164 6461  open"/>.   <adda
+000027a0: 6374 696f 6e20 6e61 6d65 3d22 6163 7469  ction name="acti
+000027b0: 6f6e 5f6d 6173 735f 6869 7374 6f67 7261  on_mass_histogra
+000027c0: 6d22 2f3e 0a20 2020 3c61 6464 6163 7469  m"/>.   <addacti
+000027d0: 6f6e 206e 616d 653d 2261 6374 696f 6e5f  on name="action_
+000027e0: 6461 7461 5f70 6c6f 7473 222f 3e0a 2020  data_plots"/>.  
+000027f0: 203c 6164 6461 6374 696f 6e20 6e61 6d65   <addaction name
+00002800: 3d22 6163 7469 6f6e 5f73 6176 655f 6461  ="action_save_da
+00002810: 7461 222f 3e0a 2020 3c2f 7769 6467 6574  ta"/>.  </widget
+00002820: 3e0a 2020 3c77 6964 6765 7420 636c 6173  >.  <widget clas
+00002830: 733d 2251 4d65 6e75 4261 7222 206e 616d  s="QMenuBar" nam
+00002840: 653d 226d 656e 7542 6172 223e 0a20 2020  e="menuBar">.   
+00002850: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00002860: 6765 6f6d 6574 7279 223e 0a20 2020 203c  geometry">.    <
+00002870: 7265 6374 3e0a 2020 2020 203c 783e 303c  rect>.     <x>0<
+00002880: 2f78 3e0a 2020 2020 203c 793e 303c 2f79  /x>.     <y>0</y
+00002890: 3e0a 2020 2020 203c 7769 6474 683e 3736  >.     <width>76
+000028a0: 383c 2f77 6964 7468 3e0a 2020 2020 203c  8</width>.     <
+000028b0: 6865 6967 6874 3e32 343c 2f68 6569 6768  height>24</heigh
+000028c0: 743e 0a20 2020 203c 2f72 6563 743e 0a20  t>.    </rect>. 
+000028d0: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+000028e0: 203c 7769 6467 6574 2063 6c61 7373 3d22   <widget class="
+000028f0: 514d 656e 7522 206e 616d 653d 226d 656e  QMenu" name="men
+00002900: 7546 696c 6522 3e0a 2020 2020 3c70 726f  uFile">.    <pro
+00002910: 7065 7274 7920 6e61 6d65 3d22 7469 746c  perty name="titl
+00002920: 6522 3e0a 2020 2020 203c 7374 7269 6e67  e">.     <string
+00002930: 3e46 696c 653c 2f73 7472 696e 673e 0a20  >File</string>. 
+00002940: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
+00002950: 2020 203c 6164 6461 6374 696f 6e20 6e61     <addaction na
+00002960: 6d65 3d22 6163 7469 6f6e 5f6f 7065 6e22  me="action_open"
+00002970: 2f3e 0a20 2020 203c 6164 6461 6374 696f  />.    <addactio
+00002980: 6e20 6e61 6d65 3d22 6163 7469 6f6e 5f73  n name="action_s
+00002990: 6176 655f 6461 7461 222f 3e0a 2020 2020  ave_data"/>.    
+000029a0: 3c61 6464 6163 7469 6f6e 206e 616d 653d  <addaction name=
+000029b0: 2261 6374 696f 6e5f 6578 706f 7274 5f61  "action_export_a
+000029c0: 6c6c 5f64 6174 6122 2f3e 0a20 2020 3c2f  ll_data"/>.   </
+000029d0: 7769 6467 6574 3e0a 2020 203c 7769 6467  widget>.   <widg
+000029e0: 6574 2063 6c61 7373 3d22 514d 656e 7522  et class="QMenu"
+000029f0: 206e 616d 653d 226d 656e 7541 6e61 7973   name="menuAnays
+00002a00: 6973 223e 0a20 2020 203c 7072 6f70 6572  is">.    <proper
+00002a10: 7479 206e 616d 653d 2274 6974 6c65 223e  ty name="title">
+00002a20: 0a20 2020 2020 3c73 7472 696e 673e 416e  .     <string>An
+00002a30: 6179 7369 733c 2f73 7472 696e 673e 0a20  aysis</string>. 
+00002a40: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
+00002a50: 2020 203c 6164 6461 6374 696f 6e20 6e61     <addaction na
+00002a60: 6d65 3d22 6163 7469 6f6e 5f63 616c 6375  me="action_calcu
+00002a70: 6c61 7465 5f62 6b67 222f 3e0a 2020 2020  late_bkg"/>.    
+00002a80: 3c61 6464 6163 7469 6f6e 206e 616d 653d  <addaction name=
+00002a90: 2261 6374 696f 6e5f 7368 6f77 5f62 6b67  "action_show_bkg
+00002aa0: 222f 3e0a 2020 2020 3c61 6464 6163 7469  "/>.    <addacti
+00002ab0: 6f6e 206e 616d 653d 2261 6374 696f 6e5f  on name="action_
+00002ac0: 6461 7461 5f66 7261 6d65 222f 3e0a 2020  data_frame"/>.  
+00002ad0: 203c 2f77 6964 6765 743e 0a20 2020 3c77   </widget>.   <w
+00002ae0: 6964 6765 7420 636c 6173 733d 2251 4d65  idget class="QMe
+00002af0: 6e75 2220 6e61 6d65 3d22 6d65 6e75 4865  nu" name="menuHe
+00002b00: 6c70 223e 0a20 2020 203c 7072 6f70 6572  lp">.    <proper
+00002b10: 7479 206e 616d 653d 2274 6974 6c65 223e  ty name="title">
+00002b20: 0a20 2020 2020 3c73 7472 696e 673e 4865  .     <string>He
+00002b30: 6c70 3c2f 7374 7269 6e67 3e0a 2020 2020  lp</string>.    
+00002b40: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00002b50: 3c61 6464 6163 7469 6f6e 206e 616d 653d  <addaction name=
+00002b60: 2261 6374 696f 6e5f 6162 6f75 7422 2f3e  "action_about"/>
+00002b70: 0a20 2020 203c 6164 6461 6374 696f 6e20  .    <addaction 
+00002b80: 6e61 6d65 3d22 6163 7469 6f6e 476f 5f74  name="actionGo_t
+00002b90: 6f5f 646f 6375 6d65 6e74 6174 696f 6e22  o_documentation"
+00002ba0: 2f3e 0a20 2020 3c2f 7769 6467 6574 3e0a  />.   </widget>.
+00002bb0: 2020 203c 6164 6461 6374 696f 6e20 6e61     <addaction na
+00002bc0: 6d65 3d22 6d65 6e75 4669 6c65 222f 3e0a  me="menuFile"/>.
+00002bd0: 2020 203c 6164 6461 6374 696f 6e20 6e61     <addaction na
+00002be0: 6d65 3d22 6d65 6e75 416e 6179 7369 7322  me="menuAnaysis"
+00002bf0: 2f3e 0a20 2020 3c61 6464 6163 7469 6f6e  />.   <addaction
+00002c00: 206e 616d 653d 226d 656e 7548 656c 7022   name="menuHelp"
+00002c10: 2f3e 0a20 203c 2f77 6964 6765 743e 0a20  />.  </widget>. 
+00002c20: 203c 6163 7469 6f6e 206e 616d 653d 2261   <action name="a
+00002c30: 6374 696f 6e5f 6f70 656e 223e 0a20 2020  ction_open">.   
+00002c40: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00002c50: 6963 6f6e 223e 0a20 2020 203c 6963 6f6e  icon">.    <icon
+00002c60: 7365 743e 0a20 2020 2020 3c6e 6f72 6d61  set>.     <norma
+00002c70: 6c6f 6666 3e49 636f 6e73 2f4f 7065 6e20  loff>Icons/Open 
+00002c80: 466f 6c64 6572 2e73 7667 3c2f 6e6f 726d  Folder.svg</norm
+00002c90: 616c 6f66 663e 4963 6f6e 732f 4f70 656e  aloff>Icons/Open
+00002ca0: 2046 6f6c 6465 722e 7376 673c 2f69 636f   Folder.svg</ico
+00002cb0: 6e73 6574 3e0a 2020 203c 2f70 726f 7065  nset>.   </prope
+00002cc0: 7274 793e 0a20 2020 3c70 726f 7065 7274  rty>.   <propert
+00002cd0: 7920 6e61 6d65 3d22 7465 7874 223e 0a20  y name="text">. 
+00002ce0: 2020 203c 7374 7269 6e67 3e4f 7065 6e3c     <string>Open<
+00002cf0: 2f73 7472 696e 673e 0a20 2020 3c2f 7072  /string>.   </pr
+00002d00: 6f70 6572 7479 3e0a 2020 203c 7072 6f70  operty>.   <prop
+00002d10: 6572 7479 206e 616d 653d 2274 6f6f 6c54  erty name="toolT
+00002d20: 6970 223e 0a20 2020 203c 7374 7269 6e67  ip">.    <string
+00002d30: 3e4f 7065 6e20 6461 7461 2066 696c 653c  >Open data file<
+00002d40: 2f73 7472 696e 673e 0a20 2020 3c2f 7072  /string>.   </pr
+00002d50: 6f70 6572 7479 3e0a 2020 203c 7072 6f70  operty>.   <prop
+00002d60: 6572 7479 206e 616d 653d 2273 686f 7274  erty name="short
+00002d70: 6375 7422 3e0a 2020 2020 3c73 7472 696e  cut">.    <strin
+00002d80: 673e 4374 726c 2b4f 3c2f 7374 7269 6e67  g>Ctrl+O</string
+00002d90: 3e0a 2020 203c 2f70 726f 7065 7274 793e  >.   </property>
+00002da0: 0a20 203c 2f61 6374 696f 6e3e 0a20 203c  .  </action>.  <
+00002db0: 6163 7469 6f6e 206e 616d 653d 2261 6374  action name="act
+00002dc0: 696f 6e5f 6d61 7373 5f68 6973 746f 6772  ion_mass_histogr
+00002dd0: 616d 223e 0a20 2020 3c70 726f 7065 7274  am">.   <propert
+00002de0: 7920 6e61 6d65 3d22 6963 6f6e 223e 0a20  y name="icon">. 
+00002df0: 2020 203c 6963 6f6e 7365 743e 0a20 2020     <iconset>.   
+00002e00: 2020 3c6e 6f72 6d61 6c6f 6666 3e49 636f    <normaloff>Ico
+00002e10: 6e73 2f31 3138 3337 202d 2048 6973 746f  ns/11837 - Histo
+00002e20: 6772 616d 2e73 7667 3c2f 6e6f 726d 616c  gram.svg</normal
+00002e30: 6f66 663e 4963 6f6e 732f 3131 3833 3720  off>Icons/11837 
+00002e40: 2d20 4869 7374 6f67 7261 6d2e 7376 673c  - Histogram.svg<
+00002e50: 2f69 636f 6e73 6574 3e0a 2020 203c 2f70  /iconset>.   </p
+00002e60: 726f 7065 7274 793e 0a20 2020 3c70 726f  roperty>.   <pro
+00002e70: 7065 7274 7920 6e61 6d65 3d22 7465 7874  perty name="text
+00002e80: 223e 0a20 2020 203c 7374 7269 6e67 3e4d  ">.    <string>M
+00002e90: 6173 7320 4869 7374 6f67 7261 6d3c 2f73  ass Histogram</s
+00002ea0: 7472 696e 673e 0a20 2020 3c2f 7072 6f70  tring>.   </prop
+00002eb0: 6572 7479 3e0a 2020 203c 7072 6f70 6572  erty>.   <proper
+00002ec0: 7479 206e 616d 653d 2274 6f6f 6c54 6970  ty name="toolTip
+00002ed0: 223e 0a20 2020 203c 7374 7269 6e67 3e48  ">.    <string>H
+00002ee0: 6973 746f 6772 616d 206f 6620 496e 7465  istogram of Inte
+00002ef0: 6e73 6974 6965 7320 666f 7220 7468 6520  nsities for the 
+00002f00: 6375 7272 656e 7420 6672 616d 653c 2f73  current frame</s
+00002f10: 7472 696e 673e 0a20 2020 3c2f 7072 6f70  tring>.   </prop
+00002f20: 6572 7479 3e0a 2020 3c2f 6163 7469 6f6e  erty>.  </action
+00002f30: 3e0a 2020 3c61 6374 696f 6e20 6e61 6d65  >.  <action name
+00002f40: 3d22 6163 7469 6f6e 5f64 6174 615f 6672  ="action_data_fr
+00002f50: 616d 6522 3e0a 2020 203c 7072 6f70 6572  ame">.   <proper
+00002f60: 7479 206e 616d 653d 2269 636f 6e22 3e0a  ty name="icon">.
+00002f70: 2020 2020 3c69 636f 6e73 6574 3e0a 2020      <iconset>.  
+00002f80: 2020 203c 6e6f 726d 616c 6f66 663e 4963     <normaloff>Ic
+00002f90: 6f6e 732f 3131 3833 3120 2d20 466c 7569  ons/11831 - Flui
+00002fa0: 6420 4d65 6368 616e 6963 732e 7376 673c  d Mechanics.svg<
+00002fb0: 2f6e 6f72 6d61 6c6f 6666 3e49 636f 6e73  /normaloff>Icons
+00002fc0: 2f31 3138 3331 202d 2046 6c75 6964 204d  /11831 - Fluid M
+00002fd0: 6563 6861 6e69 6373 2e73 7667 3c2f 6963  echanics.svg</ic
+00002fe0: 6f6e 7365 743e 0a20 2020 3c2f 7072 6f70  onset>.   </prop
+00002ff0: 6572 7479 3e0a 2020 203c 7072 6f70 6572  erty>.   <proper
+00003000: 7479 206e 616d 653d 2274 6578 7422 3e0a  ty name="text">.
+00003010: 2020 2020 3c73 7472 696e 673e 5472 656e      <string>Tren
+00003020: 6473 3c2f 7374 7269 6e67 3e0a 2020 203c  ds</string>.   <
+00003030: 2f70 726f 7065 7274 793e 0a20 2020 3c70  /property>.   <p
+00003040: 726f 7065 7274 7920 6e61 6d65 3d22 746f  roperty name="to
+00003050: 6f6c 5469 7022 3e0a 2020 2020 3c73 7472  olTip">.    <str
+00003060: 696e 673e 5368 6f77 2074 7265 6e64 7320  ing>Show trends 
+00003070: 6f76 6572 2066 7261 6d65 733c 2f73 7472  over frames</str
+00003080: 696e 673e 0a20 2020 3c2f 7072 6f70 6572  ing>.   </proper
+00003090: 7479 3e0a 2020 3c2f 6163 7469 6f6e 3e0a  ty>.  </action>.
+000030a0: 2020 3c61 6374 696f 6e20 6e61 6d65 3d22    <action name="
+000030b0: 6163 7469 6f6e 5f64 6174 615f 706c 6f74  action_data_plot
+000030c0: 7322 3e0a 2020 203c 7072 6f70 6572 7479  s">.   <property
+000030d0: 206e 616d 653d 2269 636f 6e22 3e0a 2020   name="icon">.  
+000030e0: 2020 3c69 636f 6e73 6574 3e0a 2020 2020    <iconset>.    
+000030f0: 203c 6e6f 726d 616c 6f66 663e 4963 6f6e   <normaloff>Icon
+00003100: 732f 3131 3836 3220 2d20 5765 6967 6874  s/11862 - Weight
+00003110: 2053 6361 6c65 2e73 7667 3c2f 6e6f 726d   Scale.svg</norm
+00003120: 616c 6f66 663e 4963 6f6e 732f 3131 3836  aloff>Icons/1186
+00003130: 3220 2d20 5765 6967 6874 2053 6361 6c65  2 - Weight Scale
+00003140: 2e73 7667 3c2f 6963 6f6e 7365 743e 0a20  .svg</iconset>. 
+00003150: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+00003160: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00003170: 2274 6578 7422 3e0a 2020 2020 3c73 7472  "text">.    <str
+00003180: 696e 673e 4d61 7373 3c2f 7374 7269 6e67  ing>Mass</string
+00003190: 3e0a 2020 203c 2f70 726f 7065 7274 793e  >.   </property>
+000031a0: 0a20 2020 3c70 726f 7065 7274 7920 6e61  .   <property na
+000031b0: 6d65 3d22 746f 6f6c 5469 7022 3e0a 2020  me="toolTip">.  
+000031c0: 2020 3c73 7472 696e 673e 5368 6f77 2069    <string>Show i
+000031d0: 6e74 656e 7369 7469 6573 206f 6620 616c  ntensities of al
+000031e0: 6c20 7468 6520 6361 6c63 756c 6174 6564  l the calculated
+000031f0: 2070 6172 7469 636c 6573 3c2f 7374 7269   particles</stri
+00003200: 6e67 3e0a 2020 203c 2f70 726f 7065 7274  ng>.   </propert
+00003210: 793e 0a20 203c 2f61 6374 696f 6e3e 0a20  y>.  </action>. 
+00003220: 203c 6163 7469 6f6e 206e 616d 653d 2261   <action name="a
+00003230: 6374 696f 6e5f 7361 7665 5f64 6174 6122  ction_save_data"
+00003240: 3e0a 2020 203c 7072 6f70 6572 7479 206e  >.   <property n
+00003250: 616d 653d 2269 636f 6e22 3e0a 2020 2020  ame="icon">.    
+00003260: 3c69 636f 6e73 6574 3e0a 2020 2020 203c  <iconset>.     <
+00003270: 6e6f 726d 616c 6f66 663e 4963 6f6e 732f  normaloff>Icons/
+00003280: 5361 7665 2e73 7667 3c2f 6e6f 726d 616c  Save.svg</normal
+00003290: 6f66 663e 4963 6f6e 732f 5361 7665 2e73  off>Icons/Save.s
+000032a0: 7667 3c2f 6963 6f6e 7365 743e 0a20 2020  vg</iconset>.   
+000032b0: 3c2f 7072 6f70 6572 7479 3e0a 2020 203c  </property>.   <
+000032c0: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
+000032d0: 6578 7422 3e0a 2020 2020 3c73 7472 696e  ext">.    <strin
+000032e0: 673e 4578 706f 7274 3c2f 7374 7269 6e67  g>Export</string
+000032f0: 3e0a 2020 203c 2f70 726f 7065 7274 793e  >.   </property>
+00003300: 0a20 2020 3c70 726f 7065 7274 7920 6e61  .   <property na
+00003310: 6d65 3d22 746f 6f6c 5469 7022 3e0a 2020  me="toolTip">.  
+00003320: 2020 3c73 7472 696e 673e 4578 706f 7274    <string>Export
+00003330: 2064 6174 6120 746f 2043 5356 3c2f 7374   data to CSV</st
+00003340: 7269 6e67 3e0a 2020 203c 2f70 726f 7065  ring>.   </prope
+00003350: 7274 793e 0a20 203c 2f61 6374 696f 6e3e  rty>.  </action>
+00003360: 0a20 203c 6163 7469 6f6e 206e 616d 653d  .  <action name=
+00003370: 2261 6374 696f 6e41 6476 616e 6365 5f46  "actionAdvance_F
+00003380: 7261 6d65 223e 0a20 2020 3c70 726f 7065  rame">.   <prope
+00003390: 7274 7920 6e61 6d65 3d22 7465 7874 223e  rty name="text">
+000033a0: 0a20 2020 203c 7374 7269 6e67 3e49 6e63  .    <string>Inc
+000033b0: 7265 6173 6520 4672 616d 653c 2f73 7472  rease Frame</str
+000033c0: 696e 673e 0a20 2020 3c2f 7072 6f70 6572  ing>.   </proper
+000033d0: 7479 3e0a 2020 203c 7072 6f70 6572 7479  ty>.   <property
+000033e0: 206e 616d 653d 2273 686f 7274 6375 7422   name="shortcut"
+000033f0: 3e0a 2020 2020 3c73 7472 696e 673e 4d65  >.    <string>Me
+00003400: 7461 2b41 6c74 2b52 6967 6874 3c2f 7374  ta+Alt+Right</st
+00003410: 7269 6e67 3e0a 2020 203c 2f70 726f 7065  ring>.   </prope
+00003420: 7274 793e 0a20 203c 2f61 6374 696f 6e3e  rty>.  </action>
+00003430: 0a20 203c 6163 7469 6f6e 206e 616d 653d  .  <action name=
+00003440: 2261 6374 696f 6e44 6563 7265 6173 655f  "actionDecrease_
+00003450: 4672 616d 6522 3e0a 2020 203c 7072 6f70  Frame">.   <prop
+00003460: 6572 7479 206e 616d 653d 2274 6578 7422  erty name="text"
+00003470: 3e0a 2020 2020 3c73 7472 696e 673e 4465  >.    <string>De
+00003480: 6372 6561 7365 2046 7261 6d65 3c2f 7374  crease Frame</st
+00003490: 7269 6e67 3e0a 2020 203c 2f70 726f 7065  ring>.   </prope
+000034a0: 7274 793e 0a20 2020 3c70 726f 7065 7274  rty>.   <propert
+000034b0: 7920 6e61 6d65 3d22 7368 6f72 7463 7574  y name="shortcut
+000034c0: 223e 0a20 2020 203c 7374 7269 6e67 3e4d  ">.    <string>M
+000034d0: 6574 612b 416c 742b 4c65 6674 3c2f 7374  eta+Alt+Left</st
+000034e0: 7269 6e67 3e0a 2020 203c 2f70 726f 7065  ring>.   </prope
+000034f0: 7274 793e 0a20 203c 2f61 6374 696f 6e3e  rty>.  </action>
+00003500: 0a20 203c 6163 7469 6f6e 206e 616d 653d  .  <action name=
+00003510: 2261 6374 696f 6e47 6f5f 746f 5f64 6f63  "actionGo_to_doc
+00003520: 756d 656e 7461 7469 6f6e 223e 0a20 2020  umentation">.   
+00003530: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00003540: 7465 7874 223e 0a20 2020 203c 7374 7269  text">.    <stri
+00003550: 6e67 3e4f 7065 6e20 446f 6375 6d65 6e74  ng>Open Document
+00003560: 6174 696f 6e3c 2f73 7472 696e 673e 0a20  ation</string>. 
+00003570: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+00003580: 3c2f 6163 7469 6f6e 3e0a 2020 3c61 6374  </action>.  <act
+00003590: 696f 6e20 6e61 6d65 3d22 6163 7469 6f6e  ion name="action
+000035a0: 5f65 7870 6f72 745f 616c 6c5f 6461 7461  _export_all_data
+000035b0: 223e 0a20 2020 3c70 726f 7065 7274 7920  ">.   <property 
+000035c0: 6e61 6d65 3d22 7465 7874 223e 0a20 2020  name="text">.   
+000035d0: 203c 7374 7269 6e67 3e45 7870 6f72 7420   <string>Export 
+000035e0: 416c 6c20 4461 7461 3c2f 7374 7269 6e67  All Data</string
+000035f0: 3e0a 2020 203c 2f70 726f 7065 7274 793e  >.   </property>
+00003600: 0a20 2020 3c70 726f 7065 7274 7920 6e61  .   <property na
+00003610: 6d65 3d22 746f 6f6c 5469 7022 3e0a 2020  me="toolTip">.  
+00003620: 2020 3c73 7472 696e 673e 4578 706f 7274    <string>Export
+00003630: 2061 6c6c 2074 6865 2069 6e66 6f72 6d61   all the informa
+00003640: 7469 6f6e 2067 6174 6865 7265 6420 6f6e  tion gathered on
+00003650: 2070 6172 7469 636c 6573 3c2f 7374 7269   particles</stri
+00003660: 6e67 3e0a 2020 203c 2f70 726f 7065 7274  ng>.   </propert
+00003670: 793e 0a20 203c 2f61 6374 696f 6e3e 0a20  y>.  </action>. 
+00003680: 203c 6163 7469 6f6e 206e 616d 653d 2261   <action name="a
+00003690: 6374 696f 6e5f 6162 6f75 7422 3e0a 2020  ction_about">.  
+000036a0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+000036b0: 2274 6578 7422 3e0a 2020 2020 3c73 7472  "text">.    <str
+000036c0: 696e 673e 4162 6f75 743c 2f73 7472 696e  ing>About</strin
+000036d0: 673e 0a20 2020 3c2f 7072 6f70 6572 7479  g>.   </property
+000036e0: 3e0a 2020 203c 7072 6f70 6572 7479 206e  >.   <property n
+000036f0: 616d 653d 2274 6f6f 6c54 6970 223e 0a20  ame="toolTip">. 
+00003700: 2020 203c 7374 7269 6e67 3e41 626f 7574     <string>About
+00003710: 204e 616e 6f51 4e54 5079 3c2f 7374 7269   NanoQNTPy</stri
+00003720: 6e67 3e0a 2020 203c 2f70 726f 7065 7274  ng>.   </propert
+00003730: 793e 0a20 203c 2f61 6374 696f 6e3e 0a20  y>.  </action>. 
+00003740: 203c 6163 7469 6f6e 206e 616d 653d 2261   <action name="a
+00003750: 6374 696f 6e5f 6361 6c63 756c 6174 655f  ction_calculate_
+00003760: 626b 6722 3e0a 2020 203c 7072 6f70 6572  bkg">.   <proper
+00003770: 7479 206e 616d 653d 2274 6578 7422 3e0a  ty name="text">.
+00003780: 2020 2020 3c73 7472 696e 673e 4361 6c63      <string>Calc
+00003790: 756c 6174 6520 4261 636b 6772 6f75 6e64  ulate Background
+000037a0: 3c2f 7374 7269 6e67 3e0a 2020 203c 2f70  </string>.   </p
+000037b0: 726f 7065 7274 793e 0a20 203c 2f61 6374  roperty>.  </act
+000037c0: 696f 6e3e 0a20 203c 6163 7469 6f6e 206e  ion>.  <action n
+000037d0: 616d 653d 2261 6374 696f 6e5f 7368 6f77  ame="action_show
+000037e0: 5f62 6b67 223e 0a20 2020 3c70 726f 7065  _bkg">.   <prope
+000037f0: 7274 7920 6e61 6d65 3d22 7465 7874 223e  rty name="text">
+00003800: 0a20 2020 203c 7374 7269 6e67 3e53 686f  .    <string>Sho
+00003810: 7720 4261 636b 6772 6f75 6e64 3c2f 7374  w Background</st
+00003820: 7269 6e67 3e0a 2020 203c 2f70 726f 7065  ring>.   </prope
+00003830: 7274 793e 0a20 203c 2f61 6374 696f 6e3e  rty>.  </action>
+00003840: 0a20 3c2f 7769 6467 6574 3e0a 203c 7461  . </widget>. <ta
+00003850: 6273 746f 7073 3e0a 2020 3c74 6162 7374  bstops>.  <tabst
+00003860: 6f70 3e66 696e 645f 7061 7274 6963 6c65  op>find_particle
+00003870: 735f 6368 6563 6b3c 2f74 6162 7374 6f70  s_check</tabstop
+00003880: 3e0a 2020 3c74 6162 7374 6f70 3e73 7461  >.  <tabstop>sta
+00003890: 7274 5f66 7261 6d65 5f6c 696e 653c 2f74  rt_frame_line</t
+000038a0: 6162 7374 6f70 3e0a 2020 3c74 6162 7374  abstop>.  <tabst
+000038b0: 6f70 3e65 6e64 5f66 7261 6d65 5f6c 696e  op>end_frame_lin
+000038c0: 653c 2f74 6162 7374 6f70 3e0a 2020 3c74  e</tabstop>.  <t
+000038d0: 6162 7374 6f70 3e65 6e67 696e 655f 626f  abstop>engine_bo
+000038e0: 783c 2f74 6162 7374 6f70 3e0a 2020 3c74  x</tabstop>.  <t
+000038f0: 6162 7374 6f70 3e73 6561 7263 685f 7261  abstop>search_ra
+00003900: 6469 7573 5f6c 696e 653c 2f74 6162 7374  dius_line</tabst
+00003910: 6f70 3e0a 2020 3c74 6162 7374 6f70 3e6d  op>.  <tabstop>m
+00003920: 696e 5f66 7261 6d65 735f 6c69 6e65 3c2f  in_frames_line</
+00003930: 7461 6273 746f 703e 0a20 203c 7461 6273  tabstop>.  <tabs
+00003940: 746f 703e 6361 6c63 756c 6174 655f 6275  top>calculate_bu
+00003950: 7474 6f6e 3c2f 7461 6273 746f 703e 0a20  tton</tabstop>. 
+00003960: 203c 7461 6273 746f 703e 7374 6570 5f73   <tabstop>step_s
+00003970: 697a 655f 6c69 6e65 3c2f 7461 6273 746f  ize_line</tabsto
+00003980: 703e 0a20 203c 7461 6273 746f 703e 6672  p>.  <tabstop>fr
+00003990: 616d 655f 736c 6964 6572 3c2f 7461 6273  ame_slider</tabs
+000039a0: 746f 703e 0a20 3c2f 7461 6273 746f 7073  top>. </tabstops
+000039b0: 3e0a 203c 7265 736f 7572 6365 733e 0a20  >. <resources>. 
+000039c0: 203c 696e 636c 7564 6520 6c6f 6361 7469   <include locati
+000039d0: 6f6e 3d22 4963 6f6e 732f 4963 6f6e 732e  on="Icons/Icons.
+000039e0: 7172 6322 2f3e 0a20 3c2f 7265 736f 7572  qrc"/>. </resour
+000039f0: 6365 733e 0a20 3c63 6f6e 6e65 6374 696f  ces>. <connectio
+00003a00: 6e73 2f3e 0a3c 2f75 693e 0a              ns/>.</ui>.
```

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11814 - Atom.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11814 - Atom.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11815 - Battery.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11815 - Battery.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11816 - Orbit.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11816 - Orbit.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11817 - Beaker.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11817 - Beaker.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11819 - Bounce.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11819 - Bounce.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11820 - Caliper.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11820 - Caliper.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11821 - Catapult.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11821 - Catapult.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11822 - Collision.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11822 - Collision.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11828 - Energy.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11828 - Energy.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11829 - Flask.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11829 - Flask.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11830 - Float.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11830 - Float.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11832 - Force.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11832 - Force.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11833 - Formula.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11833 - Formula.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11834 - Gears.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11834 - Gears.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11835 - Gravity.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11835 - Gravity.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11837 - Histogram.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11837 - Histogram.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11839 - Magnet.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11839 - Magnet.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11841 - Metronome.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11841 - Metronome.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11843 - Molecule.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11843 - Molecule.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11844 - Motion.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11844 - Motion.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11848 - Planet.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11848 - Planet.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11850 - Power.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11850 - Power.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11851 - Press.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11851 - Press.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11852 - Proton.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11852 - Proton.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11853 - Pulley.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11853 - Pulley.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11854 - Reflection.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11854 - Reflection.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11855 - Resistor.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11855 - Resistor.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11856 - Rolling.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11856 - Rolling.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11857 - Rotate.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11857 - Rotate.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11859 - Temperature.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11859 - Temperature.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11861 - Waves.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11861 - Waves.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/Icons/Save.svg` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/Save.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0/nanoqnt/view/GUI/scan_control.ui` & `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/scan_control.ui`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, Unicode text, UTF-8 text, with CRLF line terminators*

 * *Files 24% similar despite different names*

```diff
@@ -1,219 +1,211 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0d0a 3c75 6920 7665 7273  F-8"?>..<ui vers
-00000030: 696f 6e3d 2234 2e30 223e 0d0a 203c 636c  ion="4.0">.. <cl
-00000040: 6173 733e 4d61 696e 5769 6e64 6f77 3c2f  ass>MainWindow</
-00000050: 636c 6173 733e 0d0a 203c 7769 6467 6574  class>.. <widget
-00000060: 2063 6c61 7373 3d22 514d 6169 6e57 696e   class="QMainWin
-00000070: 646f 7722 206e 616d 653d 224d 6169 6e57  dow" name="MainW
-00000080: 696e 646f 7722 3e0d 0a20 203c 7072 6f70  indow">..  <prop
-00000090: 6572 7479 206e 616d 653d 2267 656f 6d65  erty name="geome
-000000a0: 7472 7922 3e0d 0a20 2020 3c72 6563 743e  try">..   <rect>
-000000b0: 0d0a 2020 2020 3c78 3e30 3c2f 783e 0d0a  ..    <x>0</x>..
-000000c0: 2020 2020 3c79 3e30 3c2f 793e 0d0a 2020      <y>0</y>..  
-000000d0: 2020 3c77 6964 7468 3e33 3734 3c2f 7769    <width>374</wi
-000000e0: 6474 683e 0d0a 2020 2020 3c68 6569 6768  dth>..    <heigh
-000000f0: 743e 3233 353c 2f68 6569 6768 743e 0d0a  t>235</height>..
-00000100: 2020 203c 2f72 6563 743e 0d0a 2020 3c2f     </rect>..  </
-00000110: 7072 6f70 6572 7479 3e0d 0a20 203c 7072  property>..  <pr
-00000120: 6f70 6572 7479 206e 616d 653d 2277 696e  operty name="win
-00000130: 646f 7754 6974 6c65 223e 0d0a 2020 203c  dowTitle">..   <
-00000140: 7374 7269 6e67 3e4d 6169 6e57 696e 646f  string>MainWindo
-00000150: 773c 2f73 7472 696e 673e 0d0a 2020 3c2f  w</string>..  </
-00000160: 7072 6f70 6572 7479 3e0d 0a20 203c 7769  property>..  <wi
-00000170: 6467 6574 2063 6c61 7373 3d22 5157 6964  dget class="QWid
-00000180: 6765 7422 206e 616d 653d 2263 656e 7472  get" name="centr
-00000190: 616c 7769 6467 6574 223e 0d0a 2020 203c  alwidget">..   <
-000001a0: 6c61 796f 7574 2063 6c61 7373 3d22 5156  layout class="QV
-000001b0: 426f 784c 6179 6f75 7422 206e 616d 653d  BoxLayout" name=
-000001c0: 2276 6572 7469 6361 6c4c 6179 6f75 7422  "verticalLayout"
-000001d0: 3e0d 0a20 2020 203c 6974 656d 3e0d 0a20  >..    <item>.. 
-000001e0: 2020 2020 3c6c 6179 6f75 7420 636c 6173      <layout clas
-000001f0: 733d 2251 466f 726d 4c61 796f 7574 2220  s="QFormLayout" 
-00000200: 6e61 6d65 3d22 666f 726d 4c61 796f 7574  name="formLayout
-00000210: 223e 0d0a 2020 2020 2020 3c69 7465 6d20  ">..      <item 
-00000220: 726f 773d 2230 2220 636f 6c75 6d6e 3d22  row="0" column="
-00000230: 3022 3e0d 0a20 2020 2020 2020 3c77 6964  0">..       <wid
-00000240: 6765 7420 636c 6173 733d 2251 4c61 6265  get class="QLabe
-00000250: 6c22 206e 616d 653d 226c 6162 656c 223e  l" name="label">
-00000260: 0d0a 2020 2020 2020 2020 3c70 726f 7065  ..        <prope
-00000270: 7274 7920 6e61 6d65 3d22 7465 7874 223e  rty name="text">
-00000280: 0d0a 2020 2020 2020 2020 203c 7374 7269  ..         <stri
-00000290: 6e67 3e53 7461 7274 2028 c2b5 6d29 3c2f  ng>Start (..m)</
-000002a0: 7374 7269 6e67 3e0d 0a20 2020 2020 2020  string>..       
-000002b0: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
-000002c0: 2020 2020 203c 2f77 6964 6765 743e 0d0a       </widget>..
-000002d0: 2020 2020 2020 3c2f 6974 656d 3e0d 0a20        </item>.. 
-000002e0: 2020 2020 203c 6974 656d 2072 6f77 3d22       <item row="
-000002f0: 3022 2063 6f6c 756d 6e3d 2231 223e 0d0a  0" column="1">..
-00000300: 2020 2020 2020 203c 7769 6467 6574 2063         <widget c
-00000310: 6c61 7373 3d22 514c 696e 6545 6469 7422  lass="QLineEdit"
-00000320: 206e 616d 653d 2273 7461 7274 5f6c 696e   name="start_lin
-00000330: 6522 3e0d 0a20 2020 2020 2020 203c 7072  e">..        <pr
-00000340: 6f70 6572 7479 206e 616d 653d 2274 6578  operty name="tex
-00000350: 7422 3e0d 0a20 2020 2020 2020 2020 3c73  t">..         <s
-00000360: 7472 696e 673e 303c 2f73 7472 696e 673e  tring>0</string>
-00000370: 0d0a 2020 2020 2020 2020 3c2f 7072 6f70  ..        </prop
-00000380: 6572 7479 3e0d 0a20 2020 2020 2020 3c2f  erty>..       </
-00000390: 7769 6467 6574 3e0d 0a20 2020 2020 203c  widget>..      <
-000003a0: 2f69 7465 6d3e 0d0a 2020 2020 2020 3c69  /item>..      <i
-000003b0: 7465 6d20 726f 773d 2231 2220 636f 6c75  tem row="1" colu
-000003c0: 6d6e 3d22 3022 3e0d 0a20 2020 2020 2020  mn="0">..       
-000003d0: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
-000003e0: 4c61 6265 6c22 206e 616d 653d 226c 6162  Label" name="lab
-000003f0: 656c 5f32 223e 0d0a 2020 2020 2020 2020  el_2">..        
-00000400: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00000410: 7465 7874 223e 0d0a 2020 2020 2020 2020  text">..        
-00000420: 203c 7374 7269 6e67 3e53 746f 7020 28c2   <string>Stop (.
-00000430: b56d 293c 2f73 7472 696e 673e 0d0a 2020  .m)</string>..  
-00000440: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
-00000450: 3e0d 0a20 2020 2020 2020 3c2f 7769 6467  >..       </widg
-00000460: 6574 3e0d 0a20 2020 2020 203c 2f69 7465  et>..      </ite
-00000470: 6d3e 0d0a 2020 2020 2020 3c69 7465 6d20  m>..      <item 
-00000480: 726f 773d 2231 2220 636f 6c75 6d6e 3d22  row="1" column="
-00000490: 3122 3e0d 0a20 2020 2020 2020 3c77 6964  1">..       <wid
-000004a0: 6765 7420 636c 6173 733d 2251 4c69 6e65  get class="QLine
-000004b0: 4564 6974 2220 6e61 6d65 3d22 7374 6f70  Edit" name="stop
-000004c0: 5f6c 696e 6522 3e0d 0a20 2020 2020 2020  _line">..       
-000004d0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-000004e0: 2274 6578 7422 3e0d 0a20 2020 2020 2020  "text">..       
-000004f0: 2020 3c73 7472 696e 673e 3235 3030 3c2f    <string>2500</
-00000500: 7374 7269 6e67 3e0d 0a20 2020 2020 2020  string>..       
-00000510: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
-00000520: 2020 2020 203c 2f77 6964 6765 743e 0d0a       </widget>..
-00000530: 2020 2020 2020 3c2f 6974 656d 3e0d 0a20        </item>.. 
-00000540: 2020 2020 203c 6974 656d 2072 6f77 3d22       <item row="
-00000550: 3222 2063 6f6c 756d 6e3d 2230 223e 0d0a  2" column="0">..
-00000560: 2020 2020 2020 203c 7769 6467 6574 2063         <widget c
-00000570: 6c61 7373 3d22 514c 6162 656c 2220 6e61  lass="QLabel" na
-00000580: 6d65 3d22 6c61 6265 6c5f 3322 3e0d 0a20  me="label_3">.. 
-00000590: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-000005a0: 206e 616d 653d 2274 6578 7422 3e0d 0a20   name="text">.. 
-000005b0: 2020 2020 2020 2020 3c73 7472 696e 673e          <string>
-000005c0: 5374 6570 2028 c2b5 6d29 3c2f 7374 7269  Step (..m)</stri
-000005d0: 6e67 3e0d 0a20 2020 2020 2020 203c 2f70  ng>..        </p
-000005e0: 726f 7065 7274 793e 0d0a 2020 2020 2020  roperty>..      
-000005f0: 203c 2f77 6964 6765 743e 0d0a 2020 2020   </widget>..    
-00000600: 2020 3c2f 6974 656d 3e0d 0a20 2020 2020    </item>..     
-00000610: 203c 6974 656d 2072 6f77 3d22 3222 2063   <item row="2" c
-00000620: 6f6c 756d 6e3d 2231 223e 0d0a 2020 2020  olumn="1">..    
-00000630: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
-00000640: 3d22 514c 696e 6545 6469 7422 206e 616d  ="QLineEdit" nam
-00000650: 653d 2273 7465 705f 6c69 6e65 223e 0d0a  e="step_line">..
-00000660: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00000670: 7920 6e61 6d65 3d22 7465 7874 223e 0d0a  y name="text">..
-00000680: 2020 2020 2020 2020 203c 7374 7269 6e67           <string
-00000690: 3e35 3c2f 7374 7269 6e67 3e0d 0a20 2020  >5</string>..   
-000006a0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-000006b0: 0d0a 2020 2020 2020 203c 2f77 6964 6765  ..       </widge
-000006c0: 743e 0d0a 2020 2020 2020 3c2f 6974 656d  t>..      </item
-000006d0: 3e0d 0a20 2020 2020 3c2f 6c61 796f 7574  >..     </layout
-000006e0: 3e0d 0a20 2020 203c 2f69 7465 6d3e 0d0a  >..    </item>..
-000006f0: 2020 2020 3c69 7465 6d3e 0d0a 2020 2020      <item>..    
-00000700: 203c 6c61 796f 7574 2063 6c61 7373 3d22   <layout class="
-00000710: 5148 426f 784c 6179 6f75 7422 206e 616d  QHBoxLayout" nam
-00000720: 653d 2268 6f72 697a 6f6e 7461 6c4c 6179  e="horizontalLay
-00000730: 6f75 7422 3e0d 0a20 2020 2020 203c 6974  out">..      <it
-00000740: 656d 3e0d 0a20 2020 2020 2020 3c77 6964  em>..       <wid
-00000750: 6765 7420 636c 6173 733d 2251 5075 7368  get class="QPush
-00000760: 4275 7474 6f6e 2220 6e61 6d65 3d22 7374  Button" name="st
-00000770: 6172 745f 6c69 7665 5f62 7574 746f 6e22  art_live_button"
-00000780: 3e0d 0a20 2020 2020 2020 203c 7072 6f70  >..        <prop
-00000790: 6572 7479 206e 616d 653d 2274 6578 7422  erty name="text"
-000007a0: 3e0d 0a20 2020 2020 2020 2020 3c73 7472  >..         <str
-000007b0: 696e 673e 5374 6172 7420 4c69 7665 3c2f  ing>Start Live</
-000007c0: 7374 7269 6e67 3e0d 0a20 2020 2020 2020  string>..       
-000007d0: 203c 2f70 726f 7065 7274 793e 0d0a 2020   </property>..  
-000007e0: 2020 2020 203c 2f77 6964 6765 743e 0d0a       </widget>..
-000007f0: 2020 2020 2020 3c2f 6974 656d 3e0d 0a20        </item>.. 
-00000800: 2020 2020 203c 6974 656d 3e0d 0a20 2020       <item>..   
-00000810: 2020 2020 3c77 6964 6765 7420 636c 6173      <widget clas
-00000820: 733d 2251 5075 7368 4275 7474 6f6e 2220  s="QPushButton" 
-00000830: 6e61 6d65 3d22 7374 6f70 5f6c 6976 655f  name="stop_live_
-00000840: 6275 7474 6f6e 223e 0d0a 2020 2020 2020  button">..      
-00000850: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00000860: 3d22 7465 7874 223e 0d0a 2020 2020 2020  ="text">..      
-00000870: 2020 203c 7374 7269 6e67 3e53 746f 7020     <string>Stop 
-00000880: 4c69 7665 3c2f 7374 7269 6e67 3e0d 0a20  Live</string>.. 
-00000890: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
-000008a0: 793e 0d0a 2020 2020 2020 203c 2f77 6964  y>..       </wid
-000008b0: 6765 743e 0d0a 2020 2020 2020 3c2f 6974  get>..      </it
-000008c0: 656d 3e0d 0a20 2020 2020 203c 6974 656d  em>..      <item
-000008d0: 3e0d 0a20 2020 2020 2020 3c77 6964 6765  >..       <widge
-000008e0: 7420 636c 6173 733d 2251 5075 7368 4275  t class="QPushBu
-000008f0: 7474 6f6e 2220 6e61 6d65 3d22 7363 616e  tton" name="scan
-00000900: 5f62 7574 746f 6e22 3e0d 0a20 2020 2020  _button">..     
-00000910: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00000920: 653d 2274 6578 7422 3e0d 0a20 2020 2020  e="text">..     
-00000930: 2020 2020 3c73 7472 696e 673e 5363 616e      <string>Scan
-00000940: 3c2f 7374 7269 6e67 3e0d 0a20 2020 2020  </string>..     
-00000950: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-00000960: 2020 2020 2020 203c 2f77 6964 6765 743e         </widget>
-00000970: 0d0a 2020 2020 2020 3c2f 6974 656d 3e0d  ..      </item>.
-00000980: 0a20 2020 2020 203c 6974 656d 3e0d 0a20  .      <item>.. 
-00000990: 2020 2020 2020 3c77 6964 6765 7420 636c        <widget cl
-000009a0: 6173 733d 2251 5075 7368 4275 7474 6f6e  ass="QPushButton
-000009b0: 2220 6e61 6d65 3d22 736e 6170 5f62 7574  " name="snap_but
-000009c0: 746f 6e22 3e0d 0a20 2020 2020 2020 203c  ton">..        <
-000009d0: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
-000009e0: 6578 7422 3e0d 0a20 2020 2020 2020 2020  ext">..         
-000009f0: 3c73 7472 696e 673e 536e 6170 3c2f 7374  <string>Snap</st
-00000a00: 7269 6e67 3e0d 0a20 2020 2020 2020 203c  ring>..        <
-00000a10: 2f70 726f 7065 7274 793e 0d0a 2020 2020  /property>..    
-00000a20: 2020 203c 2f77 6964 6765 743e 0d0a 2020     </widget>..  
-00000a30: 2020 2020 3c2f 6974 656d 3e0d 0a20 2020      </item>..   
-00000a40: 2020 3c2f 6c61 796f 7574 3e0d 0a20 2020    </layout>..   
-00000a50: 203c 2f69 7465 6d3e 0d0a 2020 2020 3c69   </item>..    <i
-00000a60: 7465 6d3e 0d0a 2020 2020 203c 6c61 796f  tem>..     <layo
-00000a70: 7574 2063 6c61 7373 3d22 5146 6f72 6d4c  ut class="QFormL
-00000a80: 6179 6f75 7422 206e 616d 653d 2266 6f72  ayout" name="for
-00000a90: 6d4c 6179 6f75 745f 3222 3e0d 0a20 2020  mLayout_2">..   
-00000aa0: 2020 203c 6974 656d 2072 6f77 3d22 3022     <item row="0"
-00000ab0: 2063 6f6c 756d 6e3d 2230 223e 0d0a 2020   column="0">..  
-00000ac0: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
-00000ad0: 7373 3d22 5150 7573 6842 7574 746f 6e22  ss="QPushButton"
-00000ae0: 206e 616d 653d 2267 6f74 6f5f 6275 7474   name="goto_butt
-00000af0: 6f6e 223e 0d0a 2020 2020 2020 2020 3c70  on">..        <p
-00000b00: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
-00000b10: 7874 223e 0d0a 2020 2020 2020 2020 203c  xt">..         <
-00000b20: 7374 7269 6e67 3e47 6f20 546f 2028 c2b5  string>Go To (..
-00000b30: 6d29 3c2f 7374 7269 6e67 3e0d 0a20 2020  m)</string>..   
-00000b40: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00000b50: 0d0a 2020 2020 2020 203c 2f77 6964 6765  ..       </widge
-00000b60: 743e 0d0a 2020 2020 2020 3c2f 6974 656d  t>..      </item
-00000b70: 3e0d 0a20 2020 2020 203c 6974 656d 2072  >..      <item r
-00000b80: 6f77 3d22 3022 2063 6f6c 756d 6e3d 2231  ow="0" column="1
-00000b90: 223e 0d0a 2020 2020 2020 203c 7769 6467  ">..       <widg
-00000ba0: 6574 2063 6c61 7373 3d22 514c 696e 6545  et class="QLineE
-00000bb0: 6469 7422 206e 616d 653d 2267 6f74 6f5f  dit" name="goto_
-00000bc0: 6c69 6e65 223e 0d0a 2020 2020 2020 2020  line">..        
-00000bd0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00000be0: 7465 7874 223e 0d0a 2020 2020 2020 2020  text">..        
-00000bf0: 203c 7374 7269 6e67 3e30 3c2f 7374 7269   <string>0</stri
-00000c00: 6e67 3e0d 0a20 2020 2020 2020 203c 2f70  ng>..        </p
-00000c10: 726f 7065 7274 793e 0d0a 2020 2020 2020  roperty>..      
-00000c20: 203c 2f77 6964 6765 743e 0d0a 2020 2020   </widget>..    
-00000c30: 2020 3c2f 6974 656d 3e0d 0a20 2020 2020    </item>..     
-00000c40: 3c2f 6c61 796f 7574 3e0d 0a20 2020 203c  </layout>..    <
-00000c50: 2f69 7465 6d3e 0d0a 2020 203c 2f6c 6179  /item>..   </lay
-00000c60: 6f75 743e 0d0a 2020 3c2f 7769 6467 6574  out>..  </widget
-00000c70: 3e0d 0a20 203c 7769 6467 6574 2063 6c61  >..  <widget cla
-00000c80: 7373 3d22 514d 656e 7542 6172 2220 6e61  ss="QMenuBar" na
-00000c90: 6d65 3d22 6d65 6e75 6261 7222 3e0d 0a20  me="menubar">.. 
-00000ca0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00000cb0: 3d22 6765 6f6d 6574 7279 223e 0d0a 2020  ="geometry">..  
-00000cc0: 2020 3c72 6563 743e 0d0a 2020 2020 203c    <rect>..     <
-00000cd0: 783e 303c 2f78 3e0d 0a20 2020 2020 3c79  x>0</x>..     <y
-00000ce0: 3e30 3c2f 793e 0d0a 2020 2020 203c 7769  >0</y>..     <wi
-00000cf0: 6474 683e 3337 343c 2f77 6964 7468 3e0d  dth>374</width>.
-00000d00: 0a20 2020 2020 3c68 6569 6768 743e 3234  .     <height>24
-00000d10: 3c2f 6865 6967 6874 3e0d 0a20 2020 203c  </height>..    <
-00000d20: 2f72 6563 743e 0d0a 2020 203c 2f70 726f  /rect>..   </pro
-00000d30: 7065 7274 793e 0d0a 2020 3c2f 7769 6467  perty>..  </widg
-00000d40: 6574 3e0d 0a20 203c 7769 6467 6574 2063  et>..  <widget c
-00000d50: 6c61 7373 3d22 5153 7461 7475 7342 6172  lass="QStatusBar
-00000d60: 2220 6e61 6d65 3d22 7374 6174 7573 6261  " name="statusba
-00000d70: 7222 2f3e 0d0a 203c 2f77 6964 6765 743e  r"/>.. </widget>
-00000d80: 0d0a 203c 7265 736f 7572 6365 732f 3e0d  .. <resources/>.
-00000d90: 0a20 3c63 6f6e 6e65 6374 696f 6e73 2f3e  . <connections/>
-00000da0: 0d0a 3c2f 7569 3e0d 0a                   ..</ui>..
+00000020: 462d 3822 3f3e 0a3c 7569 2076 6572 7369  F-8"?>.<ui versi
+00000030: 6f6e 3d22 342e 3022 3e0a 203c 636c 6173  on="4.0">. <clas
+00000040: 733e 4d61 696e 5769 6e64 6f77 3c2f 636c  s>MainWindow</cl
+00000050: 6173 733e 0a20 3c77 6964 6765 7420 636c  ass>. <widget cl
+00000060: 6173 733d 2251 4d61 696e 5769 6e64 6f77  ass="QMainWindow
+00000070: 2220 6e61 6d65 3d22 4d61 696e 5769 6e64  " name="MainWind
+00000080: 6f77 223e 0a20 203c 7072 6f70 6572 7479  ow">.  <property
+00000090: 206e 616d 653d 2267 656f 6d65 7472 7922   name="geometry"
+000000a0: 3e0a 2020 203c 7265 6374 3e0a 2020 2020  >.   <rect>.    
+000000b0: 3c78 3e30 3c2f 783e 0a20 2020 203c 793e  <x>0</x>.    <y>
+000000c0: 303c 2f79 3e0a 2020 2020 3c77 6964 7468  0</y>.    <width
+000000d0: 3e33 3734 3c2f 7769 6474 683e 0a20 2020  >374</width>.   
+000000e0: 203c 6865 6967 6874 3e32 3335 3c2f 6865   <height>235</he
+000000f0: 6967 6874 3e0a 2020 203c 2f72 6563 743e  ight>.   </rect>
+00000100: 0a20 203c 2f70 726f 7065 7274 793e 0a20  .  </property>. 
+00000110: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000120: 2277 696e 646f 7754 6974 6c65 223e 0a20  "windowTitle">. 
+00000130: 2020 3c73 7472 696e 673e 4d61 696e 5769    <string>MainWi
+00000140: 6e64 6f77 3c2f 7374 7269 6e67 3e0a 2020  ndow</string>.  
+00000150: 3c2f 7072 6f70 6572 7479 3e0a 2020 3c77  </property>.  <w
+00000160: 6964 6765 7420 636c 6173 733d 2251 5769  idget class="QWi
+00000170: 6467 6574 2220 6e61 6d65 3d22 6365 6e74  dget" name="cent
+00000180: 7261 6c77 6964 6765 7422 3e0a 2020 203c  ralwidget">.   <
+00000190: 6c61 796f 7574 2063 6c61 7373 3d22 5156  layout class="QV
+000001a0: 426f 784c 6179 6f75 7422 206e 616d 653d  BoxLayout" name=
+000001b0: 2276 6572 7469 6361 6c4c 6179 6f75 7422  "verticalLayout"
+000001c0: 3e0a 2020 2020 3c69 7465 6d3e 0a20 2020  >.    <item>.   
+000001d0: 2020 3c6c 6179 6f75 7420 636c 6173 733d    <layout class=
+000001e0: 2251 466f 726d 4c61 796f 7574 2220 6e61  "QFormLayout" na
+000001f0: 6d65 3d22 666f 726d 4c61 796f 7574 223e  me="formLayout">
+00000200: 0a20 2020 2020 203c 6974 656d 2072 6f77  .      <item row
+00000210: 3d22 3022 2063 6f6c 756d 6e3d 2230 223e  ="0" column="0">
+00000220: 0a20 2020 2020 2020 3c77 6964 6765 7420  .       <widget 
+00000230: 636c 6173 733d 2251 4c61 6265 6c22 206e  class="QLabel" n
+00000240: 616d 653d 226c 6162 656c 223e 0a20 2020  ame="label">.   
+00000250: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00000260: 616d 653d 2274 6578 7422 3e0a 2020 2020  ame="text">.    
+00000270: 2020 2020 203c 7374 7269 6e67 3e53 7461       <string>Sta
+00000280: 7274 2028 c2b5 6d29 3c2f 7374 7269 6e67  rt (..m)</string
+00000290: 3e0a 2020 2020 2020 2020 3c2f 7072 6f70  >.        </prop
+000002a0: 6572 7479 3e0a 2020 2020 2020 203c 2f77  erty>.       </w
+000002b0: 6964 6765 743e 0a20 2020 2020 203c 2f69  idget>.      </i
+000002c0: 7465 6d3e 0a20 2020 2020 203c 6974 656d  tem>.      <item
+000002d0: 2072 6f77 3d22 3022 2063 6f6c 756d 6e3d   row="0" column=
+000002e0: 2231 223e 0a20 2020 2020 2020 3c77 6964  "1">.       <wid
+000002f0: 6765 7420 636c 6173 733d 2251 4c69 6e65  get class="QLine
+00000300: 4564 6974 2220 6e61 6d65 3d22 7374 6172  Edit" name="star
+00000310: 745f 6c69 6e65 223e 0a20 2020 2020 2020  t_line">.       
+00000320: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000330: 2274 6578 7422 3e0a 2020 2020 2020 2020  "text">.        
+00000340: 203c 7374 7269 6e67 3e30 3c2f 7374 7269   <string>0</stri
+00000350: 6e67 3e0a 2020 2020 2020 2020 3c2f 7072  ng>.        </pr
+00000360: 6f70 6572 7479 3e0a 2020 2020 2020 203c  operty>.       <
+00000370: 2f77 6964 6765 743e 0a20 2020 2020 203c  /widget>.      <
+00000380: 2f69 7465 6d3e 0a20 2020 2020 203c 6974  /item>.      <it
+00000390: 656d 2072 6f77 3d22 3122 2063 6f6c 756d  em row="1" colum
+000003a0: 6e3d 2230 223e 0a20 2020 2020 2020 3c77  n="0">.       <w
+000003b0: 6964 6765 7420 636c 6173 733d 2251 4c61  idget class="QLa
+000003c0: 6265 6c22 206e 616d 653d 226c 6162 656c  bel" name="label
+000003d0: 5f32 223e 0a20 2020 2020 2020 203c 7072  _2">.        <pr
+000003e0: 6f70 6572 7479 206e 616d 653d 2274 6578  operty name="tex
+000003f0: 7422 3e0a 2020 2020 2020 2020 203c 7374  t">.         <st
+00000400: 7269 6e67 3e53 746f 7020 28c2 b56d 293c  ring>Stop (..m)<
+00000410: 2f73 7472 696e 673e 0a20 2020 2020 2020  /string>.       
+00000420: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+00000430: 2020 2020 3c2f 7769 6467 6574 3e0a 2020      </widget>.  
+00000440: 2020 2020 3c2f 6974 656d 3e0a 2020 2020      </item>.    
+00000450: 2020 3c69 7465 6d20 726f 773d 2231 2220    <item row="1" 
+00000460: 636f 6c75 6d6e 3d22 3122 3e0a 2020 2020  column="1">.    
+00000470: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
+00000480: 3d22 514c 696e 6545 6469 7422 206e 616d  ="QLineEdit" nam
+00000490: 653d 2273 746f 705f 6c69 6e65 223e 0a20  e="stop_line">. 
+000004a0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+000004b0: 206e 616d 653d 2274 6578 7422 3e0a 2020   name="text">.  
+000004c0: 2020 2020 2020 203c 7374 7269 6e67 3e32         <string>2
+000004d0: 3530 303c 2f73 7472 696e 673e 0a20 2020  500</string>.   
+000004e0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
+000004f0: 0a20 2020 2020 2020 3c2f 7769 6467 6574  .       </widget
+00000500: 3e0a 2020 2020 2020 3c2f 6974 656d 3e0a  >.      </item>.
+00000510: 2020 2020 2020 3c69 7465 6d20 726f 773d        <item row=
+00000520: 2232 2220 636f 6c75 6d6e 3d22 3022 3e0a  "2" column="0">.
+00000530: 2020 2020 2020 203c 7769 6467 6574 2063         <widget c
+00000540: 6c61 7373 3d22 514c 6162 656c 2220 6e61  lass="QLabel" na
+00000550: 6d65 3d22 6c61 6265 6c5f 3322 3e0a 2020  me="label_3">.  
+00000560: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00000570: 6e61 6d65 3d22 7465 7874 223e 0a20 2020  name="text">.   
+00000580: 2020 2020 2020 3c73 7472 696e 673e 5374        <string>St
+00000590: 6570 2028 c2b5 6d29 3c2f 7374 7269 6e67  ep (..m)</string
+000005a0: 3e0a 2020 2020 2020 2020 3c2f 7072 6f70  >.        </prop
+000005b0: 6572 7479 3e0a 2020 2020 2020 203c 2f77  erty>.       </w
+000005c0: 6964 6765 743e 0a20 2020 2020 203c 2f69  idget>.      </i
+000005d0: 7465 6d3e 0a20 2020 2020 203c 6974 656d  tem>.      <item
+000005e0: 2072 6f77 3d22 3222 2063 6f6c 756d 6e3d   row="2" column=
+000005f0: 2231 223e 0a20 2020 2020 2020 3c77 6964  "1">.       <wid
+00000600: 6765 7420 636c 6173 733d 2251 4c69 6e65  get class="QLine
+00000610: 4564 6974 2220 6e61 6d65 3d22 7374 6570  Edit" name="step
+00000620: 5f6c 696e 6522 3e0a 2020 2020 2020 2020  _line">.        
+00000630: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00000640: 7465 7874 223e 0a20 2020 2020 2020 2020  text">.         
+00000650: 3c73 7472 696e 673e 353c 2f73 7472 696e  <string>5</strin
+00000660: 673e 0a20 2020 2020 2020 203c 2f70 726f  g>.        </pro
+00000670: 7065 7274 793e 0a20 2020 2020 2020 3c2f  perty>.       </
+00000680: 7769 6467 6574 3e0a 2020 2020 2020 3c2f  widget>.      </
+00000690: 6974 656d 3e0a 2020 2020 203c 2f6c 6179  item>.     </lay
+000006a0: 6f75 743e 0a20 2020 203c 2f69 7465 6d3e  out>.    </item>
+000006b0: 0a20 2020 203c 6974 656d 3e0a 2020 2020  .    <item>.    
+000006c0: 203c 6c61 796f 7574 2063 6c61 7373 3d22   <layout class="
+000006d0: 5148 426f 784c 6179 6f75 7422 206e 616d  QHBoxLayout" nam
+000006e0: 653d 2268 6f72 697a 6f6e 7461 6c4c 6179  e="horizontalLay
+000006f0: 6f75 7422 3e0a 2020 2020 2020 3c69 7465  out">.      <ite
+00000700: 6d3e 0a20 2020 2020 2020 3c77 6964 6765  m>.       <widge
+00000710: 7420 636c 6173 733d 2251 5075 7368 4275  t class="QPushBu
+00000720: 7474 6f6e 2220 6e61 6d65 3d22 7374 6172  tton" name="star
+00000730: 745f 6c69 7665 5f62 7574 746f 6e22 3e0a  t_live_button">.
+00000740: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00000750: 7920 6e61 6d65 3d22 7465 7874 223e 0a20  y name="text">. 
+00000760: 2020 2020 2020 2020 3c73 7472 696e 673e          <string>
+00000770: 5374 6172 7420 4c69 7665 3c2f 7374 7269  Start Live</stri
+00000780: 6e67 3e0a 2020 2020 2020 2020 3c2f 7072  ng>.        </pr
+00000790: 6f70 6572 7479 3e0a 2020 2020 2020 203c  operty>.       <
+000007a0: 2f77 6964 6765 743e 0a20 2020 2020 203c  /widget>.      <
+000007b0: 2f69 7465 6d3e 0a20 2020 2020 203c 6974  /item>.      <it
+000007c0: 656d 3e0a 2020 2020 2020 203c 7769 6467  em>.       <widg
+000007d0: 6574 2063 6c61 7373 3d22 5150 7573 6842  et class="QPushB
+000007e0: 7574 746f 6e22 206e 616d 653d 2273 746f  utton" name="sto
+000007f0: 705f 6c69 7665 5f62 7574 746f 6e22 3e0a  p_live_button">.
+00000800: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00000810: 7920 6e61 6d65 3d22 7465 7874 223e 0a20  y name="text">. 
+00000820: 2020 2020 2020 2020 3c73 7472 696e 673e          <string>
+00000830: 5374 6f70 204c 6976 653c 2f73 7472 696e  Stop Live</strin
+00000840: 673e 0a20 2020 2020 2020 203c 2f70 726f  g>.        </pro
+00000850: 7065 7274 793e 0a20 2020 2020 2020 3c2f  perty>.       </
+00000860: 7769 6467 6574 3e0a 2020 2020 2020 3c2f  widget>.      </
+00000870: 6974 656d 3e0a 2020 2020 2020 3c69 7465  item>.      <ite
+00000880: 6d3e 0a20 2020 2020 2020 3c77 6964 6765  m>.       <widge
+00000890: 7420 636c 6173 733d 2251 5075 7368 4275  t class="QPushBu
+000008a0: 7474 6f6e 2220 6e61 6d65 3d22 7363 616e  tton" name="scan
+000008b0: 5f62 7574 746f 6e22 3e0a 2020 2020 2020  _button">.      
+000008c0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+000008d0: 3d22 7465 7874 223e 0a20 2020 2020 2020  ="text">.       
+000008e0: 2020 3c73 7472 696e 673e 5363 616e 3c2f    <string>Scan</
+000008f0: 7374 7269 6e67 3e0a 2020 2020 2020 2020  string>.        
+00000900: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00000910: 2020 203c 2f77 6964 6765 743e 0a20 2020     </widget>.   
+00000920: 2020 203c 2f69 7465 6d3e 0a20 2020 2020     </item>.     
+00000930: 203c 6974 656d 3e0a 2020 2020 2020 203c   <item>.       <
+00000940: 7769 6467 6574 2063 6c61 7373 3d22 5150  widget class="QP
+00000950: 7573 6842 7574 746f 6e22 206e 616d 653d  ushButton" name=
+00000960: 2273 6e61 705f 6275 7474 6f6e 223e 0a20  "snap_button">. 
+00000970: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00000980: 206e 616d 653d 2274 6578 7422 3e0a 2020   name="text">.  
+00000990: 2020 2020 2020 203c 7374 7269 6e67 3e53         <string>S
+000009a0: 6e61 703c 2f73 7472 696e 673e 0a20 2020  nap</string>.   
+000009b0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
+000009c0: 0a20 2020 2020 2020 3c2f 7769 6467 6574  .       </widget
+000009d0: 3e0a 2020 2020 2020 3c2f 6974 656d 3e0a  >.      </item>.
+000009e0: 2020 2020 203c 2f6c 6179 6f75 743e 0a20       </layout>. 
+000009f0: 2020 203c 2f69 7465 6d3e 0a20 2020 203c     </item>.    <
+00000a00: 6974 656d 3e0a 2020 2020 203c 6c61 796f  item>.     <layo
+00000a10: 7574 2063 6c61 7373 3d22 5146 6f72 6d4c  ut class="QFormL
+00000a20: 6179 6f75 7422 206e 616d 653d 2266 6f72  ayout" name="for
+00000a30: 6d4c 6179 6f75 745f 3222 3e0a 2020 2020  mLayout_2">.    
+00000a40: 2020 3c69 7465 6d20 726f 773d 2230 2220    <item row="0" 
+00000a50: 636f 6c75 6d6e 3d22 3022 3e0a 2020 2020  column="0">.    
+00000a60: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
+00000a70: 3d22 5150 7573 6842 7574 746f 6e22 206e  ="QPushButton" n
+00000a80: 616d 653d 2267 6f74 6f5f 6275 7474 6f6e  ame="goto_button
+00000a90: 223e 0a20 2020 2020 2020 203c 7072 6f70  ">.        <prop
+00000aa0: 6572 7479 206e 616d 653d 2274 6578 7422  erty name="text"
+00000ab0: 3e0a 2020 2020 2020 2020 203c 7374 7269  >.         <stri
+00000ac0: 6e67 3e47 6f20 546f 2028 c2b5 6d29 3c2f  ng>Go To (..m)</
+00000ad0: 7374 7269 6e67 3e0a 2020 2020 2020 2020  string>.        
+00000ae0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00000af0: 2020 203c 2f77 6964 6765 743e 0a20 2020     </widget>.   
+00000b00: 2020 203c 2f69 7465 6d3e 0a20 2020 2020     </item>.     
+00000b10: 203c 6974 656d 2072 6f77 3d22 3022 2063   <item row="0" c
+00000b20: 6f6c 756d 6e3d 2231 223e 0a20 2020 2020  olumn="1">.     
+00000b30: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
+00000b40: 2251 4c69 6e65 4564 6974 2220 6e61 6d65  "QLineEdit" name
+00000b50: 3d22 676f 746f 5f6c 696e 6522 3e0a 2020  ="goto_line">.  
+00000b60: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00000b70: 6e61 6d65 3d22 7465 7874 223e 0a20 2020  name="text">.   
+00000b80: 2020 2020 2020 3c73 7472 696e 673e 303c        <string>0<
+00000b90: 2f73 7472 696e 673e 0a20 2020 2020 2020  /string>.       
+00000ba0: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+00000bb0: 2020 2020 3c2f 7769 6467 6574 3e0a 2020      </widget>.  
+00000bc0: 2020 2020 3c2f 6974 656d 3e0a 2020 2020      </item>.    
+00000bd0: 203c 2f6c 6179 6f75 743e 0a20 2020 203c   </layout>.    <
+00000be0: 2f69 7465 6d3e 0a20 2020 3c2f 6c61 796f  /item>.   </layo
+00000bf0: 7574 3e0a 2020 3c2f 7769 6467 6574 3e0a  ut>.  </widget>.
+00000c00: 2020 3c77 6964 6765 7420 636c 6173 733d    <widget class=
+00000c10: 2251 4d65 6e75 4261 7222 206e 616d 653d  "QMenuBar" name=
+00000c20: 226d 656e 7562 6172 223e 0a20 2020 3c70  "menubar">.   <p
+00000c30: 726f 7065 7274 7920 6e61 6d65 3d22 6765  roperty name="ge
+00000c40: 6f6d 6574 7279 223e 0a20 2020 203c 7265  ometry">.    <re
+00000c50: 6374 3e0a 2020 2020 203c 783e 303c 2f78  ct>.     <x>0</x
+00000c60: 3e0a 2020 2020 203c 793e 303c 2f79 3e0a  >.     <y>0</y>.
+00000c70: 2020 2020 203c 7769 6474 683e 3337 343c       <width>374<
+00000c80: 2f77 6964 7468 3e0a 2020 2020 203c 6865  /width>.     <he
+00000c90: 6967 6874 3e32 343c 2f68 6569 6768 743e  ight>24</height>
+00000ca0: 0a20 2020 203c 2f72 6563 743e 0a20 2020  .    </rect>.   
+00000cb0: 3c2f 7072 6f70 6572 7479 3e0a 2020 3c2f  </property>.  </
+00000cc0: 7769 6467 6574 3e0a 2020 3c77 6964 6765  widget>.  <widge
+00000cd0: 7420 636c 6173 733d 2251 5374 6174 7573  t class="QStatus
+00000ce0: 4261 7222 206e 616d 653d 2273 7461 7475  Bar" name="statu
+00000cf0: 7362 6172 222f 3e0a 203c 2f77 6964 6765  sbar"/>. </widge
+00000d00: 743e 0a20 3c72 6573 6f75 7263 6573 2f3e  t>. <resources/>
+00000d10: 0a20 3c63 6f6e 6e65 6374 696f 6e73 2f3e  . <connections/>
+00000d20: 0a3c 2f75 693e 0a                        .</ui>.
```

### Comparing `nanoqnt-0.2.0/nanoqnt/view/main_window.py` & `nanoqnt-0.2.0rc1/nanoqnt/view/main_window.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,248 +1,245 @@
-import time
-from pathlib import Path
-
-import matplotlib.pyplot as plt
-from PyQt5 import uic
-from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import QApplication, QFileDialog, QMainWindow, QMessageBox
-import pyqtgraph as pg
-
-from nanoqnt.view import VIEW_FOLDER
-from nanoqnt.view.channel_selector import ChannelSelector
-from nanoqnt.view.particle_widget import ParticleWidget
-
-home_path = Path.home()
-
-
-class NanoQNTMainWindow(QMainWindow):
-    def __init__(self, model=None):
-        """
-        :param AnalyzeNanoQNT model: Model used to analyze the data
-        """
-        super().__init__(parent=None)
-        uic.loadUi(str(VIEW_FOLDER / 'GUI' / 'data_exploration.ui'), self)
-        self.setWindowTitle('NanoQNT Analysis')
-
-        self.analyze_model = model
-
-        self.action_open.triggered.connect(self.open)
-        self.action_mass_histogram.triggered.connect(self.histogram_mass)
-        self.action_data_frame.triggered.connect(self.data_over_frame)
-        self.action_data_plots.triggered.connect(self.total_histograms)
-        self.action_export_all_data.triggered.connect(self.export_all_data)
-        self.action_save_data.triggered.connect(self.export_data)
-        self.action_calculate_bkg.triggered.connect(self.calculate_background)
-        self.action_show_bkg.triggered.connect(self.show_background)
-
-        self.frame_slider.valueChanged.connect(self.update_slider)
-        self.step_size_line.editingFinished.connect(self.calculate_concentration)
-        self.find_particles_check.toggled.connect(self.update_images)
-        self.calculate_button.clicked.connect(self.calculate_all)
-        self.action_about.triggered.connect(self.show_about)
-
-        self.circles = []
-        self.curr_index = 0
-
-        self.channel_widget = ChannelSelector()
-        self.channel_widget.accept_button.clicked.connect(self.channels_updated)
-
-        self.nanoqnt_images = []
-
-    def open(self):
-        last_dir = self.analyze_model.metadata.get('last_dir', home_path)
-        file = QFileDialog.getOpenFileName(self, 'Open Data', str(last_dir), filter='*.tif')[0]
-        if file != '':
-            file = Path(file)
-        else:
-            return
-
-        self.channel_widget.show()
-
-        self.analyze_model.open(str(file))
-        self.setWindowTitle(f'NanoQNT Analysis: {file.name}')
-
-    def update_slider(self, index):
-        self.curr_index = index - 1
-        self.frame_num.setText(str(index))
-        self.update_images()
-
-    def update_images(self, auto_range=False, auto_levels=False):
-        if self.analyze_model.data is None:
-            return
-
-
-        for i, channel_image in enumerate(self.nanoqnt_images):
-            index = self.curr_index*len(self.nanoqnt_images) + i
-            circles = None
-            if self.find_particles_check.isChecked():
-                diameter = int(channel_image.size_line.text())
-                minmass = int(channel_image.min_mass_line.text())
-                method = self.engine_box.currentText()
-
-                self.analyze_model.find_particles(index, diameter, minmass, method=method)
-                particles_df = self.analyze_model.particle_df[index]
-                circles = [pg.CircleROI([p[1] - 12, p[0] - 12], [25, 25],
-                              pen=pg.mkPen('r', width=2),
-                              movable=False,
-                              resizable=False,
-                              rotatable=False,
-                              removable=False,
-                              )
-                    for p in zip(particles_df['x'], particles_df['y'])]
-            channel_image.update_image(self.analyze_model.data[index], circles, auto_range=auto_range,
-                                       auto_levels=auto_levels)
-
-    def histogram_mass(self):
-        index = self.curr_index
-        diameter = int(self.size_line.text())
-        minmass = int(self.min_mass_line.text())
-
-        self.analyze_model.find_particles(index, diameter, minmass)
-
-        fig, ax = plt.subplots(1)
-        ax.hist(self.analyze_model.particle_df[index]['mass'], bins=50)
-        fig.suptitle(f'Mass Histogram Frame Number: {self.curr_index}')
-        fig.show()
-
-    def calculate_all(self):
-        QApplication.setOverrideCursor(Qt.BusyCursor)
-        diameter = [int(channel_image.size_line.text()) for channel_image in self.nanoqnt_images]
-        minmass = [int(channel_image.min_mass_line.text()) for channel_image in self.nanoqnt_images]
-        engine = self.engine_box.currentText()
-        frames_no = [int(self.start_frame_line.text())-1, int(self.end_frame_line.text())]
-        self.analyze_model.find_all_particles(frames_no, diameter, minmass, engine)
-        search_radius = int(self.search_radius_line.text())
-        min_frames = int(self.min_frames_line.text())
-        self.analyze_model.link_particles(search_radius, memory=0, min_frames=min_frames)
-        self.analyze_model.calculate_intensities()
-        self.analyze_model.multi_color_link()
-        self.calculate_concentration()
-        QApplication.setOverrideCursor(Qt.ArrowCursor)
-
-    def data_over_frame(self):
-        t1 = self.analyze_model.linked_particles
-
-        fig, ax = plt.subplots(3, sharex=True)
-        ax[0].plot(t1['ecc'].groupby('frame').mean())
-        ax[0].set_ylabel('Eccentricity')
-        ax[1].plot(t1['size'].groupby('frame').mean())
-        ax[1].set_ylabel('Size')
-        ax[2].plot(t1['mass'].groupby('frame').mean())
-        ax[2].set_ylabel('Mass')
-        ax[2].set_xlabel('Frame Num')
-        fig.show()
-
-    def total_histograms(self):
-        if self.analyze_model.linked_particles is None:
-            print('No particles to plot!')
-            msg = QMessageBox.warning(self, "Run Analysis First", "Before being able to show the histogram of "
-                                                                      "all "
-                                                                      "the particles, you must run the analysis using "
-                                                                      "the calculate all button.",
-                                      QMessageBox.Ok)
-            return
-
-        for channel in range(self.analyze_model.num_channels):
-            t1 = self.analyze_model.summary_data[channel]
-            fig1, ax1 = plt.subplots(1)
-            t1[f'i_{channel}'].hist(bins=100, ax=ax1)
-            ax1.set_xlabel('Total Intensity (counts)')
-            ax1.set_title(f'Channel: {channel}')
-            fig1.show()
-
-            for channel_2 in range(channel+1, self.analyze_model.num_channels):
-                fig, ax = plt.subplots(1) #, figsize=(10, 8))
-                ax.plot(self.analyze_model.summary_data[channel][f'i_{channel}'],
-                        self.analyze_model.summary_data[channel][f'i_{channel_2}'],
-                        'o',
-                        alpha=0.1)
-                ax.set_xlabel(self.channel_names[channel], fontsize=14)
-                ax.set_ylabel(self.channel_names[channel_2], fontsize=14)
-                plt.gca().tick_params(labelsize=12)
-                # ax.set_yscale('log')
-                # ax.set_xscale('log')
-                fig.show()
-
-    def calculate_concentration(self):
-        step_size = float(self.step_size_line.text())
-        self.analyze_model.calculate_concentration(step_size)
-        for i in range(self.analyze_model.num_channels):
-            self.nanoqnt_images[i].concentration_line.setText(f"{self.analyze_model.concentration[i]:.2E}")
-            self.nanoqnt_images[i].total_particles_line.setText(f"{self.analyze_model.total_num_particles[i]}")
-
-    def export_all_data(self):
-        path = self.analyze_model.filename.parent
-        filename = QFileDialog.getSaveFileName(self, 'Save to file', str(path), '*.csv')[0]
-
-        if filename is not None:
-            self.analyze_model.save_all_data(filename)
-
-    def export_data(self):
-        path = self.analyze_model.filename.parent
-        filename = QFileDialog.getSaveFileName(self, 'Save to file', str(path), '*.csv')[0]
-
-        if filename is not None:
-            self.analyze_model.save_data(filename)
-
-    def channels_updated(self):
-        self.analyze_model.num_channels = self.channel_widget.channel_box.currentIndex()+1
-        self.channel_names = [line.text() for line in self.channel_widget.channels]
-
-
-        self.nanoqnt_images = [ParticleWidget() for _ in range(self.analyze_model.num_channels)]
-
-        plot_layout = self.video_widget.layout()
-        for i in reversed(range(plot_layout.count())):
-            plot_layout.itemAt(i).widget().setParent(None)
-
-        if self.analyze_model.num_channels == 1:
-            plot_layout.addWidget(self.nanoqnt_images[0], 0, 0)
-        elif self.analyze_model.num_channels == 2:
-            plot_layout.addWidget(self.nanoqnt_images[0], 0, 0)
-            plot_layout.addWidget(self.nanoqnt_images[1], 0, 1)
-        elif self.analyze_model.num_channels == 3:
-            plot_layout.addWidget(self.nanoqnt_images[0], 0, 0)
-            plot_layout.addWidget(self.nanoqnt_images[1], 0, 1)
-            plot_layout.addWidget(self.nanoqnt_images[2], 1, 0)
-        elif self.analyze_model.num_channels == 4:
-            plot_layout.addWidget(self.nanoqnt_images[0], 0, 0)
-            plot_layout.addWidget(self.nanoqnt_images[1], 0, 1)
-            plot_layout.addWidget(self.nanoqnt_images[2], 1, 0)
-            plot_layout.addWidget(self.nanoqnt_images[3], 1, 1)
-
-            # print(plot_layout.itemAt(i).widget().image.view.state)
-
-        if self.analyze_model.num_channels > 1:
-            for i, plot in enumerate(self.nanoqnt_images[:-1]):
-                view = plot.image.view
-                view.linkView(self.nanoqnt_images[i+1].image.view.XAxis, self.nanoqnt_images[i+1].image.view)
-                view.linkView(self.nanoqnt_images[i+1].image.view.YAxis, self.nanoqnt_images[i+1].image.view)
-
-        self.frame_slider.setRange(1, int(self.analyze_model.num_frames/self.analyze_model.num_channels))
-        self.frame_slider.setEnabled(True)
-        self.start_frame_line.setText("1")
-        self.end_frame_line.setText(str(int(self.analyze_model.num_frames/self.analyze_model.num_channels)))
-        self.update_slider(1)
-
-        self.update_images(auto_range=True, auto_levels=True)
-        for i in reversed(range(plot_layout.count())):
-            plot_layout.itemAt(i).widget().autoRange()
-            plot_layout.itemAt(i).widget().min_mass_line.editingFinished.connect(self.update_images)
-            plot_layout.itemAt(i).widget().size_line.editingFinished.connect(self.update_images)
-
-    def calculate_background(self):
-        print('Calculating background')
-        QApplication.setOverrideCursor(Qt.BusyCursor)
-        frames_no = [int(self.start_frame_line.text())-1, int(self.end_frame_line.text())]
-        self.analyze_model.calculate_background(frames_no=frames_no)
-        QApplication.setOverrideCursor(Qt.ArrowCursor)
-        print('Done calculating background')
-
-    def show_background(self):
-        fig, ax = plt.subplots(1)
-        ax.imshow(self.analyze_model.bkg)
-        fig.suptitle(f'Mass Histogram Frame Number: {self.curr_index}')
-        fig.show()
-
-    def show_about(self):
-        QMessageBox.about(self, 'About NanoQNTPy', 'Beta version 0.1')
+from pathlib import Path
+
+import matplotlib.pyplot as plt
+import pyqtgraph as pg
+from PyQt5 import uic
+from PyQt5.QtCore import Qt
+from PyQt5.QtWidgets import QApplication, QFileDialog, QMainWindow, QMessageBox
+
+from nanoqnt.view import VIEW_FOLDER
+from nanoqnt.view.channel_selector import ChannelSelector
+from nanoqnt.view.particle_widget import ParticleWidget
+
+home_path = Path.home()
+
+
+class NanoQNTMainWindow(QMainWindow):
+    def __init__(self, model=None):
+        """
+        :param AnalyzeNanoQNT model: Model used to analyze the data
+        """
+        super().__init__(parent=None)
+        uic.loadUi(str(VIEW_FOLDER / 'GUI' / 'data_exploration.ui'), self)
+        self.setWindowTitle('NanoQNT Analysis')
+
+        self.analyze_model = model
+
+        self.action_open.triggered.connect(self.open)
+        self.action_mass_histogram.triggered.connect(self.histogram_mass)
+        self.action_data_frame.triggered.connect(self.data_over_frame)
+        self.action_data_plots.triggered.connect(self.total_histograms)
+        self.action_export_all_data.triggered.connect(self.export_all_data)
+        self.action_save_data.triggered.connect(self.export_data)
+        self.action_calculate_bkg.triggered.connect(self.calculate_background)
+        self.action_show_bkg.triggered.connect(self.show_background)
+
+        self.frame_slider.valueChanged.connect(self.update_slider)
+        self.step_size_line.editingFinished.connect(self.calculate_concentration)
+        self.find_particles_check.toggled.connect(self.update_images)
+        self.calculate_button.clicked.connect(self.calculate_all)
+        self.action_about.triggered.connect(self.show_about)
+
+        self.circles = []
+        self.curr_index = 0
+
+        self.channel_widget = ChannelSelector()
+        self.channel_widget.accept_button.clicked.connect(self.channels_updated)
+
+        self.nanoqnt_images = []
+
+    def open(self):
+        last_dir = self.analyze_model.metadata.get('last_dir', home_path)
+        file = QFileDialog.getOpenFileName(self, 'Open Data', str(last_dir), filter='*.tif')[0]
+        if file != '':
+            file = Path(file)
+        else:
+            return
+
+        self.channel_widget.show()
+
+        self.analyze_model.open(str(file))
+        self.setWindowTitle(f'NanoQNT Analysis: {file.name}')
+
+    def update_slider(self, index):
+        self.curr_index = index - 1
+        self.frame_num.setText(str(index))
+        self.update_images()
+
+    def update_images(self, auto_range=False, auto_levels=False):
+        if self.analyze_model.data is None:
+            return
+
+        for i, channel_image in enumerate(self.nanoqnt_images):
+            index = self.curr_index * len(self.nanoqnt_images) + i
+            circles = None
+            if self.find_particles_check.isChecked():
+                diameter = int(channel_image.size_line.text())
+                minmass = int(channel_image.min_mass_line.text())
+                method = self.engine_box.currentText()
+
+                self.analyze_model.find_particles(index, diameter, minmass, method=method)
+                particles_df = self.analyze_model.particle_df[index]
+                circles = [pg.CircleROI([p[1] - 12, p[0] - 12], [25, 25],
+                                        pen=pg.mkPen('r', width=2),
+                                        movable=False,
+                                        resizable=False,
+                                        rotatable=False,
+                                        removable=False,
+                                        )
+                           for p in zip(particles_df['x'], particles_df['y'])]
+            channel_image.update_image(self.analyze_model.data[index], circles, auto_range=auto_range,
+                                       auto_levels=auto_levels)
+
+    def histogram_mass(self):
+        index = self.curr_index
+        diameter = int(self.size_line.text())
+        minmass = int(self.min_mass_line.text())
+
+        self.analyze_model.find_particles(index, diameter, minmass)
+
+        fig, ax = plt.subplots(1)
+        ax.hist(self.analyze_model.particle_df[index]['mass'], bins=50)
+        fig.suptitle(f'Mass Histogram Frame Number: {self.curr_index}')
+        fig.show()
+
+    def calculate_all(self):
+        QApplication.setOverrideCursor(Qt.BusyCursor)
+        diameter = [int(channel_image.size_line.text()) for channel_image in self.nanoqnt_images]
+        minmass = [int(channel_image.min_mass_line.text()) for channel_image in self.nanoqnt_images]
+        engine = self.engine_box.currentText()
+        frames_no = [int(self.start_frame_line.text()) - 1, int(self.end_frame_line.text())]
+        self.analyze_model.find_all_particles(frames_no, diameter, minmass, engine)
+        search_radius = int(self.search_radius_line.text())
+        min_frames = int(self.min_frames_line.text())
+        self.analyze_model.link_particles(search_radius, memory=0, min_frames=min_frames)
+        self.analyze_model.calculate_intensities()
+        self.analyze_model.multi_color_link()
+        self.calculate_concentration()
+        QApplication.setOverrideCursor(Qt.ArrowCursor)
+
+    def data_over_frame(self):
+        t1 = self.analyze_model.linked_particles
+
+        fig, ax = plt.subplots(3, sharex=True)
+        ax[0].plot(t1['ecc'].groupby('frame').mean())
+        ax[0].set_ylabel('Eccentricity')
+        ax[1].plot(t1['size'].groupby('frame').mean())
+        ax[1].set_ylabel('Size')
+        ax[2].plot(t1['mass'].groupby('frame').mean())
+        ax[2].set_ylabel('Mass')
+        ax[2].set_xlabel('Frame Num')
+        fig.show()
+
+    def total_histograms(self):
+        if self.analyze_model.linked_particles is None:
+            print('No particles to plot!')
+            msg = QMessageBox.warning(self, "Run Analysis First", "Before being able to show the histogram of "
+                                                                  "all "
+                                                                  "the particles, you must run the analysis using "
+                                                                  "the calculate all button.",
+                                      QMessageBox.Ok)
+            return
+
+        for channel in range(self.analyze_model.num_channels):
+            t1 = self.analyze_model.summary_data[channel]
+            fig1, ax1 = plt.subplots(1)
+            t1[f'i_{channel}'].hist(bins=100, ax=ax1)
+            ax1.set_xlabel('Total Intensity (counts)')
+            ax1.set_title(f'Channel: {channel}')
+            fig1.show()
+
+            for channel_2 in range(channel + 1, self.analyze_model.num_channels):
+                fig, ax = plt.subplots(1)  # , figsize=(10, 8))
+                ax.plot(self.analyze_model.summary_data[channel][f'i_{channel}'],
+                        self.analyze_model.summary_data[channel][f'i_{channel_2}'],
+                        'o',
+                        alpha=0.1)
+                ax.set_xlabel(self.channel_names[channel], fontsize=14)
+                ax.set_ylabel(self.channel_names[channel_2], fontsize=14)
+                plt.gca().tick_params(labelsize=12)
+                # ax.set_yscale('log')
+                # ax.set_xscale('log')
+                fig.show()
+
+    def calculate_concentration(self):
+        step_size = float(self.step_size_line.text())
+        self.analyze_model.calculate_concentration(step_size)
+        for i in range(self.analyze_model.num_channels):
+            self.nanoqnt_images[i].concentration_line.setText(f"{self.analyze_model.concentration[i]:.2E}")
+            self.nanoqnt_images[i].total_particles_line.setText(f"{self.analyze_model.total_num_particles[i]}")
+
+    def export_all_data(self):
+        path = self.analyze_model.filename.parent
+        filename = QFileDialog.getSaveFileName(self, 'Save to file', str(path), '*.csv')[0]
+
+        if filename is not None:
+            self.analyze_model.save_all_data(filename)
+
+    def export_data(self):
+        path = self.analyze_model.filename.parent
+        filename = QFileDialog.getSaveFileName(self, 'Save to file', str(path), '*.csv')[0]
+
+        if filename is not None:
+            self.analyze_model.save_data(filename)
+
+    def channels_updated(self):
+        self.analyze_model.num_channels = self.channel_widget.channel_box.currentIndex() + 1
+        self.channel_names = [line.text() for line in self.channel_widget.channels]
+
+        self.nanoqnt_images = [ParticleWidget() for _ in range(self.analyze_model.num_channels)]
+
+        plot_layout = self.video_widget.layout()
+        for i in reversed(range(plot_layout.count())):
+            plot_layout.itemAt(i).widget().setParent(None)
+
+        if self.analyze_model.num_channels == 1:
+            plot_layout.addWidget(self.nanoqnt_images[0], 0, 0)
+        elif self.analyze_model.num_channels == 2:
+            plot_layout.addWidget(self.nanoqnt_images[0], 0, 0)
+            plot_layout.addWidget(self.nanoqnt_images[1], 0, 1)
+        elif self.analyze_model.num_channels == 3:
+            plot_layout.addWidget(self.nanoqnt_images[0], 0, 0)
+            plot_layout.addWidget(self.nanoqnt_images[1], 0, 1)
+            plot_layout.addWidget(self.nanoqnt_images[2], 1, 0)
+        elif self.analyze_model.num_channels == 4:
+            plot_layout.addWidget(self.nanoqnt_images[0], 0, 0)
+            plot_layout.addWidget(self.nanoqnt_images[1], 0, 1)
+            plot_layout.addWidget(self.nanoqnt_images[2], 1, 0)
+            plot_layout.addWidget(self.nanoqnt_images[3], 1, 1)
+
+            # print(plot_layout.itemAt(i).widget().image.view.state)
+
+        if self.analyze_model.num_channels > 1:
+            for i, plot in enumerate(self.nanoqnt_images[:-1]):
+                view = plot.image.view
+                view.linkView(self.nanoqnt_images[i + 1].image.view.XAxis, self.nanoqnt_images[i + 1].image.view)
+                view.linkView(self.nanoqnt_images[i + 1].image.view.YAxis, self.nanoqnt_images[i + 1].image.view)
+
+        self.frame_slider.setRange(1, int(self.analyze_model.num_frames / self.analyze_model.num_channels))
+        self.frame_slider.setEnabled(True)
+        self.start_frame_line.setText("1")
+        self.end_frame_line.setText(str(int(self.analyze_model.num_frames / self.analyze_model.num_channels)))
+        self.update_slider(1)
+
+        self.update_images(auto_range=True, auto_levels=True)
+        for i in reversed(range(plot_layout.count())):
+            plot_layout.itemAt(i).widget().autoRange()
+            plot_layout.itemAt(i).widget().min_mass_line.editingFinished.connect(self.update_images)
+            plot_layout.itemAt(i).widget().size_line.editingFinished.connect(self.update_images)
+
+    def calculate_background(self):
+        print('Calculating background')
+        QApplication.setOverrideCursor(Qt.BusyCursor)
+        frames_no = [int(self.start_frame_line.text()) - 1, int(self.end_frame_line.text())]
+        self.analyze_model.calculate_background(frames_no=frames_no)
+        QApplication.setOverrideCursor(Qt.ArrowCursor)
+        print('Done calculating background')
+
+    def show_background(self):
+        fig, ax = plt.subplots(1)
+        ax.imshow(self.analyze_model.bkg)
+        fig.suptitle(f'Mass Histogram Frame Number: {self.curr_index}')
+        fig.show()
+
+    def show_about(self):
+        QMessageBox.about(self, 'About NanoQNTPy', 'Beta version 0.1')
```

### Comparing `nanoqnt-0.2.0/nanoqnt/view/particle_widget.py` & `nanoqnt-0.2.0rc1/nanoqnt/view/particle_widget.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,62 @@
-from PyQt5 import uic
-from PyQt5.QtWidgets import QWidget
-import pyqtgraph as pg
-from nanoqnt.view import VIEW_FOLDER
-
-
-class ParticleWidget(QWidget):
-    """Wrapper class to display image data with few signals to update the frame. It is meant to handle also
-    multi-color data"""
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        uic.loadUi(str(VIEW_FOLDER / 'GUI' / 'particles_widget.ui'), self)
-        self.image = pg.ImageView()
-        self.image.setPredefinedGradient('thermal')
-
-        self.circles = []
-
-        plot_layout = self.video_widget.layout()
-        plot_layout.addWidget(self.image)
-
-    def autoRange(self):
-        """ Wrapper to the default PyQtGraph auto range to see if it integrates better with the overall UI"""
-        # self.image.view.setXRange(0, 2000)
-        self.image.view.setRange(xRange=(0, 2000), yRange=(0,2000))
-
-    def update_image(self, image, circles=None, auto_range=False, auto_levels=False):
-        for r in self.circles:
-            self.image.removeItem(r)
-            self.circles = []
-
-        self.image.setImage(image, autoRange=auto_range, autoLevels=auto_levels)
-
-        if circles is not None:
-
-            self.circles = circles
-
-            for p in self.circles:
-                try:  # Very dangerous, but this is a feature fixed by PyQtGraph only on version > 0.13.2
-                    p.removeHandle(0)
-                except:
-                    pass
-                self.image.addItem(p)
-            self.found_particles_line.setText(str(len(circles)))
-
-        if auto_range:
-            self.autoRange()
-        if auto_levels:
-            self.image.autoLevels()
-
-    def removeItem(self, r):
-        self.image.removeItem(r)
-
-    def setImage(self, *args, **kwarks):
-        self.image.setImage(*args, **kwarks)
-
-    def addItem(self, p):
-        self.image.addItem(p)
-
-    def autoLevels(self):
-        self.image.autoLevels()
+import pyqtgraph as pg
+from PyQt5 import uic
+from PyQt5.QtWidgets import QWidget
+
+from nanoqnt.view import VIEW_FOLDER
+
+
+class ParticleWidget(QWidget):
+    """Wrapper class to display image data with few signals to update the frame. It is meant to handle also
+    multi-color data"""
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        uic.loadUi(str(VIEW_FOLDER / 'GUI' / 'particles_widget.ui'), self)
+        self.image = pg.ImageView()
+        self.image.setPredefinedGradient('thermal')
+
+        self.circles = []
+
+        plot_layout = self.video_widget.layout()
+        plot_layout.addWidget(self.image)
+
+    def autoRange(self):
+        """ Wrapper to the default PyQtGraph auto range to see if it integrates better with the overall UI"""
+        # self.image.view.setXRange(0, 2000)
+        self.image.view.setRange(xRange=(0, 2000), yRange=(0, 2000))
+
+    def update_image(self, image, circles=None, auto_range=False, auto_levels=False):
+        for r in self.circles:
+            self.image.removeItem(r)
+            self.circles = []
+
+        self.image.setImage(image, autoRange=auto_range, autoLevels=auto_levels)
+
+        if circles is not None:
+
+            self.circles = circles
+
+            for p in self.circles:
+                try:  # Very dangerous, but this is a feature fixed by PyQtGraph only on version > 0.13.2
+                    p.removeHandle(0)
+                except:
+                    pass
+                self.image.addItem(p)
+            self.found_particles_line.setText(str(len(circles)))
+
+        if auto_range:
+            self.autoRange()
+        if auto_levels:
+            self.image.autoLevels()
+
+    def removeItem(self, r):
+        self.image.removeItem(r)
+
+    def setImage(self, *args, **kwarks):
+        self.image.setImage(*args, **kwarks)
+
+    def addItem(self, p):
+        self.image.addItem(p)
+
+    def autoLevels(self):
+        self.image.autoLevels()
```

### Comparing `nanoqnt-0.2.0/nanoqnt/view/stage_control.py` & `nanoqnt-0.2.0rc1/nanoqnt/view/stage_control.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from threading import Thread
-
-from PyQt5 import uic
-from PyQt5.QtWidgets import QMainWindow, QMessageBox
-
-from nanoqnt.view import VIEW_FOLDER
-
-
-class StageControlWindow(QMainWindow):
-    def __init__(self, model=None):
-        """
-        :param StageControl model: Model used to control the stage
-        """
-        super().__init__(parent=None)
-        uic.loadUi(str(VIEW_FOLDER/'GUI'/'scan_control.ui'), self)
-        self.model = model
-
-        self.start_live_button.clicked.connect(self.model.live)
-        self.stop_live_button.clicked.connect(self.model.stop_live)
-        self.snap_button.clicked.connect(self.model.snap)
-        self.scan_button.clicked.connect(self.scan)
-        self.goto_button.clicked.connect(self.move)
-
-    def scan(self):
-        start = int(self.start_line.text())
-        end = int(self.stop_line.text())
-        step_size = int(self.step_line.text())
-        self.model.prepare_scan(start)
-
-        self.msgbox = QMessageBox()
-        self.msgbox.setText(f'Open Multi-D Acq. in Micromanager and set the count to {int((end-start)/step_size)}')
-        self.msgbox.exec()
-
-        self.scan_thread = Thread(
-            target=self.model.scan, args=(start, end, step_size)
-            )
-        self.scan_thread.start()
-
-    def move(self):
-        goto = int(self.goto_line.text())
-        self.model.move(goto)
+from threading import Thread
+
+from PyQt5 import uic
+from PyQt5.QtWidgets import QMainWindow, QMessageBox
+
+from nanoqnt.view import VIEW_FOLDER
+
+
+class StageControlWindow(QMainWindow):
+    def __init__(self, model=None):
+        """
+        :param StageControl model: Model used to control the stage
+        """
+        super().__init__(parent=None)
+        uic.loadUi(str(VIEW_FOLDER / 'GUI' / 'scan_control.ui'), self)
+        self.model = model
+
+        self.start_live_button.clicked.connect(self.model.live)
+        self.stop_live_button.clicked.connect(self.model.stop_live)
+        self.snap_button.clicked.connect(self.model.snap)
+        self.scan_button.clicked.connect(self.scan)
+        self.goto_button.clicked.connect(self.move)
+
+    def scan(self):
+        start = int(self.start_line.text())
+        end = int(self.stop_line.text())
+        step_size = int(self.step_line.text())
+        self.model.prepare_scan(start)
+
+        self.msgbox = QMessageBox()
+        self.msgbox.setText(f'Open Multi-D Acq. in Micromanager and set the count to {int((end - start) / step_size)}')
+        self.msgbox.exec()
+
+        self.scan_thread = Thread(
+            target=self.model.scan, args=(start, end, step_size)
+            )
+        self.scan_thread.start()
+
+    def move(self):
+        goto = int(self.goto_line.text())
+        self.model.move(goto)
```

### Comparing `nanoqnt-0.2.0/PKG-INFO` & `nanoqnt-0.2.0rc1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: nanoqnt
-Version: 0.2.0
+Version: 0.2.0rc1
 Summary: 
 Author: Aquiles Carattino
 Author-email: carattino@dispertech.com
-Requires-Python: ==3.11.3
+Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PIMS (>=0.6.1,<0.7.0)
 Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pyqt5 (>=5.15.9,<6.0.0)
 Requires-Dist: pyqtgraph (>=0.13.3,<0.14.0)
 Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
```

