# Comparing `tmp/brax-0.9.0.tar.gz` & `tmp/brax-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brax-0.9.0.tar", last modified: Thu Mar 30 22:28:37 2023, max compression
+gzip compressed data, was "brax-0.9.1.tar", last modified: Mon Jun 12 19:26:27 2023, max compression
```

## Comparing `brax-0.9.0.tar` & `brax-0.9.1.tar`

### file list

```diff
@@ -1,389 +1,422 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.125046 brax-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-30 22:28:21.000000 brax-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-30 22:28:21.000000 brax-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-03-30 22:28:37.125046 brax-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-03-30 22:28:21.000000 brax-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.085045 brax-0.9.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-30 22:28:21.000000 brax-0.9.0/bin/learn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.085045 brax-0.9.0/brax/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-30 22:28:21.000000 brax-0.9.0/brax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-30 22:28:21.000000 brax-0.9.0/brax/actuator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-03-30 22:28:21.000000 brax-0.9.0/brax/actuator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21329 2023-03-30 22:28:21.000000 brax-0.9.0/brax/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-03-30 22:28:21.000000 brax-0.9.0/brax/com.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-03-30 22:28:21.000000 brax-0.9.0/brax/com_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.089045 brax-0.9.0/brax/envs/
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/ant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.089045 brax-0.9.0/brax/envs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/assets/ant.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/assets/half_cheetah.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/assets/hopper.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/assets/humanoid.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)     9495 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/assets/humanoidstandup.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/assets/inverted_double_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/assets/inverted_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/assets/pusher.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/assets/reacher.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/assets/walker2d.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/env_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/half_cheetah.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/hopper.py
--rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/humanoid.py
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/humanoidstandup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/inverted_double_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/inverted_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/pusher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/reacher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/walker2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-03-30 22:28:21.000000 brax-0.9.0/brax/envs/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.089045 brax-0.9.0/brax/generalized/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/generalized/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-03-30 22:28:21.000000 brax-0.9.0/brax/generalized/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-03-30 22:28:21.000000 brax-0.9.0/brax/generalized/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-30 22:28:21.000000 brax-0.9.0/brax/generalized/constraint_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-03-30 22:28:21.000000 brax-0.9.0/brax/generalized/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-03-30 22:28:21.000000 brax-0.9.0/brax/generalized/dynamics_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-03-30 22:28:21.000000 brax-0.9.0/brax/generalized/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-03-30 22:28:21.000000 brax-0.9.0/brax/generalized/mass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-30 22:28:21.000000 brax-0.9.0/brax/generalized/mass_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-30 22:28:21.000000 brax-0.9.0/brax/generalized/perf_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-03-30 22:28:21.000000 brax-0.9.0/brax/generalized/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-30 22:28:21.000000 brax-0.9.0/brax/generalized/pipeline_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.089045 brax-0.9.0/brax/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-30 22:28:21.000000 brax-0.9.0/brax/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18937 2023-03-30 22:28:21.000000 brax-0.9.0/brax/geometry/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-03-30 22:28:21.000000 brax-0.9.0/brax/geometry/contact_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19828 2023-03-30 22:28:21.000000 brax-0.9.0/brax/geometry/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-03-30 22:28:21.000000 brax-0.9.0/brax/geometry/math_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-03-30 22:28:21.000000 brax-0.9.0/brax/geometry/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-03-30 22:28:21.000000 brax-0.9.0/brax/geometry/mesh_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.093045 brax-0.9.0/brax/io/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-03-30 22:28:21.000000 brax-0.9.0/brax/io/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-03-30 22:28:21.000000 brax-0.9.0/brax/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-30 22:28:21.000000 brax-0.9.0/brax/io/json_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-03-30 22:28:21.000000 brax-0.9.0/brax/io/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    18984 2023-03-30 22:28:21.000000 brax-0.9.0/brax/io/mjcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-03-30 22:28:21.000000 brax-0.9.0/brax/io/mjcf_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-30 22:28:21.000000 brax-0.9.0/brax/io/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-03-30 22:28:21.000000 brax-0.9.0/brax/kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-03-30 22:28:21.000000 brax-0.9.0/brax/kinematics_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-03-30 22:28:21.000000 brax-0.9.0/brax/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-03-30 22:28:21.000000 brax-0.9.0/brax/math_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.093045 brax-0.9.0/brax/positional/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/positional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-30 22:28:21.000000 brax-0.9.0/brax/positional/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-03-30 22:28:21.000000 brax-0.9.0/brax/positional/collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-03-30 22:28:21.000000 brax-0.9.0/brax/positional/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-03-30 22:28:21.000000 brax-0.9.0/brax/positional/joints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-03-30 22:28:21.000000 brax-0.9.0/brax/positional/joints_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-30 22:28:21.000000 brax-0.9.0/brax/positional/perf_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-03-30 22:28:21.000000 brax-0.9.0/brax/positional/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-03-30 22:28:21.000000 brax-0.9.0/brax/positional/pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-03-30 22:28:21.000000 brax-0.9.0/brax/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-03-30 22:28:21.000000 brax-0.9.0/brax/scan_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.093045 brax-0.9.0/brax/spring/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/spring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-03-30 22:28:21.000000 brax-0.9.0/brax/spring/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-03-30 22:28:21.000000 brax-0.9.0/brax/spring/collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-30 22:28:21.000000 brax-0.9.0/brax/spring/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-03-30 22:28:21.000000 brax-0.9.0/brax/spring/joints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-30 22:28:21.000000 brax-0.9.0/brax/spring/joints_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-30 22:28:21.000000 brax-0.9.0/brax/spring/perf_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-03-30 22:28:21.000000 brax-0.9.0/brax/spring/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-03-30 22:28:21.000000 brax-0.9.0/brax/spring/pipeline_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.097046 brax-0.9.0/brax/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/capsule.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/colour_objects.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/convex_convex.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/double_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/double_prismatic.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.081045 brax-0.9.0/brax/test_data/laikago/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.105046 brax-0.9.0/brax/test_data/laikago/meshes/
--rw-r--r--   0 runner    (1001) docker     (123)   711948 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/chassis.obj
--rw-r--r--   0 runner    (1001) docker     (123)   311084 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/chassis.stl
--rw-r--r--   0 runner    (1001) docker     (123)   169189 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/chassis_mod.obj
--rw-r--r--   0 runner    (1001) docker     (123)    23708 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/chassis_vhacd.obj
--rw-r--r--   0 runner    (1001) docker     (123)    32143 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/chassis_vhacd_mod.obj
--rw-r--r--   0 runner    (1001) docker     (123)    66809 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/chassis_vhacd_mod_zup.obj
--rw-r--r--   0 runner    (1001) docker     (123)   746953 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/chassis_zup.obj
--rw-r--r--   0 runner    (1001) docker     (123)    72588 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/chassis_zup_lores.obj
--rw-r--r--   0 runner    (1001) docker     (123)    59569 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/hip_motor.obj
--rw-r--r--   0 runner    (1001) docker     (123)    40484 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/hip_motor.stl
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/hip_motor_lores.obj
--rw-r--r--   0 runner    (1001) docker     (123)    59686 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/hip_motor_mirror.obj
--rw-r--r--   0 runner    (1001) docker     (123)    40484 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/hip_motor_mirror.stl
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/hip_motor_mirror_lores.obj
--rw-r--r--   0 runner    (1001) docker     (123)   330874 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/lower_leg3.obj
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/lower_leg3_lores.obj
--rw-r--r--   0 runner    (1001) docker     (123)   188884 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/lower_leg_3.stl
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/lower_leg_3_collision.stl
--rw-r--r--   0 runner    (1001) docker     (123)   112984 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/upper_leg.stl
--rw-r--r--   0 runner    (1001) docker     (123)   210097 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_left.obj
--rw-r--r--   0 runner    (1001) docker     (123)   210149 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_left2.obj
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_left2_lores.obj
--rw-r--r--   0 runner    (1001) docker     (123)    16386 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_left_lores.obj
--rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_left_vhacd.obj
--rw-r--r--   0 runner    (1001) docker     (123)   180144 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_mirror.obj
--rw-r--r--   0 runner    (1001) docker     (123)   112984 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_mirror.stl
--rw-r--r--   0 runner    (1001) docker     (123)   180145 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_mirror2.obj
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_mirror2_lores.obj
--rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_mirror_lores.obj
--rw-r--r--   0 runner    (1001) docker     (123)   199652 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_right.obj
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_right_vhacd.obj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.105046 brax-0.9.0/brax/test_data/meshes/
--rw-r--r--   0 runner    (1001) docker     (123)    20884 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/meshes/cylinder.stl
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/meshes/dodecahedron.stl
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/meshes/pyramid.stl
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/meshes/tetrahedron.stl
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/nonzero_joint_ref.xml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/prismaversal_2dof_joint.xml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/prismaversal_3dof_joint.xml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/single_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/single_pendulum_motor.xml
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/single_pendulum_position.xml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/single_prismatic.xml
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/single_spherical_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/single_spherical_pendulum_motor.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/single_spherical_pendulum_position.xml
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/single_universal_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/triple_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/triple_pendulum_motor.xml
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/triple_prismatic.xml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_data/world_body_transform.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-03-30 22:28:21.000000 brax-0.9.0/brax/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.105046 brax-0.9.0/brax/training/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.105046 brax-0.9.0/brax/training/acme/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/acme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/acme/running_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/acme/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/acme/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/acting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.105046 brax-0.9.0/brax/training/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.105046 brax-0.9.0/brax/training/agents/apg/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/apg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/apg/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/apg/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/apg/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.105046 brax-0.9.0/brax/training/agents/ars/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/ars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/ars/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/ars/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/ars/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.105046 brax-0.9.0/brax/training/agents/es/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/es/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/es/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/es/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.109046 brax-0.9.0/brax/training/agents/ppo/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/ppo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/ppo/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/ppo/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/ppo/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/ppo/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.109046 brax-0.9.0/brax/training/agents/sac/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/sac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/sac/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/sac/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/sac/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/agents/sac/train_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/pmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/replay_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/replay_buffers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/spectral_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-03-30 22:28:21.000000 brax-0.9.0/brax/training/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.109046 brax-0.9.0/brax/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.109046 brax-0.9.0/brax/v1/envs/
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/acrobot.py
--rw-r--r--   0 runner    (1001) docker     (123)    26290 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/ant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    27963 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/grasp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24287 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/half_cheetah.py
--rw-r--r--   0 runner    (1001) docker     (123)    16976 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/hopper.py
--rw-r--r--   0 runner    (1001) docker     (123)    43652 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/humanoid.py
--rw-r--r--   0 runner    (1001) docker     (123)    45541 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/humanoid_standup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/inverted_double_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/inverted_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (123)    20254 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/pusher.py
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/reacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/reacherangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/swimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/to_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14733 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/ur5e.py
--rw-r--r--   0 runner    (1001) docker     (123)    22667 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/walker2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    14892 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/envs/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.109046 brax-0.9.0/brax/v1/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.109046 brax-0.9.0/brax/v1/experimental/biggym/
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/biggym/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/biggym/registry/ant/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/registry/ant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/biggym/registry/ant/components/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/registry/ant/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/registry/ant/components/ant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/biggym/registry/jump/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/registry/jump/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/biggym/registry/jump/envs/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/registry/jump/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/registry/jump/envs/cheetah.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/biggym/registry/proant/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/registry/proant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/biggym/registry/proant/components/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/registry/proant/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/registry/proant/components/ant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/biggym/registry/proant/envs/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/registry/proant/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/registry/proant/envs/ant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/biggym/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/braxlines/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/braxlines/common/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/common/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/common/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/common/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/common/logger_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/common/sim_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/braxlines/envs/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/envs/obs_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/envs/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/braxlines/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/experiments/chase_ma_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/experiments/composer_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/experiments/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/experiments/dmin_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/experiments/mimax_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/experiments/sumo_ma_sweep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/braxlines/irl_smm/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/irl_smm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/irl_smm/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/irl_smm/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    13557 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/irl_smm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.113046 brax-0.9.0/brax/v1/experimental/braxlines/training/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/training/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    20552 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/training/ppo.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/training/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.117046 brax-0.9.0/brax/v1/experimental/braxlines/vgcrl/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/vgcrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/vgcrl/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/vgcrl/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    14671 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/braxlines/vgcrl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.117046 brax-0.9.0/brax/v1/experimental/composer/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/agent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/component_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.117046 brax-0.9.0/brax/v1/experimental/composer/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/components/ant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/components/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/components/ground.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/components/halfcheetah.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/components/humanoid.py
--rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/components/octopus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/components/pro_ant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/components/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    20635 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/composer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/data_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.117046 brax-0.9.0/brax/v1/experimental/composer/envs/
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/envs/ma_descs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/envs/sa_descs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/observers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/reward_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.117046 brax-0.9.0/brax/v1/experimental/composer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/tests/composer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.117046 brax-0.9.0/brax/v1/experimental/composer/training/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23341 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/composer/training/mappo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.117046 brax-0.9.0/brax/v1/experimental/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/tracing/customize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/tracing/randomizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/tracing/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/experimental/tracing/wrappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.121046 brax-0.9.0/brax/v1/io/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/io/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/io/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/io/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/io/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/io/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/io/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/io/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/io/npy_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/io/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18608 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/jumpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.121046 brax-0.9.0/brax/v1/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/physics/actuators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/physics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/physics/bodies.py
--rw-r--r--   0 runner    (1001) docker     (123)    40679 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/physics/colliders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17184 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/physics/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/physics/forces.py
--rw-r--r--   0 runner    (1001) docker     (123)    37491 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/physics/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/physics/integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/physics/joints.py
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/physics/spring_joints.py
--rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/physics/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/pytree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.121046 brax-0.9.0/brax/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tests/colliders_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tests/env_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tests/geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tests/grasp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tests/jumpy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tests/math_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23529 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tests/physics_legacy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    29993 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tests/physics_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tests/running_statistics_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tests/urdf_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.121046 brax-0.9.0/brax/v1/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20203 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tools/mujoco.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tools/mujoco_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tools/print_mesh_com.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tools/urdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-03-30 22:28:21.000000 brax-0.9.0/brax/v1/tools/urdf_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.121046 brax-0.9.0/brax/visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-03-30 22:28:21.000000 brax-0.9.0/brax/visualizer/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-30 22:28:21.000000 brax-0.9.0/brax/visualizer/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.121046 brax-0.9.0/brax/visualizer/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-03-30 22:28:21.000000 brax-0.9.0/brax/visualizer/js/animator.js
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-03-30 22:28:21.000000 brax-0.9.0/brax/visualizer/js/selector.js
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-03-30 22:28:21.000000 brax-0.9.0/brax/visualizer/js/system.js
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-03-30 22:28:21.000000 brax-0.9.0/brax/visualizer/js/viewer.js
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-03-30 22:28:21.000000 brax-0.9.0/brax/visualizer/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 22:28:37.085045 brax-0.9.0/brax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-03-30 22:28:36.000000 brax-0.9.0/brax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-03-30 22:28:37.000000 brax-0.9.0/brax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 22:28:36.000000 brax-0.9.0/brax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-30 22:28:36.000000 brax-0.9.0/brax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-30 22:28:36.000000 brax-0.9.0/brax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 22:28:37.125046 brax-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-03-30 22:28:21.000000 brax-0.9.0/setup.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.559918 brax-0.9.1/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    11356 2023-06-12 19:02:01.000000 brax-0.9.1/LICENSE
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      124 2023-06-12 19:02:01.000000 brax-0.9.1/MANIFEST.in
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6632 2023-06-12 19:26:27.559918 brax-0.9.1/PKG-INFO
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     5955 2023-06-12 19:02:01.000000 brax-0.9.1/README.md
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.511918 brax-0.9.1/bin/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      130 2023-06-12 19:02:01.000000 brax-0.9.1/bin/learn
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.515918 brax-0.9.1/brax/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      801 2023-06-12 19:02:01.000000 brax-0.9.1/brax/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1785 2023-06-12 19:02:01.000000 brax-0.9.1/brax/actuator.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     7604 2023-06-12 19:02:01.000000 brax-0.9.1/brax/actuator_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    21958 2023-06-12 19:02:01.000000 brax-0.9.1/brax/base.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1995 2023-06-12 19:02:01.000000 brax-0.9.1/brax/com.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2947 2023-06-12 19:02:01.000000 brax-0.9.1/brax/com_test.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.515918 brax-0.9.1/brax/envs/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3130 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    14345 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/ant.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.519918 brax-0.9.1/brax/envs/assets/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     5864 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/assets/ant.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6107 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/assets/half_cheetah.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3583 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/assets/hopper.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     9017 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/assets/humanoid.xml
+-rwxr-x---   0 btaba    (689214) primarygroup (89939)     9495 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/assets/humanoidstandup.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2195 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/assets/inverted_double_pendulum.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1586 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/assets/inverted_pendulum.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     5961 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/assets/pusher.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2704 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/assets/reacher.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4633 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/assets/walker2d.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4797 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/base.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1687 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/env_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2062 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/fast.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     9982 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/half_cheetah.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    11839 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/hopper.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    23141 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/humanoid.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    21224 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/humanoidstandup.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6866 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/inverted_double_pendulum.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     5381 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/inverted_pendulum.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    12195 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/pusher.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    10532 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/reacher.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    12036 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/walker2d.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.519918 brax-0.9.1/brax/envs/wrappers/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/wrappers/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3965 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/wrappers/dm_env.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     5187 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/wrappers/gym.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1678 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/wrappers/torch.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6121 2023-06-12 19:02:01.000000 brax-0.9.1/brax/envs/wrappers/training.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2884 2023-06-12 19:02:01.000000 brax-0.9.1/brax/fluid.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4317 2023-06-12 19:02:01.000000 brax-0.9.1/brax/fluid_test.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.519918 brax-0.9.1/brax/generalized/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/generalized/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3072 2023-06-12 19:02:01.000000 brax-0.9.1/brax/generalized/base.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     7887 2023-06-12 19:02:01.000000 brax-0.9.1/brax/generalized/constraint.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3182 2023-06-12 19:02:01.000000 brax-0.9.1/brax/generalized/constraint_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     8129 2023-06-12 19:02:01.000000 brax-0.9.1/brax/generalized/dynamics.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2787 2023-06-12 19:02:01.000000 brax-0.9.1/brax/generalized/dynamics_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2601 2023-06-12 19:02:01.000000 brax-0.9.1/brax/generalized/integrator.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3098 2023-06-12 19:02:01.000000 brax-0.9.1/brax/generalized/mass.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1553 2023-06-12 19:02:01.000000 brax-0.9.1/brax/generalized/mass_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1424 2023-06-12 19:02:01.000000 brax-0.9.1/brax/generalized/perf_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2692 2023-06-12 19:02:01.000000 brax-0.9.1/brax/generalized/pipeline.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1668 2023-06-12 19:02:01.000000 brax-0.9.1/brax/generalized/pipeline_test.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.519918 brax-0.9.1/brax/geometry/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      663 2023-06-12 19:02:01.000000 brax-0.9.1/brax/geometry/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    20626 2023-06-12 19:02:01.000000 brax-0.9.1/brax/geometry/contact.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    18064 2023-06-12 19:02:01.000000 brax-0.9.1/brax/geometry/contact_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    20103 2023-06-12 19:02:01.000000 brax-0.9.1/brax/geometry/math.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    15084 2023-06-12 19:02:01.000000 brax-0.9.1/brax/geometry/math_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     8264 2023-06-12 19:02:01.000000 brax-0.9.1/brax/geometry/mesh.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     5976 2023-06-12 19:02:01.000000 brax-0.9.1/brax/geometry/mesh_test.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.523918 brax-0.9.1/brax/io/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/io/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2301 2023-06-12 19:02:01.000000 brax-0.9.1/brax/io/html.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     7369 2023-06-12 19:02:01.000000 brax-0.9.1/brax/io/image.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1202 2023-06-12 19:02:01.000000 brax-0.9.1/brax/io/image_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4232 2023-06-12 19:02:01.000000 brax-0.9.1/brax/io/json.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1615 2023-06-12 19:02:01.000000 brax-0.9.1/brax/io/json_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1485 2023-06-12 19:02:01.000000 brax-0.9.1/brax/io/metrics.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    19766 2023-06-12 19:02:01.000000 brax-0.9.1/brax/io/mjcf.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6572 2023-06-12 19:02:01.000000 brax-0.9.1/brax/io/mjcf_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      982 2023-06-12 19:02:01.000000 brax-0.9.1/brax/io/model.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2993 2023-06-12 19:02:01.000000 brax-0.9.1/brax/io/torch.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    12906 2023-06-12 19:02:01.000000 brax-0.9.1/brax/kinematics.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     5900 2023-06-12 19:02:01.000000 brax-0.9.1/brax/kinematics_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    11971 2023-06-12 19:02:01.000000 brax-0.9.1/brax/math.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2690 2023-06-12 19:02:01.000000 brax-0.9.1/brax/math_test.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.523918 brax-0.9.1/brax/positional/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/positional/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1273 2023-06-12 19:02:01.000000 brax-0.9.1/brax/positional/base.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     8399 2023-06-12 19:02:01.000000 brax-0.9.1/brax/positional/collisions.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2755 2023-06-12 19:02:01.000000 brax-0.9.1/brax/positional/integrator.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     9194 2023-06-12 19:02:01.000000 brax-0.9.1/brax/positional/joints.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3429 2023-06-12 19:02:01.000000 brax-0.9.1/brax/positional/joints_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1335 2023-06-12 19:02:01.000000 brax-0.9.1/brax/positional/perf_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4128 2023-06-12 19:02:01.000000 brax-0.9.1/brax/positional/pipeline.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6175 2023-06-12 19:02:01.000000 brax-0.9.1/brax/positional/pipeline_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6700 2023-06-12 19:02:01.000000 brax-0.9.1/brax/scan.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4427 2023-06-12 19:02:01.000000 brax-0.9.1/brax/scan_test.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.523918 brax-0.9.1/brax/spring/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/spring/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1362 2023-06-12 19:02:01.000000 brax-0.9.1/brax/spring/base.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4126 2023-06-12 19:02:01.000000 brax-0.9.1/brax/spring/collisions.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1872 2023-06-12 19:02:01.000000 brax-0.9.1/brax/spring/integrator.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    10668 2023-06-12 19:02:01.000000 brax-0.9.1/brax/spring/joints.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2504 2023-06-12 19:02:01.000000 brax-0.9.1/brax/spring/joints_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1337 2023-06-12 19:02:01.000000 brax-0.9.1/brax/spring/perf_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3810 2023-06-12 19:02:01.000000 brax-0.9.1/brax/spring/pipeline.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    10700 2023-06-12 19:02:01.000000 brax-0.9.1/brax/spring/pipeline_test.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.527918 brax-0.9.1/brax/test_data/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      890 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/capsule.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1358 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/colour_objects.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1483 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/convex_convex.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1067 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/double_pendulum.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      525 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/double_prismatic.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      463 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/fat_cylinder.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      465 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/flat_cylinder.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      511 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/fluid_box.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      929 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/fluid_box_offset_com.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      563 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/fluid_ellipsoid.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      565 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/fluid_sphere.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      859 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/fluid_two_spheres.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      519 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/fluid_wind.xml
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.527918 brax-0.9.1/brax/test_data/laikago/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    16099 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/laikago_toes_zup.urdf
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    14646 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/laikago_viz.urdf
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.539918 brax-0.9.1/brax/test_data/laikago/meshes/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)   711948 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/chassis.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)   311084 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/chassis.stl
+-rw-r-----   0 btaba    (689214) primarygroup (89939)   169189 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/chassis_mod.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    23708 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/chassis_vhacd.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    32143 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/chassis_vhacd_mod.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    66809 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/chassis_vhacd_mod_zup.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)   746953 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/chassis_zup.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    72588 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/chassis_zup_lores.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    59569 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/hip_motor.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    40484 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/hip_motor.stl
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     7666 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/hip_motor_lores.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    59686 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/hip_motor_mirror.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    40484 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/hip_motor_mirror.stl
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6807 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/hip_motor_mirror_lores.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    12904 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/laikago.urdf
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    12527 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/laikago_no_toes.urdf
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    15792 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/laikago_toes.urdf
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    16088 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/laikago_toes_limits.urdf
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    15992 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/laikago_toes_zup.urdf
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    18044 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/laikago_toes_zup_chassis_collision.urdf
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    20646 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/laikago_toes_zup_chassis_collision_xyz_spherical.urdf
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    16183 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/laikago_toes_zup_joint_order.urdf
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    16070 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/laikago_toes_zup_lores.urdf
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    18770 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/laikago_toes_zup_xyz_xyzrot.urdf
+-rw-r-----   0 btaba    (689214) primarygroup (89939)   330874 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/lower_leg3.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     8677 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/lower_leg3_lores.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)   188884 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/lower_leg_3.stl
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     9484 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/lower_leg_3_collision.stl
+-rw-r-----   0 btaba    (689214) primarygroup (89939)   112984 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/upper_leg.stl
+-rw-r-----   0 btaba    (689214) primarygroup (89939)   210097 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_left.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)   210149 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_left2.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    11416 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_left2_lores.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    16386 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_left_lores.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    17380 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_left_vhacd.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)   180144 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_mirror.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)   112984 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_mirror.stl
+-rw-r-----   0 btaba    (689214) primarygroup (89939)   180145 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_mirror2.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    14652 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_mirror2_lores.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    15141 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_mirror_lores.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)   199652 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_right.obj
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    17337 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_right_vhacd.obj
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.539918 brax-0.9.1/brax/test_data/meshes/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    20884 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/meshes/cylinder.stl
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1884 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/meshes/dodecahedron.stl
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      384 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/meshes/pyramid.stl
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      284 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/meshes/tetrahedron.stl
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2803 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/nonzero_joint_ref.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      606 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/prismaversal_2dof_joint.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      803 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/prismaversal_3dof_joint.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      341 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/single_pendulum.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      755 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/single_pendulum_motor.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      721 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/single_pendulum_position.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      751 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/single_pendulum_position_frclimit.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      717 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/single_pendulum_velocity.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      446 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/single_prismatic.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      543 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/single_spherical_pendulum.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1075 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/single_spherical_pendulum_motor.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1084 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/single_spherical_pendulum_position.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      476 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/single_universal_pendulum.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      409 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/solver_params_v2.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1157 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/triple_pendulum.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1414 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/triple_pendulum_motor.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      784 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/triple_prismatic.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      842 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_data/world_body_transform.xml
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4174 2023-06-12 19:02:01.000000 brax-0.9.1/brax/test_utils.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.539918 brax-0.9.1/brax/training/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/__init__.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.539918 brax-0.9.1/brax/training/acme/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/acme/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     9571 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/acme/running_statistics.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1045 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/acme/specs.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1181 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/acme/types.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4863 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/acting.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.539918 brax-0.9.1/brax/training/agents/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/__init__.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.539918 brax-0.9.1/brax/training/agents/apg/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/apg/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2453 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/apg/networks.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     9244 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/apg/train.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2571 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/apg/train_test.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.539918 brax-0.9.1/brax/training/agents/ars/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/ars/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1706 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/ars/networks.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    10854 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/ars/train.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1965 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/ars/train_test.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.543918 brax-0.9.1/brax/training/agents/es/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/es/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2463 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/es/networks.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    13060 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/es/train.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2175 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/es/train_test.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.543918 brax-0.9.1/brax/training/agents/ppo/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/ppo/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6408 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/ppo/losses.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3257 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/ppo/networks.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    13427 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/ppo/train.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3342 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/ppo/train_test.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.543918 brax-0.9.1/brax/training/agents/sac/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/sac/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4322 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/sac/losses.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2745 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/sac/networks.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    18541 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/sac/train.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2755 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/agents/sac/train_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     5170 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/distribution.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2155 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/gradients.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    11348 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/learner.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6904 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/networks.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2083 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/pmap.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    16740 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/replay_buffers.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    22646 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/replay_buffers_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4597 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/spectral_norm.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2423 2023-06-12 19:02:01.000000 brax-0.9.1/brax/training/types.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.543918 brax-0.9.1/brax/v1/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      972 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/__init__.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/envs/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4335 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     5749 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/acrobot.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    26290 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/ant.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2859 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/env.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1904 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/fast.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    17282 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/fetch.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    27963 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/grasp.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    24287 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/half_cheetah.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    16976 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/hopper.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    43652 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/humanoid.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    45541 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/humanoid_standup.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    10497 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/inverted_double_pendulum.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     8172 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/inverted_pendulum.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    20254 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/pusher.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    14084 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/reacher.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     8179 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/reacherangle.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    16065 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/swimmer.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2146 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/to_torch.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    14733 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/ur5e.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    22667 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/walker2d.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    14892 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/envs/wrappers.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/experimental/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/__init__.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/experimental/biggym/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    10567 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/__init__.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/experimental/biggym/registry/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      914 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/registry/__init__.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/experimental/biggym/registry/ant/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      921 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/registry/ant/__init__.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/experimental/biggym/registry/ant/components/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/registry/ant/components/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      660 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/registry/ant/components/ant.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/experimental/biggym/registry/jump/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      996 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/registry/jump/__init__.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/experimental/biggym/registry/jump/envs/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/registry/jump/envs/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2204 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/registry/jump/envs/cheetah.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/experimental/biggym/registry/proant/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1033 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/registry/proant/__init__.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/experimental/biggym/registry/proant/components/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/registry/proant/components/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      706 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/registry/proant/components/ant.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/experimental/biggym/registry/proant/envs/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/registry/proant/envs/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1214 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/registry/proant/envs/ant.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3749 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/biggym/tasks.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/experimental/braxlines/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/__init__.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/experimental/braxlines/common/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/common/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6231 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/common/config_utils.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1254 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/common/dist_utils.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4519 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/common/evaluators.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     9959 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/common/logger_utils.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4813 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/common/sim_utils.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.547918 brax-0.9.1/brax/v1/experimental/braxlines/envs/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/envs/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1379 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/envs/obs_indices.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      984 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/envs/wrappers.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.551918 brax-0.9.1/brax/v1/experimental/braxlines/experiments/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    14122 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/experiments/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1271 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/experiments/chase_ma_sweep.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1370 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/experiments/composer_sweep.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4751 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/experiments/defaults.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1310 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/experiments/dmin_sweep.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1268 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/experiments/mimax_sweep.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1528 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/experiments/sumo_ma_sweep.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.551918 brax-0.9.1/brax/v1/experimental/braxlines/irl_smm/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/irl_smm/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4846 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/irl_smm/evaluators.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6920 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/irl_smm/train.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    13557 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/irl_smm/utils.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.551918 brax-0.9.1/brax/v1/experimental/braxlines/training/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/training/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3050 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/training/env.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    20552 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/training/ppo.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      814 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/training/utils.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.551918 brax-0.9.1/brax/v1/experimental/braxlines/vgcrl/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/vgcrl/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    11166 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/vgcrl/evaluators.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6717 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/vgcrl/train.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    14671 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/braxlines/vgcrl/utils.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.551918 brax-0.9.1/brax/v1/experimental/composer/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      887 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4946 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/agent_utils.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6029 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/component_editor.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.551918 brax-0.9.1/brax/v1/experimental/composer/components/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2701 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/components/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1590 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/components/ant.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1795 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/components/common.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      996 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/components/ground.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1089 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/components/halfcheetah.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1238 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/components/humanoid.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    22588 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/components/octopus.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3433 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/components/pro_ant.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1605 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/components/singleton.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    20635 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/composer.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2264 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/composer_utils.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4439 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/data_utils.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.555918 brax-0.9.1/brax/v1/experimental/composer/envs/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3712 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/envs/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    13125 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/envs/ma_descs.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     5099 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/envs/sa_descs.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     9890 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/observers.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     8499 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/reward_functions.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.555918 brax-0.9.1/brax/v1/experimental/composer/tests/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/tests/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3229 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/tests/composer_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3328 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/train.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.555918 brax-0.9.1/brax/v1/experimental/composer/training/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/training/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    23341 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/composer/training/mappo.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4412 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/normalization.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.555918 brax-0.9.1/brax/v1/experimental/tracing/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/tracing/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1581 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/tracing/customize.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3231 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/tracing/randomizers.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3200 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/tracing/wrappers.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1775 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/experimental/tracing/wrappers_test.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.555918 brax-0.9.1/brax/v1/io/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/io/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1867 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/io/export.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1374 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/io/file.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2340 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/io/html.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     7168 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/io/image.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2470 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/io/json.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1988 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/io/mesh.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1532 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/io/metrics.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      970 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/io/model.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1107 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/io/npy_file.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3441 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/io/torch.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    18608 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/jumpy.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6403 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/math.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.559918 brax-0.9.1/brax/v1/physics/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/physics/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6357 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/physics/actuators.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     8223 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/physics/base.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3685 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/physics/bodies.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    40679 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/physics/colliders.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    17184 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/physics/config_pb2.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4892 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/physics/forces.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    37491 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/physics/geometry.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     4822 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/physics/integrators.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    17079 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/physics/joints.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    13484 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/physics/spring_joints.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    15157 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/physics/system.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2017 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/pytree.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.559918 brax-0.9.1/brax/v1/tests/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tests/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     9982 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tests/colliders_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2246 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tests/env_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    14262 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tests/geometry_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1966 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tests/grasp_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1332 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tests/jumpy_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1379 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tests/math_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    23529 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tests/physics_legacy_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    29993 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tests/physics_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     5778 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tests/running_statistics_test.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2997 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tests/urdf_test.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.559918 brax-0.9.1/brax/v1/tools/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      582 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tools/__init__.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    20203 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tools/mujoco.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2997 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tools/mujoco_converter.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1291 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tools/print_mesh_com.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    10947 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tools/urdf.py
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     3024 2023-06-12 19:02:01.000000 brax-0.9.1/brax/v1/tools/urdf_converter.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.559918 brax-0.9.1/brax/visualizer/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    15406 2023-06-12 19:02:01.000000 brax-0.9.1/brax/visualizer/favicon.ico
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     1256 2023-06-12 19:02:01.000000 brax-0.9.1/brax/visualizer/index.html
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.559918 brax-0.9.1/brax/visualizer/js/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2933 2023-06-12 19:02:01.000000 brax-0.9.1/brax/visualizer/js/animator.js
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2882 2023-06-12 19:02:01.000000 brax-0.9.1/brax/visualizer/js/selector.js
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     9385 2023-06-12 19:02:01.000000 brax-0.9.1/brax/visualizer/js/system.js
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    11339 2023-06-12 19:02:01.000000 brax-0.9.1/brax/visualizer/js/viewer.js
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     5479 2023-06-12 19:02:01.000000 brax-0.9.1/brax/visualizer/visualizer.py
+drwxr-x---   0 btaba    (689214) primarygroup (89939)        0 2023-06-12 19:26:27.515918 brax-0.9.1/brax.egg-info/
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     6632 2023-06-12 19:26:27.000000 brax-0.9.1/brax.egg-info/PKG-INFO
+-rw-r-----   0 btaba    (689214) primarygroup (89939)    12950 2023-06-12 19:26:27.000000 brax-0.9.1/brax.egg-info/SOURCES.txt
+-rw-r-----   0 btaba    (689214) primarygroup (89939)        1 2023-06-12 19:26:27.000000 brax-0.9.1/brax.egg-info/dependency_links.txt
+-rw-r-----   0 btaba    (689214) primarygroup (89939)      257 2023-06-12 19:26:27.000000 brax-0.9.1/brax.egg-info/requires.txt
+-rw-r-----   0 btaba    (689214) primarygroup (89939)        5 2023-06-12 19:26:27.000000 brax-0.9.1/brax.egg-info/top_level.txt
+-rw-r-----   0 btaba    (689214) primarygroup (89939)       38 2023-06-12 19:26:27.559918 brax-0.9.1/setup.cfg
+-rw-r-----   0 btaba    (689214) primarygroup (89939)     2249 2023-06-12 19:02:01.000000 brax-0.9.1/setup.py
```

### Comparing `brax-0.9.0/LICENSE` & `brax-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/PKG-INFO` & `brax-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brax
-Version: 0.9.0
+Version: 0.9.1
 Summary: A differentiable physics engine written in JAX.
 Home-page: http://github.com/google/brax
 Author: Brax Authors
 Author-email: no-reply@google.com
 License: Apache 2.0
 Keywords: JAX reinforcement learning rigidbody physics
 Classifier: Development Status :: 4 - Beta
