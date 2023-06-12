# Comparing `tmp/snagboot-1.0.tar.gz` & `tmp/snagboot-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snagboot-1.0.tar", last modified: Tue May 23 14:38:41 2023, max compression
+gzip compressed data, was "snagboot-1.1.tar", last modified: Mon Jun 12 08:44:06 2023, max compression
```

## Comparing `snagboot-1.0.tar` & `snagboot-1.1.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-05-23 14:38:41.864355 snagboot-1.0/
--rw-r--r--   0 rgant     (1000) rgant     (1000)    18092 2023-05-19 12:46:21.000000 snagboot-1.0/LICENSE
--rw-r--r--   0 rgant     (1000) rgant     (1000)      347 2023-05-23 07:14:40.000000 snagboot-1.0/MANIFEST.in
--rw-r--r--   0 rgant     (1000) rgant     (1000)     3965 2023-05-23 14:38:41.864355 snagboot-1.0/PKG-INFO
--rw-r--r--   0 rgant     (1000) rgant     (1000)     3468 2023-05-23 09:37:51.000000 snagboot-1.0/README.md
--rw-r--r--   0 rgant     (1000) rgant     (1000)     2498 2023-05-23 07:16:32.000000 snagboot-1.0/pyproject.toml
--rw-r--r--   0 rgant     (1000) rgant     (1000)       38 2023-05-23 14:38:41.864355 snagboot-1.0/setup.cfg
-drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-05-23 14:38:41.851355 snagboot-1.0/src/
-drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-05-23 14:38:41.853356 snagboot-1.0/src/snagboot.egg-info/
--rw-r--r--   0 rgant     (1000) rgant     (1000)     3965 2023-05-23 14:38:41.000000 snagboot-1.0/src/snagboot.egg-info/PKG-INFO
--rw-r--r--   0 rgant     (1000) rgant     (1000)     2685 2023-05-23 14:38:41.000000 snagboot-1.0/src/snagboot.egg-info/SOURCES.txt
--rw-r--r--   0 rgant     (1000) rgant     (1000)        1 2023-05-23 14:38:41.000000 snagboot-1.0/src/snagboot.egg-info/dependency_links.txt
--rw-r--r--   0 rgant     (1000) rgant     (1000)       82 2023-05-23 14:38:41.000000 snagboot-1.0/src/snagboot.egg-info/entry_points.txt
--rw-r--r--   0 rgant     (1000) rgant     (1000)      139 2023-05-23 14:38:41.000000 snagboot-1.0/src/snagboot.egg-info/requires.txt
--rw-r--r--   0 rgant     (1000) rgant     (1000)       22 2023-05-23 14:38:41.000000 snagboot-1.0/src/snagboot.egg-info/top_level.txt
-drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-05-23 14:38:41.854355 snagboot-1.0/src/snagflash/
--rw-r--r--   0 rgant     (1000) rgant     (1000)       46 2023-05-19 08:49:49.000000 snagboot-1.0/src/snagflash/__init__.py
-drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-05-23 14:38:41.855355 snagboot-1.0/src/snagflash/bmaptools/
--rw-r--r--   0 rgant     (1000) rgant     (1000)    37922 2023-05-19 08:49:49.000000 snagboot-1.0/src/snagflash/bmaptools/BmapCopy.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)    13417 2023-05-19 08:49:49.000000 snagboot-1.0/src/snagflash/bmaptools/BmapCreate.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     4389 2023-05-19 08:49:49.000000 snagboot-1.0/src/snagflash/bmaptools/BmapHelpers.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)    20678 2023-05-19 08:49:49.000000 snagboot-1.0/src/snagflash/bmaptools/Filemap.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)        0 2023-05-19 08:49:49.000000 snagboot-1.0/src/snagflash/bmaptools/__init__.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     4398 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagflash/cli.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     2047 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagflash/dfu.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     1768 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagflash/fastboot.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     3481 2023-05-23 07:30:28.000000 snagboot-1.0/src/snagflash/ums.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     1225 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagflash/utils.py
-drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-05-23 14:38:41.856356 snagboot-1.0/src/snagrecover/
--rw-r--r--   0 rgant     (1000) rgant     (1000)     6552 2023-05-15 12:19:39.000000 snagboot-1.0/src/snagrecover/80-snagboot.rules
--rw-r--r--   0 rgant     (1000) rgant     (1000)       52 2023-05-19 08:49:49.000000 snagboot-1.0/src/snagrecover/__init__.py
--rwxr-xr-x   0 rgant     (1000) rgant     (1000)     6196 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/am335x_usb_setup.sh
--rw-r--r--   0 rgant     (1000) rgant     (1000)     6346 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/cli.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     3779 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/config.py
-drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-05-23 14:38:41.858355 snagboot-1.0/src/snagrecover/firmware/
--rw-r--r--   0 rgant     (1000) rgant     (1000)       97 2023-05-19 08:49:49.000000 snagboot-1.0/src/snagrecover/firmware/__init__.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     5535 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/firmware/am335x_fw.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     4101 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/firmware/firmware.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     7033 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/firmware/imx_fw.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     4434 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/firmware/ivt.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     4192 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/firmware/rom_container.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     2200 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/firmware/sama5_fw.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     6735 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/firmware/samba_applet.py
-drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-05-23 14:38:41.859356 snagboot-1.0/src/snagrecover/firmware/sunxi_fw/
--rw-r--r--   0 rgant     (1000) rgant     (1000)        0 2023-05-19 08:49:49.000000 snagboot-1.0/src/snagrecover/firmware/sunxi_fw/__init__.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     4704 2023-05-09 10:22:17.000000 snagboot-1.0/src/snagrecover/firmware/sunxi_fw/fel-to-spl-thunk.S
--rw-r--r--   0 rgant     (1000) rgant     (1000)      276 2023-05-09 10:22:17.000000 snagboot-1.0/src/snagrecover/firmware/sunxi_fw/fel-to-spl-thunk.bin
--rw-r--r--   0 rgant     (1000) rgant     (1000)     6604 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/firmware/sunxi_fw/mmu.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     8741 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/firmware/sunxi_fw/soc_info.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)    16299 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/firmware/sunxi_fw/sunxi_fw.py
-drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-05-23 14:38:41.860355 snagboot-1.0/src/snagrecover/protocols/
--rw-r--r--   0 rgant     (1000) rgant     (1000)      211 2023-05-19 08:49:49.000000 snagboot-1.0/src/snagrecover/protocols/__init__.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     3751 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/protocols/bootp.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     6445 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/protocols/dfu.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     5638 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/protocols/fastboot.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     6443 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/protocols/fel.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     2198 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/protocols/hab_constants.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     8328 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/protocols/imx_sdp.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     1890 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/protocols/memory_ops.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     2619 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/protocols/sambamon.py
-drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-05-23 14:38:41.862356 snagboot-1.0/src/snagrecover/recoveries/
--rw-r--r--   0 rgant     (1000) rgant     (1000)      167 2023-05-19 08:49:49.000000 snagboot-1.0/src/snagrecover/recoveries/__init__.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     1810 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/recoveries/am335x.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)      771 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/recoveries/am62x.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     5145 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/recoveries/imx.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     4050 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/recoveries/sama5.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     2367 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/recoveries/stm32_flashlayout.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     2959 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/recoveries/stm32mp1.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     2777 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/recoveries/sunxi.py
--rw-r--r--   0 rgant     (1000) rgant     (1000)     1852 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/supported_socs.yaml
-drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-05-23 14:38:41.864355 snagboot-1.0/src/snagrecover/templates/
--rw-r--r--   0 rgant     (1000) rgant     (1000)       68 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/templates/am335x-beaglebone-black.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)       87 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/templates/am62x-beagle-play.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)       31 2023-05-10 11:51:16.000000 snagboot-1.0/src/snagrecover/templates/imx28-evk.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)       40 2023-05-09 10:22:17.000000 snagboot-1.0/src/snagrecover/templates/imx6-colibri-imx6ull.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)      196 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/templates/imx6-var-som-mx6.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)       40 2023-05-09 10:22:17.000000 snagboot-1.0/src/snagrecover/templates/imx7-colibri-imx7d.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)      182 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/templates/imx8-dart-mx8m-mini.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)      454 2023-05-19 08:49:24.000000 snagboot-1.0/src/snagrecover/templates/sama5-sama5d2xplained.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)      454 2023-05-19 08:49:24.000000 snagboot-1.0/src/snagrecover/templates/sama5-sama5d3xplained.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)      454 2023-05-19 08:49:24.000000 snagboot-1.0/src/snagrecover/templates/sama5-sama5d4xplained.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)       65 2023-05-11 14:59:15.000000 snagboot-1.0/src/snagrecover/templates/stm32mp1-stm32mp135f-dk.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)       66 2023-05-11 14:37:47.000000 snagboot-1.0/src/snagrecover/templates/stm32mp1-stm32mp157f-dk2.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)       58 2023-05-09 10:22:17.000000 snagboot-1.0/src/snagrecover/templates/sunxi-orangepi-pc.yaml
--rw-r--r--   0 rgant     (1000) rgant     (1000)     1362 2023-05-23 07:14:40.000000 snagboot-1.0/src/snagrecover/utils.py
+drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-06-12 08:44:06.649531 snagboot-1.1/
+-rw-r--r--   0 rgant     (1000) rgant     (1000)    18092 2023-05-19 12:46:21.000000 snagboot-1.1/LICENSE
+-rw-r--r--   0 rgant     (1000) rgant     (1000)      347 2023-06-12 08:05:36.000000 snagboot-1.1/MANIFEST.in
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     4461 2023-06-12 08:44:06.649531 snagboot-1.1/PKG-INFO
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     3964 2023-06-12 08:05:36.000000 snagboot-1.1/README.md
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     2498 2023-06-12 08:11:22.000000 snagboot-1.1/pyproject.toml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       38 2023-06-12 08:44:06.649531 snagboot-1.1/setup.cfg
+drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-06-12 08:44:06.636531 snagboot-1.1/src/
+drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-06-12 08:44:06.638531 snagboot-1.1/src/snagboot.egg-info/
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     4461 2023-06-12 08:44:06.000000 snagboot-1.1/src/snagboot.egg-info/PKG-INFO
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     2768 2023-06-12 08:44:06.000000 snagboot-1.1/src/snagboot.egg-info/SOURCES.txt
+-rw-r--r--   0 rgant     (1000) rgant     (1000)        1 2023-06-12 08:44:06.000000 snagboot-1.1/src/snagboot.egg-info/dependency_links.txt
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       82 2023-06-12 08:44:06.000000 snagboot-1.1/src/snagboot.egg-info/entry_points.txt
+-rw-r--r--   0 rgant     (1000) rgant     (1000)      139 2023-06-12 08:44:06.000000 snagboot-1.1/src/snagboot.egg-info/requires.txt
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       22 2023-06-12 08:44:06.000000 snagboot-1.1/src/snagboot.egg-info/top_level.txt
+drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-06-12 08:44:06.639531 snagboot-1.1/src/snagflash/
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       46 2023-05-19 08:49:49.000000 snagboot-1.1/src/snagflash/__init__.py
+drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-06-12 08:44:06.640531 snagboot-1.1/src/snagflash/bmaptools/
+-rw-r--r--   0 rgant     (1000) rgant     (1000)    37922 2023-05-19 08:49:49.000000 snagboot-1.1/src/snagflash/bmaptools/BmapCopy.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)    13417 2023-05-19 08:49:49.000000 snagboot-1.1/src/snagflash/bmaptools/BmapCreate.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     4389 2023-05-19 08:49:49.000000 snagboot-1.1/src/snagflash/bmaptools/BmapHelpers.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)    20678 2023-05-19 08:49:49.000000 snagboot-1.1/src/snagflash/bmaptools/Filemap.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)        0 2023-05-19 08:49:49.000000 snagboot-1.1/src/snagflash/bmaptools/__init__.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     4398 2023-05-24 08:56:19.000000 snagboot-1.1/src/snagflash/cli.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     2047 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagflash/dfu.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     1768 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagflash/fastboot.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     3481 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagflash/ums.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     1224 2023-06-12 08:05:36.000000 snagboot-1.1/src/snagflash/utils.py
+drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-06-12 08:44:06.641531 snagboot-1.1/src/snagrecover/
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     6493 2023-06-12 08:05:36.000000 snagboot-1.1/src/snagrecover/50-snagboot.rules
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       52 2023-05-19 08:49:49.000000 snagboot-1.1/src/snagrecover/__init__.py
+-rwxr-xr-x   0 rgant     (1000) rgant     (1000)     6196 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/am335x_usb_setup.sh
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     6346 2023-06-12 08:05:36.000000 snagboot-1.1/src/snagrecover/cli.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     3779 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/config.py
+drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-06-12 08:44:06.642531 snagboot-1.1/src/snagrecover/firmware/
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       97 2023-05-19 08:49:49.000000 snagboot-1.1/src/snagrecover/firmware/__init__.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     5535 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/firmware/am335x_fw.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     4101 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/firmware/firmware.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     7587 2023-06-12 08:05:31.000000 snagboot-1.1/src/snagrecover/firmware/imx_fw.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     4434 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/firmware/ivt.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     4179 2023-06-12 08:05:31.000000 snagboot-1.1/src/snagrecover/firmware/rom_container.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     2200 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/firmware/sama5_fw.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     6735 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/firmware/samba_applet.py
+drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-06-12 08:44:06.643531 snagboot-1.1/src/snagrecover/firmware/sunxi_fw/
+-rw-r--r--   0 rgant     (1000) rgant     (1000)        0 2023-05-19 08:49:49.000000 snagboot-1.1/src/snagrecover/firmware/sunxi_fw/__init__.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     4704 2023-05-09 10:22:17.000000 snagboot-1.1/src/snagrecover/firmware/sunxi_fw/fel-to-spl-thunk.S
+-rw-r--r--   0 rgant     (1000) rgant     (1000)      276 2023-05-09 10:22:17.000000 snagboot-1.1/src/snagrecover/firmware/sunxi_fw/fel-to-spl-thunk.bin
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     6604 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/firmware/sunxi_fw/mmu.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     8741 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/firmware/sunxi_fw/soc_info.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)    16299 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/firmware/sunxi_fw/sunxi_fw.py
+drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-06-12 08:44:06.645531 snagboot-1.1/src/snagrecover/protocols/
+-rw-r--r--   0 rgant     (1000) rgant     (1000)      211 2023-05-19 08:49:49.000000 snagboot-1.1/src/snagrecover/protocols/__init__.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     3751 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/protocols/bootp.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     6445 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/protocols/dfu.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     5638 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/protocols/fastboot.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     6443 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/protocols/fel.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     2198 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/protocols/hab_constants.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     8670 2023-06-12 08:05:31.000000 snagboot-1.1/src/snagrecover/protocols/imx_sdp.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     1890 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/protocols/memory_ops.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     2619 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/protocols/sambamon.py
+drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-06-12 08:44:06.646531 snagboot-1.1/src/snagrecover/recoveries/
+-rw-r--r--   0 rgant     (1000) rgant     (1000)      167 2023-05-19 08:49:49.000000 snagboot-1.1/src/snagrecover/recoveries/__init__.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     1810 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/recoveries/am335x.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)      771 2023-05-23 07:14:40.000000 snagboot-1.1/src/snagrecover/recoveries/am62x.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     5258 2023-06-12 08:05:31.000000 snagboot-1.1/src/snagrecover/recoveries/imx.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     4050 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/recoveries/sama5.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     2367 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/recoveries/stm32_flashlayout.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     2959 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/recoveries/stm32mp1.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     2777 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/recoveries/sunxi.py
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     1852 2023-06-12 08:05:31.000000 snagboot-1.1/src/snagrecover/supported_socs.yaml
+drwxr-xr-x   0 rgant     (1000) rgant     (1000)        0 2023-06-12 08:44:06.648531 snagboot-1.1/src/snagrecover/templates/
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       68 2023-05-23 07:14:40.000000 snagboot-1.1/src/snagrecover/templates/am335x-beaglebone-black.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       87 2023-05-23 07:14:40.000000 snagboot-1.1/src/snagrecover/templates/am62x-beagle-play.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       29 2023-06-12 08:05:31.000000 snagboot-1.1/src/snagrecover/templates/imx28-evk.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       40 2023-05-09 10:22:17.000000 snagboot-1.1/src/snagrecover/templates/imx6-colibri-imx6ull.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)      196 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/templates/imx6-var-som-mx6.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       40 2023-05-09 10:22:17.000000 snagboot-1.1/src/snagrecover/templates/imx7-colibri-imx7d.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)      182 2023-05-24 07:07:01.000000 snagboot-1.1/src/snagrecover/templates/imx8-dart-mx8m-mini.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       55 2023-06-12 08:05:31.000000 snagboot-1.1/src/snagrecover/templates/imx8qm-mek.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       61 2023-06-12 08:05:31.000000 snagboot-1.1/src/snagrecover/templates/imx93-evk.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)      454 2023-05-19 08:49:24.000000 snagboot-1.1/src/snagrecover/templates/sama5-sama5d2xplained.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)      454 2023-05-19 08:49:24.000000 snagboot-1.1/src/snagrecover/templates/sama5-sama5d3xplained.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)      454 2023-05-19 08:49:24.000000 snagboot-1.1/src/snagrecover/templates/sama5-sama5d4xplained.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       65 2023-05-11 14:59:15.000000 snagboot-1.1/src/snagrecover/templates/stm32mp1-stm32mp135f-dk.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       66 2023-05-11 14:37:47.000000 snagboot-1.1/src/snagrecover/templates/stm32mp1-stm32mp157f-dk2.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)       58 2023-05-09 10:22:17.000000 snagboot-1.1/src/snagrecover/templates/sunxi-orangepi-pc.yaml
+-rw-r--r--   0 rgant     (1000) rgant     (1000)     1362 2023-05-23 07:14:40.000000 snagboot-1.1/src/snagrecover/utils.py
```

### Comparing `snagboot-1.0/LICENSE` & `snagboot-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/PKG-INFO` & `snagboot-1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snagboot
-Version: 1.0
+Version: 1.1
 Summary: Generic recovery and reflashing tool for embedded platforms
 Author-email: Romain Gantois <romain.gantois@bootlin.com>
 Project-URL: Source Code, https://github.com/bootlin/snagboot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
