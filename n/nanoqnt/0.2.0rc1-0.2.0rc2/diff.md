# Comparing `tmp/nanoqnt-0.2.0rc1.tar.gz` & `tmp/nanoqnt-0.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoqnt-0.2.0rc1.tar", max compression
+gzip compressed data, was "nanoqnt-0.2.0rc2.tar", max compression
```

## Comparing `nanoqnt-0.2.0rc1.tar` & `nanoqnt-0.2.0rc2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0       43 2023-06-12 12:02:24.897116 nanoqnt-0.2.0rc1/README.md
--rw-r--r--   0        0        0        0 2023-01-02 14:34:22.063965 nanoqnt-0.2.0rc1/nanoqnt/__init__.py
--rw-r--r--   0        0        0     4154 2023-06-12 12:02:24.898367 nanoqnt-0.2.0rc1/nanoqnt/dispertech-logo.ico
--rw-r--r--   0        0        0      820 2023-06-12 12:02:24.899141 nanoqnt-0.2.0rc1/nanoqnt/main.py
--rw-r--r--   0        0        0        0 2022-12-20 12:52:00.514018 nanoqnt-0.2.0rc1/nanoqnt/model/__init__.py
--rw-r--r--   0        0        0    13247 2023-06-12 12:02:24.899813 nanoqnt-0.2.0rc1/nanoqnt/model/analyze_nanoqnt.py
--rw-r--r--   0        0        0      280 2023-06-12 12:02:24.900270 nanoqnt-0.2.0rc1/nanoqnt/model/decorators.py
--rw-r--r--   0        0        0       34 2023-06-12 12:02:24.900680 nanoqnt-0.2.0rc1/nanoqnt/model/exceptions.py
--rw-r--r--   0        0        0      385 2023-06-12 12:02:24.901046 nanoqnt-0.2.0rc1/nanoqnt/stage_main.py
--rw-r--r--   0        0        0      351 2023-06-12 12:02:24.901498 nanoqnt-0.2.0rc1/nanoqnt/util/__init__.py
--rw-r--r--   0        0        0     1202 2023-06-12 12:02:24.901860 nanoqnt-0.2.0rc1/nanoqnt/util/make_hdf5.py
--rw-r--r--   0        0        0     3759 2022-03-16 14:59:30.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg
--rw-r--r--   0        0        0     4715 2022-03-16 14:59:22.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11814 - Atom.svg
--rw-r--r--   0        0        0     3727 2022-03-16 14:59:14.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11815 - Battery.svg
--rw-r--r--   0        0        0     5275 2022-03-16 14:59:06.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11816 - Orbit.svg
--rw-r--r--   0        0        0     2802 2022-03-16 14:58:58.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11817 - Beaker.svg
--rw-r--r--   0        0        0     4637 2022-03-16 14:58:50.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg
--rw-r--r--   0        0        0     1936 2022-03-16 14:58:44.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11819 - Bounce.svg
--rw-r--r--   0        0        0     2442 2022-03-16 14:58:36.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11820 - Caliper.svg
--rw-r--r--   0        0        0     2191 2022-03-16 14:58:28.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11821 - Catapult.svg
--rw-r--r--   0        0        0     2594 2022-03-16 14:58:22.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11822 - Collision.svg
--rw-r--r--   0        0        0     2347 2022-03-16 14:58:14.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg
--rw-r--r--   0        0        0     2347 2022-03-16 14:58:04.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg
--rw-r--r--   0        0        0     2710 2022-03-16 14:57:56.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg
--rw-r--r--   0        0        0     3426 2022-03-16 15:19:36.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg
--rw-r--r--   0        0        0     3508 2022-03-16 14:57:38.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg
--rw-r--r--   0        0        0     3527 2022-03-16 14:57:30.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11828 - Energy.svg
--rw-r--r--   0        0        0     1821 2022-03-16 14:57:22.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11829 - Flask.svg
--rw-r--r--   0        0        0     4901 2022-03-16 14:57:14.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11830 - Float.svg
--rw-r--r--   0        0        0     1522 2022-03-16 14:57:06.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg
--rw-r--r--   0        0        0     8697 2022-03-16 14:56:58.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11832 - Force.svg
--rw-r--r--   0        0        0     3310 2022-03-16 14:56:48.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11833 - Formula.svg
--rw-r--r--   0        0        0     2416 2022-03-16 14:56:40.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11834 - Gears.svg
--rw-r--r--   0        0        0     4479 2022-03-16 14:56:32.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11835 - Gravity.svg
--rw-r--r--   0        0        0     4165 2022-03-16 14:56:24.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg
--rw-r--r--   0        0        0     3653 2022-03-16 14:56:16.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11837 - Histogram.svg
--rw-r--r--   0        0        0     2013 2022-03-16 14:56:08.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg
--rw-r--r--   0        0        0     2576 2022-03-16 14:56:00.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11839 - Magnet.svg
--rw-r--r--   0        0        0     5579 2022-03-16 14:55:54.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg
--rw-r--r--   0        0        0     3646 2022-03-16 14:55:46.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11841 - Metronome.svg
--rw-r--r--   0        0        0     1706 2022-03-16 14:55:38.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg
--rw-r--r--   0        0        0     3307 2022-03-16 14:55:32.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11843 - Molecule.svg
--rw-r--r--   0        0        0     2707 2022-03-16 14:55:24.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11844 - Motion.svg
--rw-r--r--   0        0        0     1163 2022-03-16 14:55:18.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg
--rw-r--r--   0        0        0     5179 2022-03-16 14:55:10.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg
--rw-r--r--   0        0        0     2264 2022-03-16 14:55:02.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg
--rw-r--r--   0        0        0     4868 2022-03-16 14:54:54.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11848 - Planet.svg
--rw-r--r--   0        0        0     9381 2022-03-16 14:54:44.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg
--rw-r--r--   0        0        0      806 2022-03-16 14:54:36.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11850 - Power.svg
--rw-r--r--   0        0        0     2581 2022-03-16 14:54:28.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11851 - Press.svg
--rw-r--r--   0        0        0     3090 2022-03-16 14:54:20.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11852 - Proton.svg
--rw-r--r--   0        0        0     2528 2022-03-16 14:54:12.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11853 - Pulley.svg
--rw-r--r--   0        0        0     4144 2022-03-16 14:54:04.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11854 - Reflection.svg
--rw-r--r--   0        0        0     3109 2022-03-16 14:53:56.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11855 - Resistor.svg
--rw-r--r--   0        0        0     2481 2022-03-16 14:53:54.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11856 - Rolling.svg
--rw-r--r--   0        0        0     3390 2022-03-16 14:53:52.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11857 - Rotate.svg
--rw-r--r--   0        0        0     2463 2022-03-16 14:53:50.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg
--rw-r--r--   0        0        0     2156 2022-03-16 14:53:48.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11859 - Temperature.svg
--rw-r--r--   0        0        0     2552 2022-03-16 14:53:48.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg
--rw-r--r--   0        0        0     2816 2022-03-16 15:41:46.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11861 - Waves.svg
--rw-r--r--   0        0        0     3799 2022-03-16 14:53:44.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg
--rw-r--r--   0        0        0       43 2022-12-20 12:57:18.786580 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/Icons.qrc
--rw-r--r--   0        0        0      342 2022-11-15 12:55:54.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/Open Folder.svg
--rw-r--r--   0        0        0      559 2022-11-15 12:55:54.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/Save.svg
--rw-r--r--   0        0        0      215 2020-07-27 20:54:42.000000 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/open.svg
--rw-r--r--   0        0        0     2193 2023-06-12 12:02:24.902373 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/channel_selector.ui
--rw-r--r--   0        0        0    14859 2023-06-12 12:02:24.902919 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/data_exploration.ui
--rw-r--r--   0        0        0     5564 2023-06-12 12:02:24.903391 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/particles_widget.ui
--rw-r--r--   0        0        0     3367 2023-01-26 21:32:32.021169 nanoqnt-0.2.0rc1/nanoqnt/view/GUI/scan_control.ui
--rw-r--r--   0        0        0       62 2023-06-12 12:02:24.903693 nanoqnt-0.2.0rc1/nanoqnt/view/__init__.py
--rw-r--r--   0        0        0      848 2023-06-12 12:02:24.903942 nanoqnt-0.2.0rc1/nanoqnt/view/channel_selector.py
--rw-r--r--   0        0        0    11311 2023-06-12 12:02:24.904324 nanoqnt-0.2.0rc1/nanoqnt/view/main_window.py
--rw-r--r--   0        0        0     1947 2023-06-12 12:02:24.904552 nanoqnt-0.2.0rc1/nanoqnt/view/particle_widget.py
--rw-r--r--   0        0        0     1359 2023-06-12 12:02:24.904821 nanoqnt-0.2.0rc1/nanoqnt/view/stage_control.py
--rw-r--r--   0        0        0      516 2023-06-12 12:17:21.653416 nanoqnt-0.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nanoqnt-0.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-06-12 12:02:24.897116 nanoqnt-0.2.0rc2/README.md
+-rw-r--r--   0        0        0        0 2023-01-02 14:34:22.063965 nanoqnt-0.2.0rc2/nanoqnt/__init__.py
+-rw-r--r--   0        0        0     4154 2023-06-12 12:02:24.898367 nanoqnt-0.2.0rc2/nanoqnt/dispertech-logo.ico
+-rw-r--r--   0        0        0      820 2023-06-12 12:02:24.899141 nanoqnt-0.2.0rc2/nanoqnt/main.py
+-rw-r--r--   0        0        0        0 2022-12-20 12:52:00.514018 nanoqnt-0.2.0rc2/nanoqnt/model/__init__.py
+-rw-r--r--   0        0        0    13247 2023-06-12 12:02:24.899813 nanoqnt-0.2.0rc2/nanoqnt/model/analyze_nanoqnt.py
+-rw-r--r--   0        0        0      280 2023-06-12 12:02:24.900270 nanoqnt-0.2.0rc2/nanoqnt/model/decorators.py
+-rw-r--r--   0        0        0       34 2023-06-12 12:02:24.900680 nanoqnt-0.2.0rc2/nanoqnt/model/exceptions.py
+-rw-r--r--   0        0        0      385 2023-06-12 12:02:24.901046 nanoqnt-0.2.0rc2/nanoqnt/stage_main.py
+-rw-r--r--   0        0        0      351 2023-06-12 12:02:24.901498 nanoqnt-0.2.0rc2/nanoqnt/util/__init__.py
+-rw-r--r--   0        0        0     1202 2023-06-12 12:02:24.901860 nanoqnt-0.2.0rc2/nanoqnt/util/make_hdf5.py
+-rw-r--r--   0        0        0     3759 2022-03-16 14:59:30.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg
+-rw-r--r--   0        0        0     4715 2022-03-16 14:59:22.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11814 - Atom.svg
+-rw-r--r--   0        0        0     3727 2022-03-16 14:59:14.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11815 - Battery.svg
+-rw-r--r--   0        0        0     5275 2022-03-16 14:59:06.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11816 - Orbit.svg
+-rw-r--r--   0        0        0     2802 2022-03-16 14:58:58.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11817 - Beaker.svg
+-rw-r--r--   0        0        0     4637 2022-03-16 14:58:50.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg
+-rw-r--r--   0        0        0     1936 2022-03-16 14:58:44.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11819 - Bounce.svg
+-rw-r--r--   0        0        0     2442 2022-03-16 14:58:36.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11820 - Caliper.svg
+-rw-r--r--   0        0        0     2191 2022-03-16 14:58:28.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11821 - Catapult.svg
+-rw-r--r--   0        0        0     2594 2022-03-16 14:58:22.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11822 - Collision.svg
+-rw-r--r--   0        0        0     2347 2022-03-16 14:58:14.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg
+-rw-r--r--   0        0        0     2347 2022-03-16 14:58:04.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg
+-rw-r--r--   0        0        0     2710 2022-03-16 14:57:56.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg
+-rw-r--r--   0        0        0     3426 2022-03-16 15:19:36.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg
+-rw-r--r--   0        0        0     3508 2022-03-16 14:57:38.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg
+-rw-r--r--   0        0        0     3527 2022-03-16 14:57:30.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11828 - Energy.svg
+-rw-r--r--   0        0        0     1821 2022-03-16 14:57:22.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11829 - Flask.svg
+-rw-r--r--   0        0        0     4901 2022-03-16 14:57:14.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11830 - Float.svg
+-rw-r--r--   0        0        0     1522 2022-03-16 14:57:06.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg
+-rw-r--r--   0        0        0     8697 2022-03-16 14:56:58.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11832 - Force.svg
+-rw-r--r--   0        0        0     3310 2022-03-16 14:56:48.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11833 - Formula.svg
+-rw-r--r--   0        0        0     2416 2022-03-16 14:56:40.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11834 - Gears.svg
+-rw-r--r--   0        0        0     4479 2022-03-16 14:56:32.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11835 - Gravity.svg
+-rw-r--r--   0        0        0     4165 2022-03-16 14:56:24.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg
+-rw-r--r--   0        0        0     3653 2022-03-16 14:56:16.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11837 - Histogram.svg
+-rw-r--r--   0        0        0     2013 2022-03-16 14:56:08.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg
+-rw-r--r--   0        0        0     2576 2022-03-16 14:56:00.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11839 - Magnet.svg
+-rw-r--r--   0        0        0     5579 2022-03-16 14:55:54.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg
+-rw-r--r--   0        0        0     3646 2022-03-16 14:55:46.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11841 - Metronome.svg
+-rw-r--r--   0        0        0     1706 2022-03-16 14:55:38.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg
+-rw-r--r--   0        0        0     3307 2022-03-16 14:55:32.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11843 - Molecule.svg
+-rw-r--r--   0        0        0     2707 2022-03-16 14:55:24.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11844 - Motion.svg
+-rw-r--r--   0        0        0     1163 2022-03-16 14:55:18.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg
+-rw-r--r--   0        0        0     5179 2022-03-16 14:55:10.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg
+-rw-r--r--   0        0        0     2264 2022-03-16 14:55:02.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg
+-rw-r--r--   0        0        0     4868 2022-03-16 14:54:54.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11848 - Planet.svg
+-rw-r--r--   0        0        0     9381 2022-03-16 14:54:44.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg
+-rw-r--r--   0        0        0      806 2022-03-16 14:54:36.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11850 - Power.svg
+-rw-r--r--   0        0        0     2581 2022-03-16 14:54:28.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11851 - Press.svg
+-rw-r--r--   0        0        0     3090 2022-03-16 14:54:20.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11852 - Proton.svg
+-rw-r--r--   0        0        0     2528 2022-03-16 14:54:12.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11853 - Pulley.svg
+-rw-r--r--   0        0        0     4144 2022-03-16 14:54:04.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11854 - Reflection.svg
+-rw-r--r--   0        0        0     3109 2022-03-16 14:53:56.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11855 - Resistor.svg
+-rw-r--r--   0        0        0     2481 2022-03-16 14:53:54.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11856 - Rolling.svg
+-rw-r--r--   0        0        0     3390 2022-03-16 14:53:52.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11857 - Rotate.svg
+-rw-r--r--   0        0        0     2463 2022-03-16 14:53:50.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg
+-rw-r--r--   0        0        0     2156 2022-03-16 14:53:48.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11859 - Temperature.svg
+-rw-r--r--   0        0        0     2552 2022-03-16 14:53:48.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg
+-rw-r--r--   0        0        0     2816 2022-03-16 15:41:46.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11861 - Waves.svg
+-rw-r--r--   0        0        0     3799 2022-03-16 14:53:44.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg
+-rw-r--r--   0        0        0       43 2022-12-20 12:57:18.786580 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/Icons.qrc
+-rw-r--r--   0        0        0      342 2022-11-15 12:55:54.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/Open Folder.svg
+-rw-r--r--   0        0        0      559 2022-11-15 12:55:54.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/Save.svg
+-rw-r--r--   0        0        0      215 2020-07-27 20:54:42.000000 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/open.svg
+-rw-r--r--   0        0        0     2193 2023-06-12 12:02:24.902373 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/channel_selector.ui
+-rw-r--r--   0        0        0    14859 2023-06-12 12:02:24.902919 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/data_exploration.ui
+-rw-r--r--   0        0        0     5564 2023-06-12 12:02:24.903391 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/particles_widget.ui
+-rw-r--r--   0        0        0     3367 2023-01-26 21:32:32.021169 nanoqnt-0.2.0rc2/nanoqnt/view/GUI/scan_control.ui
+-rw-r--r--   0        0        0       62 2023-06-12 12:02:24.903693 nanoqnt-0.2.0rc2/nanoqnt/view/__init__.py
+-rw-r--r--   0        0        0      848 2023-06-12 12:02:24.903942 nanoqnt-0.2.0rc2/nanoqnt/view/channel_selector.py
+-rw-r--r--   0        0        0    11311 2023-06-12 12:02:24.904324 nanoqnt-0.2.0rc2/nanoqnt/view/main_window.py
+-rw-r--r--   0        0        0     1947 2023-06-12 12:02:24.904552 nanoqnt-0.2.0rc2/nanoqnt/view/particle_widget.py
+-rw-r--r--   0        0        0     1359 2023-06-12 12:02:24.904821 nanoqnt-0.2.0rc2/nanoqnt/view/stage_control.py
+-rw-r--r--   0        0        0      515 2023-06-12 12:29:11.995279 nanoqnt-0.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 nanoqnt-0.2.0rc2/PKG-INFO
```

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/dispertech-logo.ico` & `nanoqnt-0.2.0rc2/nanoqnt/dispertech-logo.ico`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/main.py` & `nanoqnt-0.2.0rc2/nanoqnt/main.py`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/model/analyze_nanoqnt.py` & `nanoqnt-0.2.0rc2/nanoqnt/model/analyze_nanoqnt.py`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/util/make_hdf5.py` & `nanoqnt-0.2.0rc2/nanoqnt/util/make_hdf5.py`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11814 - Atom.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11814 - Atom.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11815 - Battery.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11815 - Battery.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11816 - Orbit.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11816 - Orbit.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11817 - Beaker.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11817 - Beaker.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11819 - Bounce.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11819 - Bounce.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11820 - Caliper.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11820 - Caliper.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11821 - Catapult.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11821 - Catapult.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11822 - Collision.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11822 - Collision.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11828 - Energy.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11828 - Energy.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11829 - Flask.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11829 - Flask.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11830 - Float.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11830 - Float.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11832 - Force.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11832 - Force.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11833 - Formula.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11833 - Formula.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11834 - Gears.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11834 - Gears.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11835 - Gravity.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11835 - Gravity.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11837 - Histogram.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11837 - Histogram.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11839 - Magnet.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11839 - Magnet.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11841 - Metronome.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11841 - Metronome.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11843 - Molecule.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11843 - Molecule.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11844 - Motion.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11844 - Motion.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11848 - Planet.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11848 - Planet.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11850 - Power.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11850 - Power.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11851 - Press.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11851 - Press.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11852 - Proton.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11852 - Proton.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11853 - Pulley.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11853 - Pulley.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11854 - Reflection.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11854 - Reflection.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11855 - Resistor.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11855 - Resistor.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11856 - Rolling.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11856 - Rolling.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11857 - Rotate.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11857 - Rotate.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11859 - Temperature.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11859 - Temperature.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11861 - Waves.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11861 - Waves.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/Icons/Save.svg` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/Icons/Save.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/channel_selector.ui` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/channel_selector.ui`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/data_exploration.ui` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/data_exploration.ui`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/particles_widget.ui` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/particles_widget.ui`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/GUI/scan_control.ui` & `nanoqnt-0.2.0rc2/nanoqnt/view/GUI/scan_control.ui`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/channel_selector.py` & `nanoqnt-0.2.0rc2/nanoqnt/view/channel_selector.py`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/main_window.py` & `nanoqnt-0.2.0rc2/nanoqnt/view/main_window.py`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/particle_widget.py` & `nanoqnt-0.2.0rc2/nanoqnt/view/particle_widget.py`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/nanoqnt/view/stage_control.py` & `nanoqnt-0.2.0rc2/nanoqnt/view/stage_control.py`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.0rc1/pyproject.toml` & `nanoqnt-0.2.0rc2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "nanoqnt"
-version = "0.2.0-rc1"
+version = "0.2.0-rc2"
 description = ""
 authors = ["Aquiles Carattino <carattino@dispertech.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "~3.11"
+python = "^3.8"
 pyqtgraph = "^0.13.3"
 numpy = "^1.24.3"
 scipy = "^1.10.1"
 scikit-image = "^0.20.0"
 PIMS = "^0.6.1"
 trackpy = "^0.6.1"
 h5py = "^3.8.0"
```

### Comparing `nanoqnt-0.2.0rc1/PKG-INFO` & `nanoqnt-0.2.0rc2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: nanoqnt
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: 
 Author: Aquiles Carattino
 Author-email: carattino@dispertech.com
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PIMS (>=0.6.1,<0.7.0)
 Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pyqt5 (>=5.15.9,<6.0.0)
 Requires-Dist: pyqtgraph (>=0.13.3,<0.14.0)
```