@@ -59,17 +59,16 @@
 and closing the gap between simulation and the real world.
 
 ## Quickstart: Colab in the Cloud
 
 Explore Brax easily and quickly through a series of colab notebooks:
 
 * [Brax Basics](https://colab.research.google.com/github/google/brax/blob/main/notebooks/basics.ipynb) introduces the Brax API, and shows how to simulate basic physics primitives.
-* [Brax Training](https://colab.research.google.com/github/google/brax/blob/main/notebooks/training.ipynb)
-introduces the Brax v2 API, and shows how to train a policy with the
-generalized backend.
+* [Brax Training](https://colab.research.google.com/github/google/brax/blob/main/notebooks/training.ipynb) introduces Brax's training algorithms, and lets you train your own policies directly within the colab. It also demonstrates loading and saving policies.
+* [Brax Training with PyTorch on GPU](https://colab.research.google.com/github/google/brax/blob/main/notebooks/training_torch.ipynb) demonstrates how Brax can be used in other ML frameworks for fast training, in this case PyTorch.
 
 ## Using Brax Locally
 
 To install Brax from pypi, install it with:
 
 ```
 python3 -m venv env
@@ -113,15 +112,15 @@
 If you would like to reference Brax in a publication, please use:
 
 ```
 @software{brax2021github,
   author = {C. Daniel Freeman and Erik Frey and Anton Raichuk and Sertan Girgin and Igor Mordatch and Olivier Bachem},
   title = {Brax - A Differentiable Physics Engine for Large Scale Rigid Body Simulation},
   url = {http://github.com/google/brax},
-  version = {0.9.0},
+  version = {0.9.1},
   year = {2021},
 }
 ```
 
 ## Acknowledgements
 
 Brax has come a long way since its original publication.  We offer gratitude and
```

### Comparing `brax-0.9.0/README.md` & `brax-0.9.1/brax.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: brax
+Version: 0.9.1
+Summary: A differentiable physics engine written in JAX.
+Home-page: http://github.com/google/brax
+Author: Brax Authors
+Author-email: no-reply@google.com
+License: Apache 2.0
+Keywords: JAX reinforcement learning rigidbody physics
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+Provides-Extra: develop
+License-File: LICENSE
+
 <img src="https://github.com/google/brax/raw/main/docs/img/brax_logo.gif" width="336" height="80" alt="BRAX"/>
 
 Brax is a fast and fully differentiable physics engine used for research and
 development of robotics, human perception, materials science, reinforcement
 learning, and other simulation-heavy applications.
 
 Brax is written in [JAX](https://github.com/google/jax) and is designed for use
@@ -40,17 +59,16 @@
 and closing the gap between simulation and the real world.
 
 ## Quickstart: Colab in the Cloud
 
 Explore Brax easily and quickly through a series of colab notebooks:
 
 * [Brax Basics](https://colab.research.google.com/github/google/brax/blob/main/notebooks/basics.ipynb) introduces the Brax API, and shows how to simulate basic physics primitives.
-* [Brax Training](https://colab.research.google.com/github/google/brax/blob/main/notebooks/training.ipynb)
-introduces the Brax v2 API, and shows how to train a policy with the
-generalized backend.
+* [Brax Training](https://colab.research.google.com/github/google/brax/blob/main/notebooks/training.ipynb) introduces Brax's training algorithms, and lets you train your own policies directly within the colab. It also demonstrates loading and saving policies.
+* [Brax Training with PyTorch on GPU](https://colab.research.google.com/github/google/brax/blob/main/notebooks/training_torch.ipynb) demonstrates how Brax can be used in other ML frameworks for fast training, in this case PyTorch.
 
 ## Using Brax Locally
 
 To install Brax from pypi, install it with:
 
 ```
 python3 -m venv env
@@ -94,15 +112,15 @@
 If you would like to reference Brax in a publication, please use:
 
 ```
 @software{brax2021github,
   author = {C. Daniel Freeman and Erik Frey and Anton Raichuk and Sertan Girgin and Igor Mordatch and Olivier Bachem},
   title = {Brax - A Differentiable Physics Engine for Large Scale Rigid Body Simulation},
   url = {http://github.com/google/brax},
-  version = {0.9.0},
+  version = {0.9.1},
   year = {2021},
 }
 ```
 
 ## Acknowledgements
 
 Brax has come a long way since its original publication.  We offer gratitude and
```

### Comparing `brax-0.9.0/brax/__init__.py` & `brax-0.9.1/brax/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Import top-level classes and functions here for encapsulation/clarity."""
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 from brax.base import Motion
 from brax.base import State
 from brax.base import System
 from brax.base import Transform
```

### Comparing `brax-0.9.0/brax/actuator_test.py` & `brax-0.9.1/brax/actuator_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     sys = test_utils.load_fixture('single_pendulum_motor.xml')
     mj_model = test_utils.load_fixture_mujoco('single_pendulum_motor.xml')
     mj_data = mujoco.MjData(mj_model)
     q, qd = jp.array(mj_data.qpos), jp.array(mj_data.qvel)
 
     tau = jp.array([0.5 * 9.81])  # -mgl sin(theta)
     act = jp.array([1.0 / 150.0 * 0.5 * 9.81])
-    tau2 = actuator.to_tau(sys, act, q)
+    tau2 = actuator.to_tau(sys, act, q, qd)
     np.testing.assert_array_almost_equal(tau, tau2, 5)
 
     q2, qd2 = _actuator_step(pipeline, sys, q, qd, act=act, dt=dt, n=n)
     np.testing.assert_array_almost_equal(q2, jp.array([0]), decimal=decimal)
     np.testing.assert_array_almost_equal(qd2, jp.array([0]), decimal=decimal)
 
   def test_position(self):
@@ -69,24 +69,61 @@
     mj_data = mujoco.MjData(mj_model)
     q, qd = jp.array(mj_data.qpos), jp.array(mj_data.qvel)
     theta = jp.pi / 2.0  # pendulum is vertical
     q = jp.array([theta])
 
     # a position actuator at the bottom should not move the pendulum
     act = jp.array([theta])
-    tau = actuator.to_tau(sys, act, q)
+    tau = actuator.to_tau(sys, act, q, qd)
     np.testing.assert_array_almost_equal(tau, jp.array([0]), 5)
 
     # put the pendulum into the horizontal position with the positional actuator
     # we know alpha = -2 theta/t^2, and I * alpha = (act-bias) * gear, and we
     # then solve for act. Semi-implicit Euler leaves off a factor of two.
     act = jp.array([-(theta * 0.5**2) / (0.01**2 * 10.0) + theta])
     q2, _ = _actuator_step(g_pipeline, sys, q, qd, act=act, dt=0.01, n=1)
     np.testing.assert_array_almost_equal(q2, jp.array([0]), 1)
 
+  def test_velocity(self):
+    """Tests a single pendulum with velocity actuator."""
+    sys = test_utils.load_fixture('single_pendulum_velocity.xml')
+    mj_model = test_utils.load_fixture_mujoco('single_pendulum_velocity.xml')
+    mj_data = mujoco.MjData(mj_model)
+    q, qd = jp.array(mj_data.qpos), jp.array(mj_data.qvel)
+    theta = jp.pi / 2.0  # pendulum is vertical
+    q = jp.array([theta])
+
+    act = jp.array([0])
+    tau = actuator.to_tau(sys, act, q, qd)
+    np.testing.assert_array_almost_equal(tau, jp.array([0]), 5)
+
+    # set the act to rotate at 1/s
+    act = jp.array([1])
+    _, qd = _actuator_step(g_pipeline, sys, q, qd, act=act, dt=0.001, n=200)
+    np.testing.assert_array_almost_equal(qd, jp.array([1]), 3)
+
+  def test_force_limitted(self):
+    """Tests that forcerange limits work on actuators."""
+    sys = test_utils.load_fixture('single_pendulum_position_frclimit.xml')
+    mj_model = test_utils.load_fixture_mujoco(
+        'single_pendulum_position_frclimit.xml'
+    )
+    mj_data = mujoco.MjData(mj_model)
+    q, qd = jp.array(mj_data.qpos), jp.array(mj_data.qvel)
+
+    for act, frclimit in [(1000, 3.1), (-1000, -2.5)]:
+      act = jp.array([act])
+      tau = actuator.to_tau(sys, act, q, qd)
+      # test that tau matches frclimit * 10, since gear=10
+      self.assertEqual(tau[0], frclimit * 10)
+      # test that tau matches MJ qfrc_actuator
+      mj_data.ctrl = act
+      mujoco.mj_step(mj_model, mj_data)
+      self.assertEqual(tau[0], mj_data.qfrc_actuator)
+
   @parameterized.parameters((g_pipeline,), (s_pipeline,), (p_pipeline,))
   def test_three_link_pendulum(self, pipeline):
     """Tests a three link pendulum with a motor actuator."""
     sys = test_utils.load_fixture('triple_pendulum_motor.xml')
     mj_model = test_utils.load_fixture_mujoco('triple_pendulum_motor.xml')
     mj_data = mujoco.MjData(mj_model)
     q, qd = jp.array(mj_data.qpos), jp.array(mj_data.qvel)
@@ -126,22 +163,25 @@
       mujoco.mj_step(mj_model, mj_data)
     mq, mqd = jp.asarray(mj_data.qpos), jp.asarray(mj_data.qvel)
 
     gq, gqd = _actuator_step(g_pipeline, sys, q, qd, act=act, dt=sys.dt, n=1000)
     np.testing.assert_array_almost_equal(gq, mq, 3)
     np.testing.assert_array_almost_equal(gqd, mqd, 3)
 
-  # TODO: test spherical pendulum once it's implemented in positional
   @parameterized.parameters(
-      ('single_pendulum_position.xml',), 'single_pendulum_motor.xml'
+      'single_pendulum_position.xml',
+      'single_pendulum_motor.xml',
+      'single_spherical_pendulum_position.xml',
   )
   def test_single_pendulum_spring_positional(self, config):
     sys = test_utils.load_fixture(config)
     act = jp.array([0.05, 0.1, 0.15])[: sys.act_size()]
+
     q, qd = sys.init_q, jp.zeros(sys.qd_size())
+
     sq, sqd = _actuator_step(s_pipeline, sys, q, qd, act=act, dt=sys.dt, n=500)
     pq, pqd = _actuator_step(p_pipeline, sys, q, qd, act=act, dt=sys.dt, n=500)
     np.testing.assert_array_almost_equal(sq, pq, 2)
     np.testing.assert_array_almost_equal(sqd, pqd, 2)
 
 
 if __name__ == '__main__':
```

### Comparing `brax-0.9.0/brax/base.py` & `brax-0.9.1/brax/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -221,16 +221,16 @@
 
 
 @struct.dataclass
 class Inertia(Base):
   """Angular inertia, mass, and center of mass location.
 
   Attributes:
-    transform: transform from inertia frame to link frame, corresponding to
-      center of mass position and orientation
+    transform: transform for the inertial frame relative to the link frame
+      (i.e. center of mass position and orientation)
     i: (3, 3) inertia matrix about a point P
     mass: scalar mass
   """
 
   transform: Transform
   i: jp.ndarray
   mass: jp.ndarray
@@ -247,16 +247,16 @@
 class Link(Base):
   """A rigid segment of an articulated body.
 
   Links are connected to each other by joints.  By moving (rotating or
   translating) the joints, the entire system can be articulated.
 
   Attributes:
-    transform: transform from link frame to its parent
-    joint: location of joint in link frame
+    transform: transform for the link frame relative to the parent frame
+    joint: transform for the joint frame relative to the link frame
     inertia: mass, center of mass location, and inertia of this link
     invweight: mean inverse inertia at init_q
     constraint_stiffness: (num_link,) constraint spring for joint.
     constraint_vel_damping: (num_link,) linear damping for constraint spring.
     constraint_limit_stiffness: (num_link,) constraint for angle limits
     constraint_ang_damping: (num_link,) angular damping for constraint spring.
   """
@@ -265,56 +265,60 @@
   joint: Transform
   inertia: Inertia
   invweight: jp.ndarray
   # only used by `brax.physics.spring`:
   constraint_stiffness: jp.ndarray
   constraint_vel_damping: jp.ndarray
   constraint_limit_stiffness: jp.ndarray
-  # only used by `brax.physics.spring` and `brax.physics.pbd`:
+  # only used by `brax.physics.spring` and `brax.physics.positional`:
   constraint_ang_damping: jp.ndarray
 
 
 @struct.dataclass
 class DoF(Base):
   """A degree of freedom in the system.
 
   Attributes:
     motion: spatial motion (linear or angular) of this DoF
     armature: models the inertia of a rotor (moving part of a motor)
     stiffness: restorative force back to zero position
     damping: restorative force back to zero velocity
     limit: tuple of min, max angle limits
     invweight: diagonal inverse inertia at init_qpos
+    solver_params: (7,) limit constraint solver parameters
   """
 
   motion: Motion
   armature: jp.ndarray
   stiffness: jp.ndarray
   damping: jp.ndarray
   limit: Tuple[jp.ndarray, jp.ndarray]
   # only used by `brax.physics.generalized`:
   invweight: jp.ndarray
+  solver_params: jp.ndarray
 
 
 @struct.dataclass
 class Geometry(Base):
   """A surface or spatial volume with a shape and material properties.
 
   Attributes:
     link_idx: Link index to which this Geometry is attached
-    transform: transform from this geometry's coordinate space to its parent
-      link, or to world space in the case of unparented geometry
+    transform: transform for the geometry frame relative to the link frame, or
+      relative to the world frame in the case of unparented geometry
     friction: resistance encountered when sliding against another geometry
     elasticity: bounce/restitution encountered when hitting another geometry
+    solver_params: (7,) solver parameters (reference, impedance)
   """
 
   link_idx: Optional[jp.ndarray]
   transform: Transform
   friction: jp.ndarray
   elasticity: jp.ndarray
+  solver_params: jp.ndarray
 
 
 @struct.dataclass
 class Sphere(Geometry):
   """A sphere.
 
   Attributes:
@@ -351,14 +355,29 @@
   """
 
   halfsize: jp.ndarray
   rgba: Optional[jp.ndarray] = None
 
 
 @struct.dataclass
+class Cylinder(Geometry):
+  """A cylinder.
+
+  Attributes:
+    radius: (1,) radius of the top and bottom of the cylinder
+    length: (1,) length of the cylinder
+    rgba: (4,) the rgba to display in the renderer
+  """
+
+  radius: jp.ndarray
+  length: jp.ndarray
+  rgba: Optional[jp.ndarray] = None
+
+
+@struct.dataclass
 class Plane(Geometry):
   """An infinite plane whose normal points at +z in its coordinate space.
 
   Attributes:
     rgba: (4,) the rgba to display in the renderer, currently unused
   """
 
@@ -406,40 +425,53 @@
   Attributes:
     pos: contact position, or average of the two closest points, in world frame
     normal: contact normal on the surface of geometry b
     penetration: penetration distance between two geometries. positive means the
       two geometries are interpenetrating, negative means they are not
     friction: resistance encountered when sliding against another geometry
     elasticity: bounce/restitution encountered when hitting another geometry
+    solver_params: (7,) collision constraint solver parameters
     link_idx: Tuple of link indices participating in contact.  The second part
       of the tuple can be None if the second geometry is static.
   """
 
   pos: jp.ndarray
   normal: jp.ndarray
   penetration: jp.ndarray
   friction: jp.ndarray
-  # only used by `brax.physics.spring` and `brax.physics.pbd`:
+  # only used by `brax.physics.spring` and `brax.physics.positional`:
   elasticity: jp.ndarray
+  solver_params: jp.ndarray
 
   link_idx: Tuple[jp.ndarray, Optional[jp.ndarray]]
 
 
 @struct.dataclass
 class Actuator(Base):
   """Actuator, transforms an input signal into a force (motor or thruster).
 
   Attributes:
-    ctrl_range: (num_actuators, 2) control range for each actuator
-    gear: (num_actuators,) a list of floats used as a scaling factor for each
-      actuator torque output
+    q_id: (num_actuators,) q index associated with an actuator
+    qd_id: (num_actuators,) qd index associated with an actuator
+    ctrl_range: (num_actuators, 2) actuator control range
+    force_range: (num_actuators, 2) actuator force range
+    gain: (num_actuators,) scaling factor for each actuator control input
+    gear: (num_actuators,) scaling factor for each actuator force output
+    bias_q: (num_actuators,) bias applied by q (e.g. position actuators)
+    bias_qd: (num_actuators,) bias applied by qd (e.g. velocity actuators)
   """
 
+  q_id: jp.ndarray
+  qd_id: jp.ndarray
   ctrl_range: jp.ndarray
+  force_range: jp.ndarray
+  gain: jp.ndarray
   gear: jp.ndarray
+  bias_q: jp.ndarray
+  bias_qd: jp.ndarray
 
 
 @struct.dataclass
 class State:
   """Dynamic state that changes after every pipeline step.
 
   Attributes:
@@ -460,82 +492,74 @@
 @struct.dataclass
 class System:
   r"""Describes a physical environment: its links, joints and geometries.
 
   Attributes:
     dt: timestep used for the simulation
     gravity: (3,) linear universal force applied during forward dynamics
+    viscosity: (1,) viscosity of the medium applied to all links
+    density: (1,) density of the medium applied to all links
     link: (num_link,) the links in the system
     dof: (qd_size,) every degree of freedom for the system
     geoms: list of batched geoms grouped by type
     actuator: actuators that can be applied to links
     init_q: (q_size,) initial q position for the system
-    solver_params_joint: (7,) joint limit constraint solver parameters
-    solver_params_contact: (7,) collision constraint solver parameters
     vel_damping: (1,) linear vel damping applied to each body.
     ang_damping: (1,) angular vel damping applied to each body.
     baumgarte_erp: how aggressively interpenetrating bodies should push away\
                 from one another
     spring_mass_scale: a float that scales mass as `mass^(1 - x)`
     spring_inertia_scale: a float that scales inertia diag as `inertia^(1 - x)`
     joint_scale_ang: scale for position-based joint rotation update
     joint_scale_pos: scale for position-based joint position update
     collide_scale: fraction of position based collide update to apply
+    enable_fluid: (1,) enables or disables fluid forces based on the
+      default viscosity and density parameters provided in the XML
     geom_masks: 64-bit mask determines whether two geoms will be contact tested.
                 lower 32 bits are type, upper 32 bits are affinity.  two geoms
                 a, b will be contact tested if a.type & b.affinity != 0
     link_names: (num_link,) link names
     link_types: (num_link,) string specifying the joint type of each link
                 valid types are:
                 * 'f': free, full 6 dof (position + rotation), no parent link
                 * '1': revolute,  1 dof, like a hinge
                 * '2': universal, 2 dof, like a drive shaft joint
                 * '3': spherical, 3 dof, like a ball joint
     link_parents: (num_link,) int list specifying the index of each link's
                   parent link, or -1 if the link has no parent
-    actuator_types: (num_actuators,) string specifying the actuator types:
-                * 't': torque
-                * 'p': position
-    actuator_link_id: (num_actuators,) the link id associated with each actuator
-    actuator_qid: (num_actuators,) the q index associated with each actuator
-    actuator_qdid: (num_actuators,) the qd index associated with each actuator
     matrix_inv_iterations: maximum number of iterations of the matrix inverse
     solver_iterations: maximum number of iterations of the constraint solver
     solver_maxls: maximum number of line searches of the constraint solver
   """
 
   dt: jp.ndarray
   gravity: jp.ndarray
+  viscosity: jp.float32
+  density: jp.float32
   link: Link
   dof: DoF
   geoms: List[Geometry]
   actuator: Actuator
   init_q: jp.ndarray
-  # only used in `brax.physics.generalized`
-  solver_params_joint: jp.ndarray
-  solver_params_contact: jp.ndarray
-  # only used in `brax.physics.spring` and `brax.physics.pbd`:
+  # only used in `brax.physics.spring` and `brax.physics.positional`:
   vel_damping: jp.float32
   ang_damping: jp.float32
   baumgarte_erp: jp.float32
   spring_mass_scale: jp.float32
   spring_inertia_scale: jp.float32
-  # only used in `brax.physics.positional`
+  # only used in `brax.physics.positional`:
   joint_scale_ang: jp.float32
   joint_scale_pos: jp.float32
   collide_scale: jp.float32
-
+  # non-pytree nodes
+  enable_fluid: bool = struct.field(pytree_node=False)
   geom_masks: List[int] = struct.field(pytree_node=False)
   link_names: List[str] = struct.field(pytree_node=False)
   link_types: str = struct.field(pytree_node=False)
   link_parents: Tuple[int, ...] = struct.field(pytree_node=False)
-  actuator_types: str = struct.field(pytree_node=False)
-  actuator_link_id: List[int] = struct.field(pytree_node=False)
-  actuator_qid: List[int] = struct.field(pytree_node=False)
-  actuator_qdid: List[int] = struct.field(pytree_node=False)
   # only used in `brax.physics.generalized`:
   matrix_inv_iterations: int = struct.field(pytree_node=False)
   solver_iterations: int = struct.field(pytree_node=False)
   solver_maxls: int = struct.field(pytree_node=False)
 
   def num_links(self) -> int:
     """Returns the number of links in the system."""
@@ -591,15 +615,15 @@
 
   def qd_size(self) -> int:
     """Returns the size of the qd vector (joint velocity) for this system."""
     return sum([QD_WIDTHS[t] for t in self.link_types])
 
   def act_size(self) -> int:
     """Returns the act dimension for the system."""
-    return sum({'m': 1, 'p': 1}[act_typ] for act_typ in self.actuator_types)
+    return self.actuator.q_id.shape[0]
 
 
 # below are some operation dispatch derivations
 
 
 @functools.singledispatch
 def _transform_do(other, self: Transform):
```

### Comparing `brax-0.9.0/brax/com.py` & `brax-0.9.1/brax/com.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/com_test.py` & `brax-0.9.1/brax/com_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/envs/__init__.py` & `brax-0.9.1/brax/envs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 from brax.envs import humanoid
 from brax.envs import humanoidstandup
 from brax.envs import inverted_double_pendulum
 from brax.envs import inverted_pendulum
 from brax.envs import pusher
 from brax.envs import reacher
 from brax.envs import walker2d
-from brax.envs import wrapper
-from brax.envs.env import Env, State
+from brax.envs.base import Env, PipelineEnv, State, Wrapper
+from brax.envs.wrappers import training
 
 _envs = {
     'ant': ant.Ant,
     'fast': fast.Fast,
     'halfcheetah': half_cheetah.Halfcheetah,
     'hopper': hopper.Hopper,
     'humanoid': humanoid.Humanoid,
@@ -91,14 +91,14 @@
 
   Returns:
     env: an environment
   """
   env = _envs[env_name](**kwargs)
 
   if episode_length is not None:
-    env = wrapper.EpisodeWrapper(env, episode_length, action_repeat)
+    env = training.EpisodeWrapper(env, episode_length, action_repeat)
   if batch_size:
-    env = wrapper.VmapWrapper(env, batch_size)
+    env = training.VmapWrapper(env, batch_size)
   if auto_reset:
-    env = wrapper.AutoResetWrapper(env)
+    env = training.AutoResetWrapper(env)
 
-  return env  # type: ignore
+  return env
```

### Comparing `brax-0.9.0/brax/envs/ant.py` & `brax-0.9.1/brax/envs/ant.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # limitations under the License.
 
 # pylint:disable=g-multiple-import
 """Trains an ant to run in the +x direction."""
 
 from brax import base
 from brax import math
-from brax.envs import env
+from brax.envs.base import PipelineEnv, State
 from brax.io import mjcf
 from etils import epath
 import jax
 from jax import numpy as jp
 
 
-class Ant(env.PipelineEnv):
+class Ant(PipelineEnv):
 
 
 
   # pyformat: disable
   """
   ### Description
 
@@ -135,43 +135,14 @@
   ### Episode Termination
 
   The episode terminates when any of the following happens:
 
   1. The episode duration reaches a 1000 timesteps
   2. The y-orientation (index 2) in the state is **not** in the range
      `[0.2, 1.0]`
-
-  ### Arguments
-
-  No additional arguments are currently supported (in v2 and lower), but
-  modifications can be made to the XML file in the assets folder (or by changing
-  the path to a modified XML file in another folder).
-
-  ```
-  env = gym.make('Ant-v2')
-  ```
-
-  v3, v4, and v5 take gym.make kwargs such as ctrl_cost_weight,
-  reset_noise_scale etc.
-
-  ```
-  env = gym.make('Ant-v5', ctrl_cost_weight=0.1, ....)
-  ```
-
-  ### Version History
-
-  * v5: ported to Brax.
-  * v4: all mujoco environments now use the mujoco bindings in mujoco>=2.1.3
-  * v3: support for gym.make kwargs such as xml_file, ctrl_cost_weight,
-        reset_noise_scale etc. rgb rendering comes from tracking camera (so
-        agent does not run away from screen)
-  * v2: All continuous control environments now use mujoco_py >= 1.50
-  * v1: max_time_steps raised to 1000 for robot based tasks. Added
-        reward_threshold to environments.
-  * v0: Initial versions release (1.0.0)
   """
   # pyformat: enable
 
 
   def __init__(
       self,
       ctrl_cost_weight=0.5,
@@ -218,15 +189,15 @@
     self._exclude_current_positions_from_observation = (
         exclude_current_positions_from_observation
     )
 
     if self._use_contact_forces:
       raise NotImplementedError('use_contact_forces not implemented.')
 
-  def reset(self, rng: jp.ndarray) -> env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     """Resets the environment to an initial state."""
     rng, rng1, rng2 = jax.random.split(rng, 3)
 
     low, hi = -self._reset_noise_scale, self._reset_noise_scale
     q = self.sys.init_q + jax.random.uniform(
         rng1, (self.sys.q_size(),), minval=low, maxval=hi
     )
@@ -244,17 +215,17 @@
         'x_position': zero,
         'y_position': zero,
         'distance_from_origin': zero,
         'x_velocity': zero,
         'y_velocity': zero,
         'forward_reward': zero,
     }
-    return env.State(pipeline_state, obs, reward, done, metrics)
+    return State(pipeline_state, obs, reward, done, metrics)
 
-  def step(self, state: env.State, action: jp.ndarray) -> env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     """Run one timestep of the environment's dynamics."""
     pipeline_state0 = state.pipeline_state
     pipeline_state = self.pipeline_step(pipeline_state0, action)
 
     velocity = (pipeline_state.x.pos[0] - pipeline_state0.x.pos[0]) / self.dt
     forward_reward = velocity[0]
```

### Comparing `brax-0.9.0/brax/envs/assets/ant.xml` & `brax-0.9.1/brax/envs/assets/ant.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/envs/assets/half_cheetah.xml` & `brax-0.9.1/brax/envs/assets/half_cheetah.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/envs/assets/humanoid.xml` & `brax-0.9.1/brax/envs/assets/humanoid.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/envs/assets/humanoidstandup.xml` & `brax-0.9.1/brax/envs/assets/humanoidstandup.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/envs/assets/inverted_double_pendulum.xml` & `brax-0.9.1/brax/envs/assets/inverted_double_pendulum.xml`

 * *Files 8% similar despite different names*

#### Comparing `brax-0.9.0/brax/envs/assets/inverted_double_pendulum.xml` & `brax-0.9.1/brax/envs/assets/inverted_double_pendulum.xml`

```diff
@@ -20,14 +20,15 @@
     <numeric data="2" name="frame_skip"/>
     <!-- brax custom params -->
     <numeric data="30000" name="constraint_stiffness"/>
     <numeric data="500 30 30" name="constraint_vel_damping"/>
     <numeric data="30000" name="constraint_limit_stiffness"/>
     <numeric data="0" name="spring_mass_scale"/>
     <numeric data="1" name="spring_inertia_scale"/>
+    <numeric data="5" name="solver_maxls"/>
   </custom>
   <default>
     <joint damping="0.05"/>
     <geom contype="0" friction="1 0.1 0.1"/>
   </default>
   <option gravity="1e-5 0 -9.81" timestep="0.01"/>
   <size nstack="3000"/>
```

### Comparing `brax-0.9.0/brax/envs/assets/inverted_pendulum.xml` & `brax-0.9.1/brax/envs/assets/inverted_pendulum.xml`

 * *Files 2% similar despite different names*

#### Comparing `brax-0.9.0/brax/envs/assets/inverted_pendulum.xml` & `brax-0.9.1/brax/envs/assets/inverted_pendulum.xml`

```diff
@@ -10,14 +10,15 @@
   <option gravity="0 0 -9.81" timestep="0.02"/>
   <custom>
     <!-- brax custom params -->
     <numeric data="10000" name="constraint_stiffness"/>
     <numeric data="10000" name="constraint_limit_stiffness"/>
     <numeric data="0" name="spring_mass_scale"/>
     <numeric data="1" name="spring_inertia_scale"/>
+    <numeric data="5" name="solver_maxls"/>
   </custom>
   <size nstack="3000"/>
   <worldbody>
     <!--geom name="ground" type="plane" pos="0 0 0" /-->
     <geom name="rail" pos="0 0 0" quat="0.707 0 0.707 0" size="0.02 1" type="capsule"/>
     <body name="cart" pos="0 0 0">
       <joint axis="1 0 0" limited="true" name="slider" pos="0 0 0" range="-1 1" type="slide"/>
```

### Comparing `brax-0.9.0/brax/envs/assets/pusher.xml` & `brax-0.9.1/brax/envs/assets/pusher.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/envs/assets/reacher.xml` & `brax-0.9.1/brax/envs/assets/reacher.xml`

 * *Files 4% similar despite different names*

#### Comparing `brax-0.9.0/brax/envs/assets/reacher.xml` & `brax-0.9.1/brax/envs/assets/reacher.xml`

```diff
@@ -13,14 +13,15 @@
     <numeric data="1000 1000 10" name="constraint_stiffness"/>
     <numeric data="1000" name="constraint_limit_stiffness"/>
     <numeric data="3 3 0.1" name="constraint_vel_damping"/>
     <numeric data="0.1" name="constraint_ang_damping"/>
     <numeric data="0.0" name="ang_damping"/>
     <numeric data="0" name="spring_mass_scale"/>
     <numeric data="1" name="spring_inertia_scale"/>
+    <numeric data="5" name="solver_maxls"/>
   </custom>
   <worldbody>
     <!-- Arena -->
     <geom conaffinity="0" contype="0" name="ground" pos="0 0 0" size="1 1 10" type="plane"/>
     <geom conaffinity="0" fromto="-.3 -.3 .01 .3 -.3 .01" name="sideS" size=".02" type="capsule"/>
     <geom conaffinity="0" fromto=" .3 -.3 .01 .3  .3 .01" name="sideE" size=".02" type="capsule"/>
     <geom conaffinity="0" fromto="-.3  .3 .01 .3  .3 .01" name="sideN" size=".02" type="capsule"/>
```

### Comparing `brax-0.9.0/brax/envs/env.py` & `brax-0.9.1/brax/envs/base.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/envs/env_test.py` & `brax-0.9.1/brax/envs/env_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/envs/fast.py` & `brax-0.9.1/brax/envs/fast.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,52 +8,53 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Gotta go fast!  This trivial Env is meant for unit testing."""
+# pylint:disable=g-multiple-import
+"""Gotta go fast!  This trivial Env is for unit testing."""
 
 from brax import base
-from brax.envs import env
-import jax.numpy as jnp
+from brax.envs.base import PipelineEnv, State
+from jax import numpy as jp
 
 
-class Fast(env.PipelineEnv):
+class Fast(PipelineEnv):
   """Trains an agent to go fast."""
 
   def __init__(self, **kwargs):
     self._dt = 0.02
     self._reset_count = 0
     self._step_count = 0
 
-  def reset(self, rng: jnp.ndarray) -> env.State:  # pytype: disable=signature-mismatch  # jax-ndarray
+  def reset(self, rng: jp.ndarray) -> State:
     self._reset_count += 1
     pipeline_state = base.State(
-        q=jnp.zeros(1),
-        qd=jnp.zeros(1),
-        x=base.Transform.create(pos=jnp.zeros(3)),
-        xd=base.Motion.create(vel=jnp.zeros(3)),
+        q=jp.zeros(1),
+        qd=jp.zeros(1),
+        x=base.Transform.create(pos=jp.zeros(3)),
+        xd=base.Motion.create(vel=jp.zeros(3)),
         contact=None
     )
-    obs = jnp.zeros(2)
-    reward, done = jnp.array(0.0), jnp.array(0.0)
-    return env.State(pipeline_state, obs, reward, done)
+    obs = jp.zeros(2)
+    reward, done = jp.array(0.0), jp.array(0.0)
+    return State(pipeline_state, obs, reward, done)
 
-  def step(self, state: env.State, action: jnp.ndarray) -> env.State:  # pytype: disable=signature-mismatch  # jax-ndarray
+  def step(self, state: State, action: jp.ndarray) -> State:
     self._step_count += 1
     vel = state.pipeline_state.xd.vel + (action > 0) * self._dt
     pos = state.pipeline_state.x.pos + vel * self._dt
 
     qp = state.pipeline_state.replace(
         x=state.pipeline_state.x.replace(pos=pos),
         xd=state.pipeline_state.xd.replace(vel=vel),
     )
-    obs = jnp.array([pos[0], vel[0]])
+    obs = jp.array([pos[0], vel[0]])
     reward = pos[0]
 
     return state.replace(pipeline_state=qp, obs=obs, reward=reward)
 
   @property
   def reset_count(self):
     return self._reset_count
```

### Comparing `brax-0.9.0/brax/envs/half_cheetah.py` & `brax-0.9.1/brax/envs/half_cheetah.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# pylint:disable=g-multiple-import
 """Trains a halfcheetah to run in the +x direction."""
 
 from brax import base
-from brax.envs import env
+from brax.envs.base import PipelineEnv, State
 from brax.io import mjcf
 from etils import epath
 import jax
 from jax import numpy as jp
 
 
-class Halfcheetah(env.PipelineEnv):
+class Halfcheetah(PipelineEnv):
 
 
 
   # pyformat: disable
   """
   ### Description
 
@@ -113,42 +114,14 @@
   [-0.1, 0.1] is added to the positional values while a standard normal noise
   with a mean of 0 and standard deviation of 0.1 is added to the initial
   velocity values of all zeros.
 
   ### Episode Termination
 
   The episode terminates when the episode length is greater than 1000.
-
-  ### Arguments
-
-  No additional arguments are currently supported (in v2 and lower), but
-  modifications can be made to the XML file in the assets folder
-  (or by changing the path to a modified XML file in another folder).
-
-  ```
-  env = gym.make('HalfCheetah-v2')
-  ```
-
-  v3, v4, and v5 take gym.make kwargs such as ctrl_cost_weight,
-  reset_noise_scale etc.
-
-  ```
-  env = gym.make('HalfCheetah-v5', ctrl_cost_weight=0.1, ....)
-
-  ### Version History
-
-  * v5: ported to Brax.
-  * v4: all mujoco environments now use the mujoco bindings in mujoco>=2.1.3
-  * v3: support for gym.make kwargs such as xml_file, ctrl_cost_weight,
-    reset_noise_scale etc. rgb rendering comes from tracking camera (so agent
-    does not run away from screen)
-  * v2: All continuous control environments now use mujoco_py >= 1.50
-  * v1: max_time_steps raised to 1000 for robot based tasks. Added
-    reward_threshold to environments.
-  * v0: Initial versions release (1.0.0)
   """
   # pyformat: enable
 
 
   def __init__(
       self,
       forward_reward_weight=1.0,
@@ -176,15 +149,15 @@
     self._forward_reward_weight = forward_reward_weight
     self._ctrl_cost_weight = ctrl_cost_weight
     self._reset_noise_scale = reset_noise_scale
     self._exclude_current_positions_from_observation = (
         exclude_current_positions_from_observation
     )
 
-  def reset(self, rng: jp.ndarray) -> env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     """Resets the environment to an initial state."""
     rng, rng1, rng2 = jax.random.split(rng, 3)
 
     low, hi = -self._reset_noise_scale, self._reset_noise_scale
     qpos = self.sys.init_q + jax.random.uniform(
         rng1, (self.sys.q_size(),), minval=low, maxval=hi
     )
@@ -196,17 +169,17 @@
     reward, done, zero = jp.zeros(3)
     metrics = {
         'x_position': zero,
         'x_velocity': zero,
         'reward_ctrl': zero,
         'reward_run': zero,
     }
-    return env.State(pipeline_state, obs, reward, done, metrics)
+    return State(pipeline_state, obs, reward, done, metrics)
 
-  def step(self, state: env.State, action: jp.ndarray) -> env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     """Runs one timestep of the environment's dynamics."""
     pipeline_state0 = state.pipeline_state
     pipeline_state = self.pipeline_step(pipeline_state0, action)
 
     x_velocity = (
         pipeline_state.x.pos[0, 0] - pipeline_state0.x.pos[0, 0]
     ) / self.dt
```

### Comparing `brax-0.9.0/brax/envs/hopper.py` & `brax-0.9.1/brax/envs/hopper.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# pylint:disable=g-multiple-import
 """Trains a hopper to run in the +x direction."""
 
 from typing import Tuple
 
 from brax import base
-from brax.envs import env
+from brax.envs.base import PipelineEnv, State
 from brax.io import mjcf
 from etils import epath
 import jax
 from jax import numpy as jp
 
 
-class Hopper(env.PipelineEnv):
+class Hopper(PipelineEnv):
 
 
 
   # pyformat: disable
   """
   ### Description
 
@@ -190,15 +191,15 @@
     self._healthy_z_range = healthy_z_range
     self._healthy_angle_range = healthy_angle_range
     self._reset_noise_scale = reset_noise_scale
     self._exclude_current_positions_from_observation = (
         exclude_current_positions_from_observation
     )
 
-  def reset(self, rng: jp.ndarray) -> env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     """Resets the environment to an initial state."""
     rng, rng1, rng2 = jax.random.split(rng, 3)
 
     low, hi = -self._reset_noise_scale, self._reset_noise_scale
     qpos = self.sys.init_q + jax.random.uniform(
         rng1, (self.sys.q_size(),), minval=low, maxval=hi
     )
@@ -213,17 +214,17 @@
     metrics = {
         'reward_forward': zero,
         'reward_ctrl': zero,
         'reward_healthy': zero,
         'x_position': zero,
         'x_velocity': zero,
     }
-    return env.State(pipeline_state, obs, reward, done, metrics)
+    return State(pipeline_state, obs, reward, done, metrics)
 
-  def step(self, state: env.State, action: jp.ndarray) -> env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     """Runs one timestep of the environment's dynamics."""
     pipeline_state0 = state.pipeline_state
     pipeline_state = self.pipeline_step(pipeline_state0, action)
 
     x_velocity = (
         pipeline_state.x.pos[0, 0] - pipeline_state0.x.pos[0, 0]
     ) / self.dt
```

### Comparing `brax-0.9.0/brax/envs/humanoid.py` & `brax-0.9.1/brax/envs/humanoid.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# pylint:disable=g-multiple-import
 """Trains a humanoid to run in the +x direction."""
 
 from brax import actuator
 from brax import base
-from brax.base import Transform
-from brax.envs import env
+from brax.envs.base import PipelineEnv, State
 from brax.io import mjcf
 from etils import epath
 import jax
 from jax import numpy as jp
 
 
-class Humanoid(env.PipelineEnv):
+class Humanoid(PipelineEnv):
 
 
 
   # pyformat: disable
   """
   ### Description
 
@@ -168,42 +168,14 @@
 
   The episode terminates when any of the following happens:
 
   1. The episode duration reaches a 1000 timesteps
   2. The z-coordinate of the torso (index 0 in state space OR index 2 in the
   table) is **not** in the range `[0.8, 2.1]` (the humanoid has fallen or is
   about to fall beyond recovery).
-
-  ### Arguments
-
-  No additional arguments are currently supported (in v2 and lower), but
-  modifications can be made to the XML file in the assets folder (or by changing
-  the path to a modified XML file in another folder).
-
-  ```
-  env = gym.make('Humanoid-v2')
-  ```
-
-  v3, v4, and v5 take gym.make kwargs such as ctrl_cost_weight, reset_noise_scale etc.
-
-  ```
-  env = gym.make('Humanoid-v5', ctrl_cost_weight=0.1, ....)
-  ```
-
-  ### Version History
-
-  * v5: ported to Brax.
-  * v4: all mujoco environments now use the mujoco bindings in mujoco>=2.1.3
-  * v3: support for gym.make kwargs such as xml_file, ctrl_cost_weight,
-    reset_noise_scale etc. rgb rendering comes from tracking camera (so agent
-    does not run away from screen)
-  * v2: All continuous control environments now use mujoco_py >= 1.50
-  * v1: max_time_steps raised to 1000 for robot based tasks. Added
-    reward_threshold to environments.
-  * v0: Initial versions release (1.0.0)
   """
   # pyformat: enable
 
 
   def __init__(
       self,
       forward_reward_weight=1.25,
@@ -239,15 +211,15 @@
     self._terminate_when_unhealthy = terminate_when_unhealthy
     self._healthy_z_range = healthy_z_range
     self._reset_noise_scale = reset_noise_scale
     self._exclude_current_positions_from_observation = (
         exclude_current_positions_from_observation
     )
 
-  def reset(self, rng: jp.ndarray) -> env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     """Resets the environment to an initial state."""
     rng, rng1, rng2 = jax.random.split(rng, 3)
 
     low, hi = -self._reset_noise_scale, self._reset_noise_scale
     qpos = self.sys.init_q + jax.random.uniform(
         rng1, (self.sys.q_size(),), minval=low, maxval=hi
     )
@@ -266,17 +238,17 @@
         'reward_alive': zero,
         'x_position': zero,
         'y_position': zero,
         'distance_from_origin': zero,
         'x_velocity': zero,
         'y_velocity': zero,
     }
-    return env.State(pipeline_state, obs, reward, done, metrics)
+    return State(pipeline_state, obs, reward, done, metrics)
 
-  def step(self, state: env.State, action: jp.ndarray) -> env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     """Runs one timestep of the environment's dynamics."""
     pipeline_state0 = state.pipeline_state
     pipeline_state = self.pipeline_step(pipeline_state0, action)
 
     com_before, *_ = self._com(pipeline_state0)
     com_after, *_ = self._com(pipeline_state)
     velocity = (com_after - com_before) / self.dt
@@ -326,23 +298,24 @@
     com, inertia, mass_sum, x_i = self._com(pipeline_state)
     cinr = x_i.replace(pos=x_i.pos - com).vmap().do(inertia)
     com_inertia = jp.hstack(
         [cinr.i.reshape((cinr.i.shape[0], -1)), inertia.mass[:, None]]
     )
 
     xd_i = (
-        Transform.create(pos=x_i.pos - pipeline_state.x.pos)
+        base.Transform.create(pos=x_i.pos - pipeline_state.x.pos)
         .vmap()
         .do(pipeline_state.xd)
     )
     com_vel = inertia.mass[:, None] * xd_i.vel / mass_sum
     com_ang = xd_i.ang
     com_velocity = jp.hstack([com_vel, com_ang])
 
-    qfrc_actuator = actuator.to_tau(self.sys, action, pipeline_state.q)
+    qfrc_actuator = actuator.to_tau(
+        self.sys, action, pipeline_state.q, pipeline_state.qd)
 
     # external_contact_forces are excluded
     return jp.concatenate([
         position,
         velocity,
         com_inertia.ravel(),
         com_velocity.ravel(),
```

### Comparing `brax-0.9.0/brax/envs/humanoidstandup.py` & `brax-0.9.1/brax/envs/humanoidstandup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# pylint:disable=g-multiple-import
 """Trains a humanoid to stand up."""
 
 from brax import actuator
 from brax import base
-from brax.base import Transform
-from brax.envs import env
+from brax.envs.base import PipelineEnv, State
 from brax.io import mjcf
 from etils import epath
 import jax
 from jax import numpy as jp
 
 
-class HumanoidStandup(env.PipelineEnv):
+class HumanoidStandup(PipelineEnv):
 
 
 
   # pyformat: disable
   """
   ### Description
 
@@ -169,51 +169,14 @@
   to make it face forward as well.
 
   ### Episode Termination
 
   The episode terminates when any of the following happens:
 
   1. The episode duration reaches a 1000 timesteps
-
-  ### Arguments
-
-  No additional arguments are currently supported (in v2 and lower), but
-  modifications can be made to the XML file in the assets folder (or by changing
-  the path to a modified XML file in another folder).
-
-  ```
-  env = gym.make('HumanoidStandup-v2')
-  ```
-
-  There is no v3 for HumanoidStandup, unlike the robot environments where a v3
-  take gym.make kwargs such as xml_file, ctrl_cost_weight, reset_noise_scale etc.
-
-  There is a v4 version that uses the mujoco-bindings
-
-  ```
-  env = gym.make('HumanoidStandup-v4')
-  ```
-
-  And a v5 version that uses Brax:
-
-  ```
-  env = gym.make('HumanoidStandup-v5')
-  ```
-
-  ### Version History
-
-  * v5: ported to Brax.
-  * v4: all mujoco environments now use the mujoco bindings in mujoco>=2.1.3
-  * v3: support for gym.make kwargs such as xml_file, ctrl_cost_weight,
-        reset_noise_scale etc. rgb rendering comes from tracking camera (so
-        agent does not run away from screen)
-  * v2: All continuous control environments now use mujoco_py >= 1.50
-  * v1: max_time_steps raised to 1000 for robot based tasks. Added
-        reward_threshold to environments.
-  * v0: Initial versions release (1.0.0)
   """
   # pyformat: enable
 
 
   def __init__(self, backend='generalized', **kwargs):
     path = epath.resource_path('brax') / 'envs/assets/humanoidstandup.xml'
     sys = mjcf.load(path)
@@ -229,15 +192,15 @@
                              350.0, 350.0, 350.0, 350.0, 350.0, 100.0, 100.0,
                              100.0, 100.0, 100.0, 100.0])))  # pyformat: disable
 
     kwargs['n_frames'] = kwargs.get('n_frames', n_frames)
 
     super().__init__(sys=sys, backend=backend, **kwargs)
 
-  def reset(self, rng: jp.ndarray) -> env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     """Resets the environment to an initial state."""
     rng, rng1, rng2 = jax.random.split(rng, 3)
 
     low, hi = -0.01, 0.01
     qpos = self.sys.init_q + jax.random.uniform(
         rng1, (self.sys.q_size(),), minval=-0.01, maxval=0.01
     )
@@ -248,17 +211,17 @@
     pipeline_state = self.pipeline_init(qpos, qvel)
     obs = self._get_obs(pipeline_state, jp.zeros(self.sys.act_size()))
     reward, done, zero = jp.zeros(3)
     metrics = {
         'reward_linup': zero,
         'reward_quadctrl': zero,
     }
-    return env.State(pipeline_state, obs, reward, done, metrics)
+    return State(pipeline_state, obs, reward, done, metrics)
 
-  def step(self, state: env.State, action: jp.ndarray) -> env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     """Runs one timestep of the environment's dynamics."""
     pipeline_state = self.pipeline_step(state.pipeline_state, action)
 
     pos_after = pipeline_state.x.pos[0, 2]  # z coordinate of torso
     uph_cost = (pos_after - 0) / self.dt
     quad_ctrl_cost = 0.01 * jp.sum(jp.square(action))
     # quad_impact_cost is not computed here
@@ -279,23 +242,24 @@
     com, inertia, mass_sum, x_i = self._com(pipeline_state)
     cinr = x_i.replace(pos=x_i.pos - com).vmap().do(inertia)
     com_inertia = jp.hstack(
         [cinr.i.reshape((cinr.i.shape[0], -1)), inertia.mass[:, None]]
     )
 
     xd_i = (
-        Transform.create(pos=x_i.pos - pipeline_state.x.pos)
+        base.Transform.create(pos=x_i.pos - pipeline_state.x.pos)
         .vmap()
         .do(pipeline_state.xd)
     )
     com_vel = inertia.mass[:, None] * xd_i.vel / mass_sum
     com_ang = xd_i.ang
     com_velocity = jp.hstack([com_vel, com_ang])
 
-    qfrc_actuator = actuator.to_tau(self.sys, action, pipeline_state.q)
+    qfrc_actuator = actuator.to_tau(
+        self.sys, action, pipeline_state.q, pipeline_state.qd)
 
     # external_contact_forces are excluded
     return jp.concatenate([
         position,
         velocity,
         com_inertia.ravel(),
         com_velocity.ravel(),
```

### Comparing `brax-0.9.0/brax/envs/inverted_double_pendulum.py` & `brax-0.9.1/brax/envs/inverted_double_pendulum.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# pylint:disable=g-multiple-import
 """An inverted pendulum environment."""
 
 from brax import base
-from brax.base import Transform
-from brax.envs import env
+from brax.envs.base import PipelineEnv, State
 from brax.io import mjcf
 from etils import epath
 import jax
 from jax import numpy as jp
 
 
-class InvertedDoublePendulum(env.PipelineEnv):
+class InvertedDoublePendulum(PipelineEnv):
 
 
 
   # pyformat: disable
   """### Description
 
   This environment originates from control theory and builds on the cartpole
@@ -108,52 +108,14 @@
   ### Episode Termination
 
   The episode terminates when any of the following happens:
 
   1. The episode duration reaches 1000 timesteps.
   2. The absolute value of the vertical angle between the pole and the cart is
   greater than 0.2 radians.
-
-  ### Arguments
-
-  No additional arguments are currently supported (in v2 and lower), but
-  modifications can be made to the XML file in the assets folder (or by changing
-  the path to a modified XML file in another folder).
-
-  ```
-  env = gym.make('InvertedDoublePendulum-v2')
-  ```
-
-  There is no v3 for InvertedDoublePendulum, unlike the robot environments where
-  a v3 and beyond take gym.make kwargs such as ctrl_cost_weight,
-  reset_noise_scale etc.
-
-  There is a v4 version that uses the mujoco-bindings
-
-  ```
-  env = gym.make('InvertedDoublePendulum-v4')
-  ```
-
-  And a v5 version that uses Brax:
-
-  ```
-  env = gym.make('InvertedDoublePendulum-v5')
-  ```
-
-  ### Version History
-
-  * v5: ported to Brax.
-  * v4: all mujoco environments now use the mujoco bindings in mujoco>=2.1.3
-  * v3: support for gym.make kwargs such as ctrl_cost_weight, reset_noise_scale
-    etc. rgb rendering comes from tracking camera (so agent does not run away
-    from screen)
-  * v2: All continuous control environments now use mujoco_py >= 1.50
-  * v1: max_time_steps raised to 1000 for robot based tasks (including inverted
-    pendulum)
-  * v0: Initial versions release (1.0.0)
   """
   # pyformat: enable
 
 
   def __init__(self, backend='generalized', **kwargs):
     path = (
         epath.resource_path('brax')
@@ -167,35 +129,35 @@
       sys = sys.replace(dt=0.005)
       n_frames = 4
 
     kwargs['n_frames'] = kwargs.get('n_frames', n_frames)
 
     super().__init__(sys=sys, backend=backend, **kwargs)
 
-  def reset(self, rng: jp.ndarray) -> env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     """Resets the environment to an initial state."""
     rng, rng1, rng2 = jax.random.split(rng, 3)
 
     q = self.sys.init_q + jax.random.uniform(
         rng1, (self.sys.q_size(),), minval=-0.01, maxval=0.01
     )
     qd = jax.random.normal(rng2, (self.sys.qd_size(),)) * 0.01
     pipeline_state = self.pipeline_init(q, qd)
 
     obs = self._get_obs(pipeline_state)
     reward, done = jp.zeros(2)
     metrics = {}
 
-    return env.State(pipeline_state, obs, reward, done, metrics)
+    return State(pipeline_state, obs, reward, done, metrics)
 
-  def step(self, state: env.State, action: jp.ndarray) -> env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     """Run one timestep of the environment's dynamics."""
     pipeline_state = self.pipeline_step(state.pipeline_state, action)
 
-    tip = Transform.create(pos=jp.array([0.0, 0.0, 0.6])).do(
+    tip = base.Transform.create(pos=jp.array([0.0, 0.0, 0.6])).do(
         pipeline_state.x.take(2)
     )
     x, _, y = tip.pos
     dist_penalty = 0.01 * x**2 + (y - 2) ** 2
     v1, v2 = pipeline_state.qd[1:]
     vel_penalty = 1e-3 * v1**2 + 5e-3 * v2**2
     alive_bonus = 10
```

### Comparing `brax-0.9.0/brax/envs/inverted_pendulum.py` & `brax-0.9.1/brax/envs/inverted_pendulum.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# pylint:disable=g-multiple-import
 """An inverted pendulum environment."""
 
 from brax import base
-from brax.envs import env
+from brax.envs.base import PipelineEnv, State
 from brax.io import mjcf
 from etils import epath
 import jax
 from jax import numpy as jp
 
 
-class InvertedPendulum(env.PipelineEnv):
+class InvertedPendulum(PipelineEnv):
 
 
 
   # pyformat: disable
   """### Description
 
   This environment is the cartpole environment based on the work done by Barto,
@@ -87,52 +88,14 @@
   ### Episode Termination
 
   The episode terminates when any of the following happens:
 
   1. The episode duration reaches 1000 timesteps.
   2. The absolute value of the vertical angle between the pole and the cart is
   greater than 0.2 radians.
-
-  ### Arguments
-
-  No additional arguments are currently supported (in v2 and lower), but
-  modifications can be made to the XML file in the assets folder (or by changing
-  the path to a modified XML file in another folder).
-
-  ```
-  env = gym.make('InvertedPendulum-v2')
-  ```
-
-  There is no v3 for InvertedPendulum, unlike the robot environments where a v3
-  and beyond take gym.make kwargs such as ctrl_cost_weight, reset_noise_scale
-  etc.
-
-  There is a v4 version that uses the mujoco-bindings
-
-  ```
-  env = gym.make('InvertedPendulum-v4')
-  ```
-
-  And a v5 version that uses Brax:
-
-  ```
-  env = gym.make('InvertedPendulum-v5')
-  ```
-
-  ### Version History
-
-  * v5: ported to Brax.
-  * v4: all mujoco environments now use the mujoco bindings in mujoco>=2.1.3
-  * v3: support for gym.make kwargs such as ctrl_cost_weight, reset_noise_scale
-    etc. rgb rendering comes from tracking camera (so agent does not run away
-    from screen)
-  * v2: All continuous control environments now use mujoco_py >= 1.50
-  * v1: max_time_steps raised to 1000 for robot based tasks (including inverted
-    pendulum)
-  * v0: Initial versions release (1.0.0)
   """
   # pyformat: enable
 
 
   def __init__(self, backend='generalized', **kwargs):
     path = epath.resource_path('brax') / 'envs/assets/inverted_pendulum.xml'
     sys = mjcf.load(path)
@@ -143,32 +106,32 @@
       sys = sys.replace(dt=0.005)
       n_frames = 4
 
     kwargs['n_frames'] = kwargs.get('n_frames', n_frames)
 
     super().__init__(sys=sys, backend=backend, **kwargs)
 
-  def reset(self, rng: jp.ndarray) -> env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     """Resets the environment to an initial state."""
     rng, rng1, rng2 = jax.random.split(rng, 3)
 
     q = self.sys.init_q + jax.random.uniform(
         rng1, (self.sys.q_size(),), minval=-0.01, maxval=0.01
     )
     qd = jax.random.uniform(
         rng2, (self.sys.qd_size(),), minval=-0.01, maxval=0.01
     )
     pipeline_state = self.pipeline_init(q, qd)
     obs = self._get_obs(pipeline_state)
     reward, done = jp.zeros(2)
     metrics = {}
 
-    return env.State(pipeline_state, obs, reward, done, metrics)
+    return State(pipeline_state, obs, reward, done, metrics)
 
-  def step(self, state: env.State, action: jp.ndarray) -> env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     """Run one timestep of the environment's dynamics."""
     pipeline_state = self.pipeline_step(state.pipeline_state, action)
     obs = self._get_obs(pipeline_state)
     reward = 1.0
     done = jp.where(jp.abs(obs[1]) > 0.2, 1.0, 0.0)
     return state.replace(
         pipeline_state=pipeline_state, obs=obs, reward=reward, done=done
```

### Comparing `brax-0.9.0/brax/envs/pusher.py` & `brax-0.9.1/brax/envs/pusher.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# pylint:disable=g-multiple-import
 """Trains a robot arm to push a ball to a target."""
 
 from brax import base
 from brax import math
-from brax.base import Transform
-from brax.envs import env
+from brax.envs.base import PipelineEnv, State
 from brax.io import mjcf
 from etils import epath
 import jax
 from jax import numpy as jp
 
 
-class Pusher(env.PipelineEnv):
+class Pusher(PipelineEnv):
 
 
 
   # pyformat: disable
   """
   ### Description
 
@@ -132,48 +132,14 @@
   The default *dt = 0.05*.
 
   ### Episode Termination
 
   The episode terminates when any of the following happens:
 
   1. The episode duration reaches a 1000 timesteps.
-
-  ### Arguments
-
-  No additional arguments are currently supported (in v2 and lower), but
-  modifications can be made to the XML file in the assets folder (or by changing
-  the path to a modified XML file in another folder)..
-
-  ```
-  env = gym.make('Pusher-v2')
-  ```
-
-  There is no v3 for Pusher, unlike the robot environments where a v3 and
-  beyond take gym.make kwargs such as xml_file, ctrl_cost_weight, reset_noise_scale etc.
-
-  There is a v4 version that uses the mujoco-bindings
-  ```
-  env = gym.make('Pusher-v4')
-  ```
-
-  And a v5 version that uses Brax:
-
-  ```
-  env = gym.make('Pusher-v5')
-  ```
-
-  ### Version History
-
-  * v5: ported to Brax.
-  * v4: all mujoco environments now use the mujoco bindings in mujoco>=2.1.3
-  * v2: All continuous control environments now use mujoco_py >= 1.50
-  * v1: max_time_steps raised to 1000 for robot based tasks (not including
-    reacher, which has a max_time_steps of 50). Added reward_threshold to
-    environments.
-  * v0: Initial versions release (1.0.0)
   """
   # pyformat: enable
 
 
   def __init__(self, backend='generalized', **kwargs):
     path = epath.resource_path('brax') / 'envs/assets/pusher.xml'
     sys = mjcf.load(path)
@@ -193,15 +159,15 @@
 
     # The tips_arm body gets fused with r_wrist_roll_link, so we use the parent
     # r_wrist_flex_link for tips_arm_idx.
     self._tips_arm_idx = self.sys.link_names.index('r_wrist_flex_link')
     self._object_idx = self.sys.link_names.index('object')
     self._goal_idx = self.sys.link_names.index('goal')
 
-  def reset(self, rng: jp.ndarray) -> env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     qpos = self.sys.init_q
 
     rng, rng1, rng2 = jax.random.split(rng, 3)
 
     # randomly orient the object
     cylinder_pos = jp.concatenate([
         jax.random.uniform(rng, (1,), minval=-0.3, maxval=-1e-6),
@@ -220,19 +186,19 @@
     qvel = qvel.at[-4:].set(0.0)
 
     pipeline_state = self.pipeline_init(qpos, qvel)
 
     obs = self._get_obs(pipeline_state)
     reward, done, zero = jp.zeros(3)
     metrics = {'reward_dist': zero, 'reward_ctrl': zero, 'reward_near': zero}
-    return env.State(pipeline_state, obs, reward, done, metrics)
+    return State(pipeline_state, obs, reward, done, metrics)
 
-  def step(self, state: env.State, action: jp.ndarray) -> env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     x_i = state.pipeline_state.x.vmap().do(
-        Transform.create(pos=self.sys.link.inertia.transform.pos)
+        base.Transform.create(pos=self.sys.link.inertia.transform.pos)
     )
     vec_1 = x_i.pos[self._object_idx] - x_i.pos[self._tips_arm_idx]
     vec_2 = x_i.pos[self._object_idx] - x_i.pos[self._goal_idx]
 
     reward_near = -math.safe_norm(vec_1)
     reward_dist = -math.safe_norm(vec_2)
     reward_ctrl = -jp.square(action).sum()
@@ -247,15 +213,15 @@
         reward_ctrl=reward_ctrl,
     )
     return state.replace(pipeline_state=pipeline_state, obs=obs, reward=reward)
 
   def _get_obs(self, pipeline_state: base.State) -> jp.ndarray:
     """Observes pusher body position and velocities."""
     x_i = pipeline_state.x.vmap().do(
-        Transform.create(pos=self.sys.link.inertia.transform.pos)
+        base.Transform.create(pos=self.sys.link.inertia.transform.pos)
     )
     return jp.concatenate([
         pipeline_state.q[:7],
         pipeline_state.qd[:7],
         x_i.pos[self._tips_arm_idx],
         x_i.pos[self._object_idx],
         x_i.pos[self._goal_idx],
```

### Comparing `brax-0.9.0/brax/envs/reacher.py` & `brax-0.9.1/brax/envs/reacher.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# pylint:disable=g-multiple-import
 """Trains a reacher to reach a target.
 
 Based on the OpenAI Gym MuJoCo Reacher environment.
 """
 
 from typing import Tuple
 
 from brax import base
 from brax import math
-from brax.base import Transform
-from brax.envs import env
+from brax.envs.base import PipelineEnv, State
 from brax.io import mjcf
 from etils import epath
 import jax
 from jax import numpy as jp
 
 
-class Reacher(env.PipelineEnv):
+class Reacher(PipelineEnv):
 
 
 
   # pyformat: disable
   """
   ### Description
 
@@ -167,15 +167,15 @@
       )
       n_frames = 4
 
     kwargs['n_frames'] = kwargs.get('n_frames', n_frames)
 
     super().__init__(sys=sys, backend=backend, **kwargs)
 
-  def reset(self, rng: jp.ndarray) -> env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     rng, rng1, rng2 = jax.random.split(rng, 3)
 
     q = self.sys.init_q + jax.random.uniform(
         rng1, (self.sys.q_size(),), minval=-0.1, maxval=0.1
     )
     qd = jax.random.uniform(
         rng2, (self.sys.qd_size(),), minval=-0.005, maxval=0.005
@@ -190,17 +190,17 @@
 
     obs = self._get_obs(pipeline_state)
     reward, done, zero = jp.zeros(3)
     metrics = {
         'reward_dist': zero,
         'reward_ctrl': zero,
     }
-    return env.State(pipeline_state, obs, reward, done, metrics)
+    return State(pipeline_state, obs, reward, done, metrics)
 
-  def step(self, state: env.State, action: jp.ndarray) -> env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     pipeline_state = self.pipeline_step(state.pipeline_state, action)
     obs = self._get_obs(pipeline_state)
 
     # vector from tip to target is last 3 entries of obs vector
     reward_dist = -math.safe_norm(obs[-3:])
     reward_ctrl = -jp.square(action).sum()
     reward = reward_dist + reward_ctrl
@@ -214,21 +214,21 @@
 
   def _get_obs(self, pipeline_state: base.State) -> jp.ndarray:
     """Returns egocentric observation of target and arm body."""
     theta = pipeline_state.q[:2]
     target_pos = pipeline_state.x.pos[2]
     tip_pos = (
         pipeline_state.x.take(1)
-        .do(Transform.create(pos=jp.array([0.11, 0, 0])))
+        .do(base.Transform.create(pos=jp.array([0.11, 0, 0])))
         .pos
     )
     # tip_vel, instead of pipeline_state.qd[:2], leads to more sensible policies
     # for a randomly initialized policy network
     tip_vel = (
-        Transform.create(pos=jp.array([0.11, 0, 0]))
+        base.Transform.create(pos=jp.array([0.11, 0, 0]))
         .do(pipeline_state.xd.take(1))
         .vel
     )
     tip_to_target = tip_pos - target_pos
 
     return jp.concatenate([
         jp.cos(theta),
```

### Comparing `brax-0.9.0/brax/envs/walker2d.py` & `brax-0.9.1/brax/envs/walker2d.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# pylint:disable=g-multiple-import
 """Trains a 2D walker to run in the +x direction."""
 
 from typing import Tuple
 
 from brax import base
-from brax.envs import env
+from brax.envs.base import PipelineEnv, State
 from brax.io import mjcf
 from etils import epath
 import jax
 from jax import numpy as jp
 
 
-class Walker2d(env.PipelineEnv):
+class Walker2d(PipelineEnv):
 
 
 
   # pyformat: disable
   """
   ### Description
 
@@ -117,43 +118,14 @@
   ### Episode Termination
 
   The episode terminates when any of the following happens:
 
   1. The episode duration reaches a 1000 timesteps
   2. The height of the walker is ***not*** in the range `[0.7, 2]`
   3. The absolute value of the angle is ***not*** in the range `[-1, 1]`
-
-  ### Arguments
-
-  No additional arguments are currently supported (in v2 and lower), but
-  modifications can be made to the XML file in the assets folder (or by changing
-  the path to a modified XML file in another folder)..
-
-  ```
-  env = gym.make('Walker2d-v2')
-  ```
-
-  v3, v4 and v5 take gym.make kwargs such as ctrl_cost_weight, reset_noise_scale
-  etc.
-
-  ```
-  env = gym.make('Walker2d-v5', ctrl_cost_weight=0.1, ....)
-  ```
-
-  ### Version History
-
-  * v5: ported to Brax.
-  * v4: all mujoco environments now use the mujoco bindings in mujoco>=2.1.3
-  * v3: support for gym.make kwargs such as xml_file, ctrl_cost_weight,
-    reset_noise_scale etc. rgb rendering comes from tracking camera (so agent
-    does not run away from screen)
-  * v2: All continuous control environments now use mujoco_py >= 1.50
-  * v1: max_time_steps raised to 1000 for robot based tasks. Added
-    reward_threshold to environments.
-  * v0: Initial versions release (1.0.0)
   """
   # pyformat: enable
 
 
   def __init__(
       self,
       forward_reward_weight: float = 1.0,
@@ -199,15 +171,15 @@
     self._healthy_z_range = healthy_z_range
     self._healthy_angle_range = healthy_angle_range
     self._reset_noise_scale = reset_noise_scale
     self._exclude_current_positions_from_observation = (
         exclude_current_positions_from_observation
     )
 
-  def reset(self, rng: jp.ndarray) -> env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     """Resets the environment to an initial state."""
     rng, rng1, rng2 = jax.random.split(rng, 3)
 
     low, hi = -self._reset_noise_scale, self._reset_noise_scale
     qpos = self.sys.init_q + jax.random.uniform(
         rng1, (self.sys.q_size(),), minval=low, maxval=hi
     )
@@ -222,17 +194,17 @@
     metrics = {
         'reward_forward': zero,
         'reward_ctrl': zero,
         'reward_healthy': zero,
         'x_position': zero,
         'x_velocity': zero,
     }
-    return env.State(pipeline_state, obs, reward, done, metrics)
+    return State(pipeline_state, obs, reward, done, metrics)
 
-  def step(self, state: env.State, action: jp.ndarray) -> env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     """Runs one timestep of the environment's dynamics."""
     pipeline_state0 = state.pipeline_state
     pipeline_state = self.pipeline_step(pipeline_state0, action)
 
     x_velocity = (
         pipeline_state.x.pos[0, 0] - pipeline_state0.x.pos[0, 0]
     ) / self.dt
```

### Comparing `brax-0.9.0/brax/envs/wrapper.py` & `brax-0.9.1/brax/envs/wrappers/training.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Wrappers for Brax to support different upstream use cases."""
+# pylint:disable=g-multiple-import
+"""Wrappers to support Brax training."""
 
 from typing import Dict, Optional
 
-from brax.envs import env as brax_env
+from brax.envs.base import Env, State, Wrapper
 from flax import struct
 import jax
 from jax import numpy as jp
 
 
-def wrap_for_training(
-    env: brax_env.Env, episode_length: int = 1000, action_repeat: int = 1
-) -> brax_env.Wrapper:
+def wrap(
+    env: Env, episode_length: int = 1000, action_repeat: int = 1
+) -> Wrapper:
   """Common wrapper pattern for all training agents.
 
   Args:
     env: environment to be wrapped
     episode_length: length of episode
     action_repeat: how many repeated actions to take per step
 
@@ -39,47 +40,45 @@
   """
   env = EpisodeWrapper(env, episode_length, action_repeat)
   env = VmapWrapper(env)
   env = AutoResetWrapper(env)
   return env
 
 
-class VmapWrapper(brax_env.Wrapper):
+class VmapWrapper(Wrapper):
   """Vectorizes Brax env."""
 
-  def __init__(self, env: brax_env.Env, batch_size: Optional[int] = None):
+  def __init__(self, env: Env, batch_size: Optional[int] = None):
     super().__init__(env)
     self.batch_size = batch_size
 
-  def reset(self, rng: jp.ndarray) -> brax_env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     if self.batch_size is not None:
       rng = jax.random.split(rng, self.batch_size)
     return jax.vmap(self.env.reset)(rng)
 
-  def step(self, state: brax_env.State, action: jp.ndarray) -> brax_env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     return jax.vmap(self.env.step)(state, action)
 
 
-class EpisodeWrapper(brax_env.Wrapper):
+class EpisodeWrapper(Wrapper):
   """Maintains episode step count and sets done at episode end."""
 
-  def __init__(
-      self, env: brax_env.Env, episode_length: int, action_repeat: int
-  ):
+  def __init__(self, env: Env, episode_length: int, action_repeat: int):
     super().__init__(env)
     self.episode_length = episode_length
     self.action_repeat = action_repeat
 
-  def reset(self, rng: jp.ndarray) -> brax_env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     state = self.env.reset(rng)
     state.info['steps'] = jp.zeros(rng.shape[:-1])
     state.info['truncation'] = jp.zeros(rng.shape[:-1])
     return state
 
-  def step(self, state: brax_env.State, action: jp.ndarray) -> brax_env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     def f(state, _):
       nstate = self.env.step(state, action)
       return nstate, nstate.reward
 
     state, rewards = jax.lax.scan(f, state, (), self.action_repeat)
     state = state.replace(reward=jp.sum(rewards, axis=0))
     steps = state.info['steps'] + self.action_repeat
@@ -90,24 +89,24 @@
     state.info['truncation'] = jp.where(
         steps >= episode_length, 1 - state.done, zero
     )
     state.info['steps'] = steps
     return state.replace(done=done)
 
 
-class AutoResetWrapper(brax_env.Wrapper):
+class AutoResetWrapper(Wrapper):
   """Automatically resets Brax envs that are done."""
 
-  def reset(self, rng: jp.ndarray) -> brax_env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     state = self.env.reset(rng)
     state.info['first_pipeline_state'] = state.pipeline_state
     state.info['first_obs'] = state.obs
     return state
 
-  def step(self, state: brax_env.State, action: jp.ndarray) -> brax_env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     if 'steps' in state.info:
       steps = state.info['steps']
       steps = jp.where(state.done, jp.zeros_like(steps), steps)
       state.info.update(steps=steps)
     state = state.replace(done=jp.zeros_like(state.done))
     state = self.env.step(state, action)
 
@@ -136,31 +135,31 @@
   """
 
   episode_metrics: Dict[str, jp.ndarray]
   active_episodes: jp.ndarray
   episode_steps: jp.ndarray
 
 
-class EvalWrapper(brax_env.Wrapper):
+class EvalWrapper(Wrapper):
   """Brax env with eval metrics."""
 
-  def reset(self, rng: jp.ndarray) -> brax_env.State:
+  def reset(self, rng: jp.ndarray) -> State:
     reset_state = self.env.reset(rng)
     reset_state.metrics['reward'] = reset_state.reward
     eval_metrics = EvalMetrics(
         episode_metrics=jax.tree_util.tree_map(
             jp.zeros_like, reset_state.metrics
         ),
         active_episodes=jp.ones_like(reset_state.reward),
         episode_steps=jp.zeros_like(reset_state.reward),
     )
     reset_state.info['eval_metrics'] = eval_metrics
     return reset_state
 
-  def step(self, state: brax_env.State, action: jp.ndarray) -> brax_env.State:
+  def step(self, state: State, action: jp.ndarray) -> State:
     state_metrics = state.info['eval_metrics']
     if not isinstance(state_metrics, EvalMetrics):
       raise ValueError(
           f'Incorrect type for state_metrics: {type(state_metrics)}'
       )
     del state.info['eval_metrics']
     nstate = self.env.step(state, action)
```

### Comparing `brax-0.9.0/brax/generalized/__init__.py` & `brax-0.9.1/brax/envs/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/generalized/base.py` & `brax-0.9.1/brax/generalized/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,46 +8,46 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# pylint:disable=g-multiple-import
+# pylint:disable=g-multiple-import, g-importing-member
 """Base types for generalized pipeline."""
 
 from brax import base
 from brax.base import Inertia, Motion, Transform
 from flax import struct
 from jax import numpy as jp
 
 
 @struct.dataclass
 class State(base.State):
   """Dynamic state that changes after every step.
 
   Attributes:
-    com: center of mass position of the kinematic tree containing the link
-    cinr: inertia in com frame
-    cd: body velocities in com frame
-    cdof: dofs in com frame
-    cdofd: cdof velocity
+    root_com: (num_links,) center of mass position of link root kinematic tree
+    cinr: (num_links,) inertia in com frame
+    cd: (num_links,) link velocities in com frame
+    cdof: (qd_size,) dofs in com frame
+    cdofd: (qd_size,) cdof velocity
     mass_mx: (qd_size, qd_size) mass matrix
     mass_mx_inv: (qd_size, qd_size) inverse mass matrix
     contact: calculated contacts
     con_jac: constraint jacobian
     con_diag: constraint A diagonal
     con_aref: constraint reference acceleration
-    qf_smooth: smooth dynamics force
+    qf_smooth: (qd_size,) smooth dynamics force
     qf_constraint: (qd_size,) force from constraints (collision etc)
     qdd: (qd_size,) joint acceleration vector
   """
 
   # position/velocity based terms are updated at the end of each step:
-  com: jp.ndarray
+  root_com: jp.ndarray
   cinr: Inertia
   cd: Motion
   cdof: Motion
   cdofd: Motion
   mass_mx: jp.ndarray
   mass_mx_inv: jp.ndarray
   con_jac: jp.ndarray
@@ -67,15 +67,15 @@
     qd_size = qd.shape[0]
     return State(  # pylint:disable=unexpected-keyword-arg  # pytype: disable=wrong-arg-types  # jax-ndarray
         q=q,
         qd=qd,
         x=x,
         xd=xd,
         contact=None,
-        com=jp.zeros(3),
+        root_com=jp.zeros(3),
         cinr=Inertia(
             Transform.zero((num_links,)),
             jp.zeros((num_links, 3, 3)),
             jp.zeros((num_links,)),
         ),
         cd=Motion.zero((num_links,)),
         cdof=Motion.zero((num_links,)),
```

### Comparing `brax-0.9.0/brax/generalized/constraint.py` & `brax-0.9.1/brax/generalized/constraint.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,60 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# pylint:disable=g-multiple-import
+# pylint:disable=g-multiple-import, g-importing-member
 """Functions for constraint satisfaction."""
 from typing import Tuple
 
 from brax import geometry
 from brax import math
 from brax import scan
 from brax.base import Motion, System, Transform
 from brax.generalized.base import State
 import jax
 from jax import numpy as jp
 import jaxopt
 
 
-def _pt_jac(
-    sys: System,
-    com: jp.ndarray,
-    cdof: Motion,
-    pos: jp.ndarray,
-    link_idx: jp.ndarray,
-) -> jp.ndarray:
-  """Calculates the point jacobian.
-
-  Args:
-    sys: a brax system
-    com: center of mass position
-    cdof: dofs in com frame
-    pos: position in world frame
-    link_idx: index of link frame to transform point jacobian
-
-  Returns:
-    pt: point jacobian
-  """
-  # backward scan up tree: build the link mask corresponding to link_idx
-  def mask_fn(mask_child, link):
-    mask = link == link_idx
-    if mask_child is not None:
-      mask += mask_child
-    return mask
-
-  mask = scan.tree(sys, mask_fn, 'l', jp.arange(sys.num_links()), reverse=True)
-  cdof = jax.vmap(lambda a, b: a * b)(cdof, jp.take(mask, sys.dof_link()))
-  off = Transform.create(pos=pos - com[link_idx])
-  return off.vmap(in_axes=(None, 0)).do(cdof).vel
-
-
 def _imp_aref(
     params: jp.ndarray, pos: jp.ndarray, vel: jp.ndarray
 ) -> Tuple[jp.ndarray, jp.ndarray]:
   """Calculates impedance and offset acceleration in constraint frame.
 
   Args:
     params: solver params
@@ -83,19 +51,56 @@
   imp = dmin + imp_y * (dmax - dmin)
   imp = jp.clip(imp, dmin, dmax)
   imp = jp.where(imp_x > 1.0, dmax, imp)
 
   b = 2 / (dmax * timeconst)
   k = 1 / (dmax * dmax * timeconst * timeconst * dampratio * dampratio)
 
+  # See https://mujoco.readthedocs.io/en/latest/modeling.html#solver-parameters
+  stiffness, damping = params[:2]
+  b = jp.where(damping <= 0, -damping / dmax, b)
+  k = jp.where(stiffness <= 0, -stiffness / (dmax * dmax), k)
+
   aref = -b * vel - k * imp * pos
 
   return imp, aref
 
 
+def point_jacobian(
+    sys: System,
+    com: jp.ndarray,
+    cdof: Motion,
+    pos: jp.ndarray,
+    link_idx: jp.ndarray,
+) -> Motion:
+  """Calculates the jacobian of a point on a link.
+
+  Args:
+    sys: a brax system
+    com: center of mass position
+    cdof: dofs in com frame
+    pos: position in world frame to calculate the jacobian
+    link_idx: index of link frame to transform point jacobian
+
+  Returns:
+    pt: point jacobian
+  """
+  # backward scan up tree: build the link mask corresponding to link_idx
+  def mask_fn(mask_child, link):
+    mask = link == link_idx
+    if mask_child is not None:
+      mask += mask_child
+    return mask
+
+  mask = scan.tree(sys, mask_fn, 'l', jp.arange(sys.num_links()), reverse=True)
+  cdof = jax.vmap(lambda a, b: a * b)(cdof, jp.take(mask, sys.dof_link()))
+  off = Transform.create(pos=pos - com[link_idx])
+  return off.vmap(in_axes=(None, 0)).do(cdof)
+
+
 def jac_limit(
     sys: System, state: State
 ) -> Tuple[jp.ndarray, jp.ndarray, jp.ndarray]:
   """Calculates the jacobian for angle limits in dof frame.
 
   Args:
     sys: a brax system
@@ -114,15 +119,16 @@
 
   pos_min = state.q[q_idx] - sys.dof.limit[0][qd_idx]
   pos_max = sys.dof.limit[1][qd_idx] - state.q[q_idx]
   pos = jp.minimum(jp.minimum(pos_min, pos_max), 0)
 
   side = ((pos_min < pos_max) * 2 - 1) * (pos < 0)
   jac = jax.vmap(jp.multiply)(jp.eye(sys.qd_size())[qd_idx], side)
-  imp, aref = _imp_aref(sys.solver_params_joint, pos, jac @ state.qd)
+  params = sys.dof.solver_params[qd_idx]
+  imp, aref = jax.vmap(_imp_aref)(params, pos, jac @ state.qd)
   diag = sys.dof.invweight[qd_idx] * (pos < 0) * (1 - imp) / (imp + 1e-8)
   aref = jax.vmap(lambda x, y: x * y)(aref, (pos < 0))
 
   return jac, diag, aref
 
 
 def jac_contact(
@@ -142,27 +148,27 @@
   contact = geometry.contact(sys, state.x)
 
   if contact is None:
     return jp.zeros((0, sys.qd_size())), jp.zeros((0,)), jp.zeros((0,))
 
   def row_fn(contact):
     link_a, link_b = contact.link_idx
-    a = _pt_jac(sys, state.com, state.cdof, contact.pos, link_a)
-    b = _pt_jac(sys, state.com, state.cdof, contact.pos, link_b)
-    diff = b - a
+    a = point_jacobian(sys, state.root_com, state.cdof, contact.pos, link_a)
+    b = point_jacobian(sys, state.root_com, state.cdof, contact.pos, link_b)
+    diff = b.vel - a.vel
 
     # 4 pyramidal friction directions
     jac = []
     for d in math.orthogonals(contact.normal):
       for f in [-contact.friction, contact.friction]:
         jac.append(diff @ (d * f - contact.normal))
 
     jac = jp.stack(jac)
     pos = -jp.tile(contact.penetration, 4)
-    imp, aref = _imp_aref(sys.solver_params_contact, pos, jac @ state.qd)
+    imp, aref = _imp_aref(contact.solver_params, pos, jac @ state.qd)
     t = sys.link.invweight[link_a] + sys.link.invweight[link_b] * (link_b > -1)
     diag = jp.tile(t + contact.friction * contact.friction * t, 4)
     diag *= 2 * contact.friction * contact.friction * (1 - imp) / (imp + 1e-8)
 
     return jax.tree_map(
         lambda x: x * (contact.penetration > 0), (jac, diag, aref),
     )
```

### Comparing `brax-0.9.0/brax/generalized/constraint_test.py` & `brax-0.9.1/brax/generalized/constraint_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,24 +16,26 @@
 """Tests for constraints."""
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from brax import test_utils
 from brax.generalized import pipeline
 import jax
+from jax import numpy as jp
 import numpy as np
 
 
 class ConstraintTest(parameterized.TestCase):
 
   @parameterized.parameters(
       ('ant.xml',),
       ('triple_pendulum.xml',),
       ('humanoid.xml',),
       ('half_cheetah.xml',),
+      ('solver_params_v2.xml',)
   )
   def test_jacobian(self, xml_file):
     """Test constraint jacobian."""
     sys = test_utils.load_fixture(xml_file)
     for mj_prev, mj_next in test_utils.sample_mujoco_states(xml_file):
       state = jax.jit(pipeline.init)(sys, mj_prev.qpos, mj_prev.qvel)
       efc_j = np.reshape(mj_next.efc_J, (-1, sys.qd_size()))
@@ -52,28 +54,30 @@
       )
 
   @parameterized.parameters(
       ('ant.xml',),
       ('triple_pendulum.xml',),
       ('humanoid.xml',),
       ('half_cheetah.xml',),
+      ('solver_params_v2.xml',)
   )
   def test_force(self, xml_file):
     """Test constraint force."""
     sys = test_utils.load_fixture(xml_file)
     # brax can offer constraint solutions that are just as good as mujoco's
     # but we have to crank up solver iterations pretty high.  improving
     # brax's constraint solver will have a significant impact on perf
     sys = sys.replace(solver_iterations=500)
     err, mj_err = 0, 0
     # force PGS so we can reference efc_AR:
     samples = test_utils.sample_mujoco_states(xml_file, force_pgs=True)
     for mj_prev, mj_next in samples:
+      act = jp.zeros(sys.act_size())
       state = jax.jit(pipeline.init)(sys, mj_prev.qpos, mj_prev.qvel)
-      state = jax.jit(pipeline.step)(sys, state, mj_prev.qfrc_applied)
+      state = jax.jit(pipeline.step)(sys, state, act)
       efc_jt = np.reshape(mj_next.efc_J, (-1, sys.qd_size())).T
       # recover con_frc by backing it out from qf_constraint
       con_frc = np.linalg.lstsq(efc_jt, state.qf_constraint, None)[0]
       err += np.sum((mj_next.efc_AR @ con_frc + mj_next.efc_b) ** 2)
       mj_err += np.sum(
           (mj_next.efc_AR @ mj_next.efc_force + mj_next.efc_b) ** 2
       )
```

### Comparing `brax-0.9.0/brax/generalized/dynamics.py` & `brax-0.9.1/brax/generalized/dynamics.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# pylint:disable=g-multiple-import
+# pylint:disable=g-multiple-import, g-importing-member
 """Functions for smooth forward and inverse dynamics."""
+from brax import fluid
 from brax import math
 from brax import scan
 from brax.base import Motion, System, Transform
 from brax.generalized.base import State
+from brax.generalized.constraint import point_jacobian
 import jax
 from jax import numpy as jp
 
 
 def transform_com(sys: System, state: State) -> State:
   """Transforms inertia, dof, and link velocity into center of mass frame.
 
@@ -34,16 +36,16 @@
   """
   x_i = state.x.vmap().do(sys.link.inertia.transform)
   root_fn = lambda i, p=sys.link_parents: i if p[i] < 0 else root_fn(p[i])
   root = jp.array([root_fn(i) for i in range(sys.num_links())])
   mass_xi = jax.vmap(jp.multiply)(sys.link.inertia.mass, x_i.pos)
   mass_xi_sum = jax.ops.segment_sum(mass_xi, root, sys.num_links())
   mass_sum = jax.ops.segment_sum(sys.link.inertia.mass, root, sys.num_links())
-  com = jax.vmap(jp.divide)(mass_xi_sum[root], mass_sum[root])
-  cinr = x_i.replace(pos=x_i.pos - com).vmap().do(sys.link.inertia)
+  root_com = jax.vmap(jp.divide)(mass_xi_sum[root], mass_sum[root])
+  cinr = x_i.replace(pos=x_i.pos - root_com).vmap().do(sys.link.inertia)
 
   # motion dofs to global frame centered at subtree-CoM
   parent_idx = jp.array(
       [
           i if t == 'f' else p
           for i, (t, p) in enumerate(zip(sys.link_types, sys.link_parents))
       ]
@@ -81,15 +83,16 @@
     motion = jax.tree_map(lambda *x: jp.column_stack(x), *jds).reshape((-1, 3))
 
     return motion
 
   cdof = scan.link_types(sys, cdof_fn, 'qd', 'd', state.q, sys.dof.motion)
   ang = jax.vmap(math.rotate)(cdof.ang, j.take(sys.dof_link()).rot)
   cdof = cdof.replace(ang=ang)
-  cdof = Transform.create(pos=com - j.pos).take(sys.dof_link()).vmap().do(cdof)
+  off = Transform.create(pos=root_com - j.pos)
+  cdof = off.take(sys.dof_link()).vmap().do(cdof)
   cdof_qd = jax.vmap(lambda x, y: x * y)(cdof, state.qd)
 
   # forward scan down tree: accumulate link center of mass velocity
   def cd_fn(cd_parent, cdof_qd, dof_idx):
     if cd_parent is None:
       num_roots = len([p for p in sys.link_parents if p == -1])
       cd_parent = Motion.zero(shape=(num_roots,))
@@ -124,15 +127,17 @@
     cdofd = cd.vmap().cross(cdof)
 
     return cdofd
 
   cd_p = cd.concatenate(Motion.zero(shape=(1,))).take(parent_idx)
   cdofd = scan.link_types(sys, cdofd_fn, 'ldd', 'd', cd_p, cdof, cdof_qd)
 
-  return state.replace(com=com, cinr=cinr, cd=cd, cdof=cdof, cdofd=cdofd)
+  return state.replace(
+      root_com=root_com, cinr=cinr, cd=cd, cdof=cdof, cdofd=cdofd
+  )
 
 
 def inverse(sys: System, state: State) -> jp.ndarray:
   """Calculates the system's forces given input motions.
 
   This function computes inverse dynamics using the Newton-Euler algorithm:
 
@@ -176,24 +181,38 @@
 
   # tau = cdof * cfrc[dof_link]
   tau = jax.vmap(lambda x, y: x.dot(y))(state.cdof, cfrc.take(sys.dof_link()))
 
   return tau
 
 
-def _passive(sys: System, q: jp.ndarray, qd: jp.ndarray) -> jp.ndarray:
+def _passive(sys: System, state: State) -> jp.ndarray:
   """Calculates the system's passive forces given input motion and position."""
-
   def stiffness_fn(typ, q, dof):
     if typ in 'fb':
       return jp.zeros_like(dof.stiffness)
     return -q * dof.stiffness
 
-  frc = scan.link_types(sys, stiffness_fn, 'qd', 'd', q, sys.dof)
-  frc -= sys.dof.damping * qd
+  frc = scan.link_types(sys, stiffness_fn, 'qd', 'd', state.q, sys.dof)
+  frc -= sys.dof.damping * state.qd
+
+  if sys.enable_fluid:
+    fluid_frc = fluid.force(
+        sys,
+        state.x,
+        state.cd,
+        sys.link.inertia.mass,
+        sys.link.inertia.i,
+        state.root_com,
+    )
+    link_idx = jp.arange(sys.num_links())
+    x_i = state.x.vmap().do(sys.link.inertia.transform)
+    jac_fn = jax.vmap(point_jacobian, in_axes=(None, None, None, 0, 0))
+    jac = jac_fn(sys, state.root_com, state.cdof, x_i.pos, link_idx)
+    frc += jax.vmap(lambda x, y: x.dot(y))(jac, fluid_frc).sum(axis=0)
 
   return frc
 
 
 def forward(sys: System, state: State, tau: jp.ndarray) -> jp.ndarray:
   """Calculates resulting joint forces given input forces.
 
@@ -206,12 +225,12 @@
     sys: a brax system
     state: generalized state
     tau: joint force input vector
 
   Returns:
     qfrc: joint force vector
   """
-  qfrc_passive = _passive(sys, state.q, state.qd)
+  qfrc_passive = _passive(sys, state)
   qfrc_bias = inverse(sys, state)
   qfrc = qfrc_passive - qfrc_bias + tau
 
   return qfrc
```

### Comparing `brax-0.9.0/brax/generalized/dynamics_test.py` & `brax-0.9.1/brax/generalized/dynamics_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,32 @@
 """Tests for dynamics."""
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from brax import test_utils
 from brax.generalized import pipeline
 import jax
+from jax import numpy as jp
 import numpy as np
 
 
 class DynamicsTest(parameterized.TestCase):
 
   @parameterized.parameters(
       'ant.xml', 'triple_pendulum.xml', ('humanoid.xml',), ('half_cheetah.xml',)
   )
   def test_transform_com(self, xml_file):
     """Test dynamics transform com."""
     sys = test_utils.load_fixture(xml_file)
     for mj_prev, mj_next in test_utils.sample_mujoco_states(xml_file):
       state = jax.jit(pipeline.init)(sys, mj_prev.qpos, mj_prev.qvel)
 
-      np.testing.assert_almost_equal(state.com[0], mj_next.subtree_com[0], 5)
+      np.testing.assert_almost_equal(
+          state.root_com[0], mj_next.subtree_com[0], 5
+      )
       mj_cinr_i = np.zeros((state.cinr.i.shape[0], 3, 3))
       mj_cinr_i[:, [0, 1, 2], [0, 1, 2]] = mj_next.cinert[1:, 0:3]  # diagonal
       mj_cinr_i[:, [0, 0, 1], [1, 2, 2]] = mj_next.cinert[1:, 3:6]  # upper tri
       mj_cinr_i[:, [1, 2, 2], [0, 0, 1]] = mj_next.cinert[1:, 3:6]  # lower tri
       mj_cinr_pos = mj_next.cinert[1:, 6:9]
 
       np.testing.assert_almost_equal(state.cinr.i, mj_cinr_i, 5)
@@ -51,16 +54,17 @@
   @parameterized.parameters(
       'ant.xml', 'triple_pendulum.xml', ('humanoid.xml',), ('half_cheetah.xml',)
   )
   def test_forward(self, xml_file):
     """Test dynamics forward."""
     sys = test_utils.load_fixture(xml_file)
     for mj_prev, mj_next in test_utils.sample_mujoco_states(xml_file):
+      act = jp.zeros(sys.act_size())
       state = jax.jit(pipeline.init)(sys, mj_prev.qpos, mj_prev.qvel)
-      state = jax.jit(pipeline.step)(sys, state, mj_prev.qfrc_applied)
+      state = jax.jit(pipeline.step)(sys, state, act)
 
       np.testing.assert_allclose(
           state.qf_smooth, mj_next.qfrc_smooth, rtol=1e-4, atol=1e-4
       )
 
 
 if __name__ == '__main__':
```

### Comparing `brax-0.9.0/brax/generalized/integrator.py` & `brax-0.9.1/brax/generalized/integrator.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/generalized/mass.py` & `brax-0.9.1/brax/generalized/mass.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/generalized/mass_test.py` & `brax-0.9.1/brax/generalized/mass_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/generalized/perf_test.py` & `brax-0.9.1/brax/generalized/perf_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,14 @@
       rng1, rng2 = jax.random.split(rng, 2)
       q = jp.array([0, 0, 0.75, 1.0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0])
       q += jax.random.uniform(rng1, (sys.q_size(),), minval=-0.1, maxval=0.1)
       qd = 0.1 * jax.random.normal(rng2, (sys.qd_size(),))
       return pipeline.init(sys, q, qd)
 
     def step_fn(state):
-      return pipeline.step(sys, state, jp.zeros(sys.qd_size()))
+      return pipeline.step(sys, state, jp.zeros(sys.act_size()))
 
     test_utils.benchmark('generalized pipeline ant', init_fn, step_fn)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `brax-0.9.0/brax/generalized/pipeline.py` & `brax-0.9.1/brax/generalized/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     act: (act_size,) actuator input vector
     debug: if True, adds contact to the state for debugging
 
   Returns:
     state: physics state after step
   """
   # calculate acceleration terms
-  tau = actuator.to_tau(sys, act, state.q)
+  tau = actuator.to_tau(sys, act, state.q, state.qd)
   state = state.replace(qf_smooth=dynamics.forward(sys, state, tau))
   state = state.replace(qf_constraint=constraint.force(sys, state))
 
   # update position/velocity level terms
   state = integrator.integrate(sys, state)
   x, xd = kinematics.forward(sys, state.q, state.qd)
   state = state.replace(x=x, xd=xd)
```

### Comparing `brax-0.9.0/brax/generalized/pipeline_test.py` & `brax-0.9.1/brax/generalized/pipeline_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 """Tests for generalized pipeline."""
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from brax import test_utils
 from brax.generalized import pipeline
 import jax
+from jax import numpy as jp
 import numpy as np
 
 
 class PipelineTest(parameterized.TestCase):
 
   @parameterized.parameters(
       ('ant.xml',),
@@ -34,15 +35,15 @@
   def test_forward(self, xml_file):
     """Test pipeline step."""
     sys = test_utils.load_fixture(xml_file)
     # crank up solver iterations just to demonstrate close match to mujoco
     sys = sys.replace(solver_iterations=500)
     for mj_prev, mj_next in test_utils.sample_mujoco_states(xml_file):
       state = jax.jit(pipeline.init)(sys, mj_prev.qpos, mj_prev.qvel)
-      state = jax.jit(pipeline.step)(sys, state, mj_prev.qfrc_applied)
+      state = jax.jit(pipeline.step)(sys, state, jp.zeros(sys.act_size()))
 
       np.testing.assert_allclose(state.q, mj_next.qpos, atol=0.002)
       np.testing.assert_allclose(state.qd, mj_next.qvel, atol=0.5)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `brax-0.9.0/brax/geometry/__init__.py` & `brax-0.9.1/brax/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/geometry/contact.py` & `brax-0.9.1/brax/geometry/contact.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 """Calculations for generating contacts."""
 
 from typing import Iterator, Optional, Tuple
 
 from brax import math
 from brax.base import (
     Capsule,
+    Cylinder,
     Contact,
     Convex,
     Geometry,
     Mesh,
     Plane,
     Sphere,
     System,
@@ -31,48 +32,35 @@
 )
 from brax.geometry import math as geom_math
 from brax.geometry import mesh as geom_mesh
 import jax
 from jax import numpy as jp
 
 
-def _combine(
-    geom_a: Geometry, geom_b: Geometry
-) -> Tuple[float, float, Tuple[int, int]]:
-  # default is to take maximum, but can override
-  friction = jp.maximum(geom_a.friction, geom_b.friction)
-  elasticity = jp.maximum(geom_a.elasticity, geom_b.elasticity)
-  link_idx = (
-      geom_a.link_idx,
-      geom_b.link_idx if geom_b.link_idx is not None else -1,
-  )
-  return friction, elasticity, link_idx  # pytype: disable=bad-return-type  # jax-ndarray
-
-
 def _sphere_plane(sphere: Sphere, plane: Plane) -> Contact:
   """Calculates one contact between a sphere and a plane."""
   n = math.rotate(jp.array([0.0, 0.0, 1.0]), plane.transform.rot)
   t = jp.dot(sphere.transform.pos - plane.transform.pos, n)
   penetration = sphere.radius - t
   # halfway between contact points on sphere and on plane
   pos = sphere.transform.pos - n * (sphere.radius - 0.5 * penetration)
-  c = Contact(pos, n, penetration, *_combine(sphere, plane))  # pytype: disable=wrong-arg-types  # jax-ndarray
-  # add a batch dimension of size 1
+  c = Contact(pos, n, penetration, *_combine(sphere, plane))
+  # returns 1 contact, so add a batch dimension of size 1
   return jax.tree_map(lambda x: jp.expand_dims(x, axis=0), c)
 
 
 def _sphere_sphere(s_a: Sphere, s_b: Sphere) -> Contact:
   """Calculates one contact between two spheres."""
   n, dist = math.normalize(s_a.transform.pos - s_b.transform.pos)
   penetration = s_a.radius + s_b.radius - dist
   s_a_pos = s_a.transform.pos - n * s_a.radius
   s_b_pos = s_b.transform.pos + n * s_b.radius
   pos = (s_a_pos + s_b_pos) * 0.5
-  c = Contact(pos, n, penetration, *_combine(s_a, s_b))  # pytype: disable=wrong-arg-types  # jax-ndarray
-  # add a batch dimension of size 1
+  c = Contact(pos, n, penetration, *_combine(s_a, s_b))
+  # returns 1 contact, so add a batch dimension of size 1
   return jax.tree_map(lambda x: jp.expand_dims(x, axis=0), c)
 
 
 def _sphere_capsule(sphere: Sphere, capsule: Capsule) -> Contact:
   """Calculates one contact between a sphere and a capsule."""
   segment = jp.array([0.0, 0.0, capsule.length * 0.5])
   segment = math.rotate(segment, capsule.transform.rot)
@@ -84,16 +72,65 @@
   n, dist = math.normalize(sphere.transform.pos - pt)
   penetration = sphere.radius + capsule.radius - dist
 
   sphere_pos = sphere.transform.pos - n * sphere.radius
   cap_pos = pt + n * capsule.radius
   pos = (sphere_pos + cap_pos) * 0.5
 
-  c = Contact(pos, n, penetration, *_combine(sphere, capsule))  # pytype: disable=wrong-arg-types  # jax-ndarray
-  # add a batch dimension of size 1
+  c = Contact(pos, n, penetration, *_combine(sphere, capsule))
+  # returns 1 contact, so add a batch dimension of size 1
+  return jax.tree_map(lambda x: jp.expand_dims(x, axis=0), c)
+
+
+def _sphere_circle(sphere: Sphere, circle: Cylinder) -> Contact:
+  """Calculates one contact between a sphere and a circle."""
+  n = math.rotate(jp.array([0.0, 0.0, 1.0]), circle.transform.rot)
+
+  # orient the normal s.t. it points at the CoM of the sphere
+  normal_dir = jp.sign(
+      (sphere.transform.pos - circle.transform.pos).dot(n))
+  n = n * normal_dir
+
+  pos = sphere.transform.pos - n * sphere.radius
+  plane_pt = circle.transform.pos
+  penetration = jp.dot(plane_pt - pos, n)
+
+  # check if the sphere radius is within the cylinder in the normal dir of the
+  # circle
+  plane_pt2 = plane_pt + n
+  line_pt = geom_math.closest_line_point(
+      plane_pt, plane_pt2, sphere.transform.pos
+  )
+  in_cylinder = (sphere.transform.pos - line_pt).dot(
+      sphere.transform.pos - line_pt
+  ) <= circle.radius**2
+
+  # get closest point on circle edge
+  perp_dir = jp.cross(n, sphere.transform.pos - plane_pt)
+  perp_dir = math.rotate(perp_dir, math.quat_rot_axis(n, -jp.pi / 2.0))
+  perp_dir, _ = math.normalize(perp_dir)
+  edge_pt = plane_pt + perp_dir * circle.radius
+  edge_contact = (sphere.transform.pos - edge_pt).dot(
+      sphere.transform.pos - edge_pt
+  ) <= sphere.radius**2
+  edge_to_sphere = sphere.transform.pos - edge_pt
+  edge_to_sphere = math.normalize(edge_to_sphere)[0]
+
+  penetration = jp.where(in_cylinder, penetration, -jp.ones_like(penetration))
+  penetration = jp.where(
+      edge_contact,
+      sphere.radius
+      - jp.sqrt(
+          (sphere.transform.pos - edge_pt).dot(sphere.transform.pos - edge_pt)
+      ),
+      penetration,
+  )
+  n = jp.where(edge_contact, edge_to_sphere, n)
+  pos = jp.where(edge_contact, edge_pt, pos)
+  c = Contact(pos, n, penetration, *_combine(sphere, circle))  # pytype: disable=wrong-arg-types  # jax-ndarray
   return jax.tree_map(lambda x: jp.expand_dims(x, axis=0), c)
 
 
 def _sphere_convex(sphere: Sphere, convex: Convex) -> Contact:
   """Calculates contacts between a sphere and a convex object."""
   # Get convex transformed normals, faces, and vertices.
   normals = geom_mesh.get_face_norm(convex.vert, convex.face)
@@ -150,15 +187,15 @@
 
   # Get the normal, penetration, and contact position.
   n, d = math.normalize(sphere.transform.pos - pt)
   spt = sphere.transform.pos - n * sphere.radius
   penetration = sphere.radius - d
   pos = (pt + spt) * 0.5
 
-  c = Contact(pos, n, penetration, *_combine(sphere, convex))  # pytype: disable=wrong-arg-types  # jax-ndarray
+  c = Contact(pos, n, penetration, *_combine(sphere, convex))
   return jax.tree_map(lambda x: jp.expand_dims(x, axis=0), c)
 
 
 def _sphere_mesh(sphere: Sphere, mesh: Mesh) -> Contact:
   """Calculates contacts between a sphere and a mesh."""
 
   @jax.vmap
@@ -170,32 +207,33 @@
 
     tri_p = geom_math.closest_triangle_point(p0, p1, p2, sphere.transform.pos)
     n = sphere.transform.pos - tri_p
     n, dist = math.normalize(n)
     penetration = sphere.radius - dist
     sph_p = sphere.transform.pos - n * sphere.radius
     pos = (tri_p + sph_p) * 0.5
-    return Contact(pos, n, penetration, *_combine(sphere, mesh))  # pytype: disable=wrong-arg-types  # jax-ndarray
+    return Contact(pos, n, penetration, *_combine(sphere, mesh))
 
   return sphere_face(jp.take(mesh.vert, mesh.face, axis=0))
 
 
 def _capsule_plane(capsule: Capsule, plane: Plane) -> Contact:
   """Calculates two contacts between a capsule and a plane."""
   segment = jp.array([0.0, 0.0, capsule.length * 0.5])
   segment = math.rotate(segment, capsule.transform.rot)
 
   results = []
   for off in [segment, -segment]:
     sphere = Sphere(
+        radius=capsule.radius,
         link_idx=capsule.link_idx,
         transform=Transform.create(pos=capsule.transform.pos + off),
         friction=capsule.friction,
         elasticity=capsule.elasticity,
-        radius=capsule.radius,
+        solver_params=capsule.solver_params,
     )
     results.append(_sphere_plane(sphere, plane))
 
   return jax.tree_map(lambda *x: jp.concatenate(x), *results)
 
 
 def _capsule_capsule(cap_a: Capsule, cap_b: Capsule) -> Contact:
@@ -213,16 +251,16 @@
   n, dist = math.normalize(pt_a - pt_b)
   penetration = cap_a.radius + cap_b.radius - dist
 
   cap_a_pos = pt_a - n * cap_a.radius
   cap_b_pos = pt_b + n * cap_b.radius
   pos = (cap_a_pos + cap_b_pos) * 0.5
 
-  c = Contact(pos, n, penetration, *_combine(cap_a, cap_b))  # pytype: disable=wrong-arg-types  # jax-ndarray
-  # add a batch dimension of size 1
+  c = Contact(pos, n, penetration, *_combine(cap_a, cap_b))
+  # returns 1 contact, so add a batch dimension of size 1
   return jax.tree_map(lambda x: jp.expand_dims(x, axis=0), c)
 
 
 def _capsule_convex(capsule: Capsule, convex: Convex) -> Contact:
   """Calculates contacts between a capsule and a convex object."""
   # Get convex transformed normals, faces, and vertices.
   normals = geom_mesh.get_face_norm(convex.vert, convex.face)
@@ -302,18 +340,17 @@
 
   # Create the contact.
   pos = jp.where(has_edge_contact, pos.at[0].set(edge_pos), pos)
   norm = jp.where(has_edge_contact, norm.at[0].set(edge_norm), norm)
   penetration = jp.where(
       has_edge_contact, penetration.at[0].set(edge_penetration), penetration
   )
-  friction, elasticity, link_idx = jax.tree_map(
-      lambda x: jp.repeat(x, 2), _combine(capsule, convex)
-  )
-  return Contact(pos, norm, penetration, friction, elasticity, link_idx)
+  tile_fn = lambda x: jp.tile(x, (2,) + tuple([1 for _ in x.shape]))
+  params = jax.tree_map(tile_fn, _combine(capsule, convex))
+  return Contact(pos, norm, penetration, *params)
 
 
 def _capsule_mesh(capsule: Capsule, mesh: Mesh) -> Contact:
   """Calculates contacts between a capsule and a mesh."""
 
   @jax.vmap
   def capsule_face(face, face_norm):
@@ -331,15 +368,15 @@
         end_a, end_b, p0, p1, p2, tri_norm
     )
     n = seg_p - tri_p
     n, dist = math.normalize(n)
     penetration = capsule.radius - dist
     cap_p = seg_p - n * capsule.radius
     pos = (tri_p + cap_p) * 0.5
-    return Contact(pos, n, penetration, *_combine(capsule, mesh))  # pytype: disable=wrong-arg-types  # jax-ndarray
+    return Contact(pos, n, penetration, *_combine(capsule, mesh))
 
   face_vert = jp.take(mesh.vert, mesh.face, axis=0)
   face_norm = geom_mesh.get_face_norm(mesh.vert, mesh.face)
   return capsule_face(face_vert, face_norm)
 
 
 def _convex_plane(convex: Convex, plane: Plane) -> Contact:
@@ -356,18 +393,17 @@
   )
   idx = geom_math.manifold_points(vertices, support > 0, n)
 
   pos = vertices[idx]
   normal = jp.stack([n] * 4, axis=0)
   unique = jp.tril(idx == idx[:, None]).sum(axis=1) == 1
   penetration = jp.where(unique, support[idx], -1)
-  friction, elasticity, link_idx = jax.tree_map(
-      lambda x: jp.repeat(x, 4), _combine(convex, plane)
-  )
-  return Contact(pos, normal, penetration, friction, elasticity, link_idx)
+  tile_fn = lambda x: jp.tile(x, (4,) + tuple([1 for _ in x.shape]))
+  params = jax.tree_map(tile_fn, _combine(convex, plane))
+  return Contact(pos, normal, penetration, *params)
 
 
 def _convex_convex(convex_a: Convex, convex_b: Convex) -> Contact:
   """Calculates contacts between two convex objects."""
   # pad face vertices so that we can broadcast between geom_i and geom_j
   sa, sb = convex_a.face.shape[-1], convex_b.face.shape[-1]
   if sa < sb:
@@ -412,45 +448,52 @@
       vertices_a,
       vertices_b,
       normals_a,
       normals_b,
       unique_edges_a,
       unique_edges_b,
   )
-  friction, elasticity, link_idx = jax.tree_map(
-      lambda x: jp.repeat(x, 4), _combine(convex_a, convex_b)
-  )
+  tile_fn = lambda x: jp.tile(x, (4,) + tuple([1 for _ in x.shape]))
+  params = jax.tree_map(tile_fn, _combine(convex_a, convex_b))
 
-  return Contact(
-      c.pos,
-      c.normal,
-      c.penetration,
-      friction,
-      elasticity,
-      link_idx,
-  )
+  return Contact(c.pos, c.normal, c.penetration, *params)
 
 
 def _mesh_plane(mesh: Mesh, plane: Plane) -> Contact:
   """Calculates contacts between a mesh and a plane."""
 
   @jax.vmap
   def point_plane(vert):
     n = math.rotate(jp.array([0.0, 0.0, 1.0]), plane.transform.rot)
     pos = mesh.transform.pos + math.rotate(vert, mesh.transform.rot)
     penetration = jp.dot(plane.transform.pos - pos, n)
-    return Contact(pos, n, penetration, *_combine(mesh, plane))  # pytype: disable=wrong-arg-types  # jax-ndarray
+    return Contact(pos, n, penetration, *_combine(mesh, plane))
 
   return point_plane(mesh.vert)
 
 
+def _combine(
+    geom_a: Geometry, geom_b: Geometry
+) -> Tuple[jp.ndarray, jp.ndarray, jp.ndarray, Tuple[jp.ndarray, jp.ndarray]]:
+  # default is to take maximum, but can override
+  friction = jp.maximum(geom_a.friction, geom_b.friction)
+  elasticity = (geom_a.elasticity + geom_b.elasticity) * 0.5
+  solver_params = (geom_a.solver_params + geom_b.solver_params) * 0.5
+  link_idx = (
+      jp.array(geom_a.link_idx if geom_a.link_idx is not None else -1),
+      jp.array(geom_b.link_idx if geom_b.link_idx is not None else -1),
+  )
+  return friction, elasticity, solver_params, link_idx
+
+
 _TYPE_FUN = {
     (Sphere, Plane): _sphere_plane,
     (Sphere, Sphere): _sphere_sphere,
     (Sphere, Capsule): _sphere_capsule,
+    (Sphere, Cylinder): _sphere_circle,
     (Sphere, Convex): _sphere_convex,
     (Sphere, Mesh): _sphere_mesh,
     (Capsule, Plane): _capsule_plane,
     (Capsule, Capsule): _capsule_capsule,
     (Capsule, Convex): _capsule_convex,
     (Capsule, Mesh): _capsule_mesh,
     (Convex, Convex): _convex_convex,
```

### Comparing `brax-0.9.0/brax/geometry/contact_test.py` & `brax-0.9.1/brax/geometry/contact_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,36 @@
     x, _ = kinematics.forward(sys, sys.init_q, jp.zeros(sys.qd_size()))
     c = geometry.contact(sys, x).take(0)
 
     np.testing.assert_array_almost_equal(c.penetration, 0.01)
     np.testing.assert_array_almost_equal(c.pos, jp.array([0.0, 0.3, 0.045]))
     np.testing.assert_array_almost_equal(c.normal, jp.array([0, 0.0, -1.0]))
 
+  _SPHERE_CYLINDER = """
+    <mujoco model="sphere_cylinder">
+      <worldbody>
+        <body name="body1" pos="0 0 0">
+          <joint axis="1 0 0" name="free1" pos="0 0 0" type="free"/>
+          <geom name="sphere1" pos="0 0.04 0" size="0.05" type="sphere"/>
+        </body>
+        <body name="body2" pos="0 0 0">
+          <joint axis="1 0 0" name="free2" pos="0 0 0" type="free"/>
+          <geom name="cyl" pos="0 0 0" size="0.1 0.001" type="cylinder"/>
+        </body>
+      </worldbody>
+    </mujoco>
+  """
+
+  def test_sphere_cylinder(self):
+    sys = mjcf.loads(self._SPHERE_CYLINDER)
+    x, _ = kinematics.forward(sys, sys.init_q, jp.zeros(sys.qd_size()))
+    c = geometry.contact(sys, x).take(0)
+
+    np.testing.assert_array_almost_equal(c.penetration, 0.01)
+
   _SPHERE_CONVEX = """
     <mujoco model="sphere_convex">
       <worldbody>
         <body name="body1" pos="0.52 0 0.52">
           <joint axis="1 0 0" name="free1" pos="0 0 0" type="free"/>
           <geom name="sphere1" pos="0 0 0" size="0.05" type="sphere"/>
         </body>
```

### Comparing `brax-0.9.0/brax/geometry/math.py` & `brax-0.9.1/brax/geometry/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,23 @@
 ) -> Tuple[jp.ndarray, jp.ndarray]:
   """Returns closest point on the line segment and the distance squared."""
   closest = closest_segment_point(a, b, pt)
   dist = (pt - closest).dot(pt - closest)
   return closest, dist
 
 
+def closest_line_point(
+    a: jp.ndarray, b: jp.ndarray, pt: jp.ndarray
+) -> jp.ndarray:
+  """Returns the closest point on the a-b line to a point pt."""
+  ab = b - a
+  t = jp.dot(pt - a, ab) / (jp.dot(ab, ab) + 1e-6)
+  return a + t * ab
+
+
 def closest_segment_to_segment_points(
     a0: jp.ndarray, a1: jp.ndarray, b0: jp.ndarray, b1: jp.ndarray
 ) -> Tuple[jp.ndarray, jp.ndarray]:
   """Returns closest points on two line segments."""
   # Gets the closest segment points by first finding the closest points
   # between two lines. Points are then clipped to be on the line segments
   # and edge cases with clipping are handled.
@@ -428,14 +437,15 @@
 
   contact = Contact(
       pos=contact_pts,
       normal=jp.stack([sep_axis] * 4, 0),
       penetration=penetration,
       friction=jp.array([]),
       elasticity=jp.array([]),
+      solver_params=jp.array([]),
       link_idx=jp.array([]),
   )
 
   return contact
 
 
 def sat_hull_hull(
```

### Comparing `brax-0.9.0/brax/geometry/math_test.py` & `brax-0.9.1/brax/geometry/math_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/geometry/mesh.py` & `brax-0.9.1/brax/geometry/mesh.py`

 * *Files 7% similar despite different names*

```diff
@@ -124,28 +124,30 @@
   return Mesh(  # pytype: disable=wrong-arg-types  # jax-ndarray
       vert=vert,
       face=face,
       link_idx=b.link_idx,
       transform=b.transform,
       friction=b.friction,
       elasticity=b.elasticity,
+      solver_params=b.solver_params,
       rgba=b.rgba,
   )
 
 
 def _box_hull(b: Box) -> Convex:
   """Creates a mesh for a box with rectangular faces."""
   vert, face = _box(b, triangulated=False)
   return Convex(  # pytype: disable=wrong-arg-types  # jax-ndarray
       vert=vert,
       face=face,
       link_idx=b.link_idx,
       transform=b.transform,
       friction=b.friction,
       elasticity=b.elasticity,
+      solver_params=b.solver_params,
       unique_edge=get_unique_edges(vert, face),
       rgba=b.rgba,
   )
 
 
 def convex_hull_2d(points: np.ndarray, normal: np.ndarray) -> np.ndarray:
   """Calculates the hull face for a set of points on a plane."""
@@ -221,14 +223,15 @@
   return Convex(  # pytype: disable=wrong-arg-types  # jax-ndarray
       vert=vert,
       face=face,
       link_idx=m.link_idx,
       transform=m.transform,
       friction=m.friction,
       elasticity=m.elasticity,
+      solver_params=m.solver_params,
       unique_edge=get_unique_edges(vert, face),
       rgba=m.rgba,
   )
 
 
 def convex_hull(obj: Union[Box, Mesh]) -> Convex:
   """Creates a convex hull from a box or mesh."""
@@ -240,10 +243,11 @@
     _CONVEX_CACHE[key] = _convex_hull(obj)
   convex = _CONVEX_CACHE[key]
   convex = convex.replace(
       link_idx=obj.link_idx,
       transform=obj.transform,
       friction=obj.friction,
       elasticity=obj.elasticity,
+      solver_params=obj.solver_params,
       rgba=obj.rgba,
   )
   return convex
```

### Comparing `brax-0.9.0/brax/geometry/mesh_test.py` & `brax-0.9.1/brax/geometry/mesh_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     """Tests a triangulated box."""
     b = Box(
         halfsize=np.repeat(0.5, 3),
         link_idx=None,
         transform=None,
         friction=0.42,
         elasticity=1,
+        solver_params=None,
     )
     m = mesh.box_tri(b)
     self.assertIsInstance(m, Mesh)
     self.assertSequenceEqual(m.vert.shape, (8, 3))  # eight box corners
     self.assertEqual(np.unique(np.abs(m.vert)), 0.5)
     self.assertSequenceEqual(m.face.shape, (12, 3))  # two triangles per face
     self.assertEqual(m.friction, 0.42)
@@ -60,14 +61,15 @@
     """Tests a polygon box."""
     b = Box(
         halfsize=np.repeat(0.5, 3).reshape(3),
         link_idx=None,
         transform=None,
         friction=0.42,
         elasticity=1,
+        solver_params=None,
     )
     h = mesh.convex_hull(b)
     self.assertIsInstance(h, Convex)
     self.assertSequenceEqual(h.vert.shape, (8, 3))
     self.assertEqual(np.unique(np.abs(h.vert)), 0.5)
     np.testing.assert_array_equal(h.unique_edge, [[0, 1], [0, 2], [0, 4]])
     self.assertSequenceEqual(h.face.shape, (6, 4))  # one rectangle per face
@@ -102,14 +104,15 @@
     pyramid = Mesh(
         link_idx=0,
         transform=Transform.zero((1,)),
         vert=vert,
         face=face,
         friction=1,
         elasticity=0,
+        solver_params=None,
     )
     h = mesh.convex_hull(pyramid)
 
     self.assertIsInstance(h, Convex)
 
     # check verts
     vidx = [0, 3, 2, 1, 4]  # verts get mixed up by trimesh
```

### Comparing `brax-0.9.0/brax/io/__init__.py` & `brax-0.9.1/brax/generalized/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/io/html.py` & `brax-0.9.1/brax/io/html.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/io/json.py` & `brax-0.9.1/brax/io/json.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 # pylint:disable=g-multiple-import
 """Saves a system config and trajectory as json."""
 
 import json
 from typing import List, Text
 
-from brax import geometry
 from brax.base import State, System
 from etils import epath
 import jax
 import jax.numpy as jp
 import numpy as np
 
 # State attributes needed for the visualizer.
@@ -94,15 +93,26 @@
 
   Args:
     sys: brax System object
     states: list of brax system states
 
   Returns:
     string containing json dump of system and states
+
+  Raises:
+    RuntimeError: if states have invalid shape
   """
+  if any((len(s.x.pos.shape), len(s.x.rot.shape)) != (2, 2) for s in states):
+    pos_shape = max(len(s.x.pos.shape) for s in states)
+    rot_shape = max(len(s.x.rot.shape) for s in states)
+    raise RuntimeError(
+        'Expected state.x position and rotation to have 2 shape dimensions but '
+        f'received len(pos.shape)={pos_shape} and len(rot.shape)={rot_shape}'
+    )
+
   d = _to_dict(sys)
 
   # TODO: move the manipulations below to javascript
 
   # fill in empty link names
   link_names = [n or f'link {i}' for i, n in enumerate(sys.link_names)]
   link_names += ['world']
```

### Comparing `brax-0.9.0/brax/io/json_test.py` & `brax-0.9.1/brax/io/json_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import json
 
 from absl.testing import absltest
 from brax import test_utils
 from brax.generalized import pipeline
 from brax.io import json as bjson
+import jax
 import jax.numpy as jp
 
 
 class JsonTest(absltest.TestCase):
 
   def test_dumps(self):
     sys = test_utils.load_fixture('convex_convex.xml')
@@ -34,10 +35,17 @@
     self.assertIsInstance(res['geoms'], dict)
     self.assertSequenceEqual(
         sorted(res['geoms'].keys()),
         ['box', 'dodecahedron', 'pyramid', 'tetrahedron', 'world'],
     )
     self.assertLen(res['geoms']['world'], 1)
 
+  def test_dumps_invalidstate_raises(self):
+    sys = test_utils.load_fixture('convex_convex.xml')
+    state = pipeline.init(sys, sys.init_q, jp.zeros(sys.qd_size()))
+    state = jax.tree_map(lambda x: jp.stack([x, x]), state)
+    with self.assertRaises(RuntimeError):
+      bjson.dumps(sys, [state])
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `brax-0.9.0/brax/io/metrics.py` & `brax-0.9.1/brax/io/metrics.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/io/mjcf.py` & `brax-0.9.1/brax/io/mjcf.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint:disable=g-multiple-import
 """Function to load MuJoCo mjcf format to Brax system."""
 
 import itertools
-from typing import Dict, Tuple, Union
+from typing import Dict, Optional, Tuple, Union
 import warnings
 from xml.etree import ElementTree
 
 from brax import math
 from brax.base import (
     Actuator,
     Box,
     Capsule,
+    Cylinder,
     DoF,
     Inertia,
     Link,
     Mesh,
     Motion,
     Plane,
     Sphere,
@@ -39,82 +40,79 @@
 from etils import epath
 import jax
 from jax import numpy as jp
 import mujoco
 import numpy as np
 
 
-# map from mujoco joint type to brax joint type string
-_JOINT_TYPE_STR = {
-    0: 'f',  # free
-    1: 'b',  # ball
-    2: 'p',  # prismatic
-    3: 'r',  # revolute
-}
-
-# map from mujoco bias type to brax actuator type string
-_ACT_TYPE_STR = {
-    0: 'm',  # motor
-    1: 'p',  # position
-}
-
-
 def _transform_do(
     pos: np.ndarray, quat: np.ndarray, cpos: np.ndarray, cquat: np.ndarray
 ) -> Tuple[np.ndarray, np.ndarray]:
   pos = pos + math.rotate_np(cpos, quat)
   rot = math.quat_mul_np(quat, cquat)
   return pos, rot
 
 
 def _fuse_bodies(elem: ElementTree.Element):
   """Fuses together parent child bodies that have no joint."""
 
   for child in list(elem):  # we will modify elem children, so make a copy
-    if child.tag == 'body' and 'joint' not in [e.tag for e in child]:
-      cpos = child.attrib.get('pos', '0 0 0')
-      cpos = np.fromstring(cpos, sep=' ')
-      cquat = child.attrib.get('quat', '1 0 0 0')
-      cquat = np.fromstring(cquat, sep=' ')
-      for grandchild in child:
-        # TODO: might need to offset more than just body, geom
-        if grandchild.tag in ('body', 'geom') and (cpos != 0).any():
-          gcpos = grandchild.attrib.get('pos', '0 0 0')
-          gcquat = grandchild.attrib.get('quat', '1 0 0 0')
-          gcpos = np.fromstring(gcpos, sep=' ')
-          gcquat = np.fromstring(gcquat, sep=' ')
-          gcpos, gcquat = _transform_do(cpos, cquat, gcpos, gcquat)
-          gcpos = ' '.join('%f' % i for i in gcpos)
-          gcquat = ' '.join('%f' % i for i in gcquat)
-          grandchild.attrib['pos'] = gcpos
-          grandchild.attrib['quat'] = gcquat
-        elem.append(grandchild)
-      elem.remove(child)
     _fuse_bodies(child)
+    # this only applies to bodies with no joints
+    if child.tag != 'body':
+      continue
+    if child.find('joint') is not None or child.find('freejoint') is not None:
+      continue
+    cpos = child.attrib.get('pos', '0 0 0')
+    cpos = np.fromstring(cpos, sep=' ')
+    cquat = child.attrib.get('quat', '1 0 0 0')
+    cquat = np.fromstring(cquat, sep=' ')
+    for grandchild in child:
+      # TODO: might need to offset more than just body, geom
+      if grandchild.tag in ('body', 'geom') and (cpos != 0).any():
+        gcpos = grandchild.attrib.get('pos', '0 0 0')
+        gcquat = grandchild.attrib.get('quat', '1 0 0 0')
+        gcpos = np.fromstring(gcpos, sep=' ')
+        gcquat = np.fromstring(gcquat, sep=' ')
+        gcpos, gcquat = _transform_do(cpos, cquat, gcpos, gcquat)
+        gcpos = ' '.join('%f' % i for i in gcpos)
+        gcquat = ' '.join('%f' % i for i in gcquat)
+        grandchild.attrib['pos'] = gcpos
+        grandchild.attrib['quat'] = gcquat
+      elem.append(grandchild)
+    elem.remove(child)
 
 
 def _get_meshdir(elem: ElementTree.Element) -> Union[str, None]:
   """Gets the mesh directory specified by the mujoco compiler tag."""
-  elem = elem.find('./mujoco/compiler')
-  return elem.get('meshdir') if elem is not None else None
+  elems = list(elem.iter('compiler'))
+  return elems[0].get('meshdir') if elems else None
 
 
 def _find_assets(
     elem: ElementTree.Element,
-    path: Union[str, epath.Path],
-    meshdir: Union[str, None] = None,
+    path: epath.Path,
+    meshdir: Optional[str],
 ) -> Dict[str, bytes]:
   """Loads assets from an xml given a base path."""
   assets = {}
-  path = epath.Path(path)
-  meshdir = meshdir or _get_meshdir(elem)
+  path = path if path.is_dir() else path.parent
   fname = elem.attrib.get('file') or elem.attrib.get('filename')
-  if fname:
-    dirname = path if path.is_dir() else path.parent
-    assets[fname] = (dirname / (meshdir or '') / fname).read_bytes()
+  if fname and fname.endswith('.xml'):
+    # an asset can be another xml!  if so, we must traverse it, too
+    asset = (path / fname).read_text()
+    asset_xml = ElementTree.fromstring(asset)
+    _fuse_bodies(asset_xml)
+    asset_meshdir = _get_meshdir(asset_xml)
+    assets[fname] = ElementTree.tostring(asset_xml)
+    assets.update(_find_assets(asset_xml, path, asset_meshdir))
+  elif fname:
+    # mesh, png, etc
+    path = path / meshdir if meshdir else path
+    assets[fname] = (path / fname).read_bytes()
 
   for child in list(elem):
     assets.update(_find_assets(child, path, meshdir))
 
   return assets
 
 
@@ -159,15 +157,15 @@
       'baumgarte_erp': (0.1, None),
       'spring_mass_scale': (0.0, None),
       'spring_inertia_scale': (0.0, None),
       'joint_scale_pos': (0.5, None),
       'joint_scale_ang': (0.2, None),
       'collide_scale': (1.0, None),
       'matrix_inv_iterations': (10, None),
-      'solver_maxls': (5, None),
+      'solver_maxls': (20, None),
       'elasticity': (0.0, 'geom'),
       'convex': (True, 'geom'),
       'constraint_stiffness': (2000.0, 'body'),
       'constraint_limit_stiffness': (1000.0, 'body'),
       'constraint_ang_damping': (0.0, 'body'),
       'constraint_vel_damping': (0.0, 'body'),
   }
@@ -235,30 +233,39 @@
 
 
 def load_model(mj: mujoco.MjModel) -> System:
   """Creates a brax system from a MuJoCo model."""
   # do some validation up front
   if any(i not in [0, 1] for i in mj.actuator_biastype):
     raise NotImplementedError('Only actuator_biastype in [0, 1] are supported.')
+  if any(i != 0 for i in mj.actuator_gaintype):
+    raise NotImplementedError('Only actuator_gaintype in [0] is supported.')
   if mj.opt.integrator != 0:
     raise NotImplementedError('Only euler integration is supported.')
   if mj.opt.cone != 0:
     raise NotImplementedError('Only pyramidal cone friction is supported.')
   if not (mj.actuator_trntype == 0).all():
     raise NotImplementedError(
         'Only joint transmission types are supported for actuators.'
     )
+  if (mj.geom_solmix[0] != mj.geom_solmix).any():
+    raise NotImplementedError('geom_solmix parameter not supported.')
+  if (mj.geom_priority[0] != mj.geom_priority).any():
+    raise NotImplementedError('geom_priority parameter not supported.')
   if mj.opt.collision == 1:
     raise NotImplementedError('Predefined collisions not supported.')
   q_width = {0: 7, 1: 4, 2: 1, 3: 1}
   non_free = np.concatenate([[j != 0] * q_width[j] for j in mj.jnt_type])
   if mj.qpos0[non_free].any():
     raise NotImplementedError(
         'The `ref` attribute on joint types is not supported.')
-
+  if (mj.geom_fluid != 0).any():
+    raise NotImplementedError('Ellipsoid fluid model not implemented.')
+  if mj.opt.wind.any():
+    raise NotImplementedError('option.wind is not implemented.')
   custom = _get_custom(mj)
 
   # create links
   joint_positions = [np.array([0.0, 0.0, 0.0])]
   for _, group in itertools.groupby(
       zip(mj.jnt_bodyid, mj.jnt_pos), key=lambda x: x[0]
   ):
@@ -318,47 +325,59 @@
     stiffnesses.append(stiffness)
   motion = jax.tree_map(lambda *x: np.concatenate(x), *motions)
 
   limit = None
   if np.any(mj.jnt_limited):
     limit = jax.tree_map(lambda *x: np.concatenate(x), *limits)
   stiffness = np.concatenate(stiffnesses)
+  solver_params_jnt = np.concatenate((mj.jnt_solref, mj.jnt_solimp), axis=1)
+  solver_params_dof = solver_params_jnt[mj.dof_jntid]
 
-  dof = DoF(  # pytype: disable=wrong-arg-types  # jax-ndarray
+  dof = DoF(  # pytype: disable=wrong-arg-types
       motion=motion,
       armature=mj.dof_armature,
       stiffness=stiffness,
       damping=mj.dof_damping,
       limit=limit,
       invweight=mj.dof_invweight0,
+      solver_params=solver_params_dof,
   )
 
+  solver_params_geom = np.concatenate((mj.geom_solref, mj.geom_solimp), axis=1)
   # group geoms so that they can be stacked.  two geoms can be stacked if:
   # - they have the same type
   # - their fields have the same shape (e.g. Mesh verts might vary)
   # - they have the same mask
   key_fn = lambda g, m: (jax.tree_map(np.shape, g), m)
-
   geom_groups = {}
   for i, typ in enumerate(mj.geom_type):
     rgba = mj.geom_rgba[i]
     if (mj.geom_rgba[i] == [0.5, 0.5, 0.5, 1.0]).all():
       # convert the default mjcf color to brax default color
       rgba = np.array([0.4, 0.33, 0.26, 1.0])
     kwargs = {
         'link_idx': mj.geom_bodyid[i] - 1 if mj.geom_bodyid[i] > 0 else None,
         'transform': Transform(pos=mj.geom_pos[i], rot=mj.geom_quat[i]),
         'friction': mj.geom_friction[i, 0],
         'elasticity': custom['elasticity'][i],
+        'solver_params': solver_params_geom[i],
         'rgba': rgba,
     }
     mask = mj.geom_contype[i] | mj.geom_conaffinity[i] << 32
     if typ == 0:  # Plane
       geom = Plane(**kwargs)
       geom_groups.setdefault(key_fn(geom, mask), []).append(geom)
+    elif typ == 5:  # Cylinder
+      radius, halflength = mj.geom_size[i, 0:2]
+      if halflength > 0.001 and mask > 0:
+        # TODO: support cylinders with depth.
+        raise NotImplementedError(
+            'Cylinders of half-length>0.001 are not supported for collision.')
+      geom = Cylinder(radius=radius, length=halflength * 2, **kwargs)
+      geom_groups.setdefault(key_fn(geom, mask), []).append(geom)
     elif typ == 2:  # Sphere
       geom = Sphere(radius=mj.geom_size[i, 0], **kwargs)
       geom_groups.setdefault(key_fn(geom, mask), []).append(geom)
     elif typ == 3:  # Capsule
       radius, halflength = mj.geom_size[i, 0:2]
       geom = Capsule(radius=radius, length=halflength * 2, **kwargs)
       geom_groups.setdefault(key_fn(geom, mask), []).append(geom)
@@ -378,38 +397,40 @@
         geom = geom_mesh.convex_hull(geom)
       geom_groups.setdefault(key_fn(geom, mask), []).append(geom)
     else:
       warnings.warn(f'unrecognized collider, geom_type: {typ}')
       continue
 
   geoms = [
-      jax.tree_map(lambda *x: jp.stack(x), *g) for g in geom_groups.values()
+      jax.tree_map(lambda *x: np.stack(x), *g) for g in geom_groups.values()
   ]
   geom_masks = [m for _, m in geom_groups.keys()]
 
   # create actuators
   ctrl_range = mj.actuator_ctrlrange
   ctrl_range[~(mj.actuator_ctrllimited == 1), :] = np.array([-np.inf, np.inf])
-  actuator = Actuator(  # pytype: disable=wrong-arg-types  # jax-ndarray
+  force_range = mj.actuator_forcerange
+  force_range[~(mj.actuator_forcelimited == 1), :] = np.array([-np.inf, np.inf])
+  q_id = np.array([mj.jnt_qposadr[i] for i in mj.actuator_trnid[:, 0]])
+  qd_id = np.array([mj.jnt_dofadr[i] for i in mj.actuator_trnid[:, 0]])
+  bias_q = mj.actuator_biasprm[:, 1] * (mj.actuator_biastype != 0)
+  bias_qd = mj.actuator_biasprm[:, 2] * (mj.actuator_biastype != 0)
+
+  # TODO: might be nice to add actuator names for debugging
+  actuator = Actuator(  # pytype: disable=wrong-arg-types
+      q_id=q_id,
+      qd_id=qd_id,
+      gain=mj.actuator_gainprm[:, 0],
       gear=mj.actuator_gear[:, 0],
       ctrl_range=ctrl_range,
+      force_range=force_range,
+      bias_q=bias_q,
+      bias_qd=bias_qd,
   )
 
-  # create generalized solver params
-  params_joint = jp.concatenate((mj.jnt_solref, mj.jnt_solimp), axis=1)
-  params_geom = jp.concatenate((mj.geom_solref, mj.geom_solimp), axis=1)
-  params_pair = jp.concatenate((mj.pair_solref, mj.pair_solimp), axis=1)
-  params_contact = jp.concatenate((params_geom, params_pair))
-  if (params_joint[0] != params_joint).any():
-    raise NotImplementedError('brax only supports one joint solver params')
-  if (params_contact[0] != params_contact).any():
-    raise NotImplementedError('brax only supports one contact solver params')
-  solver_params_joint = params_joint[0]
-  solver_params_contact = params_contact[0]
-
   # create non-pytree params.  these do not live on device directly, and they
   # cannot be differentiated, but they do change the emitted control flow
   link_names = [_get_name(mj, i) for i in mj.name_bodyadr[1:]]
   # convert stacked joints to 1, 2, or 3
   link_types = ''
   for _, group in itertools.groupby(
       zip(mj.jnt_bodyid, mj.jnt_type), key=lambda x: x[0]
@@ -422,61 +443,43 @@
     elif 1 in typs:
       raise NotImplementedError('ball joints not supported')
     else:
       typ = str(len(typs))
     link_types += typ
   link_parents = tuple(mj.body_parentid - 1)[1:]
 
-  # create non-pytree params for actuators.
-  actuator_types = ''.join([_ACT_TYPE_STR[bt] for bt in mj.actuator_biastype])
-  actuator_link_id = [mj.jnt_bodyid[i] - 1 for i in mj.actuator_trnid[:, 0]]
-  unsupported_act_links = set(link_types[i] for i in actuator_link_id) - {
-      '1',
-      '2',
-      '3',
-  }
-  if unsupported_act_links:
-    raise NotImplementedError(
-        f'Link types {unsupported_act_links} are not supported for actuators.'
-    )
-  actuator_qid = [mj.jnt_qposadr[i] for i in mj.actuator_trnid[:, 0]]
-  actuator_qdid = [mj.jnt_dofadr[i] for i in mj.actuator_trnid[:, 0]]
-
   # mujoco stores free q in world frame, so clear link transform for free links
   if 'f' in link_types:
     free_idx = np.array([i for i, typ in enumerate(link_types) if typ == 'f'])
     link.transform.pos[free_idx] = np.zeros(3)
     link.transform.rot[free_idx] = np.array([1.0, 0.0, 0.0, 0.0])
 
   sys = System(  # pytype: disable=wrong-arg-types  # jax-ndarray
       dt=mj.opt.timestep,
       gravity=mj.opt.gravity,
+      viscosity=mj.opt.viscosity,
+      density=mj.opt.density,
       link=link,
       dof=dof,
       geoms=geoms,
       actuator=actuator,
       init_q=custom['init_qpos'] if 'init_qpos' in custom else mj.qpos0,
-      solver_params_joint=solver_params_joint,
-      solver_params_contact=solver_params_contact,
       vel_damping=custom['vel_damping'],
       ang_damping=custom['ang_damping'],
       baumgarte_erp=custom['baumgarte_erp'],
       spring_mass_scale=custom['spring_mass_scale'],
       spring_inertia_scale=custom['spring_inertia_scale'],
       joint_scale_ang=custom['joint_scale_ang'],
       joint_scale_pos=custom['joint_scale_pos'],
       collide_scale=custom['collide_scale'],
+      enable_fluid=(mj.opt.viscosity > 0) | (mj.opt.density > 0),
       geom_masks=geom_masks,
       link_names=link_names,
       link_types=link_types,
       link_parents=link_parents,
-      actuator_types=actuator_types,
-      actuator_link_id=actuator_link_id,
-      actuator_qid=actuator_qid,
-      actuator_qdid=actuator_qdid,
       matrix_inv_iterations=int(custom['matrix_inv_iterations']),
       solver_iterations=mj.opt.iterations,
       solver_maxls=int(custom['solver_maxls']),
   )
 
   sys = jax.tree_map(jp.array, sys)
 
@@ -490,23 +493,28 @@
   return ElementTree.tostring(xml, encoding='unicode')
 
 
 def loads(xml: str, asset_path: Union[str, epath.Path, None] = None) -> System:
   """Loads a brax system from a MuJoCo mjcf xml string."""
   elem = ElementTree.fromstring(xml)
   _fuse_bodies(elem)
-  assets = {} if asset_path is None else _find_assets(elem, asset_path)
+  assets = {}
+  if asset_path is not None:
+    meshdir = _get_meshdir(elem)
+    asset_path = epath.Path(asset_path)
+    assets = _find_assets(elem, asset_path, meshdir)
   xml = ElementTree.tostring(elem, encoding='unicode')
   mj = mujoco.MjModel.from_xml_string(xml, assets=assets)
 
   return load_model(mj)
 
 
 def load(path: Union[str, epath.Path]):
   """Loads a brax system from a MuJoCo mjcf file path."""
   elem = ElementTree.fromstring(epath.Path(path).read_text())
   _fuse_bodies(elem)
-  assets = _find_assets(elem, path)
+  meshdir = _get_meshdir(elem)
+  assets = _find_assets(elem, epath.Path(path), meshdir)
   xml = ElementTree.tostring(elem, encoding='unicode')
   mj = mujoco.MjModel.from_xml_string(xml, assets=assets)
 
   return load_model(mj)
```

### Comparing `brax-0.9.0/brax/io/mjcf_test.py` & `brax-0.9.1/brax/io/mjcf_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -167,10 +167,38 @@
         sys.geoms[1].transform.rot, np.array([[r, 0.0, r, 0.0]]), 5
     )
     # child body is transformed wrt world body
     assert_almost_equal(
         sys.init_q, np.array([1.245, 0.0, 0.0, 0.5, 0.5, 0.5, -0.5])
     )
 
+  def test_load_flat_cylinder(self):
+    sys = test_utils.load_fixture('flat_cylinder.xml')
+    self.assertEqual(sys.geoms[1].radius, 0.25)
+    self.assertEqual(sys.geoms[1].length, 0.002)
+
+  def test_load_fat_cylinder(self):
+    with self.assertRaisesRegex(
+        NotImplementedError, 'Cylinders of half-length'
+    ):
+      test_utils.load_fixture('fat_cylinder.xml')
+
+  def test_load_fluid_box(self):
+    sys = test_utils.load_fixture('fluid_box.xml')
+    assert_almost_equal(sys.density, 1.2)
+    assert_almost_equal(sys.viscosity, 0.15)
+
+  def test_load_fluid_ellipsoid(self):
+    with self.assertRaisesRegex(
+        NotImplementedError, 'Ellipsoid fluid model not implemented'
+    ):
+      test_utils.load_fixture('fluid_ellipsoid.xml')
+
+  def test_load_wind(self):
+    with self.assertRaisesRegex(
+        NotImplementedError, 'option.wind is not implemented'
+    ):
+      test_utils.load_fixture('fluid_wind.xml')
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `brax-0.9.0/brax/io/model.py` & `brax-0.9.1/brax/io/model.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/kinematics.py` & `brax-0.9.1/brax/kinematics.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,15 @@
       j_stack, jd_stack = j.reshape(s), jd.reshape(s)
 
       # accumulate j and jd one dof at a time
       j, jd = j_stack.take(0, axis=1), jd_stack.take(0, axis=1)
       for i in range(1, num_dofs):
         j_i, jd_i = j_stack.take(i, axis=1), jd_stack.take(i, axis=1)
         j = j.vmap().do(j_i)
+        # TODO: fix qd->jd calculation for stacked/offset joints
         jd = jd + Motion(
             ang=jax.vmap(math.rotate)(jd_i.ang, j_i.rot),
             vel=jax.vmap(math.rotate)(
                 jd_i.vel + jax.vmap(jp.cross)(j_i.pos, jd_i.ang), j_i.rot
             ),
         )
 
@@ -84,24 +85,24 @@
   anchor = Transform.create(rot=j.rot).vmap().do(sys.link.joint)
   j = j.replace(pos=j.pos + sys.link.joint.pos - anchor.pos)  # joint pos offset
   j = sys.link.transform.vmap().do(j)  # link transform
 
   def world(parent, j, jd):
     """Convert transform/motion from joint frame to world frame."""
     if parent is None:
+      jd = jd.replace(ang=jax.vmap(math.rotate)(jd.ang, j.rot))
       return j, jd
-    x, xd = parent
-    # TODO: determine why the motion `do` is inverted
-    x = x.vmap().do(j)
-    xd = xd + Motion(
-        ang=jax.vmap(math.rotate)(jd.ang, x.rot),
-        vel=jax.vmap(math.rotate)(
-            jd.vel + jax.vmap(jp.cross)(x.pos, jd.ang), x.rot
-        ),
-    )
+    x_p, xd_p = parent
+    x = x_p.vmap().do(j)
+    # get the linear velocity at the tip of the parent
+    vel = xd_p.vel + jax.vmap(jp.cross)(xd_p.ang, x.pos - x_p.pos)
+    # add in the child linear velocity in the world frame
+    vel += jax.vmap(math.rotate)(jd.vel, x_p.rot)
+    ang = xd_p.ang + jax.vmap(math.rotate)(jd.ang, x.rot)
+    xd = Motion(vel=vel, ang=ang)
     return x, xd
 
   x, xd = scan.tree(sys, world, 'll', j, jd)
 
   x = x.replace(rot=jax.vmap(math.normalize)(x.rot)[0])
 
   return x, xd
@@ -122,15 +123,15 @@
   j = a_c.vmap().to_local(a_p)
 
   # find world velocity of joint location point on parent
   xd_wj = Transform.create(pos=x_p.pos - a_p.pos).vmap().do(xd_p)
 
   # move into joint coordinates
   xd_joint = xd - xd_wj
-  inv_rotate = jax.vmap(lambda x, y: math.rotate(x, math.quat_inv(y)))
+  inv_rotate = jax.vmap(math.inv_rotate)
   jd = jax.tree_map(lambda x: inv_rotate(x, a_p.rot), xd_joint)
 
   return j, jd, a_p, a_c
 
 
 def link_to_joint_frame(motion: Motion) -> Tuple[Motion, float]:
   """Calculates 3-dof frames for joints corresponding to a given link motion.
@@ -154,14 +155,17 @@
   Combined, these two rotations move the identity link-frame into the joint
   frame, where the new local-x and local-y point along the directions specified
   in the system dof.
 
   We also need translational components because the prismatic components of a
   joint might not be aligned with the rotational components of the joint.
   """
+  if motion.ang.shape[0] > 3 or motion.ang.shape[0] == 0:
+    raise AssertionError('Motion shape must be in (0, 3], '
+                         f'got {motion.ang.shape[0]}')
 
   # 1-dof
   if motion.ang.shape[0] == 1:
     ortho_ang = math.orthogonals(motion.ang[0])
     ang_frame = jp.array([motion.ang[0], ortho_ang[0], ortho_ang[1]])
     ang_frame = jp.where(motion.ang[0].any(), ang_frame, jp.eye(3))
     ortho_vel = math.orthogonals(motion.vel[0])
@@ -278,24 +282,22 @@
     Joint frame axis, angles, and auxiliary axes
   """
 
   v_rot = jax.vmap(math.rotate, in_axes=[0, None])
   child_frame = v_rot(joint_motion.ang, j.rot)
 
   line_of_nodes = jp.cross(child_frame[2], joint_motion.ang[0])
-  line_of_nodes = line_of_nodes / (1e-10 + math.safe_norm(line_of_nodes))
+  line_of_nodes, _ = math.normalize(line_of_nodes)
   y_n_normal = joint_motion.ang[0]
   psi = math.signed_angle(y_n_normal, joint_motion.ang[1], line_of_nodes)
   axis_1_p_in_xz_c = (
       jp.dot(joint_motion.ang[0], child_frame[0]) * child_frame[0]
       + jp.dot(joint_motion.ang[0], child_frame[1]) * child_frame[1]
   )
-  axis_1_p_in_xz_c = axis_1_p_in_xz_c / (
-      1e-10 + math.safe_norm(axis_1_p_in_xz_c)
-  )
+  axis_1_p_in_xz_c, _ = math.normalize(axis_1_p_in_xz_c)
   ang_between_1_p_xz_c = jp.dot(axis_1_p_in_xz_c, joint_motion.ang[0])
   theta = math.safe_arccos(jp.clip(ang_between_1_p_xz_c, -1, 1)) * jp.sign(
       jp.dot(joint_motion.ang[0], child_frame[2])
   )
   yc_n_normal = -child_frame[2] * parity
   phi = math.signed_angle(yc_n_normal, child_frame[1], line_of_nodes)
 
@@ -327,18 +329,21 @@
 
 
 def inverse(
     sys: System, j: Transform, jd: Motion
 ) -> Tuple[jp.ndarray, jp.ndarray]:
   """Translates maximal coordinates into reduced coordinates."""
 
-  def free(x, xd, _):
-    return jp.concatenate([x.pos, x.rot]), jp.concatenate([xd.vel, xd.ang])
-
-  def x_dof(j, jd, motion, x):
+  def free(x, xd, *_):
+    ang = math.inv_rotate(xd.ang, x.rot)
+    return jp.concatenate([x.pos, x.rot]), jp.concatenate([xd.vel, ang])
+
+  def x_dof(j, jd, parent_idx, motion, x):
+    j_rot = jp.where(parent_idx == -1, j.rot, jp.array([1.0, 0.0, 0.0, 0.0]))
+    jd = jd.replace(ang=math.inv_rotate(jd.ang, j_rot))
     joint_frame, parity = link_to_joint_frame(motion)
     axis, angles, _ = axis_angle_ang(j, joint_frame, parity)
     angle_vels = jax.tree_map(lambda x: jp.dot(x, jd.ang), axis)
     _, slides, slide_vels = axis_slide_vel(j, jd, motion)
     # TODO: investigate removing this `where`
     q = jp.where(
         motion.ang.any(axis=1), jp.array(angles[:x]), jp.array(slides[:x])
@@ -346,25 +351,27 @@
     qd = jp.where(
         motion.ang.any(axis=1),
         jp.array(angle_vels[:x]),
         jp.array(slide_vels[:x]),
     )
     return q, qd
 
-  def q_fn(typ, j, jd, motion):
+  def q_fn(typ, j, jd, parent_idx, motion):
     motion = jax.tree_map(
         lambda y: y.reshape((-1, base.QD_WIDTHS[typ], 3)), motion
     )
     q_fn_map = {
         'f': free,
         '1': functools.partial(x_dof, x=1),
         '2': functools.partial(x_dof, x=2),
         '3': functools.partial(x_dof, x=3),
     }
 
-    q, qd = jax.vmap(q_fn_map[typ])(j, jd, motion)
+    q, qd = jax.vmap(q_fn_map[typ])(j, jd, parent_idx, motion)
 
     # transposed to preserve order of outputs
     return jp.array(q).reshape(-1), jp.array(qd).reshape(-1)
 
-  q, qd = scan.link_types(sys, q_fn, 'lld', 'qd', j, jd, sys.dof.motion)
+  parent_idx = jp.array(sys.link_parents)
+  q, qd = scan.link_types(sys, q_fn, 'llld', 'qd', j, jd, parent_idx,
+                          sys.dof.motion)
   return q, qd
```

### Comparing `brax-0.9.0/brax/kinematics_test.py` & `brax-0.9.1/brax/kinematics_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,49 +17,71 @@
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from brax import base
 from brax import kinematics
 from brax import scan
 from brax import test_utils
+from brax.base import Motion
 import jax
 import jax.numpy as jp
 import numpy as np
 
 
 class KinematicsTest(parameterized.TestCase):
 
   @parameterized.parameters(
       ('ant.xml',), ('humanoid.xml',), ('reacher.xml',), ('half_cheetah.xml',)
   )
-  def test_forward_q(self, xml_file):
+  def test_forward(self, xml_file):
     """Test dynamics forward q."""
     sys = test_utils.load_fixture(xml_file)
-    for mj_prev, mj_next in test_utils.sample_mujoco_states(xml_file):
-      x, _ = jax.jit(kinematics.forward)(sys, mj_prev.qpos, mj_prev.qvel)
+
+    for mj_prev, mj_next in test_utils.sample_mujoco_states(
+        xml_file, random_init=True, vel_to_local=False):
+      x, xd = jax.jit(kinematics.forward)(sys, mj_prev.qpos, mj_prev.qvel)
+
       np.testing.assert_almost_equal(x.pos, mj_next.xpos[1:], 3)
+      # handle quat rotations +/- 2pi
+      quat_sign = np.allclose(
+          np.sum(mj_next.xquat[1:]) - np.sum(x.rot), 0, atol=1e-2)
+      quat_sign = 1 if quat_sign else -1
+      x = x.replace(rot=x.rot * quat_sign)
       np.testing.assert_almost_equal(x.rot, mj_next.xquat[1:], 3)
 
+      # xd vel/ang were added to linvel/angmom in `sample_mujoco_states`
+      xd_mj = Motion(
+          vel=mj_next.subtree_linvel[1:], ang=mj_next.subtree_angmom[1:])
+
+      if xml_file == 'humanoid.xml':
+        # TODO: get forward to match MJ for stacked/offset joints
+        return
+
+      np.testing.assert_array_almost_equal(xd.ang, xd_mj.ang, 3)
+      np.testing.assert_array_almost_equal(xd.vel, xd_mj.vel, 3)
+
   def test_init_q(self):
     sys = test_utils.load_fixture('ant.xml')
     np.testing.assert_almost_equal(
         sys.init_q,
         np.array([0, 0, 0.55, 1, 0, 0, 0, 0, 1, 0, -1, 0, -1, 0, 1]),
         7,
     )
 
   @parameterized.parameters(
       ('ant.xml',), ('humanoid.xml',), ('reacher.xml',), ('half_cheetah.xml',)
   )
   def test_inverse(self, xml_file):
+    np.random.seed(0)
     sys = test_utils.load_fixture(xml_file)
-    # # test at random init
+    # test at random init
     rand_q = np.random.rand(sys.init_q.shape[0])
-    # normalize quaternion part of init_q
-    rand_q[3:7] = rand_q[3:7] / np.linalg.norm(rand_q[3:7])
+    if sys.link_types[0] == 'f':
+      # normalize quaternion part of init_q
+      rand_q[3:7] = rand_q[3:7] / np.linalg.norm(rand_q[3:7])
     rand_q = jp.array(rand_q)
     rand_qd = jp.array(np.random.rand(sys.qd_size())) * 0.1
 
     x, xd = kinematics.forward(sys, rand_q, rand_qd)
     j, jd, _, _ = kinematics.world_to_joint(sys, x, xd)
     q, qd = kinematics.inverse(sys, j, jd)
     np.testing.assert_array_almost_equal(q, rand_q, decimal=5)
@@ -89,18 +111,19 @@
                     [[0.0, 1.0, 0.0], [0.0, -1.0, 0.0], [0.0, 0.0, 1.0]]
                 ),
                 vel=np.array(
                     [[0.0, 0.0, 0.0], [0.0, 0.0, 0.0], [0.0, 0.0, 0.0]]
                 ),
             ),
             armature=np.array([0.0, 0.0, 0.0, 0.0]),
-            invweight=np.array([0.0, 0.0, 0.0, 0.0]),
             stiffness=np.array([0.0, 0.0, 0.0, 0.0]),
             damping=np.array([0.0, 0.0, 0.0, 0.0]),
             limit=None,
+            invweight=np.array([0.0, 0.0, 0.0, 0.0]),
+            solver_params=np.zeros((4, 7)),
         )
     )
 
     joint_motion = scan.link_types(
         sys, _collect_frame, 'd', 'l', sys.dof.motion
     )
     # joint x-axes should correspond to dof angular degrees of freedom
@@ -124,18 +147,19 @@
                     [0.0, 0.0, 0.0],
                     [0.0, 0.0, 0.0],
                     [0.0, 0.0, 0.0],
                     [0.0, 0.0, 0.0],
                 ]),
             ),
             armature=np.array([0.0, 0.0, 0.0, 0.0]),
-            invweight=np.array([0.0, 0.0, 0.0, 0.0]),
             stiffness=np.array([0.0, 0.0, 0.0, 0.0]),
             damping=np.array([0.0, 0.0, 0.0, 0.0]),
             limit=None,
+            invweight=np.array([0.0, 0.0, 0.0, 0.0]),
+            solver_params=np.zeros((4, 7)),
         )
     )
 
     joint_motion = scan.link_types(
         sys, _collect_frame, 'd', 'l', sys.dof.motion
     )
     # check universal joint axes
```

### Comparing `brax-0.9.0/brax/math.py` & `brax-0.9.1/brax/math.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,27 @@
     raise ValueError('vec must have no batch dimensions.')
   s, u = quat[0], quat[1:]
   r = 2 * (jp.dot(u, vec) * u) + (s * s - jp.dot(u, u)) * vec
   r = r + 2 * s * jp.cross(u, vec)
   return r
 
 
+def inv_rotate(vec: jp.ndarray, quat: jp.ndarray):
+  """Rotates a vector vec by an inverted unit quaternion quat.
+
+  Args:
+    vec: (3,) a vector
+    quat: (4,) a quaternion
+
+  Returns:
+    ndarray(3) containing vec rotated by the inverse of quat.
+  """
+  return rotate(vec, quat_inv(quat))
+
+
 def rotate_np(vec: np.ndarray, quat: np.ndarray):
   """Rotates a vector vec by a unit quaternion quat.
 
   Args:
     vec: (3,) a vector
     quat: (4,) a quaternion
```

### Comparing `brax-0.9.0/brax/math_test.py` & `brax-0.9.1/brax/math_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/positional/__init__.py` & `brax-0.9.1/brax/io/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/positional/base.py` & `brax-0.9.1/brax/spring/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,33 +9,37 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint:disable=g-multiple-import
-"""Base types for positional pipeline."""
+"""Base types for spring pipeline."""
 
 from brax import base
 from brax.base import Motion, Transform
 from flax import struct
+from jax import numpy as jp
 
 
 @struct.dataclass
 class State(base.State):
   """Dynamic state that changes after every step.
 
   Attributes:
-    x_i: link center of mass in world frame
-    xd_i: link center of mass motion in world frame
+    x_i: (num_links,) link center of mass position in world frame
+    xd_i: (num_links,) link center of mass velocity in world frame
     j: link position in joint frame
     jd: link motion in joint frame
     a_p: joint parent anchor in world frame
     a_c: joint child anchor in world frame
+    i_inv: link inverse inertia
+    mass: link mass
   """
-
   x_i: Transform
   xd_i: Motion
   j: Transform
   jd: Motion
   a_p: Transform
   a_c: Transform
+  i_inv: jp.ndarray
+  mass: jp.ndarray
```

### Comparing `brax-0.9.0/brax/positional/collisions.py` & `brax-0.9.1/brax/positional/collisions.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/positional/integrator.py` & `brax-0.9.1/brax/positional/integrator.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/positional/joints.py` & `brax-0.9.1/brax/positional/joints.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 from brax.base import DoF, Force, Link, Motion, System, Transform
 from brax.positional.base import State
 import jax
 from jax import numpy as jp
 from jax.ops import segment_sum
 
 
-def acceleration_update(sys: System, state: State, tau: jp.ndarray) -> Motion:
+def acceleration_update(sys: System, state: State, tau: jp.ndarray) -> Force:
   """Calculates forces to apply to links resulting from joint constraints.
 
   Args:
     sys: System defining kinematic tree of joints
     state: positional pipeline state
     tau: joint force vector
 
   Returns:
-    xdd_i: acceleration to apply to link center of mass in world frame
+    xf_i: force to apply to link center of mass in world frame
   """
 
   def _free_joint(*_) -> Force:
     return Force(vel=jp.zeros(3), ang=jp.zeros(3))
 
   def _damp(link: Link, jd: Motion, dof: DoF, tau: jp.ndarray):
     vel = jp.sum(jax.vmap(jp.multiply)(tau, dof.motion.vel), axis=0)
@@ -73,24 +73,15 @@
   fc = Transform.create(pos=state.a_c.pos - state.x_i.pos).vmap().do(xf)
   # also add opposite force to parent link at center of mass
   parent_idx = jp.array(sys.link_parents)
   x_i_parent = state.x_i.take(parent_idx)
   fp = Transform.create(pos=state.a_p.pos - x_i_parent.pos).vmap().do(xf)
   fp = jax.tree_map(lambda x: segment_sum(x, parent_idx, sys.num_links()), fp)
   xf_i = fc - fp
-
-  # convert to acceleration
-  inv_mass = 1 / (sys.link.inertia.mass ** (1 - sys.spring_mass_scale))
-  inv_inertia = com.inv_inertia(sys, state.x)
-  xdd_i = Motion(
-      ang=jax.vmap(lambda x, y: x @ y)(inv_inertia, xf_i.ang),
-      vel=jax.vmap(lambda x, y: x * y)(inv_mass, xf_i.vel),
-  )
-
-  return xdd_i
+  return xf_i
 
 
 def position_update(sys: System, state: State) -> Transform:
   """Calculates position-level joint updates in CoM coordinates for joints.
 
   Args:
     sys: System defining kinematic tree of joints
```

### Comparing `brax-0.9.0/brax/positional/joints_test.py` & `brax-0.9.1/brax/positional/joints_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/positional/perf_test.py` & `brax-0.9.1/brax/positional/perf_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,14 @@
     def init_fn(rng):
       rng1, rng2 = jax.random.split(rng, 2)
       q = jax.random.uniform(rng1, (sys.q_size(),), minval=-0.1, maxval=0.1)
       qd = 0.1 * jax.random.normal(rng2, (sys.qd_size(),))
       return pipeline.init(sys, q, qd)
 
     def step_fn(state):
-      return pipeline.step(sys, state, jp.zeros(sys.qd_size()))
+      return pipeline.step(sys, state, jp.zeros(sys.act_size()))
 
     test_utils.benchmark('pbd pipeline ant', init_fn, step_fn)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `brax-0.9.0/brax/positional/pipeline.py` & `brax-0.9.1/brax/positional/pipeline.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Physics pipeline for fully articulated dynamics and collisiion."""
 # pylint:disable=g-multiple-import
 from brax import actuator
 from brax import com
+from brax import fluid
 from brax import geometry
 from brax import kinematics
 from brax.base import Motion, System
 from brax.positional import collisions
 from brax.positional import integrator
 from brax.positional import joints
 from brax.positional.base import State
+import jax
 from jax import numpy as jp
 
 
 def init(
     sys: System, q: jp.ndarray, qd: jp.ndarray, debug: bool = False
 ) -> State:
   """Initializes physics state.
@@ -41,16 +43,16 @@
     state: initial physics state
   """
   # position/velocity level terms
   x, xd = kinematics.forward(sys, q, qd)
   j, jd, a_p, a_c = kinematics.world_to_joint(sys, x, xd)
   x_i, xd_i = com.from_world(sys, x, xd)
   contact = geometry.contact(sys, x) if debug else None
-
-  return State(q, qd, x, xd, contact, x_i, xd_i, j, jd, a_p, a_c)
+  mass = sys.link.inertia.mass ** (1 - sys.spring_mass_scale)
+  return State(q, qd, x, xd, contact, x_i, xd_i, j, jd, a_p, a_c, mass)
 
 
 def step(
     sys: System, state: State, act: jp.ndarray, debug: bool = False
 ) -> State:
   """Performs a single physics step using position-based dynamics.
 
@@ -66,17 +68,25 @@
   Returns:
     x: updated link transform in world frame
     xd: updated link motion in world frame
   """
   x_i_prev = state.x_i
 
   # calculate acceleration level updates
-  tau = actuator.to_tau(sys, act, state.q)
+  tau = actuator.to_tau(sys, act, state.q, state.qd)
   xdd_i = Motion.create(vel=sys.gravity)
-  xdd_i += joints.acceleration_update(sys, state, tau)
+  # get joint constraint forces
+  xf_i = joints.acceleration_update(sys, state, tau)
+  if sys.enable_fluid:
+    inertia = sys.link.inertia.i ** (1 - sys.spring_inertia_scale)
+    xf_i += fluid.force(sys, state.x, state.xd, state.mass, inertia)
+  xdd_i += Motion(
+      ang=jax.vmap(lambda x, y: x @ y)(com.inv_inertia(sys, state.x), xf_i.ang),
+      vel=jax.vmap(lambda x, y: x * y)(1 / state.mass, xf_i.vel),
+  )
 
   # semi-implicit euler: apply acceleration update before resolving collisions
   x_i, xd_i = integrator.integrate_xdd(sys, state.x_i, state.xd_i, xdd_i)
   x, xd = com.to_world(sys, x_i, xd_i)
   state = state.replace(x=x, xd=xd, x_i=x_i, xd_i=xd_i)
 
   # perform position level joint updates
@@ -98,9 +108,8 @@
   xd_i = integrator.integrate_xdv(sys, xd_i, xdv_i)
 
   x, xd = com.to_world(sys, x_i, xd_i)
   j, jd, a_p, a_c = kinematics.world_to_joint(sys, x, xd)
   q, qd = kinematics.inverse(sys, j, jd)
   contact = geometry.contact(sys, x) if debug else None
 
-  return State(q, qd, x, xd, contact, x_i, xd_i, j, jd, a_p, a_c)
-
+  return State(q, qd, x, xd, contact, x_i, xd_i, j, jd, a_p, a_c, state.mass)
```

### Comparing `brax-0.9.0/brax/positional/pipeline_test.py` & `brax-0.9.1/brax/positional/pipeline_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint:disable=g-multiple-import
 """Tests for spring physics pipeline."""
 
 from absl.testing import absltest
+from brax import com
 from brax import kinematics
 from brax import test_utils
+from brax.base import Transform
 from brax.generalized import pipeline as g_pipeline
 from brax.positional import pipeline
 import jax
 from jax import numpy as jp
 import numpy as np
 
 
@@ -32,24 +34,24 @@
     sys = sys.replace(dt=0.0005)
     sys = sys.replace(
         link=sys.link.replace(constraint_vel_damping=jp.zeros(sys.num_links()))
     )
     state = pipeline.init(sys, sys.init_q, jp.zeros(sys.qd_size()))
     j_pos_step = jax.jit(pipeline.step)
     for _ in range(2_000):
-      state = j_pos_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_pos_step(sys, state, jp.zeros(sys.act_size()))
     x = state.x
 
     # compare against generalized step
     q, qd = jp.zeros(sys.q_size()), jp.zeros(sys.qd_size())
     state = g_pipeline.init(sys, q, qd)
     j_g_step = jax.jit(g_pipeline.step)
     j_forward = jax.jit(kinematics.forward)
     for _ in range(2_000):
-      state = j_g_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_g_step(sys, state, jp.zeros(sys.act_size()))
     x_g, _ = j_forward(sys, state.q, state.qd)
 
     # trajectories should be close after .1 second of simulation
     self.assertLess(jp.linalg.norm(x_g.pos - x.pos), 2e-2)
 
   def test_spherical_pendulum(self):
     sys = test_utils.load_fixture('single_spherical_pendulum.xml')
@@ -62,26 +64,33 @@
     link = link.replace(constraint_ang_damping=jp.array([0.0] * 3))
     sys = sys.replace(link=link)
     sys = sys.replace(ang_damping=0.0)
     sys = sys.replace(dt=0.001)
     sys = sys.replace(solver_iterations=500)
 
     state = pipeline.init(sys, init_q, init_qd)
+    # the qd calculation for pbd/spring doesn't match generalized, so we get xd
+    # from generalized and plug it back into pbd
+    # TODO: remove this xd override once kinematics.forward is fixed
+    state_g = g_pipeline.init(sys, init_q, init_qd)
+    off = state_g.x.pos - state_g.root_com
+    xd = Transform.create(pos=off).vmap().do(state_g.cd)
+    state = state.replace(xd=xd, xd_i=com.from_world(sys, state.x, xd)[1])
+
     j_pos_step = jax.jit(pipeline.step)
     for _ in range(1000):
-      state = j_pos_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_pos_step(sys, state, jp.zeros(sys.act_size()))
     x = state.x
 
     # compare against generalized step
-    q, qd = init_q, init_qd
-    state = g_pipeline.init(sys, q, qd)
     j_g_step = jax.jit(g_pipeline.step)
     j_forward = jax.jit(kinematics.forward)
+    state = state_g
     for _ in range(1000):
-      state = j_g_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_g_step(sys, state, jp.zeros(sys.act_size()))
     x_g, _ = j_forward(sys, state.q, state.qd)
 
     # trajectories should be close after 1 second of simulation
     self.assertLess(jp.linalg.norm(x_g.rot - x.rot), 1e-2)
 
   def test_3d_sliding_joint(self):
     # tests launching a capsule at a wall with 3 sliding dofs
@@ -93,15 +102,15 @@
     qd = qd.at[1].set(2.5)
     qd = qd.at[2].set(2.5)
 
     state = pipeline.init(sys, sys.init_q, qd)
     j_pos_step = jax.jit(pipeline.step)
     states = []
     for _ in range(1000):
-      state = j_pos_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_pos_step(sys, state, jp.zeros(sys.act_size()))
       states.append(state)
     x, xd = state.x, state.xd
 
     # capsule not rotating
     np.testing.assert_allclose(
         x.rot, jp.array([[1.0, 0.0, 0.0, 0.0]]), atol=1e-3
     )
@@ -120,15 +129,15 @@
     qd = qd.at[1].set(2.5)
     qd = qd.at[2].set(2.5)
 
     state = pipeline.init(sys, sys.init_q, qd)
     j_pos_step = jax.jit(pipeline.step)
     states = []
     for _ in range(1000):
-      state = j_pos_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_pos_step(sys, state, jp.zeros(sys.act_size()))
       states.append(state)
 
     # reflects off limits and is still traveling close to 2.5 m/s
     # note that pbd limit reflection not perfectly elastic
     np.testing.assert_array_less(
         jp.array([state.xd.vel[0, 0], state.xd.vel[0, 2]]),
         jp.array([-1.18, -1.18]),
@@ -144,15 +153,15 @@
 
     qd = jp.zeros(sys.qd_size())
     qd = qd.at[0].set(5.0)
 
     state = pipeline.init(sys, sys.init_q, qd)
     j_pos_step = jax.jit(pipeline.step)
     for _ in range(1000):
-      state = j_pos_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_pos_step(sys, state, jp.zeros(sys.act_size()))
     x, xd = state.x, state.xd
 
     # capsule slides to a stop
     self.assertAlmostEqual(x.pos[0, 2], 0.25, delta=1e-2)
     np.testing.assert_allclose(
         x.rot, jp.array([[1.0, 0.0, 0.0, 0.0]]), atol=1e-3
     )
```

### Comparing `brax-0.9.0/brax/scan.py` & `brax-0.9.1/brax/scan.py`

 * *Files 17% similar despite different names*

```diff
@@ -187,60 +187,7 @@
           _take(ys[idxs], [order.index(i) for i in range(len(order))])
       )
     else:
       out_ys.append(ys[idxs])
   y = out_ys[0] if len(out_types) == 1 else out_ys
 
   return y
-
-
-def actuator_types(
-    sys: System, f: Callable[..., Y], in_types: str, out_type: str, *args
-) -> Y:
-  r"""Scan a function over System actuator type ranges.
-
-  Args:
-    sys: system defining the kinematic tree and other properties
-    f: a function to be scanned with the following type signature:\
-        def f(typ, link, q, qd) -> y
-       where
-         ``typ`` is the actuator, link type string
-         ``*args`` are input arguments with types matching ``in_types``
-         ``y`` is an output arguments with types matching ``out_type``
-    in_types: string specifying the type of each input arg:
-        'a' is an input to be split according to act ranges
-        'l' is an input to be split according to link ranges
-        'q' is an input to be split according to q ranges
-        'd' is an input to be split according to qd ranges
-    out_type: string specifying the type of the output
-    *args: the input arguments corresponding to ``in_types``
-
-  Returns:
-    The stacked outputs of ``f`` matching the system actuator order.
-  """
-  typ_order = sorted(set(sys.actuator_types), key=sys.actuator_types.find)
-
-  typ_order_idxs = []
-  for i, t in enumerate(sys.actuator_types):
-    order = typ_order.index(t)
-    while order >= len(typ_order_idxs):
-      typ_order_idxs.append({'a': [], 'l': [], 'q': [], 'd': []})
-    typ_order_idxs[order]['a'].append(i)
-    typ_order_idxs[order]['l'].append(sys.actuator_link_id[i])
-    typ_order_idxs[order]['q'].append(sys.actuator_qid[i])
-    typ_order_idxs[order]['d'].append(sys.actuator_qdid[i])
-
-  ys = []
-  for typ, typ_idxs in zip(typ_order, typ_order_idxs):
-    in_args = [_take(a, typ_idxs[t]) for a, t in zip(args, in_types)]
-    ys.append(f(typ, *in_args))
-
-  y = jax.tree_map(lambda *x: jp.concatenate(x), *ys)
-
-  # we concatenated results out of order, so put back in order if needed
-
-  order = sum([t[out_type] for t in typ_order_idxs], [])
-
-  if order != list(range(len(order))):
-    y = _take(y, [order.index(i) for i in range(len(order))])
-
-  return y
```

### Comparing `brax-0.9.0/brax/scan_test.py` & `brax-0.9.1/brax/scan_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint:disable=g-multiple-import
 """Tests for scan functions."""
 
 from absl.testing import absltest
-from absl.testing import parameterized
 from brax import scan
 from brax import test_utils
 import numpy as np
 
 
 class ScanTest(absltest.TestCase):
 
@@ -151,69 +150,9 @@
     np.testing.assert_array_equal(qs[1], np.arange(7, 15))
 
     self.assertLen(qds, 2)
     np.testing.assert_array_equal(qds[0], np.arange(0, 6))
     np.testing.assert_array_equal(qds[1], np.arange(6, 14))
 
 
-class ParametrizedScanTest(parameterized.TestCase):
-
-  @parameterized.parameters(
-      (
-          'single_spherical_pendulum_position.xml',
-          ['p'],
-          [0, 1, 2],  # act_id
-          [0, 0, 0],  # act_link_id
-          [2, 0, 1],  # q_id
-          [2, 0, 1],  # qd_id
-      ),
-      (
-          'ant.xml',
-          ['m'],
-          list(range(8)),
-          [7, 8, 1, 2, 3, 4, 5, 6],
-          [13, 14, 7, 8, 9, 10, 11, 12],
-          [12, 13, 6, 7, 8, 9, 10, 11],
-      ),
-  )
-  def test_scan_actuator_types(
-      self, fname, act_typs, act_id, act_link_id, q_id, qd_id
-  ):
-    """Test scanning actuators."""
-    sys = test_utils.load_fixture(fname)
-
-    typs, links, qs, qds = [], [], [], []
-
-    def f(typ, act, link, q, qd):
-      typs.append(typ)
-      links.append(link)
-      qs.append(q)
-      qds.append(qd)
-      return act
-
-    out = scan.actuator_types(
-        sys,
-        f,
-        'alqd',
-        'a',
-        np.arange(sys.act_size()),
-        np.arange(sys.num_links()),
-        np.arange(sys.q_size()),
-        np.arange(sys.qd_size()),
-    )
-
-    self.assertSequenceEqual(typs, act_typs)
-    np.testing.assert_array_equal(out, np.array(act_id))
-
-    self.assertLen(links, 1)
-    self.assertSequenceEqual(sys.actuator_link_id, act_link_id)
-    np.testing.assert_array_equal(links[0], np.array(sys.actuator_link_id))
-
-    self.assertLen(qs, 1)
-    np.testing.assert_array_equal(qs[0], np.array(q_id))
-
-    self.assertLen(qds, 1)
-    np.testing.assert_array_equal(qds[0], np.array(qd_id))
-
-
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `brax-0.9.0/brax/spring/__init__.py` & `brax-0.9.1/brax/positional/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/spring/base.py` & `brax-0.9.1/brax/positional/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,37 +9,36 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint:disable=g-multiple-import
-"""Base types for spring pipeline."""
+"""Base types for positional pipeline."""
 
 from brax import base
 from brax.base import Motion, Transform
 from flax import struct
-from jax import numpy as jp
+import jax.numpy as jp
 
 
 @struct.dataclass
 class State(base.State):
   """Dynamic state that changes after every step.
 
   Attributes:
-    x_i: (num_links,) link center of mass position in world frame
-    xd_i: (num_links,) link center of mass velocity in world frame
+    x_i: link center of mass in world frame
+    xd_i: link center of mass motion in world frame
     j: link position in joint frame
     jd: link motion in joint frame
     a_p: joint parent anchor in world frame
     a_c: joint child anchor in world frame
-    i_inv: link inverse inertia
     mass: link mass
   """
+
   x_i: Transform
   xd_i: Motion
   j: Transform
   jd: Motion
   a_p: Transform
   a_c: Transform
-  i_inv: jp.ndarray
   mass: jp.ndarray
```

### Comparing `brax-0.9.0/brax/spring/collisions.py` & `brax-0.9.1/brax/spring/collisions.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/spring/integrator.py` & `brax-0.9.1/brax/spring/integrator.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/spring/joints.py` & `brax-0.9.1/brax/spring/joints.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,24 +305,24 @@
         * jp.sum(jax.vmap(jp.multiply)(vel_axis, dvel), 0)
         * (is_translational)
     )
 
   return Force(ang=ang, vel=vel)
 
 
-def resolve(sys: System, state: State, tau: jp.ndarray) -> Motion:
+def resolve(sys: System, state: State, tau: jp.ndarray) -> Force:
   """Calculates forces to apply to links resulting from joint constraints.
 
   Args:
     sys: System defining kinematic tree of joints
     state: spring pipeline state
     tau: joint force vector
 
   Returns:
-    xdd_i: acceleration to apply to link center of mass in world frame
+    xf_i: force to apply to link center of mass in world frame
   """
 
   def j_fn(typ, link, j, jd, dof, tau):
     # change dof-shape variables into link-shape
     reshape_fn = lambda x: x.reshape((j.pos.shape[0], -1) + x.shape[1:])
     tau, dof = jax.tree_map(reshape_fn, (tau, dof))
     j_fn_map = {
@@ -342,15 +342,8 @@
   fc = Transform.create(pos=state.a_c.pos - state.x_i.pos).vmap().do(xf)
   # also add opposite force to parent link at center of mass
   parent_idx = jp.array(sys.link_parents)
   x_i_parent = state.x_i.take(parent_idx)
   fp = Transform.create(pos=state.a_p.pos - x_i_parent.pos).vmap().do(xf)
   fp = jax.tree_map(lambda x: segment_sum(x, parent_idx, sys.num_links()), fp)
   xf_i = fc - fp
-
-  # convert to acceleration
-  xdd_i = Motion(
-      ang=jax.vmap(lambda x, y: x @ y)(state.i_inv, xf_i.ang),
-      vel=jax.vmap(lambda x, y: x / y)(xf_i.vel, state.mass),
-  )
-
-  return xdd_i
+  return xf_i
```

### Comparing `brax-0.9.0/brax/spring/joints_test.py` & `brax-0.9.1/brax/spring/joints_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/spring/perf_test.py` & `brax-0.9.1/brax/spring/perf_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,14 @@
     def init_fn(rng):
       rng1, rng2 = jax.random.split(rng, 2)
       q = jax.random.uniform(rng1, (sys.q_size(),), minval=-0.1, maxval=0.1)
       qd = 0.1 * jax.random.normal(rng2, (sys.qd_size(),))
       return pipeline.init(sys, q, qd)
 
     def step_fn(state):
-      return pipeline.step(sys, state, jp.zeros(sys.qd_size()))
+      return pipeline.step(sys, state, jp.zeros(sys.act_size()))
 
     test_utils.benchmark('spring pipeline ant', init_fn, step_fn)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `brax-0.9.0/brax/spring/pipeline.py` & `brax-0.9.1/brax/spring/pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,21 +13,23 @@
 # limitations under the License.
 
 # pylint:disable=g-multiple-import
 """Physics pipeline for fully articulated dynamics and collisiion."""
 
 from brax import actuator
 from brax import com
+from brax import fluid
 from brax import geometry
 from brax import kinematics
 from brax.base import Motion, System
 from brax.spring import collisions
 from brax.spring import integrator
 from brax.spring import joints
 from brax.spring.base import State
+import jax
 from jax import numpy as jp
 
 
 def init(
     sys: System, q: jp.ndarray, qd: jp.ndarray, debug: bool = False
 ) -> State:
   """Initializes physics state.
@@ -83,16 +85,25 @@
     x: updated link transform in world frame
     xd: updated link motion in world frame
   """
   # pre-calculate some auxiliary terms used further down
   state = state.replace(i_inv=com.inv_inertia(sys, state.x))
 
   # calculate acceleration and delta-velocity terms
-  tau = actuator.to_tau(sys, act, state.q)
-  xdd_i = joints.resolve(sys, state, tau) + Motion.create(vel=sys.gravity)
+  tau = actuator.to_tau(sys, act, state.q, state.qd)
+  xdd_i = Motion.create(vel=sys.gravity)
+  xf_i = joints.resolve(sys, state, tau)
+  if sys.enable_fluid:
+    inertia = sys.link.inertia.i ** (1 - sys.spring_inertia_scale)
+    xf_i += fluid.force(sys, state.x, state.xd, state.mass, inertia)
+  xdd_i += Motion(
+      ang=jax.vmap(lambda x, y: x @ y)(state.i_inv, xf_i.ang),
+      vel=jax.vmap(lambda x, y: x / y)(xf_i.vel, state.mass),
+  )
+
   # semi-implicit euler: apply acceleration update before resolving collisions
   state = state.replace(xd_i=state.xd_i + xdd_i * sys.dt)
   xdv_i = collisions.resolve(sys, state)
 
   # now integrate and update position/velocity-level terms
   x_i, xd_i = integrator.integrate(sys, state.x_i, state.xd_i, xdv_i)
   x, xd = com.to_world(sys, x_i, xd_i)
```

### Comparing `brax-0.9.0/brax/spring/pipeline_test.py` & `brax-0.9.1/brax/spring/pipeline_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint:disable=g-multiple-import
 """Tests for spring physics pipeline."""
 
 from absl.testing import absltest
+from brax import com
 from brax import kinematics
 from brax import test_utils
+from brax.base import Transform
 from brax.generalized import pipeline as g_pipeline
 from brax.spring import pipeline
 import jax
 from jax import numpy as jp
 import numpy as np
 
 
@@ -33,24 +35,24 @@
     sys = sys.replace(
         link=sys.link.replace(constraint_stiffness=jp.array([800_000.0] * 3))
     )
 
     state = pipeline.init(sys, sys.init_q, jp.zeros(sys.qd_size()))
     j_spring_step = jax.jit(pipeline.step)
     for _ in range(10_000):
-      state = j_spring_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_spring_step(sys, state, jp.zeros(sys.act_size()))
     x = state.x
 
     # compare against generalized step
     q, qd = jp.zeros(sys.q_size()), jp.zeros(sys.qd_size())
     state = g_pipeline.init(sys, q, qd)
     j_g_step = jax.jit(g_pipeline.step)
     j_forward = jax.jit(kinematics.forward)
     for _ in range(10_000):
-      state = j_g_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_g_step(sys, state, jp.zeros(sys.act_size()))
     x_g, _ = j_forward(sys, state.q, state.qd)
 
     # trajectories should be close after 1 second of simulation
     self.assertLess(jp.linalg.norm(x_g.pos - x.pos), 2e-2)
 
   def test_universal_pendulum(self):
     sys = test_utils.load_fixture('single_universal_pendulum.xml')
@@ -67,28 +69,27 @@
     sys = sys.replace(ang_damping=0.0)
     sys = sys.replace(dt=0.001)
     sys = sys.replace(solver_iterations=500)
 
     state = pipeline.init(sys, init_q, init_qd)
     j_spring_step = jax.jit(pipeline.step)
     for _ in range(1000):
-      state = j_spring_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_spring_step(sys, state, jp.zeros(sys.act_size()))
     x = state.x
 
     # compare against generalized step
-    q, qd = init_q, init_qd
-    state = g_pipeline.init(sys, q, qd)
+    state = g_pipeline.init(sys, init_q, init_qd)
     j_g_step = jax.jit(g_pipeline.step)
     j_forward = jax.jit(kinematics.forward)
     for _ in range(1000):
       state = j_g_step(sys, state, jp.zeros(sys.qd_size()))
     x_g, _ = j_forward(sys, state.q, state.qd)
 
     # trajectories should be close after 1 second of simulation
-    self.assertLess(jp.linalg.norm(x_g.rot - x.rot), 1.5e-2)
+    self.assertLess(jp.linalg.norm(x_g.rot - x.rot), 1.51e-2)
 
   def test_spherical_pendulum(self):
     sys = test_utils.load_fixture('single_spherical_pendulum.xml')
 
     init_q = jp.array([0.1, 0.2, 0.3])
     init_qd = jax.random.uniform(jax.random.PRNGKey(0), (3,)) / 10.0
 
@@ -99,26 +100,33 @@
     link = link.replace(constraint_vel_damping=jp.array([200.0] * 3))
     sys = sys.replace(link=link)
     sys = sys.replace(ang_damping=0.0)
     sys = sys.replace(dt=0.001)
     sys = sys.replace(solver_iterations=500)
 
     state = pipeline.init(sys, init_q, init_qd)
+    # the qd calculation for pbd/spring doesn't match generalized, so we get xd
+    # from generalized and plug it back into pbd
+    # TODO: remove this xd override once kinematics.forward is fixed
+    state_g = g_pipeline.init(sys, init_q, init_qd)
+    off = state_g.x.pos - state_g.root_com
+    xd = Transform.create(pos=off).vmap().do(state_g.cd)
+    state = state.replace(xd=xd, xd_i=com.from_world(sys, state.x, xd)[1])
+
     j_spring_step = jax.jit(pipeline.step)
     for _ in range(1000):
-      state = j_spring_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_spring_step(sys, state, jp.zeros(sys.act_size()))
     x = state.x
 
     # compare against generalized step
-    q, qd = init_q, init_qd
-    state = g_pipeline.init(sys, q, qd)
+    state = state_g
     j_g_step = jax.jit(g_pipeline.step)
     j_forward = jax.jit(kinematics.forward)
     for _ in range(1000):
-      state = j_g_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_g_step(sys, state, jp.zeros(sys.act_size()))
     x_g, _ = j_forward(sys, state.q, state.qd)
 
     # trajectories should be close after 1 second of simulation
     self.assertLess(jp.linalg.norm(x_g.rot - x.rot), 1e-2)
 
   def test_prismatic_joint(self):
     # tests launching a mass along a slide joint in the [1,1,1] direction
@@ -136,15 +144,15 @@
     sys = sys.replace(ang_damping=0.0)
     sys = sys.replace(dt=0.001)
     sys = sys.replace(solver_iterations=500)
 
     state = pipeline.init(sys, init_q, init_qd)
     j_spring_step = jax.jit(pipeline.step)
     for _ in range(1000):
-      state = j_spring_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_spring_step(sys, state, jp.zeros(sys.act_size()))
     x = state.x
 
     # compare against generalized step
     state = g_pipeline.init(sys, init_q, init_qd)
     j_g_step = jax.jit(g_pipeline.step)
     j_forward = jax.jit(kinematics.forward)
     for _ in range(1000):
@@ -168,15 +176,15 @@
     qd = qd.at[0].set(2.5)
     qd = qd.at[1].set(2.5)
 
     state = pipeline.init(sys, sys.init_q, qd)
     j_spring_step = jax.jit(pipeline.step)
     states = []
     for _ in range(1000):
-      state = j_spring_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_spring_step(sys, state, jp.zeros(sys.act_size()))
       states.append(state)
     x, xd = state.x, state.xd
 
     # capsule still constrained to the plane and not rotating
     self.assertAlmostEqual(x.pos[0, 2], 0.0, delta=1e-2)
     np.testing.assert_allclose(
         x.rot, jp.array([[1.0, 0.0, 0.0, 0.0]]), atol=1e-3
@@ -197,15 +205,15 @@
     qd = qd.at[1].set(2.5)
     qd = qd.at[2].set(2.5)
 
     state = pipeline.init(sys, sys.init_q, qd)
     j_spring_step = jax.jit(pipeline.step)
     states = []
     for _ in range(1000):
-      state = j_spring_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_spring_step(sys, state, jp.zeros(sys.act_size()))
       states.append(state)
     x, xd = state.x, state.xd
 
     # capsule not rotating
     np.testing.assert_allclose(
         x.rot, jp.array([[1.0, 0.0, 0.0, 0.0]]), atol=1e-3
     )
@@ -224,15 +232,15 @@
     qd = qd.at[0].set(2.5)
     qd = qd.at[1].set(2.5)
 
     state = pipeline.init(sys, sys.init_q, qd)
     j_spring_step = jax.jit(pipeline.step)
     states = []
     for _ in range(1000):
-      state = j_spring_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_spring_step(sys, state, jp.zeros(sys.act_size()))
       states.append(state)
 
     # reflects off limits and is still traveling 2.5 m/s
     np.testing.assert_allclose(state.qd, jp.array([-2.5, -2.5]), atol=1e-3)
     np.testing.assert_allclose(
         state.xd.ang[0], jp.array([0.0, -2.5, 0.0]), atol=1e-4
     )
@@ -247,15 +255,15 @@
     qd = qd.at[1].set(2.5)
     qd = qd.at[2].set(2.5)
 
     state = pipeline.init(sys, sys.init_q, qd)
     j_spring_step = jax.jit(pipeline.step)
     states = []
     for _ in range(1000):
-      state = j_spring_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_spring_step(sys, state, jp.zeros(sys.act_size()))
       states.append(state)
 
     # reflects off limits and is still traveling 2.5 m/s
     np.testing.assert_allclose(
         state.qd, jp.array([-2.5, -2.5, -2.5]), atol=1e-3
     )
     np.testing.assert_allclose(
@@ -268,15 +276,15 @@
 
     qd = jp.zeros(sys.qd_size())
     qd = qd.at[0].set(5.0)
 
     state = pipeline.init(sys, sys.init_q, qd)
     j_spring_step = jax.jit(pipeline.step)
     for _ in range(1000):
-      state = j_spring_step(sys, state, jp.zeros(sys.qd_size()))
+      state = j_spring_step(sys, state, jp.zeros(sys.act_size()))
     x, xd = state.x, state.xd
 
     # capsule slides to a stop
     self.assertAlmostEqual(x.pos[0, 2], 0.25, delta=1e-3)
     np.testing.assert_allclose(
         x.rot, jp.array([[1.0, 0.0, 0.0, 0.0]]), atol=1e-3
     )
```

### Comparing `brax-0.9.0/brax/test_data/capsule.xml` & `brax-0.9.1/brax/test_data/capsule.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/colour_objects.xml` & `brax-0.9.1/brax/test_data/colour_objects.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/convex_convex.xml` & `brax-0.9.1/brax/test_data/convex_convex.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/double_pendulum.xml` & `brax-0.9.1/brax/test_data/double_pendulum.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/double_prismatic.xml` & `brax-0.9.1/brax/test_data/double_prismatic.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/chassis.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/chassis.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/chassis.stl` & `brax-0.9.1/brax/test_data/laikago/meshes/chassis.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/chassis_mod.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/chassis_mod.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/chassis_vhacd.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/chassis_vhacd.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/chassis_vhacd_mod.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/chassis_vhacd_mod.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/chassis_vhacd_mod_zup.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/chassis_vhacd_mod_zup.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/chassis_zup.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/chassis_zup.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/chassis_zup_lores.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/chassis_zup_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/hip_motor.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/hip_motor.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/hip_motor.stl` & `brax-0.9.1/brax/test_data/laikago/meshes/hip_motor.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/hip_motor_lores.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/hip_motor_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/hip_motor_mirror.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/hip_motor_mirror.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/hip_motor_mirror.stl` & `brax-0.9.1/brax/test_data/laikago/meshes/hip_motor_mirror.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/hip_motor_mirror_lores.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/hip_motor_mirror_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/lower_leg3.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/lower_leg3.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/lower_leg3_lores.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/lower_leg3_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/lower_leg_3.stl` & `brax-0.9.1/brax/test_data/laikago/meshes/lower_leg_3.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/lower_leg_3_collision.stl` & `brax-0.9.1/brax/test_data/laikago/meshes/lower_leg_3_collision.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/upper_leg.stl` & `brax-0.9.1/brax/test_data/laikago/meshes/upper_leg.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_left.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_left.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_left2.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_left2.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_left2_lores.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_left2_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_left_lores.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_left_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_left_vhacd.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_left_vhacd.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_mirror.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_mirror.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_mirror.stl` & `brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_mirror.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_mirror2.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_mirror2.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_mirror2_lores.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_mirror2_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_mirror_lores.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_mirror_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_right.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_right.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/laikago/meshes/upper_leg_right_vhacd.obj` & `brax-0.9.1/brax/test_data/laikago/meshes/upper_leg_right_vhacd.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/meshes/cylinder.stl` & `brax-0.9.1/brax/test_data/meshes/cylinder.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/meshes/dodecahedron.stl` & `brax-0.9.1/brax/test_data/meshes/dodecahedron.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/nonzero_joint_ref.xml` & `brax-0.9.1/brax/test_data/nonzero_joint_ref.xml`

 * *Files 19% similar despite different names*

#### Comparing `brax-0.9.0/brax/test_data/nonzero_joint_ref.xml` & `brax-0.9.1/brax/test_data/nonzero_joint_ref.xml`

```diff
@@ -1,52 +1,47 @@
 <?xml version="1.0" encoding="utf-8"?>
 <mujoco model="hopper">
-  <compiler angle="degree" coordinate="global" inertiafromgeom="true"/>
-  <default>
-    <joint armature="1" damping="1" limited="true"/>
-    <geom conaffinity="1" condim="1" contype="1" margin="0.001" material="geom" rgba="0.8 0.6 .4 1" solimp=".8 .8 .01" solref=".02 1"/>
-    <motor ctrllimited="true" ctrlrange="-.4 .4"/>
-  </default>
-  <option timestep="0.002"/>
+  <compiler angle="radian" autolimits="true"/>
   <visual>
     <map znear="0.02"/>
   </visual>
+  <default class="main">
+    <joint limited="true" armature="1" damping="1"/>
+    <geom condim="1" solimp="0.8 0.8 0.01 0.5 2" margin="0.001" material="geom" rgba="0.8 0.6 0.4 1"/>
+    <general ctrllimited="true" ctrlrange="-0.4 0.4"/>
+  </default>
+  <asset>
+    <texture type="skybox" builtin="gradient" rgb1="0.4 0.5 0.6" rgb2="0 0 0" width="100" height="600"/>
+    <texture type="cube" name="texgeom" builtin="flat" mark="cross" rgb1="0.8 0.6 0.4" rgb2="0.8 0.6 0.4" markrgb="1 1 1" width="127" height="762"/>
+    <texture type="2d" name="texplane" builtin="checker" rgb1="0 0 0" rgb2="0.8 0.8 0.8" width="100" height="100"/>
+    <material name="MatPlane" texture="texplane" texrepeat="60 60" specular="1" shininess="1" reflectance="0.5"/>
+    <material name="geom" texture="texgeom" texuniform="true"/>
+  </asset>
   <worldbody>
-    <light cutoff="100" diffuse="1 1 1" dir="-0 0 -1.3" directional="true" exponent="1" pos="0 0 1.3" specular=".1 .1 .1"/>
-    <geom conaffinity="1" condim="3" name="floor" pos="0 0 0" rgba="0.8 0.9 0.8 1" size="20 20 .125" type="plane" material="MatPlane"/>
-    <body name="dummy" pos="1 2 3">
-      <joint armature="0" axis="1 0 0" damping="0" limited="false" name="free" pos="0 0 0" type="free"/>
-      <geom friction="0.9" fromto="0 0 1.45 0 0 1.05" name="dummy_geom" size="0.05" type="capsule"/>
-      <body name="torso" pos="0 0 1.25">
-        <camera name="track" mode="trackcom" pos="0 -3 1" xyaxes="1 0 0 0 0 1"/>
-        <joint armature="0" axis="1 0 0" damping="0" limited="false" name="rootx" pos="0 0 0" stiffness="0" type="slide"/>
-        <joint armature="0" axis="0 0 1" damping="0" limited="false" name="rootz" pos="0 0 0" ref="1.25" stiffness="0" type="slide"/>
-        <joint armature="0" axis="0 1 0" damping="0" limited="false" name="rooty" pos="0 0 1.25" stiffness="0" type="hinge"/>
-        <geom friction="0.9" fromto="0 0 1.45 0 0 1.05" name="torso_geom" size="0.05" type="capsule"/>
-        <body name="thigh" pos="0 0 1.05">
-          <joint axis="0 -1 0" name="thigh_joint" pos="0 0 1.05" range="-150 0" type="hinge"/>
-          <geom friction="0.9" fromto="0 0 1.05 0 0 0.6" name="thigh_geom" size="0.05" type="capsule"/>
-          <body name="leg" pos="0 0 0.35">
-            <joint axis="0 -1 0" name="leg_joint" pos="0 0 0.6" range="-150 0" type="hinge"/>
-            <geom friction="0.9" fromto="0 0 0.6 0 0 0.1" name="leg_geom" size="0.04" type="capsule"/>
-            <body name="foot" pos="0.13 0 0">
-              <joint axis="0 -1 0" name="foot_joint" pos="0 0 0.1" range="-45 45" type="hinge"/>
-              <geom friction="2.0" fromto="-0.13 0 0.1 0.26 0 0.1" name="foot_geom" size="0.06" type="capsule"/>
-            </body>
+    <geom name="floor" size="20 20 0.125" type="plane" condim="3" material="MatPlane" rgba="0.8 0.9 0.8 1"/>
+    <light pos="0 0 1.3" dir="0 0 -1" directional="true" cutoff="100" exponent="1" diffuse="1 1 1" specular="0.1 0.1 0.1"/>
+    <body name="torso" pos="0 0 1.25">
+      <joint name="rootx" pos="0 0 -1.25" axis="1 0 0" limited="false" type="slide" armature="0" damping="0"/>
+      <joint name="rootz" pos="0 0 -1.25" axis="0 0 1" limited="false" type="slide" ref="1.25" armature="0" damping="0"/>
+      <joint name="rooty" pos="0 0 0" axis="0 1 0" limited="false" armature="0" damping="0"/>
+      <geom name="torso_geom" size="0.05 0.2" type="capsule" friction="0.9 0.005 0.0001"/>
+      <camera name="track" pos="0 -3 -0.25" quat="0.707107 0.707107 0 0" mode="trackcom"/>
+      <body name="thigh" pos="0 0 -0.2">
+        <joint name="thigh_joint" pos="0 0 0" axis="0 -1 0" range="-2.61799 0"/>
+        <geom name="thigh_geom" size="0.05 0.225" pos="0 0 -0.225" type="capsule" friction="0.9 0.005 0.0001"/>
+        <body name="leg" pos="0 0 -0.7">
+          <joint name="leg_joint" pos="0 0 0.25" axis="0 -1 0" range="-2.61799 0"/>
+          <geom name="leg_geom" size="0.04 0.25" type="capsule" friction="0.9 0.005 0.0001"/>
+          <body name="foot" pos="0.13 0 -0.35">
+            <joint name="foot_joint" pos="-0.13 0 0.1" axis="0 -1 0" range="-0.785398 0.785398"/>
+            <geom name="foot_geom" size="0.06 0.195" pos="-0.065 0 0.1" quat="0.707107 0 -0.707107 0" type="capsule" friction="2 0.005 0.0001"/>
           </body>
         </body>
       </body>
     </body>
   </worldbody>
   <actuator>
-    <motor ctrllimited="true" ctrlrange="-1.0 1.0" gear="200.0" joint="thigh_joint"/>
-    <motor ctrllimited="true" ctrlrange="-1.0 1.0" gear="200.0" joint="leg_joint"/>
-    <motor ctrllimited="true" ctrlrange="-1.0 1.0" gear="200.0" joint="foot_joint"/>
+    <general joint="thigh_joint" ctrlrange="-1 1" gear="200 0 0 0 0 0"/>
+    <general joint="leg_joint" ctrlrange="-1 1" gear="200 0 0 0 0 0"/>
+    <general joint="foot_joint" ctrlrange="-1 1" gear="200 0 0 0 0 0"/>
   </actuator>
-  <asset>
-    <texture type="skybox" builtin="gradient" rgb1=".4 .5 .6" rgb2="0 0 0" width="100" height="100"/>
-    <texture builtin="flat" height="1278" mark="cross" markrgb="1 1 1" name="texgeom" random="0.01" rgb1="0.8 0.6 0.4" rgb2="0.8 0.6 0.4" type="cube" width="127"/>
-    <texture builtin="checker" height="100" name="texplane" rgb1="0 0 0" rgb2="0.8 0.8 0.8" type="2d" width="100"/>
-    <material name="MatPlane" reflectance="0.5" shininess="1" specular="1" texrepeat="60 60" texture="texplane"/>
-    <material name="geom" texture="texgeom" texuniform="true"/>
-  </asset>
 </mujoco>
```

### Comparing `brax-0.9.0/brax/test_data/prismaversal_2dof_joint.xml` & `brax-0.9.1/brax/test_data/prismaversal_2dof_joint.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/prismaversal_3dof_joint.xml` & `brax-0.9.1/brax/test_data/prismaversal_3dof_joint.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/single_pendulum_motor.xml` & `brax-0.9.1/brax/test_data/single_pendulum_motor.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/single_pendulum_position.xml` & `brax-0.9.1/brax/test_data/single_pendulum_position.xml`

 * *Files 8% similar despite different names*

#### Comparing `brax-0.9.0/brax/test_data/single_pendulum_position.xml` & `brax-0.9.1/brax/test_data/single_pendulum_position.xml`

```diff
@@ -12,10 +12,10 @@
   <worldbody>
     <body name="body1" pos="0 0 0">
       <joint axis="1 0 0" name="hinge1" pos="0 0 0" type="hinge"/>
       <geom name="sphere1" pos="0 0.5 0" size=".15" mass="1" type="sphere"/>
     </body>
   </worldbody>
   <actuator>
-    <position ctrllimited="false" joint="hinge1" gear="10 0 0 0 0 0"/>
+    <position ctrllimited="false" joint="hinge1" kp="10"/>
   </actuator>
 </mujoco>
```

### Comparing `brax-0.9.0/brax/test_data/single_spherical_pendulum.xml` & `brax-0.9.1/brax/test_data/single_spherical_pendulum.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/single_spherical_pendulum_motor.xml` & `brax-0.9.1/brax/test_data/single_spherical_pendulum_motor.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/single_spherical_pendulum_position.xml` & `brax-0.9.1/brax/test_data/single_spherical_pendulum_position.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/triple_pendulum.xml` & `brax-0.9.1/brax/test_data/triple_pendulum.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/triple_pendulum_motor.xml` & `brax-0.9.1/brax/test_data/triple_pendulum_motor.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/triple_prismatic.xml` & `brax-0.9.1/brax/test_data/triple_prismatic.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_data/world_body_transform.xml` & `brax-0.9.1/brax/test_data/world_body_transform.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/test_utils.py` & `brax-0.9.1/brax/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -33,33 +33,54 @@
     full_path = epath.resource_path('brax') / f'envs/assets/{path}'
   xml = mjcf.fuse_bodies(full_path.read_text())
   model = mujoco.MjModel.from_xml_string(xml)
 
   return model
 
 
+def _normalize_q(model: mujoco.MjModel, q: np.ndarray):
+  """Normalizes the quaternion part of q."""
+  q = np.array(q)
+  q_idx = 0
+  for typ in model.jnt_type:
+    q_dim = 7 if typ == 0 else 1
+    if typ == 0:
+      q[q_idx + 3:q_idx + 7] = (
+          q[q_idx + 3:q_idx + 7] / np.linalg.norm(q[q_idx + 3:q_idx + 7]))
+    q_idx += q_dim
+  return q
+
+
 def sample_mujoco_states(
-    path: str, count: int = 500, modulo: int = 20, force_pgs: bool = False
+    path: str, count: int = 500, modulo: int = 20, force_pgs: bool = False,
+    random_init: bool = False, random_q_scale: float = 1.0,
+    random_qd_scale: float = 0.1, vel_to_local: bool = True, seed: int = 42
 ) -> Iterable[Tuple[mujoco.MjData, mujoco.MjData]]:
   """Samples count / modulo states from mujoco for comparison."""
+  np.random.seed(seed)
   model = load_fixture_mujoco(path)
   model.opt.iterations = 50  # return to default for high-precision comparison
   if force_pgs:
     model.opt.solver = 0
   data = mujoco.MjData(model)
   # give a little kick to avoid symmetry
   data.qvel = np.random.uniform(low=-0.01, high=0.01, size=(model.nv,))
+  if random_init:
+    data.qpos = np.random.uniform(model.nq) * random_q_scale
+    data.qpos = _normalize_q(model, data.qpos)
+    data.qvel = np.random.uniform(size=(model.nv,)) * random_qd_scale
   for i in range(count):
     before = copy.deepcopy(data)
     mujoco.mj_step(model, data)
     if i % modulo == 0:
       # hijack subtree_angmom, subtree_linvel (unused) to store xang, xvel
       for i in range(model.nbody):
         vel = np.zeros((6,))
-        mujoco.mj_objectVelocity(model, data, 2, i, vel, 1)
+        mujoco.mj_objectVelocity(
+            model, data, mujoco.mjtObj.mjOBJ_XBODY.value, i, vel, vel_to_local)
         data.subtree_angmom[i] = vel[:3]
         data.subtree_linvel[i] = vel[3:]
       yield before, data
 
 
 def load_fixture(path: str) -> System:
   full_path = epath.resource_path('brax') / f'test_data/{path}'
```

### Comparing `brax-0.9.0/brax/training/__init__.py` & `brax-0.9.1/brax/spring/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/acme/__init__.py` & `brax-0.9.1/brax/training/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/acme/running_statistics.py` & `brax-0.9.1/brax/training/acme/running_statistics.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/acme/specs.py` & `brax-0.9.1/brax/training/acme/specs.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/acme/types.py` & `brax-0.9.1/brax/training/acme/types.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/acting.py` & `brax-0.9.1/brax/training/acting.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,34 +11,37 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Brax training acting functions."""
 
 import time
-from typing import Callable, Sequence, Tuple
+from typing import Callable, Sequence, Tuple, Union
 
+from brax import envs
 from brax.training.types import Metrics
 from brax.training.types import Policy
 from brax.training.types import PolicyParams
 from brax.training.types import PRNGKey
 from brax.training.types import Transition
-# TODO: use v2 envs here, some weird type annotations to figure out.
-from brax.v1 import envs
+from brax.v1 import envs as envs_v1
 import jax
 import numpy as np
 
+State = Union[envs.State, envs_v1.State]
+Env = Union[envs.Env, envs_v1.Env, envs_v1.Wrapper]
+
 
 def actor_step(
-    env: envs.Env,
-    env_state: envs.State,
+    env: Env,
+    env_state: State,
     policy: Policy,
     key: PRNGKey,
     extra_fields: Sequence[str] = ()
-) -> Tuple[envs.State, Transition]:
+) -> Tuple[State, Transition]:
   """Collect data."""
   actions, policy_extras = policy(env_state.obs, key)
   nstate = env.step(env_state, actions)
   state_extras = {x: nstate.info[x] for x in extra_fields}
   return nstate, Transition(  # pytype: disable=wrong-arg-types  # jax-ndarray
       observation=env_state.obs,
       action=actions,
@@ -48,21 +51,21 @@
       extras={
           'policy_extras': policy_extras,
           'state_extras': state_extras
       })
 
 
 def generate_unroll(
-    env: envs.Env,
-    env_state: envs.State,
+    env: Env,
+    env_state: State,
     policy: Policy,
     key: PRNGKey,
     unroll_length: int,
     extra_fields: Sequence[str] = ()
-) -> Tuple[envs.State, Transition]:
+) -> Tuple[State, Transition]:
   """Collect trajectories of given unroll_length."""
 
   @jax.jit
   def f(carry, unused_t):
     state, current_key = carry
     current_key, next_key = jax.random.split(current_key)
     nstate, transition = actor_step(
@@ -91,18 +94,18 @@
       episode_length: Maximum length of an episode.
       action_repeat: Number of physics steps per env step.
       key: RNG key.
     """
     self._key = key
     self._eval_walltime = 0.
 
-    eval_env = envs.wrappers.EvalWrapper(eval_env)
+    eval_env = envs.training.EvalWrapper(eval_env)
 
     def generate_eval_unroll(policy_params: PolicyParams,
-                             key: PRNGKey) -> envs.State:
+                             key: PRNGKey) -> State:
       reset_keys = jax.random.split(key, num_eval_envs)
       eval_first_state = eval_env.reset(reset_keys)
       return generate_unroll(
           eval_env,
           eval_first_state,
           eval_policy_fn(policy_params),
           key,
```

### Comparing `brax-0.9.0/brax/training/agents/__init__.py` & `brax-0.9.1/brax/training/acme/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/apg/__init__.py` & `brax-0.9.1/brax/training/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/apg/networks.py` & `brax-0.9.1/brax/training/agents/apg/networks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/apg/train.py` & `brax-0.9.1/brax/training/agents/apg/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 """Analytic policy gradient training."""
 
 import functools
 import time
 from typing import Callable, Optional, Tuple, Union
 
 from absl import logging
-from brax.v1 import envs as envs_v1
+from brax import envs
 from brax.training import acting
 from brax.training import pmap
 from brax.training import types
 from brax.training.acme import running_statistics
 from brax.training.acme import specs
 from brax.training.agents.apg import networks as apg_networks
 from brax.training.types import Params
 from brax.training.types import PRNGKey
-from brax import envs
+from brax.v1 import envs as envs_v1
 import flax
 import jax
 import jax.numpy as jnp
 import optax
 
 InferenceParams = Tuple[running_statistics.NestedMeanStd, Params]
 Metrics = types.Metrics
@@ -88,15 +88,15 @@
     assert truncation_length > 0
 
   num_evals_after_init = max(num_evals - 1, 1)
 
   assert num_envs % device_count == 0
   env = environment
   if isinstance(env, envs.Env):
-    wrap_for_training = envs.wrapper.wrap_for_training
+    wrap_for_training = envs.training.wrap
   else:
     wrap_for_training = envs_v1.wrappers.wrap_for_training
 
   env = wrap_for_training(
       env, episode_length=episode_length, action_repeat=action_repeat)
 
   normalize = lambda x, y: x
@@ -220,14 +220,15 @@
       functools.partial(make_policy, deterministic=deterministic_eval),
       num_eval_envs=num_eval_envs,
       episode_length=episode_length,
       action_repeat=action_repeat,
       key=eval_key)
 
   # Run initial eval
+  metrics = {}
   if process_id == 0 and num_evals > 1:
     metrics = evaluator.run_evaluation(
         _unpmap(
             (training_state.normalizer_params, training_state.policy_params)),
         training_metrics={})
     logging.info(metrics)
     progress_fn(0, metrics)
```

### Comparing `brax-0.9.0/brax/training/agents/apg/train_test.py` & `brax-0.9.1/brax/training/agents/apg/train_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/ars/__init__.py` & `brax-0.9.1/brax/training/agents/apg/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/ars/networks.py` & `brax-0.9.1/brax/training/agents/ars/networks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/ars/train.py` & `brax-0.9.1/brax/training/agents/ars/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 See: https://arxiv.org/pdf/1803.07055.pdf
 """
 
 import time
 from typing import Callable, Optional, Tuple, Union
 
 from absl import logging
-from brax.v1 import envs as envs_v1
+from brax import envs
 from brax.training import acting
 from brax.training import types
 from brax.training.acme import running_statistics
 from brax.training.acme import specs
 from brax.training.agents.ars import networks as ars_networks
 from brax.training.types import Params
 from brax.training.types import PRNGKey
-from brax import envs
+from brax.v1 import envs as envs_v1
 import flax
 import jax
 import jax.numpy as jnp
 import optax
 
 Metrics = types.Metrics
 InferenceParams = Tuple[running_statistics.NestedMeanStd, Params]
@@ -86,15 +86,15 @@
 
   num_env_steps_between_evals = num_timesteps // num_evals
   next_eval_step = num_timesteps - (num_evals - 1) * num_env_steps_between_evals
 
   assert num_envs % local_devices_to_use == 0
   env = environment
   if isinstance(env, envs.Env):
-    wrap_for_training = envs.wrapper.wrap_for_training
+    wrap_for_training = envs.training.wrap
   else:
     wrap_for_training = envs_v1.wrappers.wrap_for_training
 
   env = wrap_for_training(
       env, episode_length=episode_length, action_repeat=action_repeat)
 
   obs_size = env.observation_size
@@ -137,36 +137,42 @@
   def add_noise(params: Params, key: PRNGKey) -> Tuple[Params, Params, Params]:
     num_vars = len(jax.tree_util.tree_leaves(params))
     treedef = jax.tree_util.tree_structure(params)
     all_keys = jax.random.split(key, num=num_vars)
     noise = jax.tree_util.tree_map(
         lambda g, k: jax.random.normal(k, shape=g.shape, dtype=g.dtype), params,
         jax.tree_util.tree_unflatten(treedef, all_keys))
-    params_with_noise = jax.tree_util.tree_map(lambda g, n: g + n * exploration_noise_std,
-                                     params, noise)
+    params_with_noise = jax.tree_util.tree_map(
+        lambda g, n: g + n * exploration_noise_std, params, noise
+    )
     params_with_anti_noise = jax.tree_util.tree_map(
         lambda g, n: g - n * exploration_noise_std, params, noise)
     return params_with_noise, params_with_anti_noise, noise
 
   prun_episode = jax.pmap(run_episode, in_axes=(None, 0, 0))
 
   @jax.jit
   def training_epoch(training_state: TrainingState,
                      key: PRNGKey) -> Tuple[TrainingState, Metrics]:
     params = jax.tree_util.tree_map(
         lambda x: jnp.repeat(
-            jnp.expand_dims(x, axis=0), number_of_directions, axis=0),
-        training_state.policy_params)
+            jnp.expand_dims(x, axis=0), number_of_directions, axis=0
+        ),
+        training_state.policy_params,
+    )
     key, key_noise, key_es_eval = jax.random.split(key, 3)
     # generate perturbations
     params_with_noise, params_with_anti_noise, noise = add_noise(
         params, key_noise)
 
-    pparams = jax.tree_util.tree_map(lambda a, b: jnp.concatenate([a, b], axis=0),
-                           params_with_noise, params_with_anti_noise)
+    pparams = jax.tree_util.tree_map(
+        lambda a, b: jnp.concatenate([a, b], axis=0),
+        params_with_noise,
+        params_with_anti_noise,
+    )
 
     pparams = jax.tree_util.tree_map(
         lambda x: jnp.reshape(x, (local_devices_to_use, -1) + x.shape[1:]),
         pparams)
 
     key_es_eval = jax.random.split(key_es_eval, local_devices_to_use)
     eval_scores, obs, obs_weights = prun_episode(
@@ -183,21 +189,25 @@
     reward_plus, reward_minus = jnp.split(eval_scores, 2, axis=0)
     reward_max = jnp.maximum(reward_plus, reward_minus)
     reward_rank = jnp.argsort(jnp.argsort(-reward_max))
     reward_weight = jnp.where(reward_rank < top_directions, 1, 0)
     reward_weight_double = jnp.concatenate([reward_weight, reward_weight],
                                            axis=0)
     reward_std = jnp.std(eval_scores, where=reward_weight_double)
+    reward_std += (reward_std == 0.0) * 1e-6
 
     noise = jax.tree_util.tree_map(
         lambda x: jnp.sum(
             jnp.transpose(
-                jnp.transpose(x) * reward_weight *
-                (reward_plus - reward_minus)),
-            axis=0), noise)
+                jnp.transpose(x) * reward_weight * (reward_plus - reward_minus)
+            ),
+            axis=0,
+        ),
+        noise,
+    )
 
     policy_params = jax.tree_util.tree_map(
         lambda x, y: x + step_size * y / (top_directions * reward_std),
         training_state.policy_params, noise)
 
     num_env_steps = training_state.num_env_steps + jnp.sum(
         obs_weights, dtype=jnp.int32) * action_repeat
```

### Comparing `brax-0.9.0/brax/training/agents/ars/train_test.py` & `brax-0.9.1/brax/training/agents/ars/train_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from brax import envs
 from brax.training.acme import running_statistics
 from brax.training.agents.ars import networks as ars_networks
 from brax.training.agents.ars import train as ars
-from brax.v1 import envs as envs_v1
 import jax
 
 
 class ARSTest(parameterized.TestCase):
   """Tests for ARS module."""
 
   @parameterized.parameters(True, False)
```

### Comparing `brax-0.9.0/brax/training/agents/es/__init__.py` & `brax-0.9.1/brax/training/agents/ars/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/es/networks.py` & `brax-0.9.1/brax/training/agents/es/networks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/es/train.py` & `brax-0.9.1/brax/training/agents/es/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 
 import enum
 import functools
 import time
 from typing import Callable, Optional, Tuple, Union
 
 from absl import logging
-from brax.v1 import envs as envs_v1
+from brax import envs
 from brax.training import acting
 from brax.training import types
 from brax.training.acme import running_statistics
 from brax.training.acme import specs
 from brax.training.agents.es import networks as es_networks
 from brax.training.types import Params
 from brax.training.types import PRNGKey
-from brax import envs
+from brax.v1 import envs as envs_v1
 import flax
 import jax
 import jax.numpy as jnp
 import optax
 
 Metrics = types.Metrics
 InferenceParams = Tuple[running_statistics.NestedMeanStd, Params]
@@ -114,15 +114,15 @@
   num_env_steps_between_evals = num_timesteps // num_evals_after_init
   next_eval_step = num_timesteps - (num_evals_after_init -
                                     1) * num_env_steps_between_evals
 
   assert num_envs % local_devices_to_use == 0
   env = environment
   if isinstance(env, envs.Env):
-    wrap_for_training = envs.wrapper.wrap_for_training
+    wrap_for_training = envs.training.wrap
   else:
     wrap_for_training = envs_v1.wrappers.wrap_for_training
 
   env = wrap_for_training(
       env, episode_length=episode_length, action_repeat=action_repeat)
 
   obs_size = env.observation_size
```

### Comparing `brax-0.9.0/brax/training/agents/es/train_test.py` & `brax-0.9.1/brax/training/agents/es/train_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/ppo/__init__.py` & `brax-0.9.1/brax/training/agents/es/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/ppo/losses.py` & `brax-0.9.1/brax/training/agents/ppo/losses.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/ppo/networks.py` & `brax-0.9.1/brax/training/agents/ppo/networks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/ppo/train.py` & `brax-0.9.1/brax/training/agents/ppo/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 """
 
 import functools
 import time
 from typing import Callable, Optional, Tuple, Union
 
 from absl import logging
-from brax.v1 import envs as envs_v1
+from brax import envs
 from brax.training import acting
 from brax.training import gradients
 from brax.training import pmap
 from brax.training import types
 from brax.training.acme import running_statistics
 from brax.training.acme import specs
 from brax.training.agents.ppo import losses as ppo_losses
 from brax.training.agents.ppo import networks as ppo_networks
 from brax.training.types import Params
 from brax.training.types import PRNGKey
-from brax import envs
+from brax.v1 import envs as envs_v1
 import flax
 import jax
 import jax.numpy as jnp
 import optax
 
 InferenceParams = Tuple[running_statistics.NestedMeanStd, Params]
 Metrics = types.Metrics
@@ -128,15 +128,15 @@
   # way for different processes.
   key_policy, key_value = jax.random.split(global_key)
   del global_key
 
   assert num_envs % device_count == 0
   env = environment
   if isinstance(env, envs.Env):
-    wrap_for_training = envs.wrapper.wrap_for_training
+    wrap_for_training = envs.training.wrap
   else:
     wrap_for_training = envs_v1.wrappers.wrap_for_training
 
   env = wrap_for_training(
       env, episode_length=episode_length, action_repeat=action_repeat)
 
   reset_fn = jax.jit(jax.vmap(env.reset))
@@ -308,14 +308,15 @@
       functools.partial(make_policy, deterministic=deterministic_eval),
       num_eval_envs=num_eval_envs,
       episode_length=episode_length,
       action_repeat=action_repeat,
       key=eval_key)
 
   # Run initial eval
+  metrics = {}
   if process_id == 0 and num_evals > 1:
     metrics = evaluator.run_evaluation(
         _unpmap(
             (training_state.normalizer_params, training_state.params.policy)),
         training_metrics={})
     logging.info(metrics)
     progress_fn(0, metrics)
```

### Comparing `brax-0.9.0/brax/training/agents/ppo/train_test.py` & `brax-0.9.1/brax/training/agents/ppo/train_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/sac/__init__.py` & `brax-0.9.1/brax/training/agents/ppo/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/sac/losses.py` & `brax-0.9.1/brax/training/agents/sac/losses.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/sac/networks.py` & `brax-0.9.1/brax/training/agents/sac/networks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/agents/sac/train.py` & `brax-0.9.1/brax/training/agents/sac/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 """
 
 import functools
 import time
 from typing import Any, Callable, Optional, Tuple, Union
 
 from absl import logging
-from brax.v1 import envs as envs_v1
+from brax import envs
 from brax.io import model
 from brax.training import acting
 from brax.training import gradients
 from brax.training import pmap
 from brax.training import replay_buffers
 from brax.training import types
 from brax.training.acme import running_statistics
 from brax.training.acme import specs
 from brax.training.agents.sac import losses as sac_losses
 from brax.training.agents.sac import networks as sac_networks
 from brax.training.types import Params
 from brax.training.types import PRNGKey
-from brax import envs
+from brax.v1 import envs as envs_v1
 import flax
 import jax
 import jax.numpy as jnp
 import optax
 
 Metrics = types.Metrics
 Transition = types.Transition
@@ -157,15 +157,15 @@
   num_training_steps_per_epoch = -(
       -(num_timesteps - num_prefill_env_steps) //
       (num_evals_after_init * env_steps_per_actor_step))
 
   assert num_envs % device_count == 0
   env = environment
   if isinstance(env, envs.Env):
-    wrap_for_training = envs.wrapper.wrap_for_training
+    wrap_for_training = envs.training.wrap
   else:
     wrap_for_training = envs_v1.wrappers.wrap_for_training
 
   env = wrap_for_training(
       env, episode_length=episode_length, action_repeat=action_repeat)
 
   obs_size = env.observation_size
@@ -310,16 +310,15 @@
     transitions = jax.tree_util.tree_map(
         lambda x: jnp.reshape(x, (grad_updates_per_step, -1) + x.shape[1:]),
         transitions)
     (training_state, _), metrics = jax.lax.scan(sgd_step,
                                                 (training_state, training_key),
                                                 transitions)
 
-    metrics['buffer_current_size'] = buffer_state.current_size
-    metrics['buffer_current_position'] = buffer_state.current_position
+    metrics['buffer_current_size'] = replay_buffer.size(buffer_state)
     return training_state, env_state, buffer_state, metrics
 
   def prefill_replay_buffer(
       training_state: TrainingState, env_state: envs.State,
       buffer_state: ReplayBufferState, key: PRNGKey
   ) -> Tuple[TrainingState, envs.State, ReplayBufferState, PRNGKey]:
 
@@ -421,14 +420,15 @@
       functools.partial(make_policy, deterministic=deterministic_eval),
       num_eval_envs=num_eval_envs,
       episode_length=episode_length,
       action_repeat=action_repeat,
       key=eval_key)
 
   # Run initial eval
+  metrics = {}
   if process_id == 0 and num_evals > 1:
     metrics = evaluator.run_evaluation(
         _unpmap(
             (training_state.normalizer_params, training_state.policy_params)),
         training_metrics={})
     logging.info(metrics)
     progress_fn(0, metrics)
```

### Comparing `brax-0.9.0/brax/training/agents/sac/train_test.py` & `brax-0.9.1/brax/training/agents/sac/train_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/distribution.py` & `brax-0.9.1/brax/training/distribution.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/gradients.py` & `brax-0.9.1/brax/training/gradients.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/learner.py` & `brax-0.9.1/brax/training/learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,16 +114,15 @@
     'larger (used for antithetic sampling.')
 flags.DEFINE_integer('top_directions', 20,
                      'Number of top directions to select.')
 flags.DEFINE_float('exploration_noise_std', 0.1,
                    'Std of a random noise added by ARS.')
 flags.DEFINE_float('reward_shift', 0.,
                    'A reward shift to get rid of "stay alive" bonus.')
-flags.DEFINE_enum('head_type', '', ['', 'clip', 'tanh'],
-                  'Which policy head to use.')
+
 # ARS hps.
 flags.DEFINE_integer('truncation_length', None,
                      'Truncation for gradient propagation in APG.')
 
 
 def main(unused_argv):
```

### Comparing `brax-0.9.0/brax/training/networks.py` & `brax-0.9.1/brax/training/networks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/pmap.py` & `brax-0.9.1/brax/training/pmap.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/replay_buffers.py` & `brax-0.9.1/brax/training/replay_buffers.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Replay buffers for Brax."""
 
 import abc
-from typing import Generic, Optional, Tuple, TypeVar
+import math
+from typing import Generic, Optional, Sequence, Tuple, TypeVar
 
 from brax.training.types import PRNGKey
 import flax
 import jax
 from jax import flatten_util
 from jax.experimental import pjit
 import jax.numpy as jnp
@@ -31,123 +32,196 @@
 class ReplayBuffer(abc.ABC, Generic[State, Sample]):
   """Contains replay buffer methods."""
 
   @abc.abstractmethod
   def init(self, key: PRNGKey) -> State:
     """Init the replay buffer."""
 
-  @abc.abstractmethod
   def insert(self, buffer_state: State, samples: Sample) -> State:
-    """Insert data in the replay buffer."""
+    """Insert data into the replay buffer."""
+    self.check_can_insert(buffer_state, samples, 1)
+    return self.insert_internal(buffer_state, samples)
 
-  @abc.abstractmethod
   def sample(self, buffer_state: State) -> Tuple[State, Sample]:
     """Sample a batch of data."""
+    self.check_can_sample(buffer_state, 1)
+    return self.sample_internal(buffer_state)
+
+  def check_can_insert(self, buffer_state: State, samples: Sample, shards: int):
+    """Checks whether insert can be performed. Do not JIT this method."""
+    pass
+
+  def check_can_sample(self, buffer_state: State, shards: int):
+    """Checks whether sampling can be performed. Do not JIT this method."""
+    pass
 
   @abc.abstractmethod
   def size(self, buffer_state: State) -> int:
     """Total amount of elements that are sampleable."""
 
+  @abc.abstractmethod
+  def insert_internal(self, buffer_state: State, samples: Sample) -> State:
+    """Insert data into the replay buffer."""
+
+  @abc.abstractmethod
+  def sample_internal(self, buffer_state: State) -> Tuple[State, Sample]:
+    """Sample a batch of data."""
+
 
 @flax.struct.dataclass
 class ReplayBufferState:
   """Contains data related to a replay buffer."""
+
   data: jnp.ndarray
-  current_position: jnp.ndarray
-  current_size: jnp.ndarray
+  insert_position: jnp.ndarray
+  sample_position: jnp.ndarray
   key: PRNGKey
 
 
 class QueueBase(ReplayBuffer[ReplayBufferState, Sample], Generic[Sample]):
   """Base class for limited-size FIFO reply buffers.
 
   Implements an `insert()` method which behaves like a limited-size queue.
   I.e. it adds samples to the end of the queue and, if necessary, removes the
   oldest samples form the queue in order to keep the maximum size within the
   specified limit.
 
   Derived classes must implement the `sample()` method.
   """
 
-  def __init__(self, max_replay_size: int, dummy_data_sample: Sample,
-               sample_batch_size: int):
+  def __init__(
+      self,
+      max_replay_size: int,
+      dummy_data_sample: Sample,
+      sample_batch_size: int,
+  ):
     self._flatten_fn = jax.vmap(lambda x: flatten_util.ravel_pytree(x)[0])
 
     dummy_flatten, self._unflatten_fn = flatten_util.ravel_pytree(
-        dummy_data_sample)
+        dummy_data_sample
+    )
     self._unflatten_fn = jax.vmap(self._unflatten_fn)
     data_size = len(dummy_flatten)
 
     self._data_shape = (max_replay_size, data_size)
     self._data_dtype = dummy_flatten.dtype
     self._sample_batch_size = sample_batch_size
+    self._size = 0
 
   def init(self, key: PRNGKey) -> ReplayBufferState:
     return ReplayBufferState(
         data=jnp.zeros(self._data_shape, self._data_dtype),
-        current_size=jnp.zeros((), jnp.int32),
-        current_position=jnp.zeros((), jnp.int32),
-        key=key)
+        sample_position=jnp.zeros((), jnp.int32),
+        insert_position=jnp.zeros((), jnp.int32),
+        key=key,
+    )
 
-  def insert(self, buffer_state: ReplayBufferState,
-             samples: Sample) -> ReplayBufferState:
+  def check_can_insert(self, buffer_state, samples, shards):
+    """Checks whether insert operation can be performed."""
+    assert isinstance(shards, int), 'This method should not be JITed.'
+    insert_size = jax.tree_flatten(samples)[0][0].shape[0] // shards
+    if self._data_shape[0] < insert_size:
+      raise ValueError(
+          'Trying to insert a batch of samples larger than the maximum replay'
+          f' size. num_samples: {insert_size}, max replay size'
+          f' {self._data_shape[0]}'
+      )
+    self._size = min(self._data_shape[0], self._size + insert_size)
+
+  def insert_internal(
+      self, buffer_state: ReplayBufferState, samples: Sample
+  ) -> ReplayBufferState:
     """Insert data in the replay buffer.
 
     Args:
       buffer_state: Buffer state
       samples: Sample to insert with a leading batch size.
 
     Returns:
       New buffer state.
     """
     if buffer_state.data.shape != self._data_shape:
       raise ValueError(
           f'buffer_state.data.shape ({buffer_state.data.shape}) '
-          f'doesn\'t match the expected value ({self._data_shape})')
+          f"doesn't match the expected value ({self._data_shape})"
+      )
 
     update = self._flatten_fn(samples)
     data = buffer_state.data
 
-    # Make sure update is not larger than the maximum replay size.
-    if len(update) > len(data):
-      raise ValueError(
-          'Trying to insert a batch of samples larger than the maximum replay '
-          f'size. num_samples: {len(update)}, max replay size {len(data)}')
-
     # If needed, roll the buffer to make sure there's enough space to fit
     # `update` after the current position.
-    position = buffer_state.current_position
+    position = buffer_state.insert_position
     roll = jnp.minimum(0, len(data) - position - len(update))
-    data = jax.lax.cond(roll, lambda: jnp.roll(data, roll, axis=0),
-                        lambda: data)
+    data = jax.lax.cond(
+        roll, lambda: jnp.roll(data, roll, axis=0), lambda: data
+    )
     position = position + roll
 
     # Update the buffer and the control numbers.
     data = jax.lax.dynamic_update_slice_in_dim(data, update, position, axis=0)
-    position = (position + len(update)) % len(data)
-    size = jnp.minimum(buffer_state.current_size + len(update), len(data))
+    position = (position + len(update)) % (len(data) + 1)
+    sample_position = jnp.maximum(0, buffer_state.sample_position + roll)
 
     return buffer_state.replace(
-        data=data, current_position=position, current_size=size)
+        data=data,
+        insert_position=position,
+        sample_position=sample_position,
+    )
 
-  def sample(
-      self,
-      buffer_state: ReplayBufferState) -> Tuple[ReplayBufferState, Sample]:
+  def sample_internal(
+      self, buffer_state: ReplayBufferState
+  ) -> Tuple[ReplayBufferState, Sample]:
     raise NotImplementedError(f'{self.__class__}.sample() is not implemented.')
 
   def size(self, buffer_state: ReplayBufferState) -> int:
-    return buffer_state.current_size  # pytype: disable=bad-return-type  # jax-ndarray
+    return buffer_state.insert_position - buffer_state.sample_position  # pytype: disable=bad-return-type  # jax-ndarray
 
 
 class Queue(QueueBase[Sample], Generic[Sample]):
   """Implements a limited-size queue replay buffer."""
 
-  def sample(
+  def __init__(
       self,
-      buffer_state: ReplayBufferState) -> Tuple[ReplayBufferState, Sample]:
+      max_replay_size: int,
+      dummy_data_sample: Sample,
+      sample_batch_size: int,
+      cyclic: bool = False,
+  ):
+    """Initializes the queue.
+
+    Args:
+      max_replay_size: Maximum number of elements queue can have.
+      dummy_data_sample: Example record to be stored in the queue, it is used to
+        derive shapes.
+      sample_batch_size: How many elements sampling from the queue should return
+        in a batch.
+      cyclic: Should sampling from the queue behave cyclicly, ie. once recently
+        inserted element was sampled, sampling starts from the beginning of the
+        buffer. For example, if the current queue content is [0, 1, 2] and
+        `sample_batch_size` is 2, then consecutive calls to sample will give:
+        [0, 1], [2, 0], [1, 2]...
+    """
+    super().__init__(max_replay_size, dummy_data_sample, sample_batch_size)
+    self._cyclic = cyclic
+
+  def check_can_sample(self, buffer_state, shards):
+    """Checks whether sampling can be performed. Do not JIT this method."""
+    assert isinstance(shards, int), 'This method should not be JITed.'
+    if self._size < self._sample_batch_size:
+      raise ValueError(
+          f'Trying to sample {self._sample_batch_size * shards} elements, but'
+          f' only {self._size * shards} available.'
+      )
+    if not self._cyclic:
+      self._size -= self._sample_batch_size
+
+  def sample_internal(
+      self, buffer_state: ReplayBufferState
+  ) -> Tuple[ReplayBufferState, Sample]:
     """Sample a batch of data.
 
     Args:
       buffer_state: Buffer state
 
     Returns:
       New buffer state and a batch with leading dimension 'sample_batch_size'.
@@ -156,64 +230,59 @@
       raise ValueError(
           f'Data shape expected by the replay buffer ({self._data_shape}) does '
           f'not match the shape of the buffer state ({buffer_state.data.shape})'
       )
 
     # Note that this may be out of bound, but the operations below would still
     # work fine as they take this number modulo the buffer size.
-    first_element_idx = (
-        buffer_state.current_position - buffer_state.current_size)
-    idx = jnp.arange(self._sample_batch_size) + first_element_idx
+    idx = (jnp.arange(self._sample_batch_size) + buffer_state.sample_position) % buffer_state.insert_position
 
     flat_batch = jnp.take(buffer_state.data, idx, axis=0, mode='wrap')
 
-    # TODO: Raise an error instead of padding with zeros
-    #                    when the buffer does not contain enough elements.
-    # If the sample batch size is larger than the number of elements in the
-    # queue, `mask` would contain 0s for all elements that are past the current
-    # position. Otherwise, `mask` will be only ones.
-    # mask.shape = (self._sample_batch_size,)
-    mask = idx < buffer_state.current_position
-    # mask.shape = (self._sample_batch_size, 1)
-    mask = jnp.expand_dims(mask, axis=range(1, flat_batch.ndim))
-    flat_batch = flat_batch * mask
-
-    # The effective size of the sampled batch.
-    sample_size = jnp.minimum(self._sample_batch_size,
-                              buffer_state.current_size)
     # Remove the sampled batch from the queue.
-    new_state = buffer_state.replace(current_size=buffer_state.current_size -
-                                     sample_size)
+    sample_position = buffer_state.sample_position + self._sample_batch_size
+    if self._cyclic:
+      sample_position = sample_position % buffer_state.insert_position
+
+    new_state = buffer_state.replace(sample_position=sample_position)
     return new_state, self._unflatten_fn(flat_batch)
 
+  def size(self, buffer_state: ReplayBufferState) -> int:
+    if self._cyclic:
+      return buffer_state.insert_position  # pytype: disable=bad-return-type  # jax-ndarray
+    else:
+      return buffer_state.insert_position - buffer_state.sample_position  # pytype: disable=bad-return-type  # jax-ndarray
+
 
 class UniformSamplingQueue(QueueBase[Sample], Generic[Sample]):
   """Implements an uniform sampling limited-size replay queue.
 
   * It behaves as a limited size queue (if buffer is full it removes the oldest
     elements when new one is inserted).
   * It supports batch insertion only (no single element)
   * It performs uniform random sampling with replacement of a batch of size
     `sample_batch_size`
   """
 
-  def sample(
-      self,
-      buffer_state: ReplayBufferState) -> Tuple[ReplayBufferState, Sample]:
+  def sample_internal(
+      self, buffer_state: ReplayBufferState
+  ) -> Tuple[ReplayBufferState, Sample]:
     if buffer_state.data.shape != self._data_shape:
       raise ValueError(
           f'Data shape expected by the replay buffer ({self._data_shape}) does '
           f'not match the shape of the buffer state ({buffer_state.data.shape})'
       )
 
     key, sample_key = jax.random.split(buffer_state.key)
     idx = jax.random.randint(
-        sample_key, (self._sample_batch_size,),
-        minval=buffer_state.current_position - buffer_state.current_size,
-        maxval=buffer_state.current_position)
+        sample_key,
+        (self._sample_batch_size,),
+        minval=buffer_state.sample_position,
+        maxval=buffer_state.insert_position,
+    )
     batch = jnp.take(buffer_state.data, idx, axis=0, mode='wrap')
     return buffer_state.replace(key=key), self._unflatten_fn(batch)
 
 
 class PmapWrapper(ReplayBuffer[State, Sample]):
   """Wrapper to distribute the buffer on multiple devices.
 
@@ -223,43 +292,56 @@
   by the size of the wrapped buffer.
   The sample size is also the number of devices multiplied by the size of the
   wrapped buffer.
   This should not be used inside a pmapped function:
   You should just use the regular replay buffer in that case.
   """
 
-  def __init__(self,
-               buffer: ReplayBuffer[State, Sample],
-               local_device_count: Optional[int] = None):
+  def __init__(
+      self,
+      buffer: ReplayBuffer[State, Sample],
+      local_device_count: Optional[int] = None,
+  ):
     self._buffer = buffer
     self._num_devices = local_device_count or jax.local_device_count()
 
   def init(self, key: PRNGKey) -> State:
     key = jax.random.fold_in(key, jax.process_index())
     keys = jax.random.split(key, self._num_devices)
     return jax.pmap(self._buffer.init)(keys)
 
   # NB: In multi-hosts setups, every host is expected to give a different batch.
   def insert(self, buffer_state: State, samples: Sample) -> State:
+    self._buffer.check_can_insert(buffer_state, samples, self._num_devices)
     samples = jax.tree_util.tree_map(
-        lambda x: jnp.reshape(x, (-1, self._num_devices) + x.shape[1:]),
-        samples)
+        lambda x: jnp.reshape(x, (-1, self._num_devices) + x.shape[1:]), samples
+    )
     # This is to enforce we're gonna iterate on the start of the batch before
     # the end of the batch.
     samples = jax.tree_util.tree_map(lambda x: jnp.swapaxes(x, 0, 1), samples)
-    return jax.pmap(self._buffer.insert)(buffer_state, samples)
+    return jax.pmap(self._buffer.insert_internal)(buffer_state, samples)
 
   # NB: In multi-hosts setups, every host will get a different batch.
   def sample(self, buffer_state: State) -> Tuple[State, Sample]:
-    buffer_state, samples = jax.pmap(self._buffer.sample)(buffer_state)
+    self._buffer.check_can_sample(buffer_state, self._num_devices)
+    buffer_state, samples = jax.pmap(self._buffer.sample_internal)(buffer_state)
     samples = jax.tree_util.tree_map(lambda x: jnp.swapaxes(x, 0, 1), samples)
     samples = jax.tree_util.tree_map(
-        lambda x: jnp.reshape(x, (-1,) + x.shape[2:]), samples)
+        lambda x: jnp.reshape(x, (-1,) + x.shape[2:]), samples
+    )
     return buffer_state, samples
 
+  def insert_internal(self, buffer_state: State, samples: Sample) -> State:
+    """Insert data into the replay buffer."""
+    raise ValueError('This function should not be called.')
+
+  def sample_internal(self, buffer_state: State) -> Tuple[State, Sample]:
+    """Sample a batch of data."""
+    raise ValueError('This function should not be called.')
+
   def size(self, buffer_state: State) -> int:
     axis_name = 'x'
 
     def psize(buffer_state):
       return jax.lax.psum(self._buffer.size(buffer_state), axis_name=axis_name)
 
     return jax.pmap(psize, axis_name=axis_name)(buffer_state)[0]
@@ -277,124 +359,97 @@
   (i.e. for random sampling, each shard will sample from the data they can see).
   """
 
   def __init__(
       self,
       buffer: ReplayBuffer[State, Sample],
       mesh: jax.sharding.Mesh,
-      axis_name: str,
-      batch_partition_spec: Optional[jax.sharding.PartitionSpec] = None,
+      axis_names: Sequence[str],
   ):
     """Constructor.
 
     Args:
       buffer: The buffer to replicate.
       mesh: Device mesh for pjitting context.
-      axis_name: The axis along which the replay buffer data should be
+      axis_names: The axes along which the replay buffer data should be
         partitionned.
-      batch_partition_spec: PartitionSpec of the inserted/sampled batch.
     """
     self._buffer = buffer
     self._mesh = mesh
-    num_devices = mesh.shape[axis_name]
+    self._num_devices = math.prod(mesh.shape[name] for name in axis_names)
 
     def init(key: PRNGKey) -> State:
-      keys = jax.random.split(key, num_devices)
+      keys = jax.random.split(key, self._num_devices)
       return jax.vmap(self._buffer.init)(keys)
 
     def insert(buffer_state: State, samples: Sample) -> State:
       samples = jax.tree_util.tree_map(
-          lambda x: jnp.reshape(x, (-1, num_devices) + x.shape[1:]), samples)
+          lambda x: jnp.reshape(x, (-1, self._num_devices) + x.shape[1:]),
+          samples,
+      )
       # This is to enforce we're gonna iterate on the start of the batch before
       # the end of the batch.
       samples = jax.tree_util.tree_map(lambda x: jnp.swapaxes(x, 0, 1), samples)
-      return jax.vmap(self._buffer.insert)(buffer_state, samples)
+      return jax.vmap(self._buffer.insert_internal)(buffer_state, samples)
 
     def sample(buffer_state: State) -> Tuple[State, Sample]:
-      buffer_state, samples = jax.vmap(self._buffer.sample)(buffer_state)
+      buffer_state, samples = jax.vmap(self._buffer.sample_internal)(
+          buffer_state
+      )
       samples = jax.tree_util.tree_map(lambda x: jnp.swapaxes(x, 0, 1), samples)
       samples = jax.tree_util.tree_map(
-          lambda x: jnp.reshape(x, (-1,) + x.shape[2:]), samples)
+          lambda x: jnp.reshape(x, (-1,) + x.shape[2:]), samples
+      )
       return buffer_state, samples
 
     def size(buffer_state: State) -> int:
       return jnp.sum(jax.vmap(self._buffer.size)(buffer_state))
 
-    partition_spec = jax.sharding.PartitionSpec((axis_name,))
-    self._partitioned_init = pjit.pjit(
-        init, in_shardings=None, out_shardings=partition_spec
-    )
+    partition_spec = jax.sharding.PartitionSpec((axis_names),)
+    self._partitioned_init = pjit.pjit(init, out_shardings=partition_spec)
     self._partitioned_insert = pjit.pjit(
         insert,
-        in_shardings=(partition_spec, batch_partition_spec),
         out_shardings=partition_spec,
     )
     self._partitioned_sample = pjit.pjit(
         sample,
-        in_shardings=partition_spec,
-        out_shardings=(partition_spec, batch_partition_spec),
+        out_shardings=partition_spec,
     )
     # This will return the TOTAL size across all devices.
-    self._partitioned_size = pjit.pjit(
-        size, in_shardings=partition_spec, out_shardings=None
-    )
+    self._partitioned_size = pjit.pjit(size, out_shardings=None)
 
   def init(self, key: PRNGKey) -> State:
     """See base class."""
     with self._mesh:
       return self._partitioned_init(key)
 
   def insert(self, buffer_state: State, samples: Sample) -> State:
     """See base class."""
+    self._buffer.check_can_insert(buffer_state, samples, self._num_devices)
     with self._mesh:
       return self._partitioned_insert(buffer_state, samples)
 
   def sample(self, buffer_state: State) -> Tuple[State, Sample]:
     """See base class."""
+    self._buffer.check_can_sample(buffer_state, self._num_devices)
     with self._mesh:
       return self._partitioned_sample(buffer_state)
 
   def size(self, buffer_state: State) -> int:
     """See base class. The total size (sum of all partitions) is returned."""
     with self._mesh:
       return self._partitioned_size(buffer_state)
 
+  def insert_internal(self, buffer_state: State, samples: Sample) -> State:
+    """Insert data into the replay buffer."""
+    raise ValueError('This function should not be called.')
+
+  def sample_internal(self, buffer_state: State) -> Tuple[State, Sample]:
+    """Sample a batch of data."""
+    raise ValueError('This function should not be called.')
+
 
 @flax.struct.dataclass
 class PrimitiveReplayBufferState(Generic[Sample]):
   """The state of the primitive replay buffer."""
 
   samples: Optional[Sample] = None
-
-
-class PrimitiveReplayBuffer(
-    ReplayBuffer[PrimitiveReplayBufferState[Sample], Sample], Generic[Sample]
-):
-  """A primitive queue that can contain at most one batch of samples."""
-
-  def init(self, key: PRNGKey) -> PrimitiveReplayBufferState[Sample]:
-    """Init the replay buffer."""
-    return PrimitiveReplayBufferState(samples=None)
-
-  def insert(
-      self, buffer_state: PrimitiveReplayBufferState[Sample], samples: Sample
-  ) -> PrimitiveReplayBufferState[Sample]:
-    """Insert data in the replay buffer."""
-    if buffer_state.samples is not None:
-      raise ValueError('The buffer is full')
-    return PrimitiveReplayBufferState(samples=samples)
-
-  def sample(
-      self, buffer_state: PrimitiveReplayBufferState[Sample]
-  ) -> Tuple[PrimitiveReplayBufferState[Sample], Sample]:
-    """Sample a batch of data."""
-    if buffer_state.samples is None:
-      raise ValueError('The buffer is empty')
-    return PrimitiveReplayBufferState(samples=None), buffer_state.samples
-
-  def size(self, buffer_state: PrimitiveReplayBufferState[Sample]) -> int:
-    """Return the total amount of elements that are sampleable."""
-    return (
-        jax.tree_flatten(buffer_state.samples)[0][0].shape[0]
-        if buffer_state.samples is not None
-        else 0
-    )
```

### Comparing `brax-0.9.0/brax/training/spectral_norm.py` & `brax-0.9.1/brax/training/spectral_norm.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/training/types.py` & `brax-0.9.1/brax/training/types.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/__init__.py` & `brax-0.9.1/brax/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/__init__.py` & `brax-0.9.1/brax/v1/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/acrobot.py` & `brax-0.9.1/brax/v1/envs/acrobot.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/ant.py` & `brax-0.9.1/brax/v1/envs/ant.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/env.py` & `brax-0.9.1/brax/v1/envs/env.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/fast.py` & `brax-0.9.1/brax/v1/envs/fast.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/fetch.py` & `brax-0.9.1/brax/v1/envs/fetch.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/grasp.py` & `brax-0.9.1/brax/v1/envs/grasp.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/half_cheetah.py` & `brax-0.9.1/brax/v1/envs/half_cheetah.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/hopper.py` & `brax-0.9.1/brax/v1/envs/hopper.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/humanoid.py` & `brax-0.9.1/brax/v1/envs/humanoid.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/humanoid_standup.py` & `brax-0.9.1/brax/v1/envs/humanoid_standup.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/inverted_double_pendulum.py` & `brax-0.9.1/brax/v1/envs/inverted_double_pendulum.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/inverted_pendulum.py` & `brax-0.9.1/brax/v1/envs/inverted_pendulum.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/pusher.py` & `brax-0.9.1/brax/v1/envs/pusher.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/reacher.py` & `brax-0.9.1/brax/v1/envs/reacher.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/reacherangle.py` & `brax-0.9.1/brax/v1/envs/reacherangle.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/swimmer.py` & `brax-0.9.1/brax/v1/envs/swimmer.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/to_torch.py` & `brax-0.9.1/brax/v1/envs/to_torch.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/ur5e.py` & `brax-0.9.1/brax/v1/envs/ur5e.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/walker2d.py` & `brax-0.9.1/brax/v1/envs/walker2d.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/envs/wrappers.py` & `brax-0.9.1/brax/v1/envs/wrappers.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/__init__.py` & `brax-0.9.1/brax/training/agents/sac/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/__init__.py` & `brax-0.9.1/brax/v1/experimental/biggym/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/registry/__init__.py` & `brax-0.9.1/brax/v1/experimental/biggym/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/registry/ant/__init__.py` & `brax-0.9.1/brax/v1/experimental/biggym/registry/ant/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/registry/ant/components/__init__.py` & `brax-0.9.1/brax/v1/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/registry/ant/components/ant.py` & `brax-0.9.1/brax/v1/experimental/biggym/registry/ant/components/ant.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/registry/jump/__init__.py` & `brax-0.9.1/brax/v1/experimental/biggym/registry/jump/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/registry/jump/envs/__init__.py` & `brax-0.9.1/brax/v1/experimental/biggym/registry/ant/components/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/registry/jump/envs/cheetah.py` & `brax-0.9.1/brax/v1/experimental/biggym/registry/jump/envs/cheetah.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/registry/proant/__init__.py` & `brax-0.9.1/brax/v1/experimental/biggym/registry/proant/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/registry/proant/components/__init__.py` & `brax-0.9.1/brax/v1/experimental/biggym/registry/jump/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/registry/proant/components/ant.py` & `brax-0.9.1/brax/v1/experimental/biggym/registry/proant/components/ant.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/registry/proant/envs/__init__.py` & `brax-0.9.1/brax/v1/experimental/biggym/registry/proant/components/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/registry/proant/envs/ant.py` & `brax-0.9.1/brax/v1/experimental/biggym/registry/proant/envs/ant.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/biggym/tasks.py` & `brax-0.9.1/brax/v1/experimental/biggym/tasks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/__init__.py` & `brax-0.9.1/brax/v1/experimental/biggym/registry/proant/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/common/__init__.py` & `brax-0.9.1/brax/v1/experimental/braxlines/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/common/config_utils.py` & `brax-0.9.1/brax/v1/experimental/braxlines/common/config_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/common/dist_utils.py` & `brax-0.9.1/brax/v1/experimental/braxlines/common/dist_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/common/evaluators.py` & `brax-0.9.1/brax/v1/experimental/braxlines/common/evaluators.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/common/logger_utils.py` & `brax-0.9.1/brax/v1/experimental/braxlines/common/logger_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/common/sim_utils.py` & `brax-0.9.1/brax/v1/experimental/braxlines/common/sim_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/envs/__init__.py` & `brax-0.9.1/brax/v1/experimental/braxlines/common/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/envs/obs_indices.py` & `brax-0.9.1/brax/v1/experimental/braxlines/envs/obs_indices.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/envs/wrappers.py` & `brax-0.9.1/brax/v1/experimental/braxlines/envs/wrappers.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/experiments/__init__.py` & `brax-0.9.1/brax/v1/experimental/braxlines/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/experiments/chase_ma_sweep.py` & `brax-0.9.1/brax/v1/experimental/braxlines/experiments/chase_ma_sweep.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/experiments/composer_sweep.py` & `brax-0.9.1/brax/v1/experimental/braxlines/experiments/composer_sweep.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/experiments/defaults.py` & `brax-0.9.1/brax/v1/experimental/braxlines/experiments/defaults.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/experiments/dmin_sweep.py` & `brax-0.9.1/brax/v1/experimental/braxlines/experiments/dmin_sweep.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/experiments/mimax_sweep.py` & `brax-0.9.1/brax/v1/experimental/braxlines/experiments/mimax_sweep.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/experiments/sumo_ma_sweep.py` & `brax-0.9.1/brax/v1/experimental/braxlines/experiments/sumo_ma_sweep.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/irl_smm/__init__.py` & `brax-0.9.1/brax/v1/experimental/braxlines/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/irl_smm/evaluators.py` & `brax-0.9.1/brax/v1/experimental/braxlines/irl_smm/evaluators.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/irl_smm/train.py` & `brax-0.9.1/brax/v1/experimental/braxlines/irl_smm/train.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/irl_smm/utils.py` & `brax-0.9.1/brax/v1/experimental/braxlines/irl_smm/utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/training/__init__.py` & `brax-0.9.1/brax/v1/experimental/braxlines/irl_smm/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/training/env.py` & `brax-0.9.1/brax/v1/experimental/braxlines/training/env.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/training/ppo.py` & `brax-0.9.1/brax/v1/experimental/braxlines/training/ppo.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/training/utils.py` & `brax-0.9.1/brax/v1/experimental/braxlines/training/utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/vgcrl/__init__.py` & `brax-0.9.1/brax/v1/experimental/braxlines/training/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/vgcrl/evaluators.py` & `brax-0.9.1/brax/v1/experimental/braxlines/vgcrl/evaluators.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/vgcrl/train.py` & `brax-0.9.1/brax/v1/experimental/braxlines/vgcrl/train.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/braxlines/vgcrl/utils.py` & `brax-0.9.1/brax/v1/experimental/braxlines/vgcrl/utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/__init__.py` & `brax-0.9.1/brax/v1/experimental/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/agent_utils.py` & `brax-0.9.1/brax/v1/experimental/composer/agent_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/component_editor.py` & `brax-0.9.1/brax/v1/experimental/composer/component_editor.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/components/__init__.py` & `brax-0.9.1/brax/v1/experimental/composer/components/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/components/ant.py` & `brax-0.9.1/brax/v1/experimental/composer/components/ant.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/components/common.py` & `brax-0.9.1/brax/v1/experimental/composer/components/common.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/components/ground.py` & `brax-0.9.1/brax/v1/experimental/composer/components/ground.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/components/halfcheetah.py` & `brax-0.9.1/brax/v1/experimental/composer/components/halfcheetah.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/components/humanoid.py` & `brax-0.9.1/brax/v1/experimental/composer/components/humanoid.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/components/octopus.py` & `brax-0.9.1/brax/v1/experimental/composer/components/octopus.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/components/pro_ant.py` & `brax-0.9.1/brax/v1/experimental/composer/components/pro_ant.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/components/singleton.py` & `brax-0.9.1/brax/v1/experimental/composer/components/singleton.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/composer.py` & `brax-0.9.1/brax/v1/experimental/composer/composer.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/composer_utils.py` & `brax-0.9.1/brax/v1/experimental/composer/composer_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/data_utils.py` & `brax-0.9.1/brax/v1/experimental/composer/data_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/envs/__init__.py` & `brax-0.9.1/brax/v1/experimental/composer/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/envs/ma_descs.py` & `brax-0.9.1/brax/v1/experimental/composer/envs/ma_descs.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/envs/sa_descs.py` & `brax-0.9.1/brax/v1/experimental/composer/envs/sa_descs.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/observers.py` & `brax-0.9.1/brax/v1/experimental/composer/observers.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/reward_functions.py` & `brax-0.9.1/brax/v1/experimental/composer/reward_functions.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/tests/__init__.py` & `brax-0.9.1/brax/v1/experimental/braxlines/vgcrl/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/tests/composer_test.py` & `brax-0.9.1/brax/v1/experimental/composer/tests/composer_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/train.py` & `brax-0.9.1/brax/v1/experimental/composer/train.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/training/__init__.py` & `brax-0.9.1/brax/v1/experimental/composer/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/composer/training/mappo.py` & `brax-0.9.1/brax/v1/experimental/composer/training/mappo.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/normalization.py` & `brax-0.9.1/brax/v1/experimental/normalization.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/tracing/__init__.py` & `brax-0.9.1/brax/v1/experimental/composer/training/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/tracing/customize.py` & `brax-0.9.1/brax/v1/experimental/tracing/customize.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/tracing/randomizers.py` & `brax-0.9.1/brax/v1/experimental/tracing/randomizers.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/tracing/wrappers.py` & `brax-0.9.1/brax/v1/experimental/tracing/wrappers.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/experimental/tracing/wrappers_test.py` & `brax-0.9.1/brax/v1/experimental/tracing/wrappers_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/io/__init__.py` & `brax-0.9.1/brax/v1/experimental/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/io/export.py` & `brax-0.9.1/brax/v1/io/export.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/io/file.py` & `brax-0.9.1/brax/v1/io/file.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/io/html.py` & `brax-0.9.1/brax/v1/io/html.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/io/image.py` & `brax-0.9.1/brax/v1/io/image.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/io/json.py` & `brax-0.9.1/brax/v1/io/json.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/io/mesh.py` & `brax-0.9.1/brax/v1/io/mesh.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/io/metrics.py` & `brax-0.9.1/brax/v1/io/metrics.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/io/model.py` & `brax-0.9.1/brax/v1/io/model.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/io/npy_file.py` & `brax-0.9.1/brax/v1/io/npy_file.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/io/torch.py` & `brax-0.9.1/brax/v1/io/torch.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/jumpy.py` & `brax-0.9.1/brax/v1/jumpy.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/math.py` & `brax-0.9.1/brax/v1/math.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/physics/__init__.py` & `brax-0.9.1/brax/v1/io/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/physics/actuators.py` & `brax-0.9.1/brax/v1/physics/actuators.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/physics/base.py` & `brax-0.9.1/brax/v1/physics/base.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/physics/bodies.py` & `brax-0.9.1/brax/v1/physics/bodies.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/physics/colliders.py` & `brax-0.9.1/brax/v1/physics/colliders.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/physics/config_pb2.py` & `brax-0.9.1/brax/v1/physics/config_pb2.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/physics/forces.py` & `brax-0.9.1/brax/v1/physics/forces.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/physics/geometry.py` & `brax-0.9.1/brax/v1/physics/geometry.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/physics/integrators.py` & `brax-0.9.1/brax/v1/physics/integrators.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/physics/joints.py` & `brax-0.9.1/brax/v1/physics/joints.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/physics/spring_joints.py` & `brax-0.9.1/brax/v1/physics/spring_joints.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/physics/system.py` & `brax-0.9.1/brax/v1/physics/system.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/pytree.py` & `brax-0.9.1/brax/v1/pytree.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tests/__init__.py` & `brax-0.9.1/brax/v1/physics/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tests/colliders_test.py` & `brax-0.9.1/brax/v1/tests/colliders_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tests/env_test.py` & `brax-0.9.1/brax/v1/tests/env_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tests/geometry_test.py` & `brax-0.9.1/brax/v1/tests/geometry_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tests/grasp_test.py` & `brax-0.9.1/brax/v1/tests/grasp_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tests/jumpy_test.py` & `brax-0.9.1/brax/v1/tests/jumpy_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tests/math_test.py` & `brax-0.9.1/brax/v1/tests/math_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tests/physics_legacy_test.py` & `brax-0.9.1/brax/v1/tests/physics_legacy_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tests/physics_test.py` & `brax-0.9.1/brax/v1/tests/physics_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tests/running_statistics_test.py` & `brax-0.9.1/brax/v1/tests/running_statistics_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tests/urdf_test.py` & `brax-0.9.1/brax/v1/tests/urdf_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tools/__init__.py` & `brax-0.9.1/brax/v1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tools/mujoco.py` & `brax-0.9.1/brax/v1/tools/mujoco.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tools/mujoco_converter.py` & `brax-0.9.1/brax/v1/tools/mujoco_converter.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tools/print_mesh_com.py` & `brax-0.9.1/brax/v1/tools/print_mesh_com.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tools/urdf.py` & `brax-0.9.1/brax/v1/tools/urdf.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/v1/tools/urdf_converter.py` & `brax-0.9.1/brax/v1/tools/urdf_converter.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/visualizer/favicon.ico` & `brax-0.9.1/brax/visualizer/favicon.ico`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/visualizer/index.html` & `brax-0.9.1/brax/visualizer/index.html`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/visualizer/js/animator.js` & `brax-0.9.1/brax/visualizer/js/animator.js`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/visualizer/js/selector.js` & `brax-0.9.1/brax/visualizer/js/selector.js`

 * *Files identical despite different names*

### Comparing `brax-0.9.0/brax/visualizer/js/system.js` & `brax-0.9.1/brax/visualizer/js/system.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -49,14 +49,24 @@
     for (let i = 0; i < geom.vert.length; i++) {
         let v = geom.vert[i];
         size = Math.max(v[0], v[1], v[2], size);
     }
     return size * 2;
 }
 
+function createCylinder(radius, height, mat) {
+    const geometry = new THREE.CylinderGeometry(radius, radius, height, 32);
+    mat.side = THREE.DoubleSide;
+    const cyl = new THREE.Mesh(geometry, mat);
+    cyl.baseMaterial = cyl.material;
+    cyl.castShadow = true;
+    cyl.layers.enable(1);
+    return cyl;
+}
+
 function createCapsule(capsule, mat) {
     const sphere_geom = new THREE.SphereGeometry(capsule.radius, 16, 16);
     const cylinder_geom = new THREE.CylinderGeometry(
         capsule.radius, capsule.radius, capsule.length);
 
     const sphere1 = new THREE.Mesh(sphere_geom, mat);
     sphere1.baseMaterial = sphere1.material;
@@ -78,15 +88,15 @@
 
     const group = new THREE.Group();
     group.add(sphere1, sphere2, cylinder);
     return group;
 }
 
 function createBox(box, mat) {
-    const geom = new THREE.BoxBufferGeometry(
+    const geom = new THREE.BoxGeometry(
         2 * box.halfsize[0], 2 * box.halfsize[1], 2 * box.halfsize[2]);
     const mesh = new THREE.Mesh(geom, mat);
     mesh.castShadow = true;
     mesh.baseMaterial = mesh.material;
     mesh.layers.enable(1);
     return mesh;
 }
@@ -139,14 +149,15 @@
         Object.entries(system.meshes).forEach(function(geom) {
             meshGeoms[geom[0]] = geom[1];
         });
     }
 
     // Add a world axis for debugging.
     const worldAxis = new THREE.AxesHelper(100);
+    const qRotx90 = new THREE.Quaternion(0.70710677, 0.0, 0.0, 0.7071067);
     worldAxis.visible = false;
     scene.add(worldAxis);
 
     let minAxisSize = 1e6;
     Object.entries(system.geoms).forEach(function(geom) {
         const name = geom[0];
         const parent = new THREE.Group();
@@ -179,25 +190,32 @@
                 axisSize = getSphereAxisSize(collider);
             } else if (collider.name == 'HeightMap') {
                 console.log('heightMap not implemented');
                 return;
             } else if (collider.name == 'Mesh') {
                 child = createMesh(collider, mat);
                 axisSize = getMeshAxisSize(collider);
+            } else if (collider.name == 'Cylinder') {
+                child = createCylinder(collider.radius, collider.length, mat);
+                axisSize = 2 * Math.max(collider.radius, collider.length);
             } else if ('clippedPlane' in collider) {
                 console.log('clippedPlane not implemented');
                 return;
             } else if (collider.name == 'Convex') {
                 console.log('convex not implemented');
                 return;
             }
             if (collider.transform.rot) {
-                child.quaternion.set(
+                const quat = new THREE.Quaternion(
                     collider.transform.rot[1], collider.transform.rot[2],
                     collider.transform.rot[3], collider.transform.rot[0]);
+                if (collider.name == 'Cylinder') {
+                    quat.multiply(qRotx90)
+                }
+                child.quaternion.fromArray(quat.toArray());
             }
             if (collider.transform.pos) {
                 child.position.set(
                     collider.transform.pos[0], collider.transform.pos[1],
                     collider.transform.pos[2]);
             }
             if (axisSize) {
```

### Comparing `brax-0.9.0/brax/visualizer/js/viewer.js` & `brax-0.9.1/brax/visualizer/js/viewer.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -111,15 +111,15 @@
             alpha: true
         });
         this.renderer.shadowMap.enabled = true;
         this.renderer.outputEncoding = THREE.sRGBEncoding;
 
         this.domElement.appendChild(this.renderer.domElement);
 
-        this.camera = new THREE.PerspectiveCamera(40, 1, 0.01, 100);
+        this.camera = new THREE.PerspectiveCamera(40, 1, 0.1, 100);
         this.camera.position.set(5, 8, 2);
         this.camera.follow = true;
         this.camera.freezeAngle = false;
         this.camera.followDistance = 10;
 
         this.scene.background = new THREE.Color(0xa0a0a0);
         this.scene.fog = new THREE.Fog(0xa0a0a0, 40, 60);
```

### Comparing `brax-0.9.0/brax/visualizer/visualizer.py` & `brax-0.9.1/brax/visualizer/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,17 +85,17 @@
       'generalized': generalized,
       'positional': positional,
       'spring': spring,
   }[request.args.get('pipeline', 'generalized')]
   steps = int(request.args.get('steps', 1000))
   act_fn = request.args.get('act', 'sin')
   solver_iterations = int(request.args.get('solver_iterations', 100))
-  force_floor = request.args.get('force_floor', 'true').lower() == 'true'
-  add_floor = request.args.get('add_floor', 'true').lower() == 'true'
-  add_act = request.args.get('add_act', 'true').lower() == 'true'
+  force_floor = request.args.get('force_floor', 'false').lower() == 'true'
+  add_floor = request.args.get('add_floor', 'false').lower() == 'true'
+  add_act = request.args.get('add_act', 'false').lower() == 'true'
 
   is_mesh = lambda g: isinstance(g, Mesh) and not isinstance(g, Convex)
 
   if force_floor:
     floors = [g for g in sys.geoms if isinstance(g, Plane)]
     if floors:
       floor = floors[0]
```

### Comparing `brax-0.9.0/brax.egg-info/PKG-INFO` & `brax-0.9.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: brax
-Version: 0.9.0
-Summary: A differentiable physics engine written in JAX.
-Home-page: http://github.com/google/brax
-Author: Brax Authors
-Author-email: no-reply@google.com
-License: Apache 2.0
-Keywords: JAX reinforcement learning rigidbody physics
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-Provides-Extra: develop
-License-File: LICENSE
-
 <img src="https://github.com/google/brax/raw/main/docs/img/brax_logo.gif" width="336" height="80" alt="BRAX"/>
 
 Brax is a fast and fully differentiable physics engine used for research and
 development of robotics, human perception, materials science, reinforcement
 learning, and other simulation-heavy applications.
 
 Brax is written in [JAX](https://github.com/google/jax) and is designed for use
@@ -59,17 +40,16 @@
 and closing the gap between simulation and the real world.
 
 ## Quickstart: Colab in the Cloud
 
 Explore Brax easily and quickly through a series of colab notebooks:
 
 * [Brax Basics](https://colab.research.google.com/github/google/brax/blob/main/notebooks/basics.ipynb) introduces the Brax API, and shows how to simulate basic physics primitives.
-* [Brax Training](https://colab.research.google.com/github/google/brax/blob/main/notebooks/training.ipynb)
-introduces the Brax v2 API, and shows how to train a policy with the
-generalized backend.
+* [Brax Training](https://colab.research.google.com/github/google/brax/blob/main/notebooks/training.ipynb) introduces Brax's training algorithms, and lets you train your own policies directly within the colab. It also demonstrates loading and saving policies.
+* [Brax Training with PyTorch on GPU](https://colab.research.google.com/github/google/brax/blob/main/notebooks/training_torch.ipynb) demonstrates how Brax can be used in other ML frameworks for fast training, in this case PyTorch.
 
 ## Using Brax Locally
 
 To install Brax from pypi, install it with:
 
 ```
 python3 -m venv env
@@ -113,15 +93,15 @@
 If you would like to reference Brax in a publication, please use:
 
 ```
 @software{brax2021github,
   author = {C. Daniel Freeman and Erik Frey and Anton Raichuk and Sertan Girgin and Igor Mordatch and Olivier Bachem},
   title = {Brax - A Differentiable Physics Engine for Large Scale Rigid Body Simulation},
   url = {http://github.com/google/brax},
-  version = {0.9.0},
+  version = {0.9.1},
   year = {2021},
 }
 ```
 
 ## Acknowledgements
 
 Brax has come a long way since its original publication.  We offer gratitude and
```

### Comparing `brax-0.9.0/brax.egg-info/SOURCES.txt` & `brax-0.9.1/brax.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,51 +5,57 @@
 bin/learn
 brax/__init__.py
 brax/actuator.py
 brax/actuator_test.py
 brax/base.py
 brax/com.py
 brax/com_test.py
+brax/fluid.py
+brax/fluid_test.py
 brax/kinematics.py
 brax/kinematics_test.py
 brax/math.py
 brax/math_test.py
 brax/scan.py
 brax/scan_test.py
 brax/test_utils.py
 brax.egg-info/PKG-INFO
 brax.egg-info/SOURCES.txt
 brax.egg-info/dependency_links.txt
 brax.egg-info/requires.txt
 brax.egg-info/top_level.txt
 brax/envs/__init__.py
 brax/envs/ant.py
-brax/envs/env.py
+brax/envs/base.py
 brax/envs/env_test.py
 brax/envs/fast.py
 brax/envs/half_cheetah.py
 brax/envs/hopper.py
 brax/envs/humanoid.py
 brax/envs/humanoidstandup.py
 brax/envs/inverted_double_pendulum.py
 brax/envs/inverted_pendulum.py
 brax/envs/pusher.py
 brax/envs/reacher.py
 brax/envs/walker2d.py
-brax/envs/wrapper.py
 brax/envs/assets/ant.xml
 brax/envs/assets/half_cheetah.xml
 brax/envs/assets/hopper.xml
 brax/envs/assets/humanoid.xml
 brax/envs/assets/humanoidstandup.xml
 brax/envs/assets/inverted_double_pendulum.xml
 brax/envs/assets/inverted_pendulum.xml
 brax/envs/assets/pusher.xml
 brax/envs/assets/reacher.xml
 brax/envs/assets/walker2d.xml
+brax/envs/wrappers/__init__.py
+brax/envs/wrappers/dm_env.py
+brax/envs/wrappers/gym.py
+brax/envs/wrappers/torch.py
+brax/envs/wrappers/training.py
 brax/generalized/__init__.py
 brax/generalized/base.py
 brax/generalized/constraint.py
 brax/generalized/constraint_test.py
 brax/generalized/dynamics.py
 brax/generalized/dynamics_test.py
 brax/generalized/integrator.py
@@ -63,20 +69,23 @@
 brax/geometry/contact_test.py
 brax/geometry/math.py
 brax/geometry/math_test.py
 brax/geometry/mesh.py
 brax/geometry/mesh_test.py
 brax/io/__init__.py
 brax/io/html.py
+brax/io/image.py
+brax/io/image_test.py
 brax/io/json.py
 brax/io/json_test.py
 brax/io/metrics.py
 brax/io/mjcf.py
 brax/io/mjcf_test.py
 brax/io/model.py
+brax/io/torch.py
 brax/positional/__init__.py
 brax/positional/base.py
 brax/positional/collisions.py
 brax/positional/integrator.py
 brax/positional/joints.py
 brax/positional/joints_test.py
 brax/positional/perf_test.py
@@ -92,43 +101,66 @@
 brax/spring/pipeline.py
 brax/spring/pipeline_test.py
 brax/test_data/capsule.xml
 brax/test_data/colour_objects.xml
 brax/test_data/convex_convex.xml
 brax/test_data/double_pendulum.xml
 brax/test_data/double_prismatic.xml
+brax/test_data/fat_cylinder.xml
+brax/test_data/flat_cylinder.xml
+brax/test_data/fluid_box.xml
+brax/test_data/fluid_box_offset_com.xml
+brax/test_data/fluid_ellipsoid.xml
+brax/test_data/fluid_sphere.xml
+brax/test_data/fluid_two_spheres.xml
+brax/test_data/fluid_wind.xml
 brax/test_data/nonzero_joint_ref.xml
 brax/test_data/prismaversal_2dof_joint.xml
 brax/test_data/prismaversal_3dof_joint.xml
 brax/test_data/single_pendulum.xml
 brax/test_data/single_pendulum_motor.xml
 brax/test_data/single_pendulum_position.xml
+brax/test_data/single_pendulum_position_frclimit.xml
+brax/test_data/single_pendulum_velocity.xml
 brax/test_data/single_prismatic.xml
 brax/test_data/single_spherical_pendulum.xml
 brax/test_data/single_spherical_pendulum_motor.xml
 brax/test_data/single_spherical_pendulum_position.xml
 brax/test_data/single_universal_pendulum.xml
+brax/test_data/solver_params_v2.xml
 brax/test_data/triple_pendulum.xml
 brax/test_data/triple_pendulum_motor.xml
 brax/test_data/triple_prismatic.xml
 brax/test_data/world_body_transform.xml
+brax/test_data/laikago/laikago_toes_zup.urdf
+brax/test_data/laikago/laikago_viz.urdf
 brax/test_data/laikago/meshes/chassis.obj
 brax/test_data/laikago/meshes/chassis.stl
 brax/test_data/laikago/meshes/chassis_mod.obj
 brax/test_data/laikago/meshes/chassis_vhacd.obj
 brax/test_data/laikago/meshes/chassis_vhacd_mod.obj
 brax/test_data/laikago/meshes/chassis_vhacd_mod_zup.obj
 brax/test_data/laikago/meshes/chassis_zup.obj
 brax/test_data/laikago/meshes/chassis_zup_lores.obj
 brax/test_data/laikago/meshes/hip_motor.obj
 brax/test_data/laikago/meshes/hip_motor.stl
 brax/test_data/laikago/meshes/hip_motor_lores.obj
 brax/test_data/laikago/meshes/hip_motor_mirror.obj
 brax/test_data/laikago/meshes/hip_motor_mirror.stl
 brax/test_data/laikago/meshes/hip_motor_mirror_lores.obj
+brax/test_data/laikago/meshes/laikago.urdf
+brax/test_data/laikago/meshes/laikago_no_toes.urdf
+brax/test_data/laikago/meshes/laikago_toes.urdf
+brax/test_data/laikago/meshes/laikago_toes_limits.urdf
+brax/test_data/laikago/meshes/laikago_toes_zup.urdf
+brax/test_data/laikago/meshes/laikago_toes_zup_chassis_collision.urdf
+brax/test_data/laikago/meshes/laikago_toes_zup_chassis_collision_xyz_spherical.urdf
+brax/test_data/laikago/meshes/laikago_toes_zup_joint_order.urdf
+brax/test_data/laikago/meshes/laikago_toes_zup_lores.urdf
+brax/test_data/laikago/meshes/laikago_toes_zup_xyz_xyzrot.urdf
 brax/test_data/laikago/meshes/lower_leg3.obj
 brax/test_data/laikago/meshes/lower_leg3_lores.obj
 brax/test_data/laikago/meshes/lower_leg_3.stl
 brax/test_data/laikago/meshes/lower_leg_3_collision.stl
 brax/test_data/laikago/meshes/upper_leg.stl
 brax/test_data/laikago/meshes/upper_leg_left.obj
 brax/test_data/laikago/meshes/upper_leg_left2.obj
```

### Comparing `brax-0.9.0/setup.py` & `brax-0.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,33 +20,35 @@
 """
 
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="brax",
-    version="0.9.0",
+    version="0.9.1",
     description=("A differentiable physics engine written in JAX."),
     author="Brax Authors",
     author_email="no-reply@google.com",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="http://github.com/google/brax",
     license="Apache 2.0",
     packages=find_packages(),
     include_package_data=True,
     scripts=["bin/learn"],
     install_requires=[
         "absl-py",
         "dataclasses; python_version < '3.7'",
+        # TODO: remove dm_env after dropping legacy v1 code
         "dm_env",
         "etils",
         "flask",
         "flask_cors",
         "flax",
+        # TODO: remove grpcio and gym after dropping legacy v1 code
         "grpcio",
         "gym",
         "jax>=0.4.6",
         "jaxlib>=0.4.6",
         "jaxopt",
         "jinja2",
         "mujoco",
```