@@ -26,15 +26,15 @@
 
 <p align="center">
   <img src="docs/tutorial_snagrecover.gif" alt="animated" />
 </p>
 
 The currently supported SoC families are ST STM32MP1, Microchip SAMA5, NXP
 i.MX6/7/8, TI AM335x, Allwinner SUNXI and TI AM62x. Please check
-[supported_socs.yaml](src/snagrecover/supported_socs.yaml) or run `snagrecover
+[supported_socs.yaml](https://github.com/bootlin/snagboot/blob/main/src/snagrecover/supported_socs.yaml) or run `snagrecover
 --list-socs` for a more precise list of supported SoCs.
 
 ## Installation
 
 Requirements:
 
  * One of the libhidapi backends. On Debian, you can install the
@@ -51,63 +51,67 @@
 $ snagflash -h
 ```
 
 You also need to install udev rules so that snagrecover has read and write
 access to the USB devices exposed by the SoCs.
 
 ```bash
-$ snagrecover --udev > 80-snagboot.rules
-$ sudo cp 80-snagboot.rules /etc/udev/rules.d/
+$ snagrecover --udev > 50-snagboot.rules
+$ sudo cp 50-snagboot.rules /etc/udev/rules.d/
 $ sudo udevadm control --reload-rules
 $ sudo udevadm trigger
 ```
 
