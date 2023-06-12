# Comparing `tmp/mo-gymnasium-0.3.4.tar.gz` & `tmp/mo-gymnasium-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo-gymnasium-0.3.4.tar", last modified: Tue Mar 14 15:33:08 2023, max compression
+gzip compressed data, was "mo-gymnasium-1.0.0.tar", last modified: Mon Jun 12 15:31:19 2023, max compression
```

## Comparing `mo-gymnasium-0.3.4.tar` & `mo-gymnasium-1.0.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.537449 mo-gymnasium-0.3.4/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1069 2023-01-16 13:11:30.000000 mo-gymnasium-0.3.4/LICENSE
--rw-r--r--   0 lucas     (1000) lucas     (1000)     5481 2023-03-14 15:33:08.537449 mo-gymnasium-0.3.4/PKG-INFO
--rw-r--r--   0 lucas     (1000) lucas     (1000)     4175 2023-02-13 19:42:27.000000 mo-gymnasium-0.3.4/README.md
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.457449 mo-gymnasium-0.3.4/mo_gymnasium/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      277 2023-03-14 15:25:22.000000 mo-gymnasium-0.3.4/mo_gymnasium/__init__.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.457449 mo-gymnasium-0.3.4/mo_gymnasium/envs/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      564 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/__init__.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.457449 mo-gymnasium-0.3.4/mo_gymnasium/envs/breakable_bottles/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      211 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/breakable_bottles/__init__.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     8851 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/breakable_bottles/breakable_bottles.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.467449 mo-gymnasium-0.3.4/mo_gymnasium/envs/continuous_mountain_car/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      237 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/continuous_mountain_car/__init__.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     2539 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/continuous_mountain_car/continuous_mountain_car.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.467449 mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      494 2023-03-14 13:56:48.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/__init__.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.477449 mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/assets/
--rw-r--r--   0 lucas     (1000) lucas     (1000)    14488 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/assets/Minecraft.ttf
--rw-r--r--   0 lucas     (1000) lucas     (1000)      661 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/assets/rock.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)    17738 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/assets/sea_bg.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)   106615 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/assets/submarine.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)      789 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/assets/treasure.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)    11421 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/deep_sea_treasure.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.477449 mo-gymnasium-0.3.4/mo_gymnasium/envs/fishwood/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      149 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/fishwood/__init__.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.487449 mo-gymnasium-0.3.4/mo_gymnasium/envs/fishwood/assets/
--rw-r--r--   0 lucas     (1000) lucas     (1000)    42842 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/fishwood/assets/Kawa.jpg
--rw-r--r--   0 lucas     (1000) lucas     (1000)    35586 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/fishwood/assets/Mori.jpg
--rw-r--r--   0 lucas     (1000) lucas     (1000)     3450 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/fishwood/fishwood.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.497449 mo-gymnasium-0.3.4/mo_gymnasium/envs/four_room/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      179 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/four_room/__init__.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)    12398 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/four_room/four_room.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.497449 mo-gymnasium-0.3.4/mo_gymnasium/envs/fruit_tree/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      148 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/fruit_tree/__init__.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)    21334 2023-02-11 11:41:04.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/fruit_tree/fruit_tree.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.497449 mo-gymnasium-0.3.4/mo_gymnasium/envs/highway/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      289 2023-02-13 11:12:54.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/highway/__init__.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     4415 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/highway/highway.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.497449 mo-gymnasium-0.3.4/mo_gymnasium/envs/lunar_lander/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      197 2023-02-01 09:34:12.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/lunar_lander/__init__.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     7190 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/lunar_lander/lunar_lander.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.497449 mo-gymnasium-0.3.4/mo_gymnasium/envs/mario/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      183 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/mario/__init__.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     3739 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/mario/joypad_space.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     6014 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/mario/mario.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.507449 mo-gymnasium-0.3.4/mo_gymnasium/envs/minecart/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      432 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/minecart/__init__.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.517449 mo-gymnasium-0.3.4/mo_gymnasium/envs/minecart/assets/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     3747 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/minecart/assets/cart.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)    12734 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/minecart/assets/mine.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1757 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/minecart/mine_config.json
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1727 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/minecart/mine_config_det.json
--rw-r--r--   0 lucas     (1000) lucas     (1000)    30052 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/minecart/minecart.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.517449 mo-gymnasium-0.3.4/mo_gymnasium/envs/mountain_car/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      195 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/mountain_car/__init__.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     2208 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/mountain_car/mountain_car.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.517449 mo-gymnasium-0.3.4/mo_gymnasium/envs/mujoco/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      449 2023-02-01 09:34:12.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/mujoco/__init__.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.517449 mo-gymnasium-0.3.4/mo_gymnasium/envs/mujoco/assets/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     3722 2023-02-01 09:34:12.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/mujoco/assets/mo_reacher.xml
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1022 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/mujoco/half_cheetah.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     2372 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/mujoco/hopper.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     3583 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/mujoco/reacher.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.517449 mo-gymnasium-0.3.4/mo_gymnasium/envs/reacher/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      226 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/reacher/__init__.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     6480 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/reacher/reacher.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.517449 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      215 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/__init__.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.527449 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      935 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/elf_down.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)      872 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/elf_left.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)      858 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/elf_right.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)      842 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/elf_up.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)      617 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/enemy.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)      417 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/gem.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)      418 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/gold.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)     3252 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/home.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)      651 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/mountain_bg1.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)      643 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/mountain_bg2.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)    12960 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/resource_gathering.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.527449 mo-gymnasium-0.3.4/mo_gymnasium/envs/water_reservoir/
--rw-r--r--   0 lucas     (1000) lucas     (1000)      149 2023-01-23 22:22:41.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/water_reservoir/__init__.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.537449 mo-gymnasium-0.3.4/mo_gymnasium/envs/water_reservoir/assets/
--rw-r--r--   0 lucas     (1000) lucas     (1000)    14488 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/water_reservoir/assets/Minecraft.ttf
--rw-r--r--   0 lucas     (1000) lucas     (1000)    28791 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/water_reservoir/assets/sky.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)      339 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/water_reservoir/assets/wall.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)      909 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/water_reservoir/assets/water.png
--rw-r--r--   0 lucas     (1000) lucas     (1000)    10826 2023-03-14 15:04:20.000000 mo-gymnasium-0.3.4/mo_gymnasium/envs/water_reservoir/dam_env.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)    12388 2023-02-11 11:41:05.000000 mo-gymnasium-0.3.4/mo_gymnasium/utils.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.457449 mo-gymnasium-0.3.4/mo_gymnasium.egg-info/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     5481 2023-03-14 15:33:08.000000 mo-gymnasium-0.3.4/mo_gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1000) lucas     (1000)     3133 2023-03-14 15:33:08.000000 mo-gymnasium-0.3.4/mo_gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)        1 2023-03-14 15:33:08.000000 mo-gymnasium-0.3.4/mo_gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)      416 2023-03-14 15:33:08.000000 mo-gymnasium-0.3.4/mo_gymnasium.egg-info/requires.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)       13 2023-03-14 15:33:08.000000 mo-gymnasium-0.3.4/mo_gymnasium.egg-info/top_level.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)     4181 2023-02-07 16:43:30.000000 mo-gymnasium-0.3.4/pyproject.toml
--rw-r--r--   0 lucas     (1000) lucas     (1000)       38 2023-03-14 15:33:08.537449 mo-gymnasium-0.3.4/setup.cfg
--rw-r--r--   0 lucas     (1000) lucas     (1000)      852 2023-03-14 13:56:48.000000 mo-gymnasium-0.3.4/setup.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2023-03-14 15:33:08.537449 mo-gymnasium-0.3.4/tests/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     6750 2023-03-14 13:56:48.000000 mo-gymnasium-0.3.4/tests/test_envs.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     4756 2023-02-01 09:34:12.000000 mo-gymnasium-0.3.4/tests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.146228 mo-gymnasium-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 15:31:06.000000 mo-gymnasium-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-12 15:31:19.146228 mo-gymnasium-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-12 15:31:06.000000 mo-gymnasium-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.130228 mo-gymnasium-1.0.0/mo_gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.130228 mo-gymnasium-1.0.0/mo_gymnasium/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.130228 mo-gymnasium-1.0.0/mo_gymnasium/envs/breakable_bottles/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/breakable_bottles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/breakable_bottles/breakable_bottles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.130228 mo-gymnasium-1.0.0/mo_gymnasium/envs/continuous_mountain_car/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/continuous_mountain_car/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/continuous_mountain_car/continuous_mountain_car.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.134228 mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.134228 mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/assets/Minecraft.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/assets/rock.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/assets/sea_bg.png
+-rw-r--r--   0 runner    (1001) docker     (123)   106615 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/assets/submarine.png
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/assets/treasure.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/deep_sea_treasure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.134228 mo-gymnasium-1.0.0/mo_gymnasium/envs/fishwood/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/fishwood/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.134228 mo-gymnasium-1.0.0/mo_gymnasium/envs/fishwood/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    42842 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/fishwood/assets/Kawa.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35586 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/fishwood/assets/Mori.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/fishwood/fishwood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.134228 mo-gymnasium-1.0.0/mo_gymnasium/envs/four_room/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/four_room/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/four_room/four_room.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.134228 mo-gymnasium-1.0.0/mo_gymnasium/envs/fruit_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/fruit_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/fruit_tree/fruit_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.134228 mo-gymnasium-1.0.0/mo_gymnasium/envs/highway/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/highway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/highway/highway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.134228 mo-gymnasium-1.0.0/mo_gymnasium/envs/lunar_lander/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/lunar_lander/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/lunar_lander/lunar_lander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.138228 mo-gymnasium-1.0.0/mo_gymnasium/envs/mario/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/mario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/mario/joypad_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/mario/mario.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.138228 mo-gymnasium-1.0.0/mo_gymnasium/envs/minecart/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/minecart/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.138228 mo-gymnasium-1.0.0/mo_gymnasium/envs/minecart/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/minecart/assets/cart.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/minecart/assets/mine.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/minecart/mine_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/minecart/mine_config_det.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30192 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/minecart/minecart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.138228 mo-gymnasium-1.0.0/mo_gymnasium/envs/mountain_car/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/mountain_car/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/mountain_car/mountain_car.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.138228 mo-gymnasium-1.0.0/mo_gymnasium/envs/mujoco/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/mujoco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.138228 mo-gymnasium-1.0.0/mo_gymnasium/envs/mujoco/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/mujoco/assets/mo_reacher.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/mujoco/half_cheetah.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/mujoco/hopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/mujoco/reacher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.138228 mo-gymnasium-1.0.0/mo_gymnasium/envs/reacher/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/reacher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/reacher/reacher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.142228 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.142228 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/elf_down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/elf_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/elf_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/elf_up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/enemy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/gem.png
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/gold.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/mountain_bg1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/mountain_bg2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13037 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/resource_gathering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.142228 mo-gymnasium-1.0.0/mo_gymnasium/envs/water_reservoir/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/water_reservoir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.142228 mo-gymnasium-1.0.0/mo_gymnasium/envs/water_reservoir/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/water_reservoir/assets/Minecraft.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    28791 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/water_reservoir/assets/sky.png
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/water_reservoir/assets/wall.png
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/water_reservoir/assets/water.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/envs/water_reservoir/dam_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/mo_gymnasium/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.130228 mo-gymnasium-1.0.0/mo_gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-12 15:31:19.000000 mo-gymnasium-1.0.0/mo_gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-12 15:31:19.000000 mo-gymnasium-1.0.0/mo_gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:31:19.000000 mo-gymnasium-1.0.0/mo_gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-12 15:31:19.000000 mo-gymnasium-1.0.0/mo_gymnasium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 15:31:19.000000 mo-gymnasium-1.0.0/mo_gymnasium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:31:19.146228 mo-gymnasium-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:31:19.146228 mo-gymnasium-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/tests/test_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-12 15:31:07.000000 mo-gymnasium-1.0.0/tests/test_wrappers.py
```

### Comparing `mo-gymnasium-0.3.4/LICENSE` & `mo-gymnasium-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/PKG-INFO` & `mo-gymnasium-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: mo-gymnasium
-Version: 0.3.4
+Version: 1.0.0
 Summary: A standard API for MORL and a diverse set of reference environments.
 Author-email: Farama Foundation <contact@farama.org>
 License: MIT License
 Project-URL: Homepage, https://mo-gymnasium.farama.org
 Project-URL: Repository, https://github.com/Farama-Foundation/MO-Gymnasium
 Project-URL: Documentation, https://mo-gymnasium.farama.org
 Project-URL: Bug Report, https://github.com/Farama-Foundation/MO-Gymnasium/issues
 Keywords: Reinforcement Learning,Multi-Objective,RL,AI,gymnasium
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: mario
 Provides-Extra: minecart
 Provides-Extra: mujoco
 Provides-Extra: highway
 Provides-Extra: box2d
 Provides-Extra: all
 Provides-Extra: testing
 License-File: LICENSE
 
 ![tests](https://github.com/Farama-Foundation/mo-gymnasium/workflows/Python%20tests/badge.svg)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-
-# MO-Gymnasium: Multi-Objective Reinforcement Learning Environments
+<p align="center">
+    <img src="docs/_static/img/MO-Gymnasium-text_small.png" width="500px"/>
+</p>
 
 <!-- start elevator-pitch -->
 
 MO-Gymnasium is an open source Python library for developing and comparing multi-objective reinforcement learning algorithms by providing a standard API to communicate between learning algorithms and environments, as well as a standard set of environments compliant with that API. Essentially, the environments follow the standard [Gymnasium API](https://github.com/Farama-Foundation/Gymnasium), but return vectorized rewards as numpy arrays.
 
 The documentation website is at [mo-gymnasium.farama.org](https://mo-gymnasium.farama.org), and we have a public discord server (which we also use to coordinate development work) that you can join here: https://discord.gg/bnJ6kubTg6.
 
@@ -93,19 +93,28 @@
 
 [MORL-Baselines](https://github.com/LucasAlegre/morl-baselines) is a repository containing various implementations of MORL algorithms by the same authors as MO-Gymnasium. It relies on the MO-Gymnasium API and shows various examples of the usage of wrappers and environments.
 
 ## Environment Versioning
 
 MO-Gymnasium keeps strict versioning for reproducibility reasons. All environments end in a suffix like "-v0".  When changes are made to environments that might impact learning results, the number is increased by one to prevent potential confusion.
 
+## Development Roadmap
+We have a roadmap for future development available here: https://github.com/Farama-Foundation/MO-Gymnasium/issues/66.
+
+## Project Maintainers
+
+Project Managers: [Lucas Alegre](https://github.com/LucasAlegre) and [Florian Felten](https://github.com/ffelten).
+
+Maintenance for this project is also contributed by the broader Farama team: [farama.org/team](https://farama.org/team).
+
 ## Citing
 
 <!-- start citation -->
 
-If you use this repository in your work, please cite:
+If you use this repository in your research, please cite:
 
 ```bibtex
 @inproceedings{Alegre+2022bnaic,
   author = {Lucas N. Alegre and Florian	Felten and El-Ghazali Talbi and Gr{\'e}goire Danoy and Ann Now{\'e} and Ana L. C. Bazzan and Bruno C. da Silva},
   title = {{MO-Gym}: A Library of Multi-Objective Reinforcement Learning Environments},
   booktitle = {Proceedings of the 34th Benelux Conference on Artificial Intelligence BNAIC/Benelearn 2022},
   year = {2022}
```

### Comparing `mo-gymnasium-0.3.4/README.md` & `mo-gymnasium-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ![tests](https://github.com/Farama-Foundation/mo-gymnasium/workflows/Python%20tests/badge.svg)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-
-# MO-Gymnasium: Multi-Objective Reinforcement Learning Environments
+<p align="center">
+    <img src="docs/_static/img/MO-Gymnasium-text_small.png" width="500px"/>
+</p>
 
 <!-- start elevator-pitch -->
 
 MO-Gymnasium is an open source Python library for developing and comparing multi-objective reinforcement learning algorithms by providing a standard API to communicate between learning algorithms and environments, as well as a standard set of environments compliant with that API. Essentially, the environments follow the standard [Gymnasium API](https://github.com/Farama-Foundation/Gymnasium), but return vectorized rewards as numpy arrays.
 
 The documentation website is at [mo-gymnasium.farama.org](https://mo-gymnasium.farama.org), and we have a public discord server (which we also use to coordinate development work) that you can join here: https://discord.gg/bnJ6kubTg6.
 
@@ -61,19 +62,28 @@
 
 [MORL-Baselines](https://github.com/LucasAlegre/morl-baselines) is a repository containing various implementations of MORL algorithms by the same authors as MO-Gymnasium. It relies on the MO-Gymnasium API and shows various examples of the usage of wrappers and environments.
 
 ## Environment Versioning
 
 MO-Gymnasium keeps strict versioning for reproducibility reasons. All environments end in a suffix like "-v0".  When changes are made to environments that might impact learning results, the number is increased by one to prevent potential confusion.
 
+## Development Roadmap
+We have a roadmap for future development available here: https://github.com/Farama-Foundation/MO-Gymnasium/issues/66.
+
+## Project Maintainers
+
+Project Managers: [Lucas Alegre](https://github.com/LucasAlegre) and [Florian Felten](https://github.com/ffelten).
+
+Maintenance for this project is also contributed by the broader Farama team: [farama.org/team](https://farama.org/team).
+
 ## Citing
 
 <!-- start citation -->
 
-If you use this repository in your work, please cite:
+If you use this repository in your research, please cite:
 
 ```bibtex
 @inproceedings{Alegre+2022bnaic,
   author = {Lucas N. Alegre and Florian	Felten and El-Ghazali Talbi and Gr{\'e}goire Danoy and Ann Now{\'e} and Ana L. C. Bazzan and Bruno C. da Silva},
   title = {{MO-Gym}: A Library of Multi-Objective Reinforcement Learning Environments},
   booktitle = {Proceedings of the 34th Benelux Conference on Artificial Intelligence BNAIC/Benelearn 2022},
   year = {2022}
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/__init__.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/breakable_bottles/breakable_bottles.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/breakable_bottles/breakable_bottles.py`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/continuous_mountain_car/continuous_mountain_car.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/continuous_mountain_car/continuous_mountain_car.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     - fuel reward: -||action||^2 , i.e. the negative of the norm of the action vector
     """
 
     def __init__(self, render_mode: Optional[str] = None, goal_velocity=0):
         super().__init__(render_mode, goal_velocity)
         EzPickle.__init__(self, render_mode, goal_velocity)
 
-        self.reward_space = spaces.Box(low=np.array([-1.0, -1.0]), high=np.array([0.0, 0.0]), shape=(2,), dtype=np.float32)
+        self.reward_space = spaces.Box(low=np.array([-1.0, -1.0]), high=np.array([0.0, 0.0]), dtype=np.float32)
         self.reward_dim = 2
 
     def step(self, action: np.ndarray):
         # Essentially a copy paste from original env, except the rewards
 
         position = self.state[0]
         velocity = self.state[1]
@@ -47,15 +47,15 @@
             position = self.min_position
         if position == self.min_position and velocity < 0:
             velocity = 0
 
         # Convert a possible numpy bool to a Python bool.
         terminated = bool(position >= self.goal_position and velocity >= self.goal_velocity)
 
-        reward = np.zeros(2)
+        reward = np.zeros(2, dtype=np.float32)
         # Time reward is negative at all timesteps except when reaching the goal
         if terminated:
             reward[0] = 0.0
         else:
             reward[0] = -1.0
 
         # Actions cost fuel, which we want to optimize too
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/assets/Minecraft.ttf` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/assets/Minecraft.ttf`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/assets/rock.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/assets/rock.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/assets/sea_bg.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/assets/sea_bg.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/assets/submarine.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/assets/submarine.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/assets/treasure.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/assets/treasure.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/deep_sea_treasure/deep_sea_treasure.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/deep_sea_treasure/deep_sea_treasure.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         self.step_count = 0.0
         state = self._get_state()
         if self.render_mode == "human":
             self.render()
         return state, {}
 
     def step(self, action):
-        next_state = self.current_state + self.dir[action]
+        next_state = self.current_state + self.dir[int(action)]
 
         if self._is_valid_state(next_state):
             self.current_state = next_state
 
         treasure_value = self._get_map_value(self.current_state)
         if treasure_value == 0 or treasure_value == -10:
             treasure_value = 0.0
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/fishwood/assets/Kawa.jpg` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/fishwood/assets/Kawa.jpg`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/fishwood/assets/Mori.jpg` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/fishwood/assets/Mori.jpg`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/fishwood/fishwood.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/fishwood/fishwood.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 
         if self.render_mode == "human":
             self.render()
         return self._state, rewards, self._timestep == self.MAX_TS, self._timestep == self.MAX_TS, {}
 
 
 if __name__ == "__main__":
-
     env = FishWood()
     terminated = False
     env.reset()
     while True:
         env.render()
         obs, r, terminated, truncated, info = env.step(env.action_space.sample())
         if terminated:
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/four_room/four_room.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/four_room/four_room.py`

 * *Files 12% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                 X indicates a barrier
                 0, 1, .... 9 indicates the type of shape to be placed in the corresponding cell
                 entries containing other characters are treated as regular empty cells
         """
         EzPickle.__init__(self, render_mode, maze)
 
         self.render_mode = render_mode
-        self.window_size = 512
+        self.window_size = int(13 * 35)
         self.window = None
         self.clock = None
 
         self.height, self.width = maze.shape
         self.maze = maze
         shape_types = ["1", "2", "3"]
         self.all_shapes = dict(zip(shape_types, range(len(shape_types))))
@@ -202,14 +202,17 @@
                 collected = list(collected)
                 collected[shape_id] = 1
                 collected = tuple(collected)
                 self.state = (s1, collected)
                 phi = self.features(old_state, action, self.state)
                 return self.state_to_array(self.state), phi, terminated, False, {}
 
+        if self.render_mode == "human":
+            self.render()
+
         # into an empty cell
         return (
             self.state_to_array(self.state),
             np.zeros(len(self.all_shapes), dtype=np.float32),
             terminated,
             False,
             {},
@@ -227,15 +230,15 @@
                 phi[shape_index] = 1.0
         elif s1 == self.goal:
             phi[nc] = np.ones(nc, dtype=np.float32)
         return phi
 
     def render(self):
         # The size of a single grid square in pixels
-        pix_square_size = self.window_size / 13
+        pix_square_size = self.window_size // 13
 
         if self.window is None and self.render_mode is not None:
             pygame.init()
             if self.render_mode == "human":
                 pygame.display.init()
                 self.window = pygame.display.set_mode((self.window_size, self.window_size))
         if self.clock is None and self.render_mode == "human":
@@ -244,14 +247,16 @@
         canvas = pygame.Surface((self.window_size, self.window_size))
         canvas.fill((255, 255, 255))
 
         pygame.font.init()
         self.font = pygame.font.SysFont(None, 48)
         img = self.font.render("G", True, BLACK)
         canvas.blit(img, (np.array(self.goal)[::-1] + 0.15) * pix_square_size)
+        img = self.font.render("S", True, BLACK)
+        canvas.blit(img, (np.array(self.initial[0])[::-1] + 0.15) * pix_square_size)
 
         for i in range(self.maze.shape[0]):
             for j in range(self.maze.shape[1]):
                 (row, col), collected = self.state
                 shape_id = self.shape_ids.get((i, j), 0)
                 if collected[shape_id] == 1 and self.maze[i, j] != "X":
                     continue
@@ -297,27 +302,35 @@
             canvas,
             (125, 125, 125),
             (np.array(self.state[0])[::-1] + 0.5) * pix_square_size,
             pix_square_size / 3,
         )
 
         for x in range(13 + 1):
-            pygame.draw.line(
+            if x == 0 or x == 13:
+                width = 3
+                dash_lenght = 0
+            else:
+                width = 1
+                dash_lenght = 3
+            draw_line_dashed(
                 canvas,
                 0,
                 (0, pix_square_size * x),
                 (self.window_size, pix_square_size * x),
-                width=1,
+                width=width,
+                dash_length=dash_lenght,
             )
-            pygame.draw.line(
+            draw_line_dashed(
                 canvas,
                 0,
                 (pix_square_size * x, 0),
                 (pix_square_size * x, self.window_size),
-                width=1,
+                width=width,
+                dash_length=dash_lenght,
             )
 
         if self.render_mode == "human":
             # The following line copies our drawings from `canvas` to the visible window
             self.window.blit(canvas, canvas.get_rect())
             pygame.event.pump()
             pygame.display.update()
@@ -330,15 +343,39 @@
 
     def close(self):
         if self.window is not None:
             pygame.display.quit()
             pygame.quit()
 
 
+def draw_line_dashed(surface, color, start_pos, end_pos, width=1, dash_length=3, exclude_corners=True):
+    """Code from https://codereview.stackexchange.com/questions/70143/drawing-a-dashed-line-with-pygame."""
+    # convert tuples to numpy arrays
+    if dash_length < 1:
+        pygame.draw.line(surface, color, start_pos, end_pos, width)
+    else:
+        start_pos = np.array(start_pos)
+        end_pos = np.array(end_pos)
+
+        # get euclidean distance between start_pos and end_pos
+        length = np.linalg.norm(end_pos - start_pos)
+
+        # get amount of pieces that line will be split up in (half of it are amount of dashes)
+        dash_amount = int(length / dash_length)
+
+        # x-y-value-pairs of where dashes start (and on next, will end)
+        dash_knots = np.array([np.linspace(start_pos[i], end_pos[i], dash_amount) for i in range(2)]).transpose()
+
+        return [
+            pygame.draw.line(surface, color, tuple(dash_knots[n]), tuple(dash_knots[n + 1]), width)
+            for n in range(int(exclude_corners), dash_amount - int(exclude_corners), 2)
+        ]
+
+
 if __name__ == "__main__":
+    import mo_gymnasium as mo_gym
 
-    env = FourRoom()
+    env = mo_gym.make("four-room-v0", render_mode="human")
     terminated = False
     env.reset()
-    while not terminated:
-        env.render()
+    while True:
         obs, r, terminated, truncated, info = env.step(env.action_space.sample())
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/fruit_tree/fruit_tree.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/fruit_tree/fruit_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Environment from https://github.com/RunzheYang/MORL/blob/master/synthetic/envs/fruit_tree.py
+from typing import List
+
 import gymnasium as gym
 import numpy as np
 from gymnasium import spaces
 from gymnasium.utils import EzPickle
 
 
 FRUITS = {
@@ -286,28 +288,41 @@
         self.current_state = np.array([0, 0], dtype=np.int32)
         self.terminal = False
 
     def get_ind(self, pos):
         return int(2 ** pos[0] - 1) + pos[1]
 
     def get_tree_value(self, pos):
-        return self.tree[self.get_ind(pos)]
+        return np.array(self.tree[self.get_ind(pos)], dtype=np.float32)
+
+    def pareto_front(self, gamma: float) -> List[np.ndarray]:
+        """Returns the discounted pareto front of the tree.
+
+        Args:
+            gamma: Discount factor.
+
+        Returns:
+            List of discounted rewards.
+        """
+        fruits = np.array(FRUITS[str(self.tree_depth)])
+        disc_fruits = fruits * gamma ** (self.tree_depth - 1)
+        return list(disc_fruits)
 
     def reset(self, seed=None, **kwargs):
         super().reset(seed=seed)
 
         self.current_state = np.array([0, 0], dtype=np.int32)
         self.terminal = False
         return self.current_state.copy(), {}
 
     def step(self, action):
         direction = {
             0: np.array([1, self.current_state[1]], dtype=np.int32),  # left
             1: np.array([1, self.current_state[1] + 1], dtype=np.int32),  # right
-        }[action]
+        }[int(action)]
 
         self.current_state = self.current_state + direction
 
         reward = self.get_tree_value(self.current_state)
         if self.current_state[0] == self.tree_depth:
             self.terminal = True
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/lunar_lander/lunar_lander.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/lunar_lander/lunar_lander.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,20 @@
     - 3: Fuel cost (side engine)
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Result reward, shaping reward, main engine cost, side engine cost
-        self.reward_space = spaces.Box(low=-np.inf, high=np.inf, shape=(4,), dtype=np.float32)
+        self.reward_space = spaces.Box(
+            low=np.array([-100, -np.inf, -1, -1]),
+            high=np.array([100, np.inf, 0, 0]),
+            shape=(4,),
+            dtype=np.float32,
+        )
         self.reward_dim = 4
 
     def step(self, action):
         assert self.lander is not None
 
         # Update wind
         assert self.lander is not None, "You forgot to call reset()"
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/mario/joypad_space.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/mario/joypad_space.py`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/mario/mario.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/mario/mario.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,19 @@
     ):
         EzPickle.__init__(self, rom_mode, lost_levels, target, objectives, render_mode)
         super().__init__(rom_mode, lost_levels, target)
 
         self.render_mode = render_mode
 
         self.objectives = set(objectives)
-        self.reward_space = gym.spaces.Box(high=np.inf, low=-np.inf, shape=(len(objectives),))
+        self.reward_space = gym.spaces.Box(
+            low=np.array([-np.inf, -np.inf, -25, 0, 0]),
+            high=np.array([np.inf, 0, 0, 100, np.inf]),
+            shape=(len(objectives),),
+        )
         self.reward_dim = len(objectives)
 
         # observation space for the environment is static across all instances
         self.observation_space = gym.spaces.Box(low=0, high=255, shape=SCREEN_SHAPE_24_BIT, dtype=np.uint8)
 
         # action space is a bitmap of button press values for the 8 NES buttons
         self.action_space = gym.spaces.Discrete(256)
@@ -159,15 +163,14 @@
         if self.render_mode == "human":
             self.render()
 
         return obs, mor, bool(done), False, info
 
 
 if __name__ == "__main__":
-
     env = MOSuperMarioBros()
     env = JoypadSpace(env, SIMPLE_MOVEMENT)
     # env = MaxAndSkipEnv(env, 4)
     env = ResizeObservation(env, (84, 84))
     env = GrayScaleObservation(env)
     # env = FrameStack(env, 4)
     env = mo_gym.LinearReward(env)
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/minecart/assets/cart.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/minecart/assets/cart.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/minecart/assets/mine.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/minecart/assets/mine.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/minecart/mine_config.json` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/minecart/mine_config.json`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/minecart/mine_config_det.json` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/minecart/mine_config_det.json`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/minecart/minecart.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/minecart/minecart.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,19 @@
                 high=255 * np.ones((WIDTH, HEIGHT, 3)),
                 dtype=np.uint8,
             )
         else:
             self.observation_space = Box(-np.ones(7), np.ones(7), dtype=np.float32)
 
         self.action_space = Discrete(6)
-        self.reward_space = Box(low=-1, high=self.capacity, shape=(self.ore_cnt + 1,))
+        self.reward_space = Box(
+            low=np.append(np.zeros(self.ore_cnt), -1.0),
+            high=np.append(np.ones(self.ore_cnt) * self.capacity, 0.0),
+            shape=(self.ore_cnt + 1,),
+        )
         self.reward_dim = self.ore_cnt + 1
 
     def convex_coverage_set(self, gamma: float, symmetric: bool = True) -> List[np.ndarray]:
         """
         Computes an approximate convex coverage set (CCS).
 
         Args:
@@ -426,25 +430,24 @@
             mine_sprite.rect = mine_sprite.image.get_rect()
             mine_sprite.rect.centerx = (mine.pos[0] * (1 - 2 * MARGIN)) * WIDTH + MARGIN * WIDTH
             mine_sprite.rect.centery = (mine.pos[1] * (1 - 2 * MARGIN)) * HEIGHT + MARGIN * HEIGHT
             self.mine_rects.append(mine_sprite.rect)
 
     def step(self, action):
         change = False  # Keep track of whether the state has changed
-        reward = np.zeros(self.ore_cnt + 1)
+        reward = np.zeros(self.ore_cnt + 1, dtype=np.float32)
 
         reward[-1] = FUEL_IDLE * self.frame_skip
 
         if action == ACT_ACCEL:
             reward[-1] += FUEL_ACC * self.frame_skip
         elif action == ACT_MINE:
             reward[-1] += FUEL_MINE * self.frame_skip
 
         for _ in range(self.frame_skip if self.incremental_frame_skip else 1):
-
             if action == ACT_LEFT:
                 self.cart.rotate(-ROTATION * (1 if self.incremental_frame_skip else self.frame_skip))
                 change = True
             elif action == ACT_RIGHT:
                 self.cart.rotate(ROTATION * (1 if self.incremental_frame_skip else self.frame_skip))
                 change = True
             elif action == ACT_ACCEL:
@@ -649,15 +652,14 @@
 
         # Draw cart content
         width = self.cart_sprite.rect.width / (2 * self.ore_cnt)
         height = self.cart_sprite.rect.height / 3
         content_width = (width + 1) * self.ore_cnt
         offset = (self.cart_sprite.rect.width - content_width) / 2
         for i in range(self.ore_cnt):
-
             rect_height = height * self.cart.content[i] / self.capacity
 
             if rect_height >= 1:
                 pygame.draw.rect(
                     self.screen,
                     self.ore_colors[i],
                     (
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/mountain_car/mountain_car.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/mountain_car/mountain_car.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,23 @@
     A multi-objective version of the MountainCar environment, where the goal is to reach the top of the mountain.
 
     See [Gymnasium's env](https://gymnasium.farama.org/environments/classic_control/mountain_car_continuous/) for more information.
 
     ## Reward space:
     The reward space is a 3D vector containing the time penalty, and penalties for reversing and going forward.
     - time penalty: -1.0 for each time step
-    - reverse penalty: -1.0 for each time step the actuin is 0 (reverse)
+    - reverse penalty: -1.0 for each time step the action is 0 (reverse)
     - forward penalty: -1.0 for each time step the action is 2 (forward)
     """
 
     def __init__(self, render_mode: Optional[str] = None, goal_velocity=0):
         super().__init__(render_mode, goal_velocity)
         EzPickle.__init__(self, render_mode, goal_velocity)
 
-        self.reward_space = spaces.Box(low=-1, high=1, shape=(3,), dtype=np.float32)
+        self.reward_space = spaces.Box(low=np.array([-1, -1, -1]), high=np.array([-1, 0, 0]), shape=(3,), dtype=np.float32)
         self.reward_dim = 3
 
     def step(self, action: int):
         assert self.action_space.contains(action), f"{action!r} ({type(action)}) invalid"
 
         position, velocity = self.state
         velocity += (action - 1) * self.force + math.cos(3 * position) * (-self.gravity)
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/mujoco/assets/mo_reacher.xml` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/mujoco/assets/mo_reacher.xml`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/mujoco/half_cheetah.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/mujoco/half_cheetah.py`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/mujoco/hopper.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/mujoco/hopper.py`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/mujoco/reacher.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/mujoco/reacher.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.action_dict = dict()
         for a1 in actions:
             for a2 in actions:
                 self.action_dict[len(self.action_dict)] = (a1, a2)
         self.action_space = Discrete(9)
         # Target goals: x1, y1, x2, y2, ... x4, y4
         self.goal = np.array([0.14, 0.0, -0.14, 0.0, 0.0, 0.14, 0.0, -0.14])
-        self.reward_space = Box(low=-np.inf, high=np.inf, shape=(4,))
+        self.reward_space = Box(low=-1.0, high=1.0, shape=(4,))
         self.reward_dim = 4
 
     def step(self, a):
         real_action = self.action_dict[int(a)]
         vec_reward = np.array(
             [
                 1 - 4 * np.linalg.norm(self.get_body_com("fingertip")[:2] - self.get_body_com("target1")[:2]),
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/reacher/reacher.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/reacher/reacher.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from pybulletgym.envs.roboschool.scenes.scene_bases import SingleRobotEmptyScene
 
 
 target_positions = list(map(lambda l: np.array(l), [(0.14, 0.0), (-0.14, 0.0), (0.0, 0.14), (0.0, -0.14)]))
 
 
 class ReacherBulletEnv(BaseBulletEnv, EzPickle):
-
     metadata = {"render_modes": ["human", "rgb_array"]}
 
     def __init__(
         self,
         render_mode: Optional[str] = None,
         target=(0.14, 0.0),
         fixed_initial_state: Optional[tuple] = (3.14, 0),
@@ -40,15 +39,15 @@
         self.action_dict = dict()
         for a1 in actions:
             for a2 in actions:
                 self.action_dict[len(self.action_dict)] = (a1, a2)
 
         self.action_space = spaces.Discrete(9)
         self.observation_space = spaces.Box(low=-np.inf, high=np.inf, shape=(5,), dtype=np.float32)
-        self.reward_space = spaces.Box(low=-np.inf, high=np.inf, shape=(4,), dtype=np.float32)
+        self.reward_space = spaces.Box(low=-1.0, high=1.0, shape=(4,), dtype=np.float32)
         self.reward_dim = 4
 
     def create_single_player_scene(self, bullet_client):
         return SingleRobotEmptyScene(bullet_client, gravity=0.0, timestep=0.0165, frame_skip=1)
 
     def step(self, a):
         real_action = self.action_dict[int(a)]
@@ -58,15 +57,15 @@
         self.scene.global_step()
 
         state = self.robot.calc_state()  # sets self.to_target_vec
 
         """ delta = np.linalg.norm(np.array(self.robot.fingertip.pose().xyz()) - np.array(self.robot.target.pose().xyz()))
         reward = 1. - 4. * delta """
 
-        phi = np.zeros(len(self.target_positions))
+        phi = np.zeros(len(self.target_positions), dtype=np.float32)
         for index, target in enumerate(self.target_positions):
             delta = np.linalg.norm(np.array(self.robot.fingertip.pose().xyz()[:2]) - target)
             phi[index] = 1.0 - 4 * delta  # 1 - 4
 
         self.HUD(state, real_action, False)
 
         if self.render_mode == "human":
@@ -144,15 +143,14 @@
                 self.gamma_dot * 0.1,
             ],
             dtype=np.float32,
         )
 
 
 if __name__ == "__main__":
-
     env = ReacherBulletEnv()
     # env.render(mode='human')
     obs = env.reset()
     print(env.observation_space.contains(obs), obs.dtype, env.observation_space)
     while True:
         env.step(env.action_space.sample())
         # env.render(mode='human')
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/elf_down.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/elf_down.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/elf_left.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/elf_left.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/elf_right.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/elf_right.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/elf_up.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/elf_up.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/enemy.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/enemy.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/home.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/home.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/mountain_bg1.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/mountain_bg1.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/assets/mountain_bg2.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/assets/mountain_bg2.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/resource_gathering/resource_gathering.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/resource_gathering/resource_gathering.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     - 0: Move up
     - 1: Move down
     - 2: Move left
     - 3: Move right
 
     ## Reward Space
     The reward is 3-dimensional:
-    - 0: +1 if returned home with gold, else 0
-    - 1: +1 if returned home with diamond, else 0
-    - 2: -1 if killed by an enemy, else 0
+    - 0: -1 if killed by an enemy, else 0
+    - 1: +1 if returned home with gold, else 0
+    - 2: +1 if returned home with diamond, else 0
 
     ## Starting State
     The agent starts at the home position with no gold or diamond.
 
     ## Episode Termination
     The episode terminates when the agent returns home, or when the agent is killed by an enemy.
 
@@ -72,15 +72,15 @@
         }
 
         self.observation_space = Box(low=0.0, high=5.0, shape=(4,), dtype=np.int32)
 
         # action space specification: 1 dimension, 0 up, 1 down, 2 left, 3 right
         self.action_space = Discrete(4)
         # reward space:
-        self.reward_space = Box(low=-1, high=1, shape=(3,), dtype=np.float32)
+        self.reward_space = Box(low=np.array([-1.0, 0.0, 0.0]), high=np.array([0.0, 1.0, 1.0]), shape=(3,), dtype=np.float32)
         self.reward_dim = 3
 
         # pygame
         self.size = 5
         self.cell_size = (64, 64)
         self.window_size = (
             self.map.shape[1] * self.cell_size[1],
@@ -268,14 +268,15 @@
         self.step_count = 0.0
         state = self.get_state()
         if self.render_mode == "human":
             self.render()
         return state, {}
 
     def step(self, action):
+        action = int(action)
         next_pos = self.current_pos + self.dir[action]
         self.last_action = action
 
         if self.is_valid_state(next_pos):
             self.current_pos = next_pos
 
         vec_reward = np.zeros(3, dtype=np.float32)
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/water_reservoir/assets/Minecraft.ttf` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/water_reservoir/assets/Minecraft.ttf`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/water_reservoir/assets/sky.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/water_reservoir/assets/sky.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/water_reservoir/assets/water.png` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/water_reservoir/assets/water.png`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/envs/water_reservoir/dam_env.py` & `mo-gymnasium-1.0.0/mo_gymnasium/envs/water_reservoir/dam_env.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,21 +21,34 @@
     Brisbane, QLD, Australia, 2012, pp. 1-8, doi: 10.1109/IJCNN.2012.6252759.
 
     ## Observation Space
     The observation is a float corresponding to the current level of the reservoir.
 
     ## Action Space
     The action is a float corresponding to the amount of water released by the dam.
+    If normalized_action is True, the action is a float between 0 and 1 corresponding to the percentage of water released by the dam.
 
     ## Reward Space
     There are up to 4 rewards:
      - cost due to excess level wrt a flooding threshold (upstream)
      - deficit in the water supply wrt the water demand
      - deficit in hydroelectric supply wrt hydroelectric demand
      - cost due to excess level wrt a flooding threshold (downstream)
+     By default, only the first two are used.
+
+     ## Starting State
+     The reservoir is initialized with a random level between 0 and 160.
+
+     ## Arguments
+        - render_mode: The render mode to use. Can be 'human', 'rgb_array' or 'ansi'.
+        - time_limit: The maximum number of steps until the episode is truncated.
+        - nO: The number of objectives to use. Can be 2, 3 or 4.
+        - penalize: Whether to penalize the agent for selecting an action out of bounds.
+        - normalized_action: Whether to normalize the action space as a percentage [0, 1].
+        - initial_state: The initial state of the reservoir. If None, a random state is used.
 
      ## Credits
      Code from:
      [Mathieu Reymond](https://gitlab.ai.vub.ac.be/mreymond/dam).
      Ported from:
      [Simone Parisi](https://github.com/sparisi/mips).
 
@@ -82,24 +95,31 @@
 
     def __init__(
         self,
         render_mode: Optional[str] = None,
         time_limit: int = 100,
         nO=2,
         penalize: bool = False,
+        normalized_action: bool = False,
+        initial_state: Optional[np.ndarray] = None,
     ):
-        EzPickle.__init__(self, render_mode, time_limit, nO, penalize)
+        EzPickle.__init__(self, render_mode, time_limit, nO, penalize, normalized_action)
         self.render_mode = render_mode
 
         self.observation_space = Box(low=0.0, high=np.inf, shape=(1,), dtype=np.float32)
-        self.action_space = Box(low=0, high=np.inf, shape=(1,), dtype=np.float32)
+        self.normalized_action = normalized_action
+        if self.normalized_action:
+            self.action_space = Box(low=0.0, high=1.0, shape=(1,), dtype=np.float32)
+        else:
+            self.action_space = Box(low=0.0, high=np.inf, shape=(1,), dtype=np.float32)
 
         self.nO = nO
         self.penalize = penalize
         self.time_limit = time_limit
+        self.initial_state = initial_state
         self.time_step = 0
         self.last_action = None
         self.dam_inflow = None
         self.excess = None
         self.defict = None
 
         low = -np.ones(nO) * np.inf  # DamEnv.antiutopia[nO]
@@ -113,18 +133,21 @@
         self.water_img = None
         self.wall_img = None
         self.sky_img = None
 
     def reset(self, *, seed: Optional[int] = None, options: Optional[dict] = None):
         super().reset(seed=seed)
         self.time_step = 0
-        if not self.penalize:
-            state = self.np_random.choice(DamEnv.s_init, size=1)
+        if self.initial_state is not None:
+            state = self.initial_state
         else:
-            state = self.np_random.randint(0, 160, size=1)
+            if not self.penalize:
+                state = self.np_random.choice(DamEnv.s_init, size=1)
+            else:
+                state = self.np_random.integers(0, 160, size=1)
 
         self.state = np.array(state, dtype=np.float32)
 
         if self.render_mode == "human":
             self.render()
 
         return self.state, {}
@@ -225,39 +248,43 @@
             return outfile.getvalue()
 
     def step(self, action):
         # bound the action
         actionLB = np.clip(self.state - DamEnv.S_MIN_REL, 0, None)
         actionUB = self.state
 
-        # Penalty proportional to the violation
-        bounded_action = np.clip(action, actionLB, actionUB)
-        penalty = -self.penalize * np.abs(bounded_action - action)
+        if self.normalized_action:
+            action = action * (actionUB - actionLB) + actionLB
+            penalty = 0.0
+        else:
+            # Penalty proportional to the violation
+            bounded_action = np.clip(action, actionLB, actionUB)
+            penalty = -self.penalize * np.abs(bounded_action - action)
+            action = bounded_action
 
         # transition dynamic
-        action = bounded_action
         self.last_action = action[0]
         self.dam_inflow = self.np_random.normal(DamEnv.DAM_INFLOW_MEAN, DamEnv.DAM_INFLOW_STD, len(self.state))[0]
         # small chance dam_inflow < 0
         n_state = np.clip(self.state + self.dam_inflow - action, 0, None).astype(np.float32)
 
         # cost due to excess level wrt a flooding threshold (upstream)
         self.excess = np.clip(n_state / DamEnv.S - DamEnv.H_FLO_U, 0, None)[0]
         r0 = -self.excess + penalty
         # deficit in the water supply wrt the water demand
         self.defict = -np.clip(DamEnv.W_IRR - action, 0, None)[0]
         r1 = self.defict + penalty
 
-        q = np.clip(action - DamEnv.Q_MEF, 0, None)
-        p_hyd = DamEnv.ETA * DamEnv.G * DamEnv.GAMMA_H2O * n_state / DamEnv.S * q / 3.6e6
+        q = np.clip(action[0] - DamEnv.Q_MEF, 0, None)
+        p_hyd = DamEnv.ETA * DamEnv.G * DamEnv.GAMMA_H2O * n_state[0] / DamEnv.S * q / 3.6e6
 
         # deficit in hydroelectric supply wrt hydroelectric demand
         r2 = -np.clip(DamEnv.W_HYD - p_hyd, 0, None) + penalty
         # cost due to excess level wrt a flooding threshold (downstream)
-        r3 = -np.clip(action - DamEnv.Q_FLO_D, 0, None) + penalty
+        r3 = -np.clip(action[0] - DamEnv.Q_FLO_D, 0, None) + penalty
 
         reward = np.array([r0, r1, r2, r3], dtype=np.float32)[: self.nO].flatten()
 
         self.state = n_state
 
         self.time_step += 1
         truncated = self.time_step >= self.time_limit
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium/utils.py` & `mo-gymnasium-1.0.0/mo_gymnasium/utils.py`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium.egg-info/PKG-INFO` & `mo-gymnasium-1.0.0/mo_gymnasium.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: mo-gymnasium
-Version: 0.3.4
+Version: 1.0.0
 Summary: A standard API for MORL and a diverse set of reference environments.
 Author-email: Farama Foundation <contact@farama.org>
 License: MIT License
 Project-URL: Homepage, https://mo-gymnasium.farama.org
 Project-URL: Repository, https://github.com/Farama-Foundation/MO-Gymnasium
 Project-URL: Documentation, https://mo-gymnasium.farama.org
 Project-URL: Bug Report, https://github.com/Farama-Foundation/MO-Gymnasium/issues
 Keywords: Reinforcement Learning,Multi-Objective,RL,AI,gymnasium
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: mario
 Provides-Extra: minecart
 Provides-Extra: mujoco
 Provides-Extra: highway
 Provides-Extra: box2d
 Provides-Extra: all
 Provides-Extra: testing
 License-File: LICENSE
 
 ![tests](https://github.com/Farama-Foundation/mo-gymnasium/workflows/Python%20tests/badge.svg)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-
-# MO-Gymnasium: Multi-Objective Reinforcement Learning Environments
+<p align="center">
+    <img src="docs/_static/img/MO-Gymnasium-text_small.png" width="500px"/>
+</p>
 
 <!-- start elevator-pitch -->
 
 MO-Gymnasium is an open source Python library for developing and comparing multi-objective reinforcement learning algorithms by providing a standard API to communicate between learning algorithms and environments, as well as a standard set of environments compliant with that API. Essentially, the environments follow the standard [Gymnasium API](https://github.com/Farama-Foundation/Gymnasium), but return vectorized rewards as numpy arrays.
 
 The documentation website is at [mo-gymnasium.farama.org](https://mo-gymnasium.farama.org), and we have a public discord server (which we also use to coordinate development work) that you can join here: https://discord.gg/bnJ6kubTg6.
 
@@ -93,19 +93,28 @@
 
 [MORL-Baselines](https://github.com/LucasAlegre/morl-baselines) is a repository containing various implementations of MORL algorithms by the same authors as MO-Gymnasium. It relies on the MO-Gymnasium API and shows various examples of the usage of wrappers and environments.
 
 ## Environment Versioning
 
 MO-Gymnasium keeps strict versioning for reproducibility reasons. All environments end in a suffix like "-v0".  When changes are made to environments that might impact learning results, the number is increased by one to prevent potential confusion.
 
+## Development Roadmap
+We have a roadmap for future development available here: https://github.com/Farama-Foundation/MO-Gymnasium/issues/66.
+
+## Project Maintainers
+
+Project Managers: [Lucas Alegre](https://github.com/LucasAlegre) and [Florian Felten](https://github.com/ffelten).
+
+Maintenance for this project is also contributed by the broader Farama team: [farama.org/team](https://farama.org/team).
+
 ## Citing
 
 <!-- start citation -->
 
-If you use this repository in your work, please cite:
+If you use this repository in your research, please cite:
 
 ```bibtex
 @inproceedings{Alegre+2022bnaic,
   author = {Lucas N. Alegre and Florian	Felten and El-Ghazali Talbi and Gr{\'e}goire Danoy and Ann Now{\'e} and Ana L. C. Bazzan and Bruno C. da Silva},
   title = {{MO-Gym}: A Library of Multi-Objective Reinforcement Learning Environments},
   booktitle = {Proceedings of the 34th Benelux Conference on Artificial Intelligence BNAIC/Benelearn 2022},
   year = {2022}
```

### Comparing `mo-gymnasium-0.3.4/mo_gymnasium.egg-info/SOURCES.txt` & `mo-gymnasium-1.0.0/mo_gymnasium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/pyproject.toml` & `mo-gymnasium-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 requires = ["setuptools >= 61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mo-gymnasium"
 description="A standard API for MORL and a diverse set of reference environments."
 readme = "README.md"
-requires-python = ">= 3.7"
+requires-python = ">= 3.8"
 authors = [{ name = "Farama Foundation", email = "contact@farama.org" }]
 license = { text = "MIT License" }
 keywords = ["Reinforcement Learning", "Multi-Objective", "RL", "AI", "gymnasium"]
 classifiers = [
     "Development Status :: 4 - Beta",  # change to `5 - Production/Stable` when ready
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
 ]
@@ -32,29 +31,29 @@
 dynamic = ["version"]
 
 [project.optional-dependencies]
 # Update dependencies in `all` if any are added or removed
 mario = ["nes-py", "gym-super-mario-bros"]
 minecart = ["scipy >=1.7.3  "]
 mujoco = ["mujoco >=2.3.0", "imageio >=2.14.1"]
-highway = ["highway-env"]
+highway = ["highway-env >=1.8"]
 box2d = ["box2d-py ==2.3.5", "pygame ==2.1.3.dev8", "swig ==4.*"]
 all = [
     # All dependencies above except accept-rom-license
     # NOTE: No need to manually remove the duplicates, setuptools automatically does that.
     # Mario
     "nes-py",
     "gym-super-mario-bros",
     # minecart
     "scipy >=1.7.3",
     # mujoco
     "imageio >=2.14.1",
-    "mujoco >=2.3.0",
+    "mujoco ==2.3.2",
     # highway
-    "highway-env >= 1.7.1",
+    "highway-env >= 1.8",
     # box2d
     "box2d-py ==2.3.5",
     "pygame ==2.1.3.dev8",
     "swig ==4.*",
 ]
 testing = ["pytest ==7.1.3"]
 
@@ -77,15 +76,15 @@
 ]
 
 # Linters and Test tools #######################################################
 
 [tool.black]
 safe = true
 line-length = 127
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
 [tool.isort]
 atomic = true
 profile = "black"
 src_paths = ["mo_gymnasium", "tests", "docs/scripts"]
 extra_standard_library = ["typing_extensions"]
@@ -95,15 +94,15 @@
 
 [tool.pyright]
 include = ["mo_gymnasium/**", "tests/**"]
 exclude = ["**/node_modules", "**/__pycache__"]
 strict = []
 
 typeCheckingMode = "basic"
-pythonVersion = "3.7"
+pythonVersion = "3.8"
 pythonPlatform = "All"
 typeshedPath = "typeshed"
 enableTypeIgnoreComments = true
 
 # This is required as the CI pre-commit does not download the module (i.e. numpy, pygame)
 #   Therefore, we have to ignore missing imports
 reportMissingImports = "none"
```

### Comparing `mo-gymnasium-0.3.4/setup.py` & `mo-gymnasium-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `mo-gymnasium-0.3.4/tests/test_envs.py` & `mo-gymnasium-1.0.0/tests/test_envs.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,29 +11,28 @@
 
 all_testing_env_specs = []
 for env_spec in gym.envs.registry.values():
     if type(env_spec.entry_point) is not str:
         continue
     # collect MO Gymnasium envs
     if env_spec.entry_point.split(".")[0] == "mo_gymnasium":
-        # Ignore highway as they do not deal with the random seed appropriately
-        if not env_spec.id.startswith("mo-highway"):
-            all_testing_env_specs.append(env_spec)
+        all_testing_env_specs.append(env_spec)
 
 
 @pytest.mark.parametrize(
     "spec",
     all_testing_env_specs,
     ids=[spec.id for spec in all_testing_env_specs],
 )
 def test_all_env_api(spec):
     """Check that all environments pass the environment checker."""
     env = mo_gym.make(spec.id)
     env = mo_gym.LinearReward(env)
     check_env(env, skip_render_check=True)
+    _test_reward_bounds(env.unwrapped)
     _test_pickle_env(env)
 
 
 @pytest.mark.parametrize("spec", all_testing_env_specs, ids=[spec.id for spec in all_testing_env_specs])
 def test_all_env_passive_env_checker(spec):
     env = mo_gym.make(spec.id)
     env.reset()
@@ -95,14 +94,27 @@
             env_1.reset(seed=SEED)
             env_2.reset(seed=SEED)
 
     env_1.close()
     env_2.close()
 
 
+def _test_reward_bounds(env: gym.Env):
+    """Test that the reward bounds are respected."""
+    assert env.reward_dim is not None
+    assert env.reward_space is not None
+    env.reset()
+    for _ in range(NUM_STEPS):
+        action = env.action_space.sample()
+        _, reward, terminated, truncated, _ = env.step(action)
+        assert env.reward_space.contains(reward)
+        if terminated or truncated:
+            env.reset()
+
+
 def _test_pickle_env(env: gym.Env):
     pickled_env = pickle.loads(pickle.dumps(env))
 
     data_equivalence(env.reset(), pickled_env.reset())
 
     action = env.action_space.sample()
     data_equivalence(env.step(action), pickled_env.step(action))
@@ -193,7 +205,29 @@
     env = mo_gym.make("deep-sea-treasure-concave-v0")
 
     known_pf = mo_gym.envs.deep_sea_treasure.deep_sea_treasure.CONCAVE_FRONT
 
     discounted_front = env.pareto_front(gamma=1.0)
     for desired, actual in zip(known_pf, discounted_front):
         np.testing.assert_array_almost_equal(desired, actual, decimal=2)
+
+
+def test_pf_fruit_tree():
+    env = mo_gym.make("fruit-tree-v0")
+    depth = 6
+
+    known_pf = np.array(mo_gym.envs.fruit_tree.fruit_tree.FRUITS[str(depth)]) * (0.99 ** (depth - 1))
+
+    discounted_front = env.pareto_front(gamma=0.99)
+    for desired, actual in zip(known_pf, discounted_front):
+        np.testing.assert_array_almost_equal(desired, actual, decimal=2)
+
+
+def test_pf_fruit_tree_no_discount():
+    env = mo_gym.make("fruit-tree-v0")
+    depth = 6
+
+    known_pf = mo_gym.envs.fruit_tree.fruit_tree.FRUITS[str(depth)]
+
+    discounted_front = env.pareto_front(gamma=1.0)
+    for desired, actual in zip(known_pf, discounted_front):
+        np.testing.assert_array_almost_equal(desired, actual, decimal=2)
```

### Comparing `mo-gymnasium-0.3.4/tests/test_wrappers.py` & `mo-gymnasium-1.0.0/tests/test_wrappers.py`

 * *Files identical despite different names*