-The affected devices will be accessible to the "plugdev" group, so please check
-that you are part of this group. You can also modify the udev rules to pick a
-more restrictive group if you wish.
-
-**Warning:** The "plugdev" group does not exist on Fedora, please make sure you
-modify the udev rules before installing them! You should replace "plugdev" with
-any group you wish, e.g. "users". 
+These rules work by adding the "uaccess" tag to the relevant USB devices.
+Systemd will then add an ACL to give access to currently logged in users. More
+info
+[here](https://enotty.pipebreaker.pl/2012/05/23/linux-automatic-user-acl-management/). 
+
+**Warning:** If your distro does not use systemd, the "uaccess" method could
+possibly not work. In this case, make sure to customize the provided udev rules
+for your specific system.
 
 Alternatively, Snagboot can be installed as a local Python wheel. An
 installation script is provided to automatically build and install the package.
 
 ```bash
 $ cd snagboot
 $ ./install.sh
 ```
 
+There is also an [AUR package](https://aur.archlinux.org/packages/snagboot)
+available.
+
 ## Usage guide
 
 **Note:** Running snagboot as root is not recommended and will typically not
 work, since it is probably installed for the current user only
 
 To recover and reflash a board using snagboot:
 
 1. Check that your SoC is supported in snagrecover by running: `snagrecover --list-socs`
-2. [Setup your board for recovery](docs/board_setup.md)
-3. [Build or download the firmware binaries necessary for recovering and reflashing the board.](docs/fw_binaries.md)
-4. [Run snagrecover](docs/snagrecover.md) and check that the recovery was a success i.e. that U-Boot is running properly.
-5. [Run snagflash](docs/snagflash.md) to reflash the board
+2. [Setup your board for recovery](https://github.com/bootlin/snagboot/blob/main/docs/board_setup.md)
+3. [Build or download the firmware binaries necessary for recovering and reflashing the board.](https://github.com/bootlin/snagboot/blob/main/docs/fw_binaries.md)
+4. [Run snagrecover](https://github.com/bootlin/snagboot/blob/main/docs/snagrecover.md) and check that the recovery was a success i.e. that U-Boot is running properly.
+5. [Run snagflash](https://github.com/bootlin/snagboot/blob/main/docs/snagflash.md) to reflash the board
 
 If you encounter issues, please take a look at the
-[troubleshooting](docs/troubleshooting.md) section.
+[troubleshooting](https://github.com/bootlin/snagboot/blob/main/docs/troubleshooting.md) section.
 
 You can play the snagrecover tutorial in your terminal!
 
 ```
 sudo apt install asciinema
 asciinema play -s=2 docs/tutorial_snagrecover.cast
 ```
 
 ## Contributing
 
 Contributions are welcome! Since Snagboot includes many different recovery
 techniques and protocols, we try to keep the code base as structured as
-possible. Please consult the [contribution guidelines](CONTRIBUTING.md).
+possible. Please consult the [contribution guidelines](https://github.com/bootlin/snagboot/blob/main/CONTRIBUTING.md).
 
 ## License
 
-Snagboot is released under the [GNU General Public License version 2](LICENSE)
+Snagboot is released under the [GNU General Public License version 2](https://github.com/bootlin/snagboot/blob/main/LICENSE)
```

### Comparing `snagboot-1.0/README.md` & `snagboot-1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 <p align="center">
   <img src="docs/tutorial_snagrecover.gif" alt="animated" />
 </p>
 
 The currently supported SoC families are ST STM32MP1, Microchip SAMA5, NXP
 i.MX6/7/8, TI AM335x, Allwinner SUNXI and TI AM62x. Please check
-[supported_socs.yaml](src/snagrecover/supported_socs.yaml) or run `snagrecover
+[supported_socs.yaml](https://github.com/bootlin/snagboot/blob/main/src/snagrecover/supported_socs.yaml) or run `snagrecover
 --list-socs` for a more precise list of supported SoCs.
 
 ## Installation
 
 Requirements:
 
  * One of the libhidapi backends. On Debian, you can install the
@@ -38,63 +38,67 @@
 $ snagflash -h
 ```
 
 You also need to install udev rules so that snagrecover has read and write
 access to the USB devices exposed by the SoCs.
 
 ```bash
-$ snagrecover --udev > 80-snagboot.rules
-$ sudo cp 80-snagboot.rules /etc/udev/rules.d/
+$ snagrecover --udev > 50-snagboot.rules
+$ sudo cp 50-snagboot.rules /etc/udev/rules.d/
 $ sudo udevadm control --reload-rules
 $ sudo udevadm trigger
 ```
 
-The affected devices will be accessible to the "plugdev" group, so please check
-that you are part of this group. You can also modify the udev rules to pick a
-more restrictive group if you wish.
-
-**Warning:** The "plugdev" group does not exist on Fedora, please make sure you
-modify the udev rules before installing them! You should replace "plugdev" with
-any group you wish, e.g. "users". 
+These rules work by adding the "uaccess" tag to the relevant USB devices.
+Systemd will then add an ACL to give access to currently logged in users. More
+info
+[here](https://enotty.pipebreaker.pl/2012/05/23/linux-automatic-user-acl-management/). 
+
+**Warning:** If your distro does not use systemd, the "uaccess" method could
+possibly not work. In this case, make sure to customize the provided udev rules
+for your specific system.
 
 Alternatively, Snagboot can be installed as a local Python wheel. An
 installation script is provided to automatically build and install the package.
 
 ```bash
 $ cd snagboot
 $ ./install.sh
 ```
 
+There is also an [AUR package](https://aur.archlinux.org/packages/snagboot)
+available.
+
 ## Usage guide
 
 **Note:** Running snagboot as root is not recommended and will typically not
 work, since it is probably installed for the current user only
 
 To recover and reflash a board using snagboot:
 
 1. Check that your SoC is supported in snagrecover by running: `snagrecover --list-socs`
-2. [Setup your board for recovery](docs/board_setup.md)
-3. [Build or download the firmware binaries necessary for recovering and reflashing the board.](docs/fw_binaries.md)
-4. [Run snagrecover](docs/snagrecover.md) and check that the recovery was a success i.e. that U-Boot is running properly.
-5. [Run snagflash](docs/snagflash.md) to reflash the board
+2. [Setup your board for recovery](https://github.com/bootlin/snagboot/blob/main/docs/board_setup.md)
+3. [Build or download the firmware binaries necessary for recovering and reflashing the board.](https://github.com/bootlin/snagboot/blob/main/docs/fw_binaries.md)
+4. [Run snagrecover](https://github.com/bootlin/snagboot/blob/main/docs/snagrecover.md) and check that the recovery was a success i.e. that U-Boot is running properly.
+5. [Run snagflash](https://github.com/bootlin/snagboot/blob/main/docs/snagflash.md) to reflash the board
 
 If you encounter issues, please take a look at the
-[troubleshooting](docs/troubleshooting.md) section.
+[troubleshooting](https://github.com/bootlin/snagboot/blob/main/docs/troubleshooting.md) section.
 
 You can play the snagrecover tutorial in your terminal!
 
 ```
 sudo apt install asciinema
 asciinema play -s=2 docs/tutorial_snagrecover.cast
 ```
 
 ## Contributing
 
 Contributions are welcome! Since Snagboot includes many different recovery
 techniques and protocols, we try to keep the code base as structured as
-possible. Please consult the [contribution guidelines](CONTRIBUTING.md).
+possible. Please consult the [contribution guidelines](https://github.com/bootlin/snagboot/blob/main/CONTRIBUTING.md).
 
 ## License
 
-Snagboot is released under the [GNU General Public License version 2](LICENSE)
+Snagboot is released under the [GNU General Public License version 2](https://github.com/bootlin/snagboot/blob/main/LICENSE)
```

### Comparing `snagboot-1.0/pyproject.toml` & `snagboot-1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "snagboot"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="Romain Gantois", email="romain.gantois@bootlin.com" },
 ]
 description = "Generic recovery and reflashing tool for embedded platforms"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `snagboot-1.0/src/snagboot.egg-info/PKG-INFO` & `snagboot-1.1/src/snagboot.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snagboot
-Version: 1.0
+Version: 1.1
 Summary: Generic recovery and reflashing tool for embedded platforms
 Author-email: Romain Gantois <romain.gantois@bootlin.com>
 Project-URL: Source Code, https://github.com/bootlin/snagboot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
@@ -26,15 +26,15 @@
 
 <p align="center">
   <img src="docs/tutorial_snagrecover.gif" alt="animated" />
 </p>
 
 The currently supported SoC families are ST STM32MP1, Microchip SAMA5, NXP
 i.MX6/7/8, TI AM335x, Allwinner SUNXI and TI AM62x. Please check
-[supported_socs.yaml](src/snagrecover/supported_socs.yaml) or run `snagrecover
+[supported_socs.yaml](https://github.com/bootlin/snagboot/blob/main/src/snagrecover/supported_socs.yaml) or run `snagrecover
 --list-socs` for a more precise list of supported SoCs.
 
 ## Installation
 
 Requirements:
 
  * One of the libhidapi backends. On Debian, you can install the
@@ -51,63 +51,67 @@
 $ snagflash -h
 ```
 
 You also need to install udev rules so that snagrecover has read and write
 access to the USB devices exposed by the SoCs.
 
 ```bash
-$ snagrecover --udev > 80-snagboot.rules
-$ sudo cp 80-snagboot.rules /etc/udev/rules.d/
+$ snagrecover --udev > 50-snagboot.rules
+$ sudo cp 50-snagboot.rules /etc/udev/rules.d/
 $ sudo udevadm control --reload-rules
 $ sudo udevadm trigger
 ```
 
-The affected devices will be accessible to the "plugdev" group, so please check
-that you are part of this group. You can also modify the udev rules to pick a
-more restrictive group if you wish.
-
-**Warning:** The "plugdev" group does not exist on Fedora, please make sure you
-modify the udev rules before installing them! You should replace "plugdev" with
-any group you wish, e.g. "users". 
+These rules work by adding the "uaccess" tag to the relevant USB devices.
+Systemd will then add an ACL to give access to currently logged in users. More
+info
+[here](https://enotty.pipebreaker.pl/2012/05/23/linux-automatic-user-acl-management/). 
+
+**Warning:** If your distro does not use systemd, the "uaccess" method could
+possibly not work. In this case, make sure to customize the provided udev rules
+for your specific system.
 
 Alternatively, Snagboot can be installed as a local Python wheel. An
 installation script is provided to automatically build and install the package.
 
 ```bash
 $ cd snagboot
 $ ./install.sh
 ```
 
+There is also an [AUR package](https://aur.archlinux.org/packages/snagboot)
+available.
+
 ## Usage guide
 
 **Note:** Running snagboot as root is not recommended and will typically not
 work, since it is probably installed for the current user only
 
 To recover and reflash a board using snagboot:
 
 1. Check that your SoC is supported in snagrecover by running: `snagrecover --list-socs`
-2. [Setup your board for recovery](docs/board_setup.md)
-3. [Build or download the firmware binaries necessary for recovering and reflashing the board.](docs/fw_binaries.md)
-4. [Run snagrecover](docs/snagrecover.md) and check that the recovery was a success i.e. that U-Boot is running properly.
-5. [Run snagflash](docs/snagflash.md) to reflash the board
+2. [Setup your board for recovery](https://github.com/bootlin/snagboot/blob/main/docs/board_setup.md)
+3. [Build or download the firmware binaries necessary for recovering and reflashing the board.](https://github.com/bootlin/snagboot/blob/main/docs/fw_binaries.md)
+4. [Run snagrecover](https://github.com/bootlin/snagboot/blob/main/docs/snagrecover.md) and check that the recovery was a success i.e. that U-Boot is running properly.
+5. [Run snagflash](https://github.com/bootlin/snagboot/blob/main/docs/snagflash.md) to reflash the board
 
 If you encounter issues, please take a look at the
-[troubleshooting](docs/troubleshooting.md) section.
+[troubleshooting](https://github.com/bootlin/snagboot/blob/main/docs/troubleshooting.md) section.
 
 You can play the snagrecover tutorial in your terminal!
 
 ```
 sudo apt install asciinema
 asciinema play -s=2 docs/tutorial_snagrecover.cast
 ```
 
 ## Contributing
 
 Contributions are welcome! Since Snagboot includes many different recovery
 techniques and protocols, we try to keep the code base as structured as
-possible. Please consult the [contribution guidelines](CONTRIBUTING.md).
+possible. Please consult the [contribution guidelines](https://github.com/bootlin/snagboot/blob/main/CONTRIBUTING.md).
 
 ## License
 
-Snagboot is released under the [GNU General Public License version 2](LICENSE)
+Snagboot is released under the [GNU General Public License version 2](https://github.com/bootlin/snagboot/blob/main/LICENSE)
```

### Comparing `snagboot-1.0/src/snagboot.egg-info/SOURCES.txt` & `snagboot-1.1/src/snagboot.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 src/snagflash/ums.py
 src/snagflash/utils.py
 src/snagflash/bmaptools/BmapCopy.py
 src/snagflash/bmaptools/BmapCreate.py
 src/snagflash/bmaptools/BmapHelpers.py
 src/snagflash/bmaptools/Filemap.py
 src/snagflash/bmaptools/__init__.py
-src/snagrecover/80-snagboot.rules
+src/snagrecover/50-snagboot.rules
 src/snagrecover/__init__.py
 src/snagrecover/am335x_usb_setup.sh
 src/snagrecover/cli.py
 src/snagrecover/config.py
 src/snagrecover/supported_socs.yaml
 src/snagrecover/utils.py
 src/snagrecover/firmware/__init__.py
@@ -60,13 +60,15 @@
 src/snagrecover/templates/am335x-beaglebone-black.yaml
 src/snagrecover/templates/am62x-beagle-play.yaml
 src/snagrecover/templates/imx28-evk.yaml
 src/snagrecover/templates/imx6-colibri-imx6ull.yaml
 src/snagrecover/templates/imx6-var-som-mx6.yaml
 src/snagrecover/templates/imx7-colibri-imx7d.yaml
 src/snagrecover/templates/imx8-dart-mx8m-mini.yaml
+src/snagrecover/templates/imx8qm-mek.yaml
+src/snagrecover/templates/imx93-evk.yaml
 src/snagrecover/templates/sama5-sama5d2xplained.yaml
 src/snagrecover/templates/sama5-sama5d3xplained.yaml
 src/snagrecover/templates/sama5-sama5d4xplained.yaml
 src/snagrecover/templates/stm32mp1-stm32mp135f-dk.yaml
 src/snagrecover/templates/stm32mp1-stm32mp157f-dk2.yaml
 src/snagrecover/templates/sunxi-orangepi-pc.yaml
```

### Comparing `snagboot-1.0/src/snagflash/bmaptools/BmapCopy.py` & `snagboot-1.1/src/snagflash/bmaptools/BmapCopy.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagflash/bmaptools/BmapCreate.py` & `snagboot-1.1/src/snagflash/bmaptools/BmapCreate.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagflash/bmaptools/BmapHelpers.py` & `snagboot-1.1/src/snagflash/bmaptools/BmapHelpers.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagflash/bmaptools/Filemap.py` & `snagboot-1.1/src/snagflash/bmaptools/Filemap.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagflash/cli.py` & `snagboot-1.1/src/snagflash/cli.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagflash/dfu.py` & `snagboot-1.1/src/snagflash/dfu.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagflash/fastboot.py` & `snagboot-1.1/src/snagflash/fastboot.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagflash/ums.py` & `snagboot-1.1/src/snagflash/ums.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagflash/utils.py` & `snagboot-1.1/src/snagflash/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import sys
 
 USB_RETRIES = 5
 
 def usb_error(vid: int, pid: int):
 	print(f"Device access error: could not open USB device {vid:04x}:{pid:04x}", file=sys.stderr)
 	print("If the device exists, make sure that you have rw access rights to it", file=sys.stderr)
-	print("If that is not the case, you can add the following line to your /etc/udev/rules.d/80-snagboot.rules file:\n", file=sys.stderr)
-	print("SUBSYSTEM==\"usb\", ATTRS{idVendor}==\"" + f"{vid:04x}" + "\", ATTRS{idProduct}==\"" + f"{pid:04x}" + "\", MODE=\"0660\", GROUP=\"plugdev\"", file=sys.stderr)
+	print("If that is not the case, you can add the following line to your /etc/udev/rules.d/50-snagboot.rules file:\n", file=sys.stderr)
+	print("SUBSYSTEM==\"usb\", ATTRS{idVendor}==\"" + f"{vid:04x}" + "\", ATTRS{idProduct}==\"" + f"{pid:04x}" + "\", MODE=\"0660\", TAG+=\"uaccess\"", file=sys.stderr)
 	sys.exit(-1)
 
 def cli_error(error: str):
 	print(f"CLI error: {error}", file=sys.stderr)
 	sys.exit(-1)
 
 def int_arg(arg: str) -> int:
```

### Comparing `snagboot-1.0/src/snagrecover/am335x_usb_setup.sh` & `snagboot-1.1/src/snagrecover/am335x_usb_setup.sh`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/cli.py` & `snagboot-1.1/src/snagrecover/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import pkg_resources
 import yaml
 import os
 import logging
 import ast
 
 def cli():
-	udev_path = os.path.dirname(__file__) + "/80-snagboot.rules"
+	udev_path = os.path.dirname(__file__) + "/50-snagboot.rules"
 	am335x_script_path = os.path.dirname(__file__) + "/am335x_usb_setup.sh"
 	template_path = os.path.dirname(__file__) + "/templates"
 	templates = [filename[:-5] for filename in os.listdir(template_path)]
 	templates.sort()
 	template_listing = "\n".join(templates)
 	example = '''Examples:
 	snagrecover -s stm32mp15 -f stm32mp15.yaml
```

### Comparing `snagboot-1.0/src/snagrecover/config.py` & `snagboot-1.1/src/snagrecover/config.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/firmware/am335x_fw.py` & `snagboot-1.1/src/snagrecover/firmware/am335x_fw.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/firmware/firmware.py` & `snagboot-1.1/src/snagrecover/firmware/firmware.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/firmware/imx_fw.py` & `snagboot-1.1/src/snagrecover/firmware/imx_fw.py`

 * *Files 18% similar despite different names*

```diff
@@ -74,26 +74,29 @@
 def imx_run(port, fw_name: str, fw_blob: bytes, subfw_name: str = ""):
 	MAX_DOWNLOAD_SIZE = 0x200000
 	soc_model = recovery_config["soc_model"]
 
 	sdp_cmd = imx_sdp.SDPCommand(port)
 	memops = memory_ops.MemoryOps(sdp_cmd)
 
-	if fw_name == "u-boot-sdps":
+	if fw_name == "flash-bin" and subfw_name == "spl-sdps":
 		write_size = rom_container.get_container_size(fw_blob)
 		ret = sdp_cmd.sdps_write(fw_blob, write_size)
 		if not ret:
 			raise ValueError("Error: failed to write first stage firmware")
 		return None
 
+	# Try to extract ivtable from binary blob
 	ivtable = ivt.IVT()
-	if ivtable.from_blob(fw_blob) is None:
-		raise ValueError("Error: No IVT header in boot image")
+	if not ivtable.from_blob(fw_blob):
+		logger.warning("IVT header not found")
 
 	if fw_name == "u-boot-with-dcd":
+		if ivtable.header is None:
+			raise ValueError("Error: No IVT header in boot image (required for DCD)")
 		# WRITE DEVICE CONFIGURATION DATA
 		print("Writing Device Configuration Data...")
 		if ivtable.dcd == 0:
 			raise ValueError("Error: No DCD data in boot image")
 		logger.info("Writing DCD...")
 		dcd_offset = ivtable.offset + ivtable.dcd - ivtable.addr
 		if fw_blob[dcd_offset] != 0xd2:
@@ -109,31 +112,40 @@
 
 	logger.info(f"Downloading firmware {fw_name}...")
 	if fw_name == "flash-bin" and subfw_name == "u-boot":
 		"""
 		get uboot/atf offset and size by assuming that it is located immediately after the
 		section of the boot image that we previously downloaded to the board
 		"""
-		write_offset = ivtable.offset + ivtable.boot_data["length"] - (ivtable.addr - ivtable.boot_data["start"])
+		if ivtable.header is not None:
+			write_offset = ivtable.offset + ivtable.boot_data["length"] - (ivtable.addr - ivtable.boot_data["start"])
+		else:
+			logger.warning("IVT header not found, extracting size from raw blob")
+			write_offset = rom_container.get_container_size(fw_blob)
 		write_size = len(fw_blob) - write_offset
 		if	write_size <= 0:
 			raise ValueError("Error: Invalid offset found for U-BOOT proper in boot image")
 		# We ask for a write at 0 but SPL should determine u-boot proper's
 		# write address on its own
 		print("Downloading file...")
 		memops.write_blob(fw_blob, 0, write_offset, write_size)
 		print("Done\nJumping to firmware...")
 		memops.jump(0)
 		return None
 	else:
-		write_size = ivtable.boot_data["length"] - (ivtable.addr - ivtable.boot_data["start"])
-		# If the IVT offset is large enough, the write can overflow the source buffer
-		if write_size > len(fw_blob) - ivtable.offset:
-			logger.warning("Write size is too large, truncating...")
-			write_size = len(fw_blob) - ivtable.offset
+		if ivtable.header is not None:
+			write_size = ivtable.boot_data["length"] - (ivtable.addr - ivtable.boot_data["start"])
+			# If the IVT offset is large enough, the write can overflow the source buffer
+			if write_size > len(fw_blob) - ivtable.offset:
+				logger.warning("Write size is too large, truncating...")
+				write_size = len(fw_blob) - ivtable.offset
+		else:
+			logger.warning("IVT header not found, extracting size from raw blob")
+			write_offset = rom_container.get_container_size(fw_blob)
+			write_size = len(fw_blob) - write_offset
 		# protocols other than SPLV/U have a maximum download size
 		# split download into chunks < MAX_DOWNLOAD_SIZE
 		chunk_offset = 0
 		print("Downloading file...")
 		for chunk in utils.dnload_iter(fw_blob[ivtable.offset:ivtable.offset + write_size], 0x200000):
 			memops.write_blob(chunk, ivtable.addr + chunk_offset, chunk_offset, len(chunk))
 			chunk_offset += MAX_DOWNLOAD_SIZE
```

### Comparing `snagboot-1.0/src/snagrecover/firmware/ivt.py` & `snagboot-1.1/src/snagrecover/firmware/ivt.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/firmware/rom_container.py` & `snagboot-1.1/src/snagrecover/firmware/rom_container.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,42 +51,42 @@
 from snagrecover.config import recovery_config
 
 CONTAINER_HDR_ALIGNMENT = 0x400
 CONTAINER_TAG = 0x87
 V2X_BOOTIMG_FLAG = 0x0b
 
 ROM_CONTAINER_STRUCT_SIZE = 16
-ROM_BOOTIMG_STRUCT_SIZE = 34
+ROM_BOOTIMG_STRUCT_SIZE = 128
 
 def get_container_size(boot_blob: bytes) -> int:
 	"""
 	This function is used to compute the size of the first stage firmware
-	container for boards socs using the SDPS protocol. It has not yet been tested.
+	container for boards socs using the SDPS protocol.
 	"""
 	soc_model = recovery_config["soc_model"]
-	if soc_model == "imx815":
+	if soc_model in ["imx815","imx93"]:
 		return len(boot_blob)
 	rom_container_tag = boot_blob[CONTAINER_HDR_ALIGNMENT + 3]
-	if rom_container_tag != b"\x87":
+	if rom_container_tag != CONTAINER_TAG:
 		return len(boot_blob)
 
 	cont_index = 1
 	romimg_offset = CONTAINER_HDR_ALIGNMENT + ROM_BOOTIMG_STRUCT_SIZE
 	romimg_flags = int.from_bytes(boot_blob[romimg_offset + 24:romimg_offset + 28], "little")
 	if romimg_flags & 0x0F == V2X_BOOTIMG_FLAG:
 		# skip V2X container
 		cont_index = 2
 		rom_container_tag = boot_blob[2 * CONTAINER_HDR_ALIGNMENT + 3]
-		if rom_container_tag != b"\x87":
+		if rom_container_tag != CONTAINER_TAG:
 			return len(boot_blob)
 	container_offset = cont_index * CONTAINER_HDR_ALIGNMENT
 	num_images = int(boot_blob[container_offset + 11])
 	romimg_offset = container_offset + ROM_CONTAINER_STRUCT_SIZE + (num_images - 1) * ROM_BOOTIMG_STRUCT_SIZE
-	romimg_offset = int.from_bytes(boot_blob[romimg_offset: romimg_offset], "little")
-	romimg_size = int.from_bytes(boot_blob[romimg_offset + 4: romimg_offset + 8], "little")
-	container_size = romimg_offset + romimg_size + cont_index * CONTAINER_HDR_ALIGNMENT
+	img_offset = int.from_bytes(boot_blob[romimg_offset: romimg_offset + 4], "little")
+	img_size = int.from_bytes(boot_blob[romimg_offset + 4: romimg_offset + 8], "little")
+	container_size = img_offset + img_size + cont_index * CONTAINER_HDR_ALIGNMENT
 	# round container size up
 	container_size = ceil(container_size / (1.0 * CONTAINER_HDR_ALIGNMENT)) * CONTAINER_HDR_ALIGNMENT
 	if container_size >= len(boot_blob):
 		raise ValueError("Error: unsupported image format or image does not contain u-boot proper")
 	return container_size
```

### Comparing `snagboot-1.0/src/snagrecover/firmware/sama5_fw.py` & `snagboot-1.1/src/snagrecover/firmware/sama5_fw.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/firmware/samba_applet.py` & `snagboot-1.1/src/snagrecover/firmware/samba_applet.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/firmware/sunxi_fw/fel-to-spl-thunk.S` & `snagboot-1.1/src/snagrecover/firmware/sunxi_fw/fel-to-spl-thunk.S`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/firmware/sunxi_fw/mmu.py` & `snagboot-1.1/src/snagrecover/firmware/sunxi_fw/mmu.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/firmware/sunxi_fw/soc_info.yaml` & `snagboot-1.1/src/snagrecover/firmware/sunxi_fw/soc_info.yaml`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/firmware/sunxi_fw/sunxi_fw.py` & `snagboot-1.1/src/snagrecover/firmware/sunxi_fw/sunxi_fw.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/protocols/bootp.py` & `snagboot-1.1/src/snagrecover/protocols/bootp.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/protocols/dfu.py` & `snagboot-1.1/src/snagrecover/protocols/dfu.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/protocols/fastboot.py` & `snagboot-1.1/src/snagrecover/protocols/fastboot.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/protocols/fel.py` & `snagboot-1.1/src/snagrecover/protocols/fel.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/protocols/hab_constants.py` & `snagboot-1.1/src/snagrecover/protocols/hab_constants.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/protocols/imx_sdp.py` & `snagboot-1.1/src/snagrecover/protocols/imx_sdp.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 """
 
 import logging
 logger = logging.getLogger("snagrecover")
 from snagrecover import utils
 from snagrecover.protocols import hab_constants
 from snagrecover.config import recovery_config
+import hid
 
 
 class SDPCommand():
 
 	command_codes = {
 	"READ_REGISTER": b"\x01\x01",
 	"WRITE_REGISTER": b"\x02\x02",
@@ -175,22 +176,30 @@
 
 	def jump(self, addr: int):
 		self.clear()
 		self.cmd = SDPCommand.command_codes["JUMP_ADDRESS"]
 		self.addr = addr
 		packet = self.build_packet()
 		self.dev.write(packet)
-		self.check_hab()
-		status = self.dev.read(65, timeout = 100)[1:]
-		if status != b"":
-			decoded_err = hab_constants.status_codes[int(status[0])] \
-				+ " | " + hab_constants.reason_codes[int(status[1])]\
-				+ " | " + hab_constants.context_codes[int(status[2])]\
-				+ " | " + hab_constants.engine_tags[int(status[3])]
-			raise ValueError(f"Error: error status {decoded_err} returned after jump to 0x{addr:x}")
+		"""
+		Looks like the following checks will fail sometimes,
+		even if the jump was successful. We still perform them 
+		though, in case the SoC actually expects them
+		"""
+		try:
+			self.check_hab()
+			status = self.dev.read(65, timeout = 100)[1:]
+			if status != b"":
+				decoded_err = hab_constants.status_codes[int(status[0])] \
+					+ " | " + hab_constants.reason_codes[int(status[1])]\
+					+ " | " + hab_constants.context_codes[int(status[2])]\
+					+ " | " + hab_constants.engine_tags[int(status[3])]
+				logger.warning(f"error status {decoded_err} returned after jump to 0x{addr:x}")
+		except hid.HIDException as err:
+			logger.warning(f"Caught HIDException {str(err)}")
 		return None
 
 	def skip_dcd_header(self):
 		logger.info("Sending SKIP_DCD_HEADER command")
 		self.clear()
 		self.cmd = SDPCommand.command_codes["SKIP_DCD_HEADER"]
 		packet1 = self.build_packet()
@@ -199,38 +208,39 @@
 		ack = self.dev.read(65, timeout=5000)[1:5]
 		self.end_cmd()
 		return ack == b"\x09\xd0\x0d\x90"
 
 	def sdps_write(self, blob: bytes, size: int) -> bool:
 		"""
 		Command used to write the first stage firmware for boards using the SDPS
-		protocol. It has not yet been tested and may require some tweaks.
+		protocol. It has not yet been tested on all supported platforms and may
+		require some tweaks.
 		"""
 		logger.info(f"SDPS write with parameters size:0x{size:x} offset:0x00")
 		soc_model = recovery_config["soc_model"]
-		if soc_model not in ["imx8qxp","imx815"]:
+		if soc_model not in ["imx8qm", "imx8qxp","imx815","imx93"]:
 			# only some mpu models require a preliminary command before the report 2
 			# transfer
 			packet1_arr = bytearray(b"\x01") # report 1
 			packet1_arr += SDPCommand.CBW_BLTC_SIGNATURE.to_bytes(4, "little")
 			packet1_arr += b"\x01\x00\x00\x00" # tag
 			packet1_arr += size.to_bytes(4, "little") # XferLength
 			packet1_arr += SDPCommand.CBW_HOST_TO_DEVICE_FLAGS.to_bytes(1, "little")
 			packet1_arr += b"\x00\x00" # reserved
 			packet1_arr += SDPCommand.BLTC_DOWNLOAD_FW.to_bytes(1, "little") # Command
 			packet1_arr += size.to_bytes(4, "big") # Length
 			packet1_arr += b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00" # reserved
 			packet1 = bytes(packet1_arr)
 			self.dev.write(packet1)
-		if soc_model == "imx815":
+		if soc_model in ["imx815","imx93"]:
 			transfer_size = 1020
 		else:
 			transfer_size = 1024
 
-		for chunk in utils.dnload_iter(blob, transfer_size):
+		for chunk in utils.dnload_iter(blob[0:size], transfer_size):
 			packet2 = b"\x02" + chunk
 			self.dev.write(packet2)
 		"""
 		self.check_hab()
 		complete_status = self.dev.read(65, timeout=5000)[1:5]
 		self.end_cmd()
 		logger.info(f"write_blob finished with complete status {complete_status}")
```

### Comparing `snagboot-1.0/src/snagrecover/protocols/memory_ops.py` & `snagboot-1.1/src/snagrecover/protocols/memory_ops.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/protocols/sambamon.py` & `snagboot-1.1/src/snagrecover/protocols/sambamon.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/recoveries/am335x.py` & `snagboot-1.1/src/snagrecover/recoveries/am335x.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/recoveries/am62x.py` & `snagboot-1.1/src/snagrecover/recoveries/am62x.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/recoveries/imx.py` & `snagboot-1.1/src/snagrecover/recoveries/imx.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,16 +85,18 @@
 	pid = recovery_config["rom_usb"][1]
 
 	try:
 		dev = hid.Device(vid, pid)
 	except hid.HIDException:
 		access_error("USB HID", f"{vid:04x}:{pid:04x}")
 	if soc_model in sdps_socs:
-		run_firmware(dev, "u-boot-sdps")
-		return None
+		run_firmware(dev, "flash-bin", "spl-sdps")
+		# On some SoCs (e.g.: i.MX8QM) we can have a second stage based on SPDV
+		if soc_model != "imx8qm":
+			return None
 	elif "u-boot-with-dcd" in recovery_config["firmware"]:
 		run_firmware(dev, "u-boot-with-dcd")
 		return None
 	elif "SPL" in recovery_config["firmware"]:
 		run_firmware(dev, "SPL")
 	else:
 		run_firmware(dev, "flash-bin", "spl")
```

### Comparing `snagboot-1.0/src/snagrecover/recoveries/sama5.py` & `snagboot-1.1/src/snagrecover/recoveries/sama5.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/recoveries/stm32_flashlayout.py` & `snagboot-1.1/src/snagrecover/recoveries/stm32_flashlayout.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/recoveries/stm32mp1.py` & `snagboot-1.1/src/snagrecover/recoveries/stm32mp1.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/recoveries/sunxi.py` & `snagboot-1.1/src/snagrecover/recoveries/sunxi.py`

 * *Files identical despite different names*

### Comparing `snagboot-1.0/src/snagrecover/supported_socs.yaml` & `snagboot-1.1/src/snagrecover/supported_socs.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,18 @@
         family: imx
   imx6ull:
         family: imx
   imx7d:
         family: imx
   imx8mm:
         family: imx
+  imx8qm:
+        family: imx
+  imx93:
+        family: imx
   r8:
         family: sunxi
   sama5d2:
         family: sama5
   sama5d3:
         family: sama5
   sama5d4:
@@ -88,20 +92,16 @@
         family: imx
   imx865:
         family: imx
   imx8dxl:
         family: imx
   imx8mq:
         family: imx
-  imx8qm:
-        family: imx
   imx8qxp:
         family: imx
-  imx93:
-        family: imx
   imxrt106x:
         family: imx
   r16:
         family: sunxi
   r329:
         family: sunxi
   r40:
```

### Comparing `snagboot-1.0/src/snagrecover/utils.py` & `snagboot-1.1/src/snagrecover/utils.py`

 * *Files identical despite different names*

