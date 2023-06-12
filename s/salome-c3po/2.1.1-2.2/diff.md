# Comparing `tmp/salome-c3po-2.1.1.tar.gz` & `tmp/salome-c3po-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salome-c3po-2.1.1.tar", last modified: Tue Nov 29 13:08:13 2022, max compression
+gzip compressed data, was "/volatile/catA/cpatricot/C3PO_public/dist/tmpc57r8xzi/salome-c3po-2.2.tar", last modified: Mon Jun 12 15:47:05 2023, max compression
```

## Comparing `salome-c3po-2.1.1.tar` & `salome-c3po-2.2.tar`

### file list

```diff
@@ -1,68 +1,83 @@
-drwxr-xr-x   0 rl222169  (1000) rl222169  (1000)        0 2022-11-29 13:08:13.210459 salome-c3po-2.1.1/
--rw-r--r--   0 rl222169  (1000) rl222169  (1000)      356 2022-11-29 13:08:13.209459 salome-c3po-2.1.1/PKG-INFO
-drwxr-xr-x   0 rl222169  (1000) rl222169  (1000)        0 2022-11-29 13:08:13.121341 salome-c3po-2.1.1/c3po/
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     8173 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/CollaborativeDataManager.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     2260 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/CollaborativeExchanger.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     2756 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/CollaborativeObject.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     2721 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/CollaborativePhysicsDriver.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     9334 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/Coupler.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    14156 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/DataAccessor.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     5625 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/DataManager.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     1994 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/Exchanger.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    16178 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/LocalDataManager.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    12196 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/LocalExchanger.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    25711 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/PhysicsDriver.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    14540 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/TimeAccumulator.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)        6 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/VERSION
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     2910 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/__init__.py
-drwxr-xr-x   0 rl222169  (1000) rl222169  (1000)        0 2022-11-29 13:08:13.130334 salome-c3po-2.1.1/c3po/couplers/
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    14345 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/couplers/AndersonCoupler.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     7128 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/couplers/FixedPointCoupler.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    12721 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/couplers/JFNKCoupler.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     1508 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/couplers/__init__.py
-drwxr-xr-x   0 rl222169  (1000) rl222169  (1000)        0 2022-11-29 13:08:13.141459 salome-c3po-2.1.1/c3po/exchangeMethods/
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     2336 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/exchangeMethods/DirectMatching.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     3228 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/exchangeMethods/ExchangeMethod.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    11055 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/exchangeMethods/SharedRemapping.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    10955 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/exchangeMethods/SharedRemappingMulti1D3D.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     1508 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/exchangeMethods/__init__.py
-drwxr-xr-x   0 rl222169  (1000) rl222169  (1000)        0 2022-11-29 13:08:13.143463 salome-c3po-2.1.1/c3po/medcouplingCompat/
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     2595 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/medcouplingCompat/__init__.py
-drwxr-xr-x   0 rl222169  (1000) rl222169  (1000)        0 2022-11-29 13:08:13.176459 salome-c3po-2.1.1/c3po/mpi/
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     5951 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPICollaborativeDataManager.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     2343 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPICollaborativePhysicsDriver.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     2937 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPICollectiveDataManager.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     2278 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPICollectiveProcess.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     7177 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPICoupler.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     9907 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPIExchanger.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     8430 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPIMasterDataManager.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     3693 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPIMasterExchanger.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    11798 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPIMasterPhysicsDriver.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     4405 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPIRecipient.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     4329 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPIRemoteProcess.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     5358 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPISender.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     2496 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPITag.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    10849 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/MPIWorker.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     2127 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/mpi/__init__.py
-drwxr-xr-x   0 rl222169  (1000) rl222169  (1000)        0 2022-11-29 13:08:13.189459 salome-c3po-2.1.1/c3po/physicsDrivers/
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     5658 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/physicsDrivers/ALCYONE2Driver.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     5575 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/physicsDrivers/APOLLO3Driver.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     8381 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/physicsDrivers/CATHARE3Driver.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    13645 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/physicsDrivers/CRONOS2Driver.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     8870 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/physicsDrivers/FLICA4Driver.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     5477 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/physicsDrivers/THEDIDriver.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     3549 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/physicsDrivers/TRUSTDriver.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     1508 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/physicsDrivers/__init__.py
-drwxr-xr-x   0 rl222169  (1000) rl222169  (1000)        0 2022-11-29 13:08:13.197458 salome-c3po-2.1.1/c3po/services/
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    33971 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/services/ListingWriter.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    21394 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/services/NameChanger.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     1508 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/services/__init__.py
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)    16490 2022-11-29 13:02:27.000000 salome-c3po-2.1.1/c3po/services/tracer.py
-drwxr-xr-x   0 rl222169  (1000) rl222169  (1000)        0 2022-11-29 13:08:13.206459 salome-c3po-2.1.1/salome_c3po.egg-info/
--rw-r--r--   0 rl222169  (1000) rl222169  (1000)      356 2022-11-29 13:08:13.000000 salome-c3po-2.1.1/salome_c3po.egg-info/PKG-INFO
--rw-r--r--   0 rl222169  (1000) rl222169  (1000)     1701 2022-11-29 13:08:13.000000 salome-c3po-2.1.1/salome_c3po.egg-info/SOURCES.txt
--rw-r--r--   0 rl222169  (1000) rl222169  (1000)        1 2022-11-29 13:08:13.000000 salome-c3po-2.1.1/salome_c3po.egg-info/dependency_links.txt
--rw-r--r--   0 rl222169  (1000) rl222169  (1000)       55 2022-11-29 13:08:13.000000 salome-c3po-2.1.1/salome_c3po.egg-info/requires.txt
--rw-r--r--   0 rl222169  (1000) rl222169  (1000)        5 2022-11-29 13:08:13.000000 salome-c3po-2.1.1/salome_c3po.egg-info/top_level.txt
--rw-r--r--   0 rl222169  (1000) rl222169  (1000)       38 2022-11-29 13:08:13.211459 salome-c3po-2.1.1/setup.cfg
--rwxr-xr-x   0 rl222169  (1000) rl222169  (1000)     4032 2022-11-29 13:07:40.000000 salome-c3po-2.1.1/setup.py
+drwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)        0 2023-06-12 15:47:05.000000 salome-c3po-2.2/
+drwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)        0 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/
+drwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)        0 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/salome_c3po.egg-info/
+-rw-------   0 cpatricot (232322) dm2s-user-cat-a (470572)     2743 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/salome_c3po.egg-info/SOURCES.txt
+-rw-------   0 cpatricot (232322) dm2s-user-cat-a (470572)        5 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/salome_c3po.egg-info/top_level.txt
+-rw-------   0 cpatricot (232322) dm2s-user-cat-a (470572)      382 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/salome_c3po.egg-info/PKG-INFO
+-rw-------   0 cpatricot (232322) dm2s-user-cat-a (470572)       40 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/salome_c3po.egg-info/requires.txt
+-rw-------   0 cpatricot (232322) dm2s-user-cat-a (470572)        1 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/salome_c3po.egg-info/dependency_links.txt
+drwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)        0 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/c3po/
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    16178 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/LocalDataManager.py
+drwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)        0 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/c3po/exchangeMethods/
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     3228 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/exchangeMethods/ExchangeMethod.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     1508 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/exchangeMethods/__init__.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     2336 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/exchangeMethods/DirectMatching.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    12825 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/exchangeMethods/SharedRemapping.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    15300 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/exchangeMethods/SharedRemappingMulti1D3D.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     1994 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/Exchanger.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     2756 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/CollaborativeObject.py
+drwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)        0 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/c3po/physicsDrivers/
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    13645 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/physicsDrivers/CRONOS2Driver.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     6046 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/physicsDrivers/ALCYONE2Driver.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     3549 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/physicsDrivers/TRUSTDriver.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     5575 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/physicsDrivers/APOLLO3Driver.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     1508 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/physicsDrivers/__init__.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     8870 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/physicsDrivers/FLICA4Driver.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     8504 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/physicsDrivers/CATHARE3Driver.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     5477 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/physicsDrivers/THEDIDriver.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     9334 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/Coupler.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    27108 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/PhysicsDriver.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    12500 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/LocalExchanger.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     8600 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/CollaborativeDataManager.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    14377 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/DataAccessor.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     3221 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/__init__.py
+drwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)        0 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/c3po/medcouplingCompat/
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     2595 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/medcouplingCompat/__init__.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     5625 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/DataManager.py
+drwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)        0 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/c3po/couplers/
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     8916 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/couplers/FixedPointCoupler.py
+-rw-------   0 cpatricot (232322) dm2s-user-cat-a (470572)    17658 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/couplers/AdaptiveResidualBalanceCoupler.py
+-rw-------   0 cpatricot (232322) dm2s-user-cat-a (470572)     7735 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/couplers/CrossedSecantCoupler.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    15052 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/couplers/AndersonCoupler.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    17604 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/couplers/DynamicResidualBalanceCoupler.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     1508 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/couplers/__init__.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    13370 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/couplers/JFNKCoupler.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     2260 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/CollaborativeExchanger.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)        4 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/VERSION
+drwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)        0 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/c3po/services/
+-rw-------   0 cpatricot (232322) dm2s-user-cat-a (470572)     3649 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/services/Printer.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     1508 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/services/__init__.py
+-rw-------   0 cpatricot (232322) dm2s-user-cat-a (470572)     9956 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/services/TransientLogger.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    22883 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/services/NameChanger.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    33971 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/services/ListingWriter.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    16634 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/services/tracer.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    15219 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/TimeAccumulator.py
+drwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)        0 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/c3po/mpi/
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    15287 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPIMasterPhysicsDriver.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     2343 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/mpi/MPICollaborativePhysicsDriver.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     3985 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPIMasterExchanger.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    16443 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPIExchanger.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     5247 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPIDomainDecompositionDataManager.py
+drwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)        0 2023-06-12 15:47:05.000000 salome-c3po-2.2/sources/c3po/mpi/mpiExchangeMethods/
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    14986 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/mpiExchangeMethods/MPISharedRemapping.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     2284 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/mpiExchangeMethods/MPIExchangeMethod.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     1508 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/mpiExchangeMethods/__init__.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    11041 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/mpiExchangeMethods/MPISharedRemappingMulti1D3D.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     2937 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/mpi/MPICollectiveDataManager.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     2278 2023-04-11 07:46:43.000000 salome-c3po-2.2/sources/c3po/mpi/MPICollectiveProcess.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     4552 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPIRecipient.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     8553 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPIMasterDataManager.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     6696 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPICollaborativeDataManager.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     2189 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPIRemoteProcess.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     2553 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/__init__.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     2707 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPITag.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     4446 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPIRemote.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     6118 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPISender.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)    12062 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPIWorker.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     7301 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPICoupler.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     2251 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/mpi/MPIRemoteProcesses.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     3687 2023-06-12 08:27:18.000000 salome-c3po-2.2/sources/c3po/CollaborativePhysicsDriver.py
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     1343 2023-06-12 08:27:17.000000 salome-c3po-2.2/README.md
+-rw-------   0 cpatricot (232322) dm2s-user-cat-a (470572)       38 2023-06-12 15:47:05.000000 salome-c3po-2.2/setup.cfg
+-rw-------   0 cpatricot (232322) dm2s-user-cat-a (470572)      382 2023-06-12 15:47:05.000000 salome-c3po-2.2/PKG-INFO
+-rwx------   0 cpatricot (232322) dm2s-user-cat-a (470572)     3949 2023-06-12 15:45:41.000000 salome-c3po-2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `salome-c3po-2.1.1/c3po/CollaborativeDataManager.py` & `salome-c3po-2.2/sources/c3po/CollaborativeDataManager.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,30 +21,36 @@
 
     def __init__(self, dataManagers):
         """! Build a CollaborativeDataManager object.
 
         @param dataManagers a list of DataManager.
         """
         self.dataManagers = dataManagers
+        self._indexToIgnore = []
         CollaborativeObject.__init__(self, self.dataManagers)
 
+    def ignoreForConstOperators(self, indexToIgnore):
+        """! INTERNAL """
+        self._indexToIgnore[:] = indexToIgnore[:]
+
     def clone(self):
         """! Return a clone of self.
 
         @return A clone of self. Data are copied.
         """
         return self * 1.
 
     def cloneEmpty(self):
         """! Return a clone of self without copying the data.
 
         @return An empty clone of self.
         """
         dataClone = [data.cloneEmpty() for data in self.dataManagers]
         output = CollaborativeDataManager(dataClone)
+        output.ignoreForConstOperators(self._indexToIgnore)
         return output
 
     def copy(self, other):
         """! Copy data of other in self.
 
         @param other a CollaborativeDataManager with the same list of data than self.
 
@@ -56,29 +62,31 @@
 
     def normMax(self):
         """! Return the infinite norm.
 
         @return The max of the absolute values of the scalars and of the infinite norms of the MED fields.
         """
         norm = 0.
-        for data in self.dataManagers:
-            localNorm = data.normMax()
-            if localNorm > norm:
-                norm = localNorm
+        for idata, data in enumerate(self.dataManagers):
+            if idata not in self._indexToIgnore:
+                localNorm = data.normMax()
+                if localNorm > norm:
+                    norm = localNorm
         return norm
 
     def norm2(self):
         """! Return the norm 2.
 
         @return sqrt(sum_i(val[i] * val[i])) where val[i] stands for each scalar and each component of the MED fields.
         """
         norm = 0.
-        for data in self.dataManagers:
-            localNorm = data.norm2()
-            norm += localNorm * localNorm
+        for idata, data in enumerate(self.dataManagers):
+            if idata not in self._indexToIgnore:
+                localNorm = data.norm2()
+                norm += localNorm * localNorm
         return math.sqrt(norm)
 
     def checkBeforeOperator(self, other):
         """! INTERNAL Make basic checks before the call of an operator. """
         if len(self.dataManagers) != len(other.dataManagers):
             raise Exception("CollaborativeDataManager.checkBeforeOperator : we cannot call an operator between two CollaborativeDataManager with different number of DataManager.")
 
@@ -205,9 +213,10 @@
         @return the scalar product of self with other.
 
         @throw Exception if self and other are not consistent.
         """
         self.checkBeforeOperator(other)
         result = 0.
         for i in range(len(self.dataManagers)):
-            result += self.dataManagers[i].dot(other.dataManagers[i])
+            if i not in self._indexToIgnore:
+                result += self.dataManagers[i].dot(other.dataManagers[i])
         return result
```

### Comparing `salome-c3po-2.1.1/c3po/CollaborativeExchanger.py` & `salome-c3po-2.2/sources/c3po/CollaborativeExchanger.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/CollaborativeObject.py` & `salome-c3po-2.2/sources/c3po/CollaborativeObject.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/CollaborativePhysicsDriver.py` & `salome-c3po-2.2/sources/c3po/mpi/MPICollaborativePhysicsDriver.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,39 +4,25 @@
 # All rights reserved.
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # 3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-""" Contain the class CollaborativePhysicsDriver. """
+""" Contain the class MPICollaborativePhysicsDriver. """
 from __future__ import print_function, division
 
-from c3po.Coupler import Coupler
-from c3po.CollaborativeObject import CollaborativeObject
+from c3po.mpi.MPICoupler import MPICoupler
+from c3po.CollaborativePhysicsDriver import CollaborativePhysicsDriver
 
 
-class CollaborativePhysicsDriver(Coupler, CollaborativeObject):
-    """! CollaborativePhysicsDriver is a PhysicsDriver (a Coupler in fact) that handles a set of PhysicsDriver as a single one.
+class MPICollaborativePhysicsDriver(CollaborativePhysicsDriver, MPICoupler):
+    """! MPICollaborativePhysicsDriver is the MPI version of CollaborativePhysicsDriver. """
 
-    The solving methods of the CollaborativePhysicsDriver call the ones of the held PhysicsDriver in a row.
-    """
-
-    def __init__(self, physics):
+    def __init__(self, physics, mpiComm=None):
         """! Build an CollaborativePhysicsDriver object.
 
         @param physics a list (or dictionary) of PhysicsDriver objects.
+        @param mpiComm MPI communicator to provide to MPICoupler. See MPICoupler.__init__().
         """
-        Coupler.__init__(self, physics=physics, exchangers=[])
-        CollaborativeObject.__init__(self, self._physicsDriversList)
-
-    def solveTimeStep(self):
-        """! See PhysicsDriver.solveTimeStep(). """
-        for physics in self._physicsDriversList:
-            physics.solve()
-        return self.getSolveStatus()
-
-    def iterateTimeStep(self):
-        """! See PhysicsDriver.iterateTimeStep(). """
-        for physics in self._physicsDriversList:
-            physics.iterate()
-        return self.getIterateStatus()
+        MPICoupler.__init__(self, physics=physics, exchangers=[], mpiComm=mpiComm)
+        CollaborativePhysicsDriver.__init__(self, self._physicsDriversList)
```

### Comparing `salome-c3po-2.1.1/c3po/Coupler.py` & `salome-c3po-2.2/sources/c3po/Coupler.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/DataAccessor.py` & `salome-c3po-2.2/sources/c3po/DataAccessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 
     class ValueType:
         """! The various possible types for fields or scalar values. """
         Double = "Double"
         Int = "Int"
         String = "String"
 
+    def getMPIComm(self):
+        """! (Optional) Return the MPI communicator used by the code for parallel computations.
+
+        @return (mpi4py.Comm) mpi4py communicator.
+        """
+        raise NotImplementedError
+
     def getInputFieldsNames(self):
         """! (Optional) Get the list of input fields accepted by the code.
 
         @return (list) the list of field names that represent inputs of the code.
         @throws AssertionError if implemented in a PhysicsDriver and called before initialize() or after terminate().
         """
         raise NotImplementedError
```

### Comparing `salome-c3po-2.1.1/c3po/DataManager.py` & `salome-c3po-2.2/sources/c3po/DataManager.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/Exchanger.py` & `salome-c3po-2.2/sources/c3po/Exchanger.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/LocalDataManager.py` & `salome-c3po-2.2/sources/c3po/LocalDataManager.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/LocalExchanger.py` & `salome-c3po-2.2/sources/c3po/LocalExchanger.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,20 @@
     def exchange(self):
         """! Trigger the exchange of data. """
         fieldsToSet = [ds.getFieldTemplate() for ds in self._fieldsToSet]
         fieldsToGet = [ds.get() for ds in self._fieldsToGet]
         valuesToGet = [ds.get() for ds in self._valuesToGet]
         fieldsToSet, valuesToSet = self._method(fieldsToGet, fieldsToSet, valuesToGet)
         if (len(fieldsToSet) != len(self._fieldsToSet) or len(valuesToSet) != len(self._valuesToSet)):
-            raise Exception("LocalExchanger.exchange the method does not have the good number of outputs.")
+            expectedNb = len(self._fieldsToSet)
+            foundNb = len(fieldsToSet)
+            if len(fieldsToSet) == len(self._fieldsToSet):
+                expectedNb = len(self._valuesToSet)
+                foundNb = len(valuesToSet)
+            raise Exception("LocalExchanger.exchange the method does not have the good number of outputs (we got {} outputs instead of {}).". format(foundNb, expectedNb))
         for i, field in enumerate(fieldsToSet):
             self._fieldsToSet[i].set(field)
         for i, value in enumerate(valuesToSet):
             self._valuesToSet[i].set(value)
 
     @staticmethod
     def _expandInputList(inputList):
```

### Comparing `salome-c3po-2.1.1/c3po/PhysicsDriver.py` & `salome-c3po-2.2/sources/c3po/PhysicsDriver.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # 3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """ Contain the class PhysicsDriver. """
 from __future__ import print_function, division
 
 from c3po.DataAccessor import DataAccessor
+from c3po.services.TransientLogger import Timekeeper, TransientPrinter
 
 
 class PhysicsDriver(DataAccessor):
     """! PhysicsDriver is an abstract class which standardizes the functionalities expected by computer codes.
 
     It follows the ICoCo (Interface for Code Coupling) V2 standard.
     The ICoCo V2 I/O (in/out) methods are defined in the mother class DataAccessor.
@@ -47,14 +48,16 @@
         Internal set up and initialization of the code should not be done here, but rather in initialize().
         """
         self._initStatus = True
         self._solveStatus = True
         self._iterateStatus = (True, True)
         self._initNb = 0
 
+        self._transientPrinter = TransientPrinter(Timekeeper())
+
     @staticmethod
     def GetICoCoMajorVersion():  # pylint: disable=invalid-name
         """! (Mandatory) Return ICoCo interface major version number.
 
         @return (int) ICoCo interface major version number (2 at present)
         """
         return 2
@@ -434,38 +437,66 @@
         @param method (string) a string specifying which method was used to save the state of the code. A code can provide
         different methods (for example in memory, on disk, etc.).
         @throws AssertionError if called before initialize() or after terminate().
         @throws ValueError if the method or label argument is invalid.
         """
         raise NotImplementedError
 
+    def setTransientLogger(self, transientLogger):
+        """! Defines the logger for solveTransient() method.
+
+        @param transientLogger (c3po.services.TransientLogger.TransientLogger) logger instance.
+        """
+        self._transientPrinter.setLogger(transientLogger)
+
+    def setTransientPrintLevel(self, level):
+        """! Set the print level for solveTransient() method (0=None, 1 keeps only the first and last lines, 2 keeps everything).
+
+        @param level (int) integer in range [0;2]. Default = 0.
+        """
+        self._transientPrinter.getPrinter().setPrintLevel(level)
+
     def solveTransient(self, tmax, finishAtTmax=False, stopIfStationary=False):
         """! Make the PhysicsDriver to advance in time until it reaches the time tmax or it asks to stop.
 
         The PhysicsDriver can ask to stop either with computeTimeStep() (always checked) or with isStationary() (only if stopIfStationary is set to True).
 
         @param tmax (float) maximum time to be reached (compared with presentTime()).
         @param finishAtTmax (bool) if set to True, the method ends with time = tmax (instead of time >= tmax).
+        In case the PhysicsDriver asks to stop before tmax is reached, resetTime(tmax) is called.
         @param stopIfStationary (bool) if set to True, the method stops also if isStationary() returns True.
         """
+
+        presentTime = self.presentTime()
+        self._transientPrinter.initTransient(self, tmax, finishAtTmax, stopIfStationary, presentTime)
+
         (dt, stop) = self.computeTimeStep()
-        while (self.presentTime() < tmax - 1.E-8 * min(tmax, dt) and not stop):
+        while (presentTime < tmax - 1.E-8 * min(tmax, dt) and not stop):
             if finishAtTmax:
-                if self.presentTime() + 1.5 * dt >= tmax:
-                    if self.presentTime() + dt >= tmax - dt * 1.E-4:
-                        dt = tmax - self.presentTime()
+                if presentTime + 1.5 * dt >= tmax:
+                    if presentTime + dt >= tmax - dt * 1.E-4:
+                        dt = tmax - presentTime
                     else:
-                        dt = 0.5 * (tmax - self.presentTime())
+                        dt = 0.5 * (tmax - presentTime)
             self.initTimeStep(dt)
             self.solve()
             ok = self.getSolveStatus()
             if ok:
                 self.validateTimeStep()
+                presentTime = self.presentTime()
+                self._transientPrinter.logValidate(dt, presentTime)
                 (dt, stop) = self.computeTimeStep()
                 if stopIfStationary:
                     stop = stop or self.isStationary()
             else:
                 self.abortTimeStep()
+                presentTime = self.presentTime()
+                self._transientPrinter.logAbort(dt, presentTime)
                 (dt2, stop) = self.computeTimeStep()
                 if dt == dt2:
                     raise Exception("PhysicsDriver.solveTransient : we are about to repeat a failed time-step calculation !")
                 dt = dt2
+        if stop and finishAtTmax:
+            self.resetTime(tmax)
+            presentTime = self.presentTime()
+
+        self._transientPrinter.terminateTransient(presentTime, stop, stopIfStationary and self.isStationary())
```

### Comparing `salome-c3po-2.1.1/c3po/TimeAccumulator.py` & `salome-c3po-2.2/sources/c3po/TimeAccumulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # 3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """ Contain the class TimeAccumulator. """
 from __future__ import print_function, division
 
 from c3po.PhysicsDriver import PhysicsDriver
+from c3po.services.Printer import warning
 
 
 class SaveAtInitTimeStep(object):
     """! Enum defining TimeAccumulator saving mode.
 
     Values:
         - never:
@@ -77,14 +78,28 @@
     def setStabilizedTransient(self, stabilizedTransient):
         """! Set stabilized transient data.
 
         @param stabilizedTransient see parameter stabilizedTransient of the <tt>__init__()</tt> method.
         """
         self._stabilizedTransient = stabilizedTransient
 
+    def setComputedTimeStep(self, dt):
+        """! Set time-step size returned by computeTimeStep().
+
+        @param dt (float) time-step size returned by computeTimeStep(). None can be set to use the time step recommended by the hold PhysicsDriver. Default: None.
+        """
+        self._macrodt = dt
+
+    def getPhysicsDriver(self):
+        """! Return the wrapped PhysicsDriver.
+
+        @return the wrapped PhysicsDriver.
+        """
+        return self._physics
+
     def getMEDCouplingMajorVersion(self):
         """! See PhysicsDriver.getMEDCouplingMajorVersion(). """
         return self._physics.getMEDCouplingMajorVersion()
 
     def isMEDCoupling64Bits(self):
         """! See PhysicsDriver.isMEDCoupling64Bits(). """
         return self._physics.isMEDCoupling64Bits()
@@ -95,17 +110,17 @@
 
     def setMPIComm(self, mpicomm):
         """! See PhysicsDriver.setMPIComm(). """
         self._physics.setMPIComm(mpicomm)
 
     def initialize(self):
         """! See PhysicsDriver.initialize(). """
-        self._physics.init()
         self._timeDifference = 0.
-        self._macrodt = None
+        self._afterAbort = False
+        self._physics.init()
         return self._physics.getInitStatus()
 
     def terminate(self):
         """! See PhysicsDriver.terminate(). """
         if self._saveParameters is not None:
             try:
                 self._physics.forget(*self._saveParameters)
@@ -269,14 +284,16 @@
 
     def setInputDoubleValue(self, name, value):
         """! See c3po.DataAccessor.DataAccessor.setInputDoubleValue().
 
         The value associated with the name "macrodt" can be used to set the time-step size returned by computeTimeStep().
         """
         if name == "macrodt":
+            warning('setInputDoubleValue("macrodt", value) is deprecated and will soon by deleted. '
+                    + "Please use setComputedTimeStep(dt).")
             self._macrodt = value
         else:
             self._physics.setInputDoubleValue(name, value)
 
     def getOutputDoubleValue(self, name):
         """! See c3po.DataAccessor.DataAccessor.getOutputDoubleValue(). """
         return self._physics.getOutputDoubleValue(name)
```

### Comparing `salome-c3po-2.1.1/c3po/__init__.py` & `salome-c3po-2.2/sources/c3po/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 from .CollaborativeDataManager import CollaborativeDataManager
 from .Coupler import Coupler, NormChoice
 from .CollaborativePhysicsDriver import CollaborativePhysicsDriver
 from .TimeAccumulator import TimeAccumulator, SaveAtInitTimeStep
 from .services.tracer import tracer
 from .services.NameChanger import nameChanger, NameChanger
 from .services.ListingWriter import ListingWriter, mergeListing, getTotalTimePhysicsDriver, getTimesExchanger
+from .services.TransientLogger import TransientLogger, Timekeeper, FortuneTeller
 from .couplers.FixedPointCoupler import FixedPointCoupler
 from .couplers.AndersonCoupler import AndersonCoupler
 from .couplers.JFNKCoupler import JFNKCoupler
+from .couplers.CrossedSecantCoupler import CrossedSecantCoupler
+from .couplers.AdaptiveResidualBalanceCoupler import AdaptiveResidualBalanceCoupler
+from .couplers.DynamicResidualBalanceCoupler import DynamicResidualBalanceCoupler
 from .exchangeMethods.ExchangeMethod import ExchangeMethod
 from .exchangeMethods.DirectMatching import DirectMatching
 from .exchangeMethods.SharedRemapping import SharedRemapping, Remapper
 from .exchangeMethods.SharedRemappingMulti1D3D import SharedRemappingMulti1D3D, Multi1D3DRemapper
```

### Comparing `salome-c3po-2.1.1/c3po/couplers/AndersonCoupler.py` & `salome-c3po-2.2/sources/c3po/couplers/AndersonCoupler.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """ Contain the class AndersonCoupler. """
 from __future__ import print_function, division
 import math
 import numpy as np
 
 from c3po.Coupler import Coupler
 from c3po.CollaborativeDataManager import CollaborativeDataManager
+from c3po.services.Printer import Printer
 
 
 def deleteQRColumn(matrixQ, matrixR, dataTemp):
     """! INTERNAL
 
     Return a new QR decomposition after deletion of one column.
     """
@@ -81,16 +82,16 @@
         @param dataManagers list of DataManager.
         """
         Coupler.__init__(self, physics, exchangers, dataManagers)
         self._tolerance = 1.E-6
         self._maxiter = 100
         self._order = 2
         self._andersonDampingFactor = 1.
-        self._isConverged = False
-        self._printLevel = 2
+        self._iterationPrinter = Printer(2)
+        self._leaveIfFailed = False
 
         if not isinstance(physics, list) or not isinstance(exchangers, list) or not isinstance(dataManagers, list):
             raise Exception("AndersonCoupler.__init__ physics, exchangers and dataManagers must be lists!")
         if len(physics) != 1:
             raise Exception("AndersonCoupler.__init__ There must be only one PhysicsDriver")
         if len(exchangers) != 2:
             raise Exception("AndersonCoupler.__init__ There must be exactly two Exchanger")
@@ -125,15 +126,22 @@
     def setPrintLevel(self, level):
         """! Set the print level during iterations (0=None, 1 keeps last iteration, 2 prints every iteration).
 
         @param level integer in range [0;2]. Default: 2.
         """
         if not level in [0, 1, 2]:
             raise Exception("AndersonCoupler.setPrintLevel level should be one of [0, 1, 2]!")
-        self._printLevel = level
+        self._iterationPrinter.setPrintLevel(level)
+
+    def setFailureManagement(self, leaveIfSolvingFailed):
+        """! Set if iterations should continue or not in case of solver failure (solveTimeStep returns False).
+
+        @param leaveIfSolvingFailed set False to continue the iterations, True to stop. Default: False.
+        """
+        self._leaveIfFailed = leaveIfSolvingFailed
 
     def solveTimeStep(self):
         """! Solve a time step using the fixed point algorithm with Anderson acceleration.
 
         Inspire de Homer Walker (walker@wpi.edu), 10/14/2011.
 
         See also c3po.PhysicsDriver.PhysicsDriver.solveTimeStep().
@@ -150,18 +158,21 @@
         matrixR = np.zeros(shape=(1, 1))
         matrixQ = [0.] * self._order
         datatmp = 0.  # pour manipulation dans deleteQRColumn
         # Tolérance sur le conditionnement de matrixR ; valeur par défaut proposée par Ansar, reprise telle quelle
         dropErr = 1.e10
 
         # Init On calcul ici l'etat "0"
-        if self._printLevel:
-            printEndOfLine = "\r" if self._printLevel == 1 else "\n"
-            print("Anderson iteration {} ".format(iiter), end=printEndOfLine)
+        if self._iterationPrinter.getPrintLevel() > 0:
+            self._iterationPrinter.print("Anderson iteration {} ".format(iiter))
+
         physics.solve()
+        if self._leaveIfFailed and not physics.getSolveStatus():
+            return False
+
         physics2Data.exchange()
 
         data = CollaborativeDataManager(self._dataManagers)
         normData = self.readNormData()
         self.normalizeData(normData)
 
         previousData = data.clone()
@@ -169,34 +180,38 @@
 
         # Premiere iteration non acceleree
         self.abortTimeStep()
         self.initTimeStep(self._dt)
         self.denormalizeData(normData)
         data2physics.exchange()
         physics.solve()
+        if self._leaveIfFailed and not physics.getSolveStatus():
+            return False
         physics2Data.exchange()
         self.normalizeData(normData)
         diffData = data - previousData
         previousData.copy(data)
 
         deltaF = diffData * -1.
         delta = previousData * -1.
 
         error = self.getNorm(diffData) / self.getNorm(data)
 
         iiter += 1
-        if self._printLevel:
-            print("Anderson iteration {} error : {:.5e} ".format(iiter - 1, error), end=printEndOfLine)
+        if self._iterationPrinter.getPrintLevel() > 0:
+            self._iterationPrinter.print("Anderson iteration {} error : {:.5e} ".format(iiter - 1, error))
 
         while error > self._tolerance and iiter < self._maxiter:
             self.abortTimeStep()
             self.initTimeStep(self._dt)
             self.denormalizeData(normData)
             data2physics.exchange()
             physics.solve()
+            if self._leaveIfFailed and not physics.getSolveStatus():
+                return False
             physics2Data.exchange()     # data contient g(u_k), previousData contient u_k
             self.normalizeData(normData)
 
             diffData.copy(data)
             diffData -= previousData
             error = self.getNorm(diffData) / self.getNorm(data)
 
@@ -282,15 +297,15 @@
                     data.imuladd(-(1. - self._andersonDampingFactor), diffData)
                     for i in range(mAA):
                         data.imuladd((1. - self._andersonDampingFactor) * matrixRgamma[i], matrixQ[i])
 
                 previousData.copy(data)
 
             iiter += 1
-            if self._printLevel:
-                print("Anderson iteration {} error : {:.5e} ".format(iiter - 1, error), end=printEndOfLine)
+            if self._iterationPrinter.getPrintLevel() > 0:
+                self._iterationPrinter.print("Anderson iteration {} error : {:.5e} ".format(iiter - 1, error))
 
-        if self._printLevel == 1:
-            print("Anderson iteration {} error : {:.5e} ".format(iiter - 1, error))
+        if self._iterationPrinter.getPrintLevel() == 1:
+            self._iterationPrinter.reprint(tmplevel=2)
 
         self.denormalizeData(normData)
         return physics.getSolveStatus() and error <= self._tolerance
```

### Comparing `salome-c3po-2.1.1/c3po/couplers/FixedPointCoupler.py` & `salome-c3po-2.2/sources/c3po/couplers/FixedPointCoupler.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 # 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # 3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """ Contain the class FixedPointCoupler. """
 from __future__ import print_function, division
 
+from c3po.PhysicsDriver import PhysicsDriver
 from c3po.Coupler import Coupler
 from c3po.CollaborativeDataManager import CollaborativeDataManager
+from c3po.services.Printer import Printer
 
 
 class FixedPointCoupler(Coupler):
     """! FixedPointCoupler inherits from Coupler and proposes a damped fixed point algorithm.
 
     The class proposes an algorithm for the resolution of F(X) = X. Thus FixedPointCoupler is a Coupler working with :
 
@@ -27,15 +29,15 @@
     Each DataManager is normalized with its own norm got after the first iteration.
     They are then used as a single DataManager using CollaborativeDataManager.
 
     At each iteration we do (with n the iteration number and alpha the damping factor):
 
         X^{n+1} = alpha * F(X^{n}) + (1 - alpha) * X^{n}
 
-    The convergence criteria is : ||F(X^{n}) - X^{n}|| / ||X^{n+1}|| < tolerance. The default norm used is the infinite norm. setNormChoice() allows to choose another one.
+    The convergence criteria is : ||F(X^{n}) - X^{n}|| / ||F(X^{n})|| < tolerance. The default norm used is the infinite norm. setNormChoice() allows to choose another one.
 
     The default value of tolerance is 1.E-6. Call setConvergenceParameters() to change it.
 
     The default maximum number of iterations is 100. Call setConvergenceParameters() to change it.
 
     The default damping factor is 1 (no damping). Call setDampingFactor() to change it.
     """
@@ -47,28 +49,34 @@
         @param exchangers list of exactly two Exchanger allowing to go from the PhysicsDriver to the DataManager and vice versa.
         @param dataManagers list of DataManager.
         """
         Coupler.__init__(self, physics, exchangers, dataManagers)
         self._tolerance = 1.E-6
         self._maxiter = 100
         self._dampingFactor = 1.
-        self._isConverged = False
-        self._printLevel = 2
+        self._iterationPrinter = Printer(2)
+        self._leaveIfFailed = False
+        self._useIterate = False
+        self._iter = 0
 
         if not isinstance(physics, list) or not isinstance(exchangers, list) or not isinstance(dataManagers, list):
             raise Exception("FixedPointCoupler.__init__ physics, exchangers and dataManagers must be lists!")
         if len(physics) != 1:
             raise Exception("FixedPointCoupler.__init__ There must be only one PhysicsDriver")
         if len(exchangers) != 2:
             raise Exception("FixedPointCoupler.__init__ There must be exactly two Exchanger")
 
+        self._data = CollaborativeDataManager(self._dataManagers)
+        self._previousData = None
+        self._normData = 0.
+
     def setConvergenceParameters(self, tolerance, maxiter):
         """! Set the convergence parameters (tolerance and maximum number of iterations).
 
-        @param tolerance the convergence threshold in ||F(X^{n}) - X^{n}|| / ||X^{n+1}|| < tolerance.
+        @param tolerance the convergence threshold in ||F(X^{n}) - X^{n}|| / ||F(X^{n})|| < tolerance.
         @param maxiter the maximal number of iterations.
         """
         self._tolerance = tolerance
         self._maxiter = maxiter
 
     def setDampingFactor(self, dampingFactor):
         """! Set the damping factor of the method.
@@ -80,68 +88,106 @@
     def setPrintLevel(self, level):
         """! Set the print level during iterations (0=None, 1 keeps last iteration, 2 prints every iteration).
 
         @param level integer in range [0;2]. Default: 2.
         """
         if not level in [0, 1, 2]:
             raise Exception("FixedPointCoupler.setPrintLevel level should be one of [0, 1, 2]!")
-        self._printLevel = level
+        self._iterationPrinter.setPrintLevel(level)
 
-    def solveTimeStep(self):
-        """! Solve a time step using the damped fixed-point algorithm.
+    def setFailureManagement(self, leaveIfSolvingFailed):
+        """! Set if iterations should continue or not in case of solver failure (solveTimeStep returns False).
 
-        See also c3po.PhysicsDriver.PhysicsDriver.solveTimeStep().
+        @param leaveIfSolvingFailed set False to continue the iterations, True to stop. Default: False.
+        """
+        self._leaveIfFailed = leaveIfSolvingFailed
+
+    def setUseIterate(self, useIterate):
+        """ ! If True is given, the iterate() method on the given PhysicsDriver is called instead of the solve() method.
+
+        @param useIterate bool. Set True to use iterate(), False to use solve(). Default: False.
+        """
+        self._useIterate = useIterate
+
+    def iterateTimeStep(self):
+        """! Make on iteration of a damped fixed-point algorithm.
+
+        See also c3po.PhysicsDriver.PhysicsDriver.iterateTimeStep().
         """
-        iiter = 0
-        error = self._tolerance + 1.
         physics = self._physicsDrivers[0]
         physics2Data = self._exchangers[0]
         data2physics = self._exchangers[1]
 
-        # Init
-        if self._printLevel:
-            printEndOfLine = "\r" if self._printLevel == 1 else "\n"
-            print("fixed-point iteration {} ".format(iiter), end=printEndOfLine)
+        if self._iter > 0:
+            if not self._useIterate:
+                physics.abortTimeStep()
+                physics.initTimeStep(self._dt)
+            data2physics.exchange()
 
-        physics.solve()
+        if self._useIterate:
+            physics.iterate()
+        else:
+            physics.solve()
         physics2Data.exchange()
 
-        data = CollaborativeDataManager(self._dataManagers)
-        normData = self.readNormData()
-        self.normalizeData(normData)
-
-        previousData = data.clone()
-        iiter += 1
-
-        while error > self._tolerance and iiter < self._maxiter:
-            self.abortTimeStep()
-            self.initTimeStep(self._dt)
-            self.denormalizeData(normData)
-            data2physics.exchange()
+        if self._iter == 0:
+            self._normData = self.readNormData()
+        self.normalizeData(self._normData)
+
+        if self._iter > 0:
+            normNewData = self.getNorm(self._data)
+            self._data -= self._previousData
+            error = self.getNorm(self._data) / normNewData
+
+            self._data *= self._dampingFactor
+            self._data += self._previousData
+
+            self._previousData.copy(self._data)
+        else:
+            error = self._tolerance + 1.
+            self._previousData = self._data.clone()
+
+        self.denormalizeData(self._normData)
+
+        if self._iterationPrinter.getPrintLevel() > 0:
+            if self._iter == 0:
+                self._iterationPrinter.print("fixed-point iteration {} ".format(self._iter))
+            else:
+                self._iterationPrinter.print("fixed-point iteration {} error : {:.5e}".format(self._iter, error))
 
-            physics.solve()
-            physics2Data.exchange()
-            self.normalizeData(normData)
+        self._iter += 1
 
-            if self._dampingFactor != 1.:
-                data *= self._dampingFactor
-                data.imuladd(1. - self._dampingFactor, previousData)
+        succeed, converged = physics.getIterateStatus() if self._useIterate else (physics.getSolveStatus(), True)
+        converged = converged and error <= self._tolerance
 
-            if iiter == 1:
-                diffData = data.clone()
-            else:
-                diffData.copy(data)
-            diffData -= previousData
-            error = self.getNorm(diffData) / self.getNorm(data)
-            error /= self._dampingFactor
-
-            previousData.copy(data)
-
-            iiter += 1
-            if self._printLevel:
-                print("fixed-point iteration {} error : {:.5e} ".format(iiter - 1, error), end=printEndOfLine)
+        return succeed, converged
 
-        if self._printLevel == 1:
-            print("fixed-point iteration {} error : {:.5e} ".format(iiter - 1, error))
+    def solveTimeStep(self):
+        """! Solve a time step using the damped fixed-point algorithm.
+
+        See also c3po.PhysicsDriver.PhysicsDriver.solveTimeStep().
+        """
+        converged = False
+        succeed = True
 
-        self.denormalizeData(normData)
-        return physics.getSolveStatus() and error <= self._tolerance
+        while (succeed or not self._leaveIfFailed) and (not converged) and self._iter < self._maxiter:
+            self.iterate()
+            succeed, converged = self.getIterateStatus()
+
+        if self._iterationPrinter.getPrintLevel() == 1:
+            self._iterationPrinter.reprint(tmplevel=2)
+
+        return succeed and converged
+
+    def getIterateStatus(self):
+        """! See PhysicsDriver.getSolveStatus(). """
+        return PhysicsDriver.getIterateStatus(self)
+
+    def getSolveStatus(self):
+        """! See PhysicsDriver.getSolveStatus(). """
+        return PhysicsDriver.getSolveStatus(self)
+
+    def initTimeStep(self, dt):
+        """ See c3po.PhysicsDriver.PhysicsDriver.initTimeStep().  """
+        self._iter = 0
+        self._previousData = 0
+        return Coupler.initTimeStep(self, dt)
```

### Comparing `salome-c3po-2.1.1/c3po/couplers/JFNKCoupler.py` & `salome-c3po-2.2/sources/c3po/couplers/JFNKCoupler.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """ Contain the class JFNKCoupler. """
 from __future__ import print_function, division
 import math
 import numpy as np
 
 from c3po.Coupler import Coupler
 from c3po.CollaborativeDataManager import CollaborativeDataManager
+from c3po.services.Printer import Printer
 
 
 def solveTriang(matrixA, vectorB):
     """! INTERNAL.
 
     Solves a triangular linear system.
     """
@@ -75,16 +76,16 @@
         """
         Coupler.__init__(self, physics, exchangers, dataManagers)
         self._newtonTolerance = 1.E-6
         self._newtonMaxIter = 10
         self._krylovTolerance = 1.E-4
         self._krylovMaxIter = 100
         self._epsilon = 1.E-4
-        self._isConverged = False
-        self._printLevel = 2
+        self._iterationPrinter = Printer(2)
+        self._leaveIfFailed = False
 
         if not isinstance(physics, list) or not isinstance(exchangers, list) or not isinstance(dataManagers, list):
             raise Exception("JFNKCoupler.__init__ physics, exchangers and dataManagers must be lists!")
         if len(physics) != 1:
             raise Exception("JFNKCoupler.__init__ There must be only one PhysicsDriver")
         if len(exchangers) != 2:
             raise Exception("JFNKCoupler.__init__ There must be exactly two Exchanger")
@@ -117,15 +118,22 @@
     def setPrintLevel(self, level):
         """! Set the print level during iterations (0=None, 1 keeps last iteration, 2 prints every iteration).
 
         @param level integer in range [0;2]. Default: 2.
         """
         if not level in [0, 1, 2]:
             raise Exception("JFNKCoupler.setPrintLevel level should be one of [0, 1, 2]!")
-        self._printLevel = level
+        self._iterationPrinter.setPrintLevel(level)
+
+    def setFailureManagement(self, leaveIfSolvingFailed):
+        """! Set if iterations should continue or not in case of solver failure (solveTimeStep returns False).
+
+        @param leaveIfSolvingFailed set False to continue the iterations, True to stop. Default: False.
+        """
+        self._leaveIfFailed = leaveIfSolvingFailed
 
     def solveTimeStep(self):
         """! Solve a time step using Jacobian-Free Newton Krylov algorithm.
 
         See also c3po.PhysicsDriver.PhysicsDriver.solveTimeStep().
         """
         physics = self._physicsDrivers[0]
@@ -133,19 +141,18 @@
         data2physics = self._exchangers[1]
         iterNewton = 0
         iterKrylov = 0
         residual = 0
         previousData = 0
         matrixQ = []
 
-        if self._printLevel:
-            printEndOfLine = "\r" if self._printLevel == 1 else "\n"
-
         # On calcul ici l'etat "0"
         physics.solve()
+        if self._leaveIfFailed and not physics.getSolveStatus():
+            return False
         physics2Data.exchange()
 
         data = CollaborativeDataManager(self._dataManagers)
         normData = self.readNormData()
         self.normalizeData(normData)
 
         errorNewton = self._newtonTolerance + 1
@@ -159,24 +166,26 @@
                 previousData.copy(data)
 
             self.abortTimeStep()
             self.initTimeStep(self._dt)
             self.denormalizeData(normData)
             data2physics.exchange()
             physics.solve()
+            if self._leaveIfFailed and not physics.getSolveStatus():
+                return False
             physics2Data.exchange()
             self.normalizeData(normData)
 
             residual -= data  # residual is the second member of the linear system: -F(x) = -(f(x)-x)
             norm2Residual = residual.norm2()
 
             errorNewton = self.getNorm(residual) / self.getNorm(data)
 
-            if self._printLevel:
-                print("JFNK Newton iteration {} initial error : {:.5e}".format(iterNewton, errorNewton), end=printEndOfLine)
+            if self._iterationPrinter.getPrintLevel() > 0:
+                self._iterationPrinter.print("JFNK Newton iteration {} initial error : {:.5e}".format(iterNewton, errorNewton))
 
             if errorNewton > self._newtonTolerance:
 
                 if len(matrixQ) < 1:
                     matrixQ.append(residual * (1. / norm2Residual))
                 else:
                     matrixQ[0].copy(residual)
@@ -199,14 +208,16 @@
                     data.imuladd(self._epsilon, matrixQ[iterKrylov - 1])
 
                     self.abortTimeStep()
                     self.initTimeStep(self._dt)
                     self.denormalizeData(normData)
                     data2physics.exchange()
                     physics.solve()
+                    if self._leaveIfFailed and not physics.getSolveStatus():
+                        return False
                     physics2Data.exchange()
                     self.normalizeData(normData)
 
                     data -= previousData
                     data.imuladd(-self._epsilon, matrixQ[iterKrylov - 1])
 
                     if len(matrixQ) < iterKrylov + 1:
@@ -250,25 +261,25 @@
                     matrixR = np.dot(rot, matrixR)
 
                     krylovResidual = np.append(krylovResidual, 0.)
                     krylovResidual = np.dot(rot, krylovResidual)
 
                     errorKrylov = abs(krylovResidual[-1]) / norm2Residual
 
-                    if self._printLevel:
-                        print("    JFNK Krylov iteration {} error : {:.5e}".format(iterKrylov - 1, errorKrylov), end=printEndOfLine)
+                    if self._iterationPrinter.getPrintLevel() > 0:
+                        self._iterationPrinter.print("    JFNK Krylov iteration {} error : {:.5e}".format(iterKrylov - 1, errorKrylov))
 
                 squareR = matrixR[0:iterKrylov, 0:iterKrylov]
                 reduceKrylovResidual = krylovResidual[0:iterKrylov]
                 krylovResu = solveTriang(squareR, reduceKrylovResidual)
 
                 data.copy(previousData)
                 for i in range(iterKrylov):
                     data.imuladd(krylovResu[i], matrixQ[i])
 
             iterNewton += 1
 
-        if self._printLevel == 1:
-            print("JFNK Newton iteration {} initial error : {:.5e}".format(iterNewton - 1, errorNewton))
+        if self._iterationPrinter.getPrintLevel() == 1:
+            self._iterationPrinter.reprint(tmplevel=2)
 
         self.denormalizeData(normData)
         return physics.getSolveStatus() and errorNewton <= self._newtonTolerance
```

### Comparing `salome-c3po-2.1.1/c3po/couplers/__init__.py` & `salome-c3po-2.2/sources/c3po/exchangeMethods/__init__.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/exchangeMethods/DirectMatching.py` & `salome-c3po-2.2/sources/c3po/exchangeMethods/DirectMatching.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/exchangeMethods/ExchangeMethod.py` & `salome-c3po-2.2/sources/c3po/exchangeMethods/ExchangeMethod.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/exchangeMethods/SharedRemapping.py` & `salome-c3po-2.2/sources/c3po/exchangeMethods/SharedRemapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,122 +12,152 @@
 from __future__ import print_function, division
 import pickle
 
 from c3po.medcouplingCompat import MEDCouplingRemapper
 from c3po.exchangeMethods.ExchangeMethod import ExchangeMethod
 
 
-class Remapper(MEDCouplingRemapper):    # pylint: disable=too-many-ancestors
+def computeCellsToScreenOut(mesh1, mesh2):
+    """! INTERNAL """
+    bary = []
+    try:
+        bary = mesh1.computeCellCenterOfMass()  # MEDCoupling 9
+    except:
+        bary = mesh1.getBarycenterAndOwner()  # MEDCoupling 7
+    _, cellsId = mesh2.getCellsContainingPoints(bary, 1.0e-8)
+    dsi = cellsId.deltaShiftIndex()
+    try:
+        return dsi.findIdsEqual(0)  # MEDCoupling 9
+    except:
+        return dsi.getIdsEqual(0)  # MEDCoupling 7
+
+
+class Remapper(object):
     """! Allow to share the mesh projection for different SharedRemapping objects by building them with the same instance of this class. """
 
-    def __init__(self, meshAlignment=False, offset=[0., 0., 0.], rescaling=1., rotation=0., outsideCellsScreening=False):
+    def __init__(self, meshAlignment=False, offset=None, rescaling=1., rotation=0., outsideCellsScreening=False, reverseTransformations=True):
         """! Build a Remapper object.
 
         @param meshAlignment If set to True, at the initialization phase of the Remapper object, meshes are translated such as their "bounding
-            box" are radially centred on (x = 0., y = 0.) and have zmin = 0.
-        @param offset Value of the 3D offset between the source and the target meshes (>0 on z means that the source mesh is above the target one).
+            box" are radially centred on (x = 0., y = 0.) and, if the meshes are 3D, have zmin = 0.
+        @param offset Value of the offset between the source and the target meshes (>0 on z means that the source mesh is above the target one).
             The given vector is used to translate the source mesh (after the mesh alignment, if any).
         @param rescaling Value of a rescaling factor to be applied between the source and the target meshes (>1 means that the source mesh is
-            initially larger than the target one). The scaling is centered on [0., 0., 0.] and is applied to the source mesh after mesh
+            initially larger than the target one). The scaling is centered on [0., 0.(, 0.)] and is applied to the source mesh after mesh
             alignment or translation, if any.
-        @param rotation Value of the rotation between the source and the target meshes. The rotation is centered on [0., 0., 0.] and is about
+        @param rotation Value of the rotation between the source and the target meshes. The rotation is centered on [0., 0.(, 0.)] and is about
             the vertical axis. >0 means that the source mesh is rotated of the given angle compared to the target one. The inverse rotation is
             applied to the source mesh, after mesh alignment or translation, if any. pi means half turn.
         @param outsideCellsScreening If set to True, target (and source) cells whose barycentre is outside of source (or target) mesh are screen
             out (defaultValue is assigned to them). It can be useful to screen out cells that are in contact with the other mesh, but that should
             not be intersected by it. On the other hand, it will screen out cells actually intersected if their barycenter is outside of the other
             mesh ! Be careful with this option.
+        @param reverseTransformations If set to True, all the transformations (translation, rescaling and rotation) applied in initialize() on
+            the provided meshes are reversed at the end of initialize().
+
+        @warning There seems to be a bug in MEDCoupling that may cause wrong results when rescaling is used with a source mesh of nature
+            ExtensiveMaximum or IntensiveConservation. In this case, it is necessary to use reverseTransformations=False and to never perform a
+            remapping on a field whose underling mesh has not been rescaled.
         """
-        MEDCouplingRemapper.__init__(self)
         self.isInit = False
         self._meshAlignment = meshAlignment
         self._offset = offset
         if rescaling <= 0.:
             raise ValueError("Remapper: rescaling must be > 0!")
         self._rescaling = rescaling
         self._rotation = rotation
         self._outsideCellsScreening = outsideCellsScreening
+        self._reverseTransformations = reverseTransformations
         self._cellsToScreenOutSource = []
         self._cellsToScreenOutTarget = []
         self._loadedMatrix = None
+        self._remapper = MEDCouplingRemapper()
 
     def initialize(self, sourceMesh, targetMesh):
         """! INTERNAL """
+        meshDimension = sourceMesh.getMeshDimension()
+        if targetMesh.getMeshDimension() != meshDimension:
+            raise Exception("Remapper : the dimension of source and target meshes are not the same ({} and {} respectively).".format(meshDimension, targetMesh.getMeshDimension()))
+        offsetAlign = []
         if self._meshAlignment:
             for mesh in [sourceMesh, targetMesh]:
-                [(xmin, xmax), (ymin, ymax), (zmin, _)] = mesh.getBoundingBox()
-                offsettmp = [-0.5 * (xmin + xmax), -0.5 * (ymin + ymax), -zmin]
-                mesh.translate(offsettmp)
-        if self._offset != [0., 0., 0.]:
+                if meshDimension == 2:
+                    [(xmin, xmax), (ymin, ymax)] = mesh.getBoundingBox()
+                else:
+                    [(xmin, xmax), (ymin, ymax), (zmin, _)] = mesh.getBoundingBox()
+                offsetAlign.append([-0.5 * (xmin + xmax), -0.5 * (ymin + ymax)] + ([zmin] if meshDimension == 3 else []))
+                mesh.translate(offsetAlign[-1])
+        if self._offset is not None and self._offset != [0.] * meshDimension:
             sourceMesh.translate([-x for x in self._offset])
         if self._rescaling != 1.:
-            sourceMesh.scale([0., 0., 0.], 1. / self._rescaling)
+            sourceMesh.scale([0.] * meshDimension, 1. / self._rescaling)
         if self._rotation != 0.:
-            sourceMesh.rotate([0., 0., 0.], [0., 0., 1.], self._rotation)
+            if meshDimension == 2:
+                sourceMesh.rotate([0., 0.], self._rotation)
+            else:
+                sourceMesh.rotate([0., 0., 0.], [0., 0., 1.], self._rotation)
 
         if self._loadedMatrix is not None:
-            try:
-                self.setCrudeMatrix(sourceMesh, targetMesh, "P0P0", self._loadedMatrix)
-            except:
-                print("Remapper.initialize: Failure to load the matrix.")
-                self.prepare(sourceMesh, targetMesh, "P0P0")
+            self._remapper.setCrudeMatrix(sourceMesh, targetMesh, "P0P0", self._loadedMatrix)
             self._loadedMatrix = None
         else:
-            self.prepare(sourceMesh, targetMesh, "P0P0")
+            self._remapper.prepare(sourceMesh, targetMesh, "P0P0")
 
         if self._outsideCellsScreening:
-            self._cellsToScreenOutTarget = self.computeCellsToScreenOut(targetMesh, sourceMesh)
-            self._cellsToScreenOutSource = self.computeCellsToScreenOut(sourceMesh, targetMesh)
+            self._cellsToScreenOutTarget = computeCellsToScreenOut(targetMesh, sourceMesh)
+            self._cellsToScreenOutSource = computeCellsToScreenOut(sourceMesh, targetMesh)
 
-        self.isInit = True
+        if self._reverseTransformations:
+            if self._rotation != 0.:
+                if meshDimension == 2:
+                    sourceMesh.rotate([0., 0.], -self._rotation)
+                else:
+                    sourceMesh.rotate([0., 0., 0.], [0., 0., 1.], -self._rotation)
+            if self._rescaling != 1.:
+                sourceMesh.scale([0.] * meshDimension, self._rescaling)
+            if self._offset is not None and self._offset != [0.] * meshDimension:
+                sourceMesh.translate([self._offset])
+            if self._meshAlignment:
+                sourceMesh.translate([-x for x in offsetAlign[0]])
+                targetMesh.translate([-x for x in offsetAlign[1]])
 
-    def computeCellsToScreenOut(self, mesh1, mesh2):
-        """! INTERNAL """
-        bary = []
-        try:
-            bary = mesh1.computeCellCenterOfMass()  # MEDCoupling 9
-        except:
-            bary = mesh1.getBarycenterAndOwner()  # MEDCoupling 7
-        _, cellsId = mesh2.getCellsContainingPoints(bary, 1.0e-8)
-        dsi = cellsId.deltaShiftIndex()
-        try:
-            return dsi.findIdsEqual(0)  # MEDCoupling 9
-        except:
-            return dsi.getIdsEqual(0)  # MEDCoupling 7
+        self.isInit = True
 
     def directRemap(self, field, defaultValue):
         """! INTERNAL """
-        outputField = MEDCouplingRemapper.transferField(self, field, defaultValue)
+        outputField = self._remapper.transferField(field, defaultValue)
         outputField.getArray()[self._cellsToScreenOutTarget] = defaultValue
         return outputField
 
     def reverseRemap(self, field, defaultValue):
         """! INTERNAL """
-        outputField = MEDCouplingRemapper.reverseTransferField(self, field, defaultValue)
+        outputField = self._remapper.reverseTransferField(field, defaultValue)
         outputField.getArray()[self._cellsToScreenOutSource] = defaultValue
         return outputField
 
     def exportMatrix(self, fileName):
         """! Export remapping matrix on file.
 
         This file can be loaded using loadMatrix() method in order to save initialization time.
 
         @param fileName name of the file to write in.
         """
         if not self.isInit:
             raise AssertionError("Remapper.export: the object is not initialized! Remapper is usually initialized by the SharedRemapping object using it at the first call.")
         with open(fileName, 'wb') as matrixFile:
-            matrix = self.getCrudeMatrix()
+            matrix = self._remapper.getCrudeMatrix()
             pickle.dump(matrix, matrixFile)
 
     def loadMatrix(self, fileName):
         """! Load remapping matrix from file.
 
         This file is usually written by exportMatrix() method.
 
+        @note This method requires scipy.
+
         @param fileName name of the file to read from.
         """
         if self.isInit:
             raise AssertionError("Remapper.export: the object is already initialized! You can load matrix only before initialization.")
         with open(fileName, 'rb') as matrixFile:
             self._loadedMatrix = pickle.load(matrixFile)
 
@@ -147,16 +177,16 @@
     The initialization of the projection method (long operation) is done only once, and can be shared with other instances of
     SharedRemapping through a Remapper object.
     """
 
     def __init__(self, remapper, reverse=False, defaultValue=0., linearTransform=(1., 0.)):
         """! Build an SharedRemapping object, to be given to an Exchanger.
 
-        @param remapper A Remapper object (defined in C3PO and inheriting from MEDCouplingRemapper) performing the projection. It
-               can thus be shared with other instances of SharedRemapping (its initialization will always be done only once).
+        @param remapper A Remapper object (defined in C3PO) performing the projection. It can thus be shared with other instances of
+               SharedRemapping (its initialization will always be done only once).
         @param reverse Allows the Remapper to be shared with an instance of SharedRemapping performing the reverse exchange (the projection
                will be done in the reverse direction if reverse is set to True).
         @param defaultValue This is the default value to be assigned, during the projection, in the meshes of the target mesh that are not
                intersected by the source mesh.
         @param linearTransform Tuple (a,b): apply a linear function to all output fields f such as they become a * f + b. The transformation
                is applied after the mesh projection.
         """
```

### Comparing `salome-c3po-2.1.1/c3po/exchangeMethods/SharedRemappingMulti1D3D.py` & `salome-c3po-2.2/sources/c3po/exchangeMethods/SharedRemappingMulti1D3D.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,122 +11,198 @@
 """ Contain the class SharedRemappingMulti1D3D. """
 from __future__ import print_function, division
 
 import c3po.medcouplingCompat as mc
 from c3po.exchangeMethods.SharedRemapping import Remapper, SharedRemapping
 
 
-class Multi1D3DRemapper(Remapper):  # pylint: disable=too-many-ancestors
+def shift1DFields(shiftMap, shiftedFieldPositions, indexTable):
+    """! INTERNAL """
+    newFieldPositions = [-1] * len(shiftedFieldPositions)
+    availableFields = []
+
+    if len(shiftMap) != len(shiftedFieldPositions):
+        raise Exception("shift1DFields: the provided shiftMap must contain as many values ({} provided) than the number of 1D fields ({}).".format(len(shiftMap), len(shiftedFieldPositions)))
+    if max(shiftMap) > len(shiftedFieldPositions) - 1:
+        raise Exception("shift1DFields: the provided shiftMap contains values ({}) greater than the number of 1D fields - 1 ({}).".format(max(shiftMap), len(shiftedFieldPositions) - 1))
+
+    for ipos, ifield in enumerate(shiftedFieldPositions):
+        if shiftMap[ipos] >= 0:
+            if newFieldPositions[shiftMap[ipos]] >= 0:
+                raise Exception("shift1DFields: the provided shiftMap contains twice the positive value ({}).".format(shiftMap[ipos]))
+            newFieldPositions[shiftMap[ipos]] = ifield
+        else:
+            availableFields.append(ifield)
+
+    count = 0
+    for ipos, ifield in enumerate(newFieldPositions):
+        if ifield < 0:
+            newFieldPositions[ipos] = availableFields[count]
+            count += 1
+
+    newIndexTable = [[] for _ in range(len(indexTable))]
+
+    for ipos, ifield in enumerate(newFieldPositions):
+        newIndexTable[ifield] = indexTable[shiftedFieldPositions[ipos]]
+
+    return availableFields, newFieldPositions, newIndexTable
+
+
+class Multi1D3DRemapper(Remapper):
     """! Allow to share the mesh projection for different SharedRemappingMulti1D3D objects by building them with the same instance of this class. """
 
-    def __init__(self, xCoordinates, yCoordinates, indexTable, weights, meshAlignment=False, offset=[0., 0., 0.], rescaling=1., rotation=0., outsideCellsScreening=False):
+    def __init__(self, xCoordinates, yCoordinates, indexTable, weights, meshAlignment=False, offset=[0., 0., 0.], rescaling=1., rotation=0., outsideCellsScreening=False, reverseTransformations=True):
         """! Build a Multi1D3DRemapper object.
 
         An intermediate inner 3D mesh is built from a 2D grid defined by the parameters.
 
-        The axial coordinates will be read from the 1D fields passed to the remapper (there are assumed to all share the same axial mesh).
+        The axial coordinates will be read from the 1D fields passed to the remapper.
 
         Each cell of this 2D grid is associated to a 1D field.
 
         @param xCoordinates x coordinates of the inner mesh to build.
         @param yCoordinates y coordinates of the inner mesh to build.
         @param indexTable For each position of the 2D grid (x coordinate changes first), the index of the 1D field to associate. Put -1 to
         associate to nothing.
         @param weights Weigh of each 1D field to take into account for extensive variables.
         @param meshAlignment see Remapper. The source mesh is the multi1D one and the target mesh the 3D one.
         @param offset see Remapper. The source mesh is the multi1D one and the target mesh the 3D one.
         @param rescaling see Remapper. The source mesh is the multi1D one and the target mesh the 3D one.
         @param rotation see Remapper. The source mesh is the multi1D one and the target mesh the 3D one.
         @param outsideCellsScreening see Remapper.
+        @param reverseTransformations see Remapper.
+
+        @warning There seems to be a bug in MEDCoupling that may cause wrong results when rescaling is used with a source mesh (multi1D) of
+            nature ExtensiveMaximum or IntensiveConservation. In this case, using reverseTransformations=False should be enough to solve
+            the problem.
         """
-        Remapper.__init__(self, meshAlignment, offset, rescaling, rotation, outsideCellsScreening)
-        self._indexTable = [[] for k in range(max(indexTable) + 1)]
+        Remapper.__init__(self, meshAlignment, offset, rescaling, rotation, outsideCellsScreening, reverseTransformations)
+        self._indexTable = [[] for _ in range(max(indexTable) + 1)]
         for position, indice1D in enumerate(indexTable):
             if indice1D >= 0:
                 self._indexTable[indice1D].append(position)
+        self._shiftedFieldPositions = list(range(len(self._indexTable)))
 
         if len(self._indexTable) != len(weights):
             raise Exception("Multi1D3DRemapper.__init__ we give " + str(len(weights)) + "weight values instead of " + str(len(self._indexTable))
                             + ", the number of 1D calculations.")
         self._weights = weights
-        self._arrayX = mc.DataArrayDouble(xCoordinates)
-        self._arrayX.setInfoOnComponent(0, "X [m]")
-        self._arrayY = mc.DataArrayDouble(yCoordinates)
-        self._arrayY.setInfoOnComponent(0, "Y [m]")
-        self._arrayZ = 0
-        self._numberOf1DPositions = (self._arrayX.getNumberOfTuples() - 1) * (self._arrayY.getNumberOfTuples() - 1)
-        self._numberOfCellsIn1D = 0
+        self._xCoordinates = xCoordinates
+        self._yCoordinates = yCoordinates
+        self._zCoordinateArrays = [[] for _ in range(len(self._indexTable))]
+        self._numberOfCellsIn1D = [0] * len(self._indexTable)
         self._innerMesh = None
         self._innerField = mc.MEDCouplingFieldDouble(mc.ON_CELLS, mc.ONE_TIME)
         self._innerField.setName("3DFieldFromMulti1D")
         self.isInnerFieldBuilt = False
 
-    def buildInnerField(self, mesh1D):
+    def buildInnerField(self, meshes1D):
         """! INTERNAL """
-        self._arrayZ = mesh1D.getCoordsAt(0)
-        cMesh = mc.MEDCouplingCMesh("3DMeshFromMulti1D")
-        cMesh.setCoords(self._arrayX, self._arrayY, self._arrayZ)
-        self._innerMesh = cMesh.buildUnstructured()
-        self._numberOfCellsIn1D = mesh1D.getNumberOfCells()
+        internal1DMeshes = []
+        if len(meshes1D) != len(self._indexTable):
+            raise Exception("Multi1D3DRemapper.buildInnerField we give " + str(len(meshes1D)) + " 1D meshes instead of " + str(len(self._indexTable)) + ".")
+        for imesh, mesh1D in enumerate(meshes1D):
+            self._zCoordinateArrays[imesh] = mesh1D.getCoordsAt(0)
+            self._numberOfCellsIn1D[imesh] = mesh1D.getNumberOfCells()
+            for fieldIndex in self._indexTable[imesh]:
+                internal1DMeshes.append(mc.MEDCouplingCMesh("3DMeshFromMulti1D"))
+                xIndex = fieldIndex % (len(self._xCoordinates) - 1)
+                yIndex = fieldIndex // (len(self._xCoordinates) - 1)
+                arrayX = mc.DataArrayDouble([self._xCoordinates[xIndex], self._xCoordinates[xIndex + 1]])
+                arrayX.setInfoOnComponent(0, "X [m]")
+                arrayY = mc.DataArrayDouble([self._yCoordinates[yIndex], self._yCoordinates[yIndex + 1]])
+                arrayY.setInfoOnComponent(0, "Y [m]")
+                internal1DMeshes[-1].setCoords(arrayX, arrayY, self._zCoordinateArrays[imesh])
+        if len(internal1DMeshes) > 0:
+            self._innerMesh = mc.MEDCouplingMesh.MergeMeshes(internal1DMeshes)
+        else:
+            self._innerMesh = mc.MEDCouplingUMesh()
+        self._innerMesh.setName("3DMeshFromMulti1D")
         self._innerField.setMesh(self._innerMesh)
         array = mc.DataArrayDouble()
-        array.alloc(self._numberOfCellsIn1D * self._numberOf1DPositions)
-        array.fillWithValue(0.)
+        if len(internal1DMeshes) > 0:
+            array.alloc(self._innerMesh.getNumberOfCells())
+            array.fillWithValue(0.)
         self._innerField.setArray(array)
         self.isInnerFieldBuilt = True
+        self.isInit = False
 
     def getInnerField(self):
         """! INTERNAL """
         return self._innerField
 
     def build3DField(self, fields1D, defaultValue=0.):
         """! INTERNAL """
         resuField = self._innerField.clone(True)
         if len(fields1D) > 0:
             resuField.setNature(fields1D[0].getNature())
         array3D = resuField.getArray()
         array3D.fillWithValue(defaultValue)
-        nbOfElems3D = array3D.getNbOfElems()
+        indexMin = 0
         for i, field in enumerate(fields1D):
             array1D = field.getArray()
             if resuField.getNature() == mc.ExtensiveMaximum or resuField.getNature() == mc.ExtensiveConservation:
                 array1D *= self._weights[i]
-            for position in self._indexTable[i]:
-                array3D.setPartOfValues1(array1D, position, nbOfElems3D, self._numberOf1DPositions, 0, 1, 1)
+            for _ in self._indexTable[i]:
+                array3D.setPartOfValues1(array1D, indexMin, indexMin + self._numberOfCellsIn1D[i], 1, 0, 1, 1)
+                indexMin += self._numberOfCellsIn1D[i]
         return resuField
 
     def build1DFields(self, field3D):
         """! INTERNAL """
         array3D = field3D.getArray()
         fields1D = []
+        indexMin = 0
         for i, list1D in enumerate(self._indexTable):
             fields1D.append(mc.MEDCouplingFieldDouble(mc.ON_CELLS, mc.ONE_TIME))
             fields1D[-1].setName(field3D.getName())
             mesh1D = mc.MEDCouplingCMesh("mesh1D")
-            mesh1D.setCoords(self._arrayZ)
+            mesh1D.setCoords(self._zCoordinateArrays[i])
             fields1D[-1].setMesh(mesh1D)
             array1D = mc.DataArrayDouble()
-            array1D.alloc(self._numberOfCellsIn1D)
+            array1D.alloc(self._numberOfCellsIn1D[i])
             array1D.fillWithValue(0.)
-            for position in list1D:
+            for _ in list1D:
                 array1Dtmp = mc.DataArrayDouble()
-                array1Dtmp.alloc(self._numberOfCellsIn1D)
-                array1Dtmp.setContigPartOfSelectedValuesSlice(0, array3D, position, array3D.getNumberOfTuples(), self._numberOf1DPositions)
+                array1Dtmp.alloc(self._numberOfCellsIn1D[i])
+                array1Dtmp.setContigPartOfSelectedValuesSlice(0, array3D, indexMin, indexMin + self._numberOfCellsIn1D[i], 1)
+                indexMin += self._numberOfCellsIn1D[i]
                 array1D.addEqual(array1Dtmp)
             if len(list1D) > 0:
                 array1D *= 1. / len(list1D)
             if field3D.getNature() == mc.ExtensiveMaximum or field3D.getNature() == mc.ExtensiveConservation:
                 array1D *= 1. / self._weights[i]
             fields1D[-1].setArray(array1D)
         return fields1D
 
     def getNumberOf1DFields(self):
         """! INTERNAL """
         return len(self._indexTable)
 
+    def shift1DFields(self, shiftMap):
+        """! This method allows to shift the index of the 1D fields provided through the indexTable parameter of constructor.
+
+        @param shiftMap a list providing for each 1D fields the index (in indexTable) of its new position (-1 can be used to indicate that the field is no more used).
+
+        @return the list of the indexes no more used.
+
+        For example, shiftMap=[3, -1, 1, 2] indicates that at first call field_0 goes to position 3, field_1 is discharged, field_2 goes to 1 and field_3 goes to 2. It returns [1].
+        At the second call with the same input, field_0 (now at position 3) goes to 2, field_1 (at 0) goes to 3, field_2 (at 1) is discharged and field_3 (at 2) goes to 1. It returns [2].
+        The thrid call returns [3], the fourth call [0].
+        """
+        availableFields, shiftedFieldPositions, indexTable = shift1DFields(shiftMap, self._shiftedFieldPositions, self._indexTable)
+        self.setShiftedIndex(shiftedFieldPositions, indexTable)
+        return availableFields
+
+    def setShiftedIndex(self, shiftedFieldPositions, indexTable):
+        """ ! INTERNAL """
+        self._shiftedFieldPositions = shiftedFieldPositions
+        self._indexTable = indexTable
+        self.isInnerFieldBuilt = False
+
 
 class SharedRemappingMulti1D3D(SharedRemapping):
     """! SharedRemappingMulti1D3D is an ExchangeMethod which projects the input fields one by one before returning them as
     outputs, in the same order.
 
     See c3po.Exchanger.Exchanger.__init__().
 
@@ -162,25 +238,28 @@
             msg = "The number of provided fields ({} 3D fields and {} 1D fields) is wrong.\n".format(numberOf3DFields, numberOf1DFields)
             msg += "According to the provided remapper object, there must be {} 1D fields for each 3D fields.".format(self._numberOf1DFields)
             raise Exception(msg)
         if numberOf3DFields == 0:
             return [], valuesToGet
 
         if not self._remapper.isInnerFieldBuilt:
-            self._remapper.buildInnerField(fieldsToSet[0].getMesh() if self._isReverse else fieldsToGet[0].getMesh())
+            self._remapper.buildInnerField([field.getMesh() for field in (fieldsToSet if self._isReverse else fieldsToGet)])
         if self._isReverse:
-            outputFields, outputValues = SharedRemapping.__call__(self, fieldsToGet, [self._remapper.getInnerField()] * len(fieldsToGet), valuesToGet)
+            innerField = self._remapper.getInnerField()
+            if numberOf1DFields > 0:
+                innerField.setNature(fieldsToSet[0].getNature())
+            outputFields, outputValues = SharedRemapping.__call__(self, fieldsToGet, [innerField] * len(fieldsToGet), valuesToGet)
             resu = []
             for field3D in outputFields:
                 resu += self._remapper.build1DFields(field3D)
             return resu, outputValues
         indexFirst = 0
         intermediate3DField = []
         while indexFirst + self._numberOf1DFields <= len(fieldsToGet):
-            fields1D = [fieldsToGet[indexFirst + k] for k in range(self._numberOf1DFields)]
+            fields1D = fieldsToGet[indexFirst:indexFirst + self._numberOf1DFields]
             intermediate3DField.append(self._remapper.build3DField(fields1D, self._defaultValue))
             indexFirst += self._numberOf1DFields
         return SharedRemapping.__call__(self, intermediate3DField, fieldsToSet, valuesToGet)
 
     def getPatterns(self):
         """! See ExchangeMethod.getPatterns. """
         if self._isReverse:
```

### Comparing `salome-c3po-2.1.1/c3po/exchangeMethods/__init__.py` & `salome-c3po-2.2/sources/c3po/physicsDrivers/__init__.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/medcouplingCompat/__init__.py` & `salome-c3po-2.2/sources/c3po/medcouplingCompat/__init__.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/mpi/MPICollaborativeDataManager.py` & `salome-c3po-2.2/sources/c3po/mpi/MPICollaborativeDataManager.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,60 +11,72 @@
 """ Contain the class MPICollaborativeDataManager. """
 from __future__ import print_function, division
 import math
 from mpi4py import MPI
 
 from c3po.CollaborativeDataManager import CollaborativeDataManager
 from c3po.CollaborativeObject import CollaborativeObject
-from c3po.mpi.MPIRemoteProcess import MPIRemoteProcess
+from c3po.mpi.MPIRemote import MPIRemote
+from c3po.mpi.MPIDomainDecompositionDataManager import MPIDomainDecompositionDataManager
+from c3po.mpi.MPICollectiveDataManager import MPICollectiveDataManager
 
 
 class MPICollaborativeDataManager(CollaborativeDataManager):
     """! MPICollaborativeDataManager is the MPI collaborative version of c3po.CollaborativeDataManager.CollaborativeDataManager
     (for collaborative MPI paradigm).
 
     It allows to handle a set of c3po.DataManager.DataManager (some of then being remote) as a single one. Thanks to this class,
     data can be distributed on different MPI processes but still used in the same way.
 
-    When at least one MPIRemoteProcess is present, MPICollaborativeDataManager uses collective MPI communications: the object must
+    When at least one MPIRemote is present, MPICollaborativeDataManager uses collective MPI communications: the object must
     be built and used in the same way for all the involved processes. They must all share the same communicator, and all the processes
     of that communicator must be involved.
     """
 
     def __init__(self, dataManagers, mpiComm=None):
         """! Build a MPICollaborativeDataManager object.
 
-        Has the same form than CollaborativeDataManager.__init__() but can also contain MPIRemoteProcess objects.
+        Has the same form than CollaborativeDataManager.__init__() but can also contain MPIRemote objects.
 
-        When at least one MPIRemoteProcess is present (or if mpiComm is not None), MPICollaborativeDataManager uses collective MPI
+        When at least one MPIRemote is present (or if mpiComm is not None), MPICollaborativeDataManager uses collective MPI
         communications: the object must be built and used in the same way for all the involved processes. They must all share the same
         communicator, and all the processes of that communicator must be involved.
 
         @param dataManagers a list of c3po.DataManager.DataManager.
         @param mpiComm If not None, forces MPICollaborativeDataManager to use collective MPI communications and to use this
         communicator.
         """
         localData = []
         self.mpiComm = mpiComm
         self.isMPI = mpiComm is not None
+        indexToIgnore = []
 
         for data in dataManagers:
-            if mpiComm is None and isinstance(data, MPIRemoteProcess):
+            if mpiComm is None and isinstance(data, MPIRemote):
                 if not self.isMPI:
                     if data.mpiComm == MPI.COMM_NULL:
                         raise Exception("MPICollaborativeDataManager.__init__ All distant processes must be part of the communicator (MPI.COMM_NULL found).")
                     self.isMPI = True
                     self.mpiComm = data.mpiComm
                 else:
                     if self.mpiComm != data.mpiComm:
                         raise Exception("MPICollaborativeDataManager.__init__ All distant processes must used the same MPI communicator")
-            if not isinstance(data, MPIRemoteProcess):
-                localData.append(data)
+            if not isinstance(data, MPIRemote):
+                if isinstance(data, MPICollaborativeDataManager):
+                    localData += data.dataManagers
+                elif isinstance(data, MPIDomainDecompositionDataManager):
+                    localView = data.getLocalView()
+                    localData.append(localView)
+                else:
+                    if isinstance(data, MPICollectiveDataManager) and data.mpiComm.Get_rank() != 0:
+                        indexToIgnore.append(len(localData))
+                    localData.append(data)
 
         CollaborativeDataManager.__init__(self, localData)
+        self.ignoreForConstOperators(indexToIgnore)
         CollaborativeObject.__init__(self, dataManagers)    # pylint: disable=non-parent-init-called
 
     def cloneEmpty(self):
         """! Return a clone of self without copying the data.
 
         @return An empty clone of self.
         """
@@ -86,17 +98,19 @@
 
     def norm2(self):
         """! Return the norm 2.
 
         @return sqrt(sum_i(val[i] * val[i])) where val[i] stands for each scalar and each component of the MED fields.
         """
         norm = CollaborativeDataManager.norm2(self)
+        #print("local :", self, norm)
         if self.isMPI:
             norm = self.mpiComm.allreduce(norm * norm, op=MPI.SUM)
             norm = math.sqrt(norm)
+        #print("global :", self, norm)
         return norm
 
     def dot(self, other):
         """! Return the scalar product of self with other.
 
         @param other a MPICollaborativeDataManager consistent with self.
```

### Comparing `salome-c3po-2.1.1/c3po/mpi/MPICollaborativePhysicsDriver.py` & `salome-c3po-2.2/sources/c3po/mpi/MPIRemoteProcesses.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,25 +4,32 @@
 # All rights reserved.
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # 3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-""" Contain the class MPICollaborativePhysicsDriver. """
+""" Contain the class MPIRemoteProcesses. """
 from __future__ import print_function, division
 
-from c3po.mpi.MPICoupler import MPICoupler
-from c3po.CollaborativePhysicsDriver import CollaborativePhysicsDriver
+from c3po.mpi.MPIRemote import MPIRemote
 
 
-class MPICollaborativePhysicsDriver(CollaborativePhysicsDriver, MPICoupler):
-    """! MPICollaborativePhysicsDriver is the MPI version of CollaborativePhysicsDriver. """
+class MPIRemoteProcesses(MPIRemote):
+    """! MPIRemoteProcesses identifies remote processes in charge of the same task.
 
-    def __init__(self, physics, mpiComm=None):
-        """! Build an CollaborativePhysicsDriver object.
+    Inherits from MPIRemote and add a list of ranks.
+    """
 
-        @param physics a list (or dictionary) of PhysicsDriver objects.
-        @param mpiComm MPI communicator to provide to MPICoupler. See MPICoupler.__init__().
+    def __init__(self, mpiComm, ranks):
+        """! Build a MPIRemoteProcesses object.
+
+        @param mpiComm MPI communicator.
+        @param ranks List of ranks of the remote processes on mpiComm.
         """
-        MPICoupler.__init__(self, physics=physics, exchangers=[], mpiComm=mpiComm)
-        CollaborativePhysicsDriver.__init__(self, self._physicsDriversList)
+        MPIRemote.__init__(self, mpiComm)
+        self.ranks = ranks
+
+    def cloneEmpty(self):
+        """! return a clone. """
+        new = MPIRemoteProcesses(self.mpiComm, self.ranks)
+        return new
```

### Comparing `salome-c3po-2.1.1/c3po/mpi/MPICollectiveDataManager.py` & `salome-c3po-2.2/sources/c3po/mpi/MPICollectiveDataManager.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/mpi/MPICollectiveProcess.py` & `salome-c3po-2.2/sources/c3po/mpi/MPICollectiveProcess.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/mpi/MPICoupler.py` & `salome-c3po-2.2/sources/c3po/mpi/MPICoupler.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,45 +9,45 @@
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """ Contain the class MPICoupler. """
 from __future__ import print_function, division
 from mpi4py import MPI
 
 from c3po.Coupler import Coupler
-from c3po.mpi.MPIRemoteProcess import MPIRemoteProcess
+from c3po.mpi.MPIRemote import MPIRemote
 
 
 class MPICoupler(Coupler):
     """! MPICoupler is the MPI collaborative version of c3po.Coupler.Coupler.
 
     The MPI functionalities are used for some collective operations.
 
     Can replace, without impact, a c3po.Coupler.Coupler for a calculation on a single process, if the MPI environment is available.
     """
 
     def __init__(self, physics, exchangers, dataManagers=[], mpiComm=None):
         """! Build a MPICoupler object.
 
-        Has the same form than Coupler.__init__() but can also contain MPIRemoteProcess (and MPICollectiveProcess) objects.
+        Has the same form than Coupler.__init__() but can also contain MPIRemote (and MPICollectiveProcess) objects.
 
-        When at least one MPIRemoteProcess is present, MPICoupler uses collective MPI communications: the object must be
+        When at least one MPIRemote is present, MPICoupler uses collective MPI communications: the object must be
         built and used in the same way for all the involved processes. They must all share the same communicator,and all
         the processes of this communicator must be involved.
 
         @param physics list (or dictionary) of c3po.PhysicsDriver.PhysicsDriver objects to be coupled.
         @param exchangers list (or dictionary) of c3po.Exchanger.Exchanger for the coupling.
         @param dataManagers list (or dictionary) of c3po.DataManager.DataManager used in the coupling.
-        @param mpiComm If not None, forces MPICoupler to make MPI communications and to use this communicator.
+        @param mpiComm If not None, forces MPICoupler to make MPI communications and to use this communicator (can also be done with setMPIComm()).
         """
         Coupler.__init__(self, physics, exchangers, dataManagers)
         self.mpiComm = mpiComm
         self._isMPI = self.mpiComm is not None
 
         for phy in self._physicsDriversList:
-            if mpiComm is None and isinstance(phy, MPIRemoteProcess):
+            if mpiComm is None and isinstance(phy, MPIRemote):
                 if not self._isMPI:
                     if phy.mpiComm == MPI.COMM_NULL:
                         raise Exception("MPICoupler.__init__ All distant processes must be part of the communicator (MPI.COMM_NULL found).")
                     self._isMPI = True
                     self.mpiComm = phy.mpiComm
                 else:
                     if self.mpiComm != phy.mpiComm:
@@ -89,14 +89,20 @@
                             resu = res
                         else:
                             raise Exception("MPICoupler.isMEDCoupling64Bits Not a unique answer.")
         if resu is None:
             raise NotImplementedError
         return resu
 
+    def setMPIComm(self, mpicomm):
+        self.mpiComm = mpicomm
+
+    def getMPIComm(self):
+        return self.mpiComm
+
     def initialize(self):
         """! See Coupler.initialize(). """
         resu = Coupler.initialize(self)
         if self._isMPI:
             resu = self.mpiComm.allreduce(resu, op=MPI.MIN)
         return resu
```

### Comparing `salome-c3po-2.1.1/c3po/mpi/MPIMasterDataManager.py` & `salome-c3po-2.2/sources/c3po/mpi/MPIMasterDataManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,18 @@
         self.idDataWorker = idDataWorker
         self.localDataManager = localDataManager
 
     def __del__(self):
         """! Destructor. """
         self.physicsDriver.setDataManagerToFree(self.idDataWorker)
 
+    def getMPIComm(self):
+        """! See PhysicsDriver.getMPIComm(). """
+        return self.physicsDriver.getMPIComm()
+
     def checkCompatibility(self, other):
         """! INTERNAL """
         if not isinstance(other, MPIMasterDataManager) or self.physicsDriver != other.physicsDriver or (self.localDataManager is not None) and (other.localDataManager is None):
             raise Exception("MPIMasterDataManager.checkCompatibility : self and other are not compatible.")
 
     def clone(self):
         """! See c3po.DataManager.DataManager.clone(). """
```

### Comparing `salome-c3po-2.1.1/c3po/mpi/MPIMasterExchanger.py` & `salome-c3po-2.2/sources/c3po/mpi/MPIMasterExchanger.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,42 +10,46 @@
 
 """ Contain the class MPIMasterExchanger. """
 from __future__ import print_function, division
 
 from c3po.Exchanger import Exchanger
 from c3po.mpi.MPITag import MPITag
 from c3po.mpi.MPIRemoteProcess import MPIRemoteProcess
+from c3po.mpi.MPIRemoteProcesses import MPIRemoteProcesses
 from c3po.mpi.MPICollectiveProcess import MPICollectiveProcess
 
 
 class MPIMasterExchanger(Exchanger):
     """! MPIMasterExchanger is used by the master to control remote c3po.Exchanger.Exchanger(s).
 
     It can, in addition, be in charge of a local one (that allows the master to participate to the calculation).
 
     The exchange() method of MPIMasterExchanger commands workers to exchange data.
     """
 
     def __init__(self, workerProcesses, idExchangerWorker, localExchanger=None):
         """! Build a MPIMasterExchanger object.
 
-        @param workerProcesses The list of MPIRemoteProcess or MPICollectiveProcess identifying the remote processes involved in the
-        exchange. In the case of MPICollectiveProcess, the mpiComm must include all the workers + the master, and only them.
+        @param workerProcesses The list of MPIRemoteProcess, MPIRemoteProcesses or MPICollectiveProcess identifying the remote processes involved in
+        the exchange. In the case of MPICollectiveProcess, the mpiComm must include all the workers + the master, and only them.
         @param idExchangerWorker Number identifying the controlled c3po.Exchanger.Exchanger in the involved workers (see c3po.mpi.MPIWorker.MPIWorker).
         @param localExchanger a c3po.Exchanger.Exchanger the MPIMasterExchanger object will run in the same time than the workers. It
         enables the master to contribute to a collective computation.
         """
         self._workerProcesses = workerProcesses
         self._idExchangerWorker = idExchangerWorker
         self._localExchanger = localExchanger
 
     def exchange(self):
         """! Trigger the exchange of data. """
         for process in self._workerProcesses:
             if isinstance(process, MPIRemoteProcess):
                 process.mpiComm.send(self._idExchangerWorker, dest=process.rank, tag=MPITag.exchange)
+            elif isinstance(process, MPIRemoteProcesses):
+                for processRank in process.ranks:
+                    process.mpiComm.send(self._idExchangerWorker, dest=processRank, tag=MPITag.exchange)
             elif isinstance(process, MPICollectiveProcess):
                 process.mpiComm.bcast((MPITag.exchange, self._idExchangerWorker), root=process.mpiComm.Get_rank())
             else:
                 raise Exception("MPIMasterExchanger.exchange : we found an unknown worker type.")
         if self._localExchanger is not None:
             self._localExchanger.exchange()
```

### Comparing `salome-c3po-2.1.1/c3po/mpi/MPIMasterPhysicsDriver.py` & `salome-c3po-2.2/sources/c3po/mpi/MPIMasterPhysicsDriver.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,21 @@
 # 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # 3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """ Contain the class MPIMasterPhysicsDriver. """
 from __future__ import print_function, division
+
+import sys
 from mpi4py import MPI
 
 from c3po.PhysicsDriver import PhysicsDriver
+from c3po.mpi.MPIRemoteProcess import MPIRemoteProcess
+from c3po.mpi.MPIRemoteProcesses import MPIRemoteProcesses
 from c3po.mpi.MPICollectiveProcess import MPICollectiveProcess
 from c3po.mpi.MPITag import MPITag
 
 
 class MPIMasterPhysicsDriver(PhysicsDriver):
     """! MPIMasterPhysicsDriver is used by a master process to control a (set of) remote c3po.PhysicsDriver.PhysicsDriver(s) as a local one.
 
@@ -27,53 +31,71 @@
     the setInput(Double/Int/String)Value methods, for convenience). Use an c3po.mpi.MPIMasterExchanger.MPIMasterExchanger to exchange
     data with the worker.
     """
 
     def __init__(self, workerProcess, localPhysicsDriver=None):
         """! Build a MPIMasterPhysicsDriver object.
 
-        @param workerProcess a c3po.mpi.MPIRemoteProcess.MPIRemoteProcess or a c3po.mpi.MPICollectiveProcess.MPICollectiveProcess
-        identifying the worker process(es). Each worker process can be in charge of only one c3po.PhysicsDriver.PhysicsDriver.
-        In case of a c3po.mpi.MPICollectiveProcess.MPICollectiveProcess, the MPIComm must include all the workers + the master,
-        and only them.
+        @param workerProcess a c3po.mpi.MPIRemoteProcess.MPIRemoteProcess, a c3po.mpi.MPIRemoteProcesses.MPIRemoteProcesses or
+        a c3po.mpi.MPICollectiveProcess.MPICollectiveProcess identifying the worker process(es). Each worker process can be in
+        charge of only one c3po.PhysicsDriver.PhysicsDriver. In case of a c3po.mpi.MPICollectiveProcess.MPICollectiveProcess, the
+        MPIComm must include all the workers + the master, and only them.
         @param localPhysicsDriver a c3po.PhysicsDriver.PhysicsDriver the MPIMasterPhysicsDriver object will run in the same
         time than the workers. It enables the master to contribute to a collaborative calculations.
         """
         PhysicsDriver.__init__(self)
         self.mpiComm = workerProcess.mpiComm
         self._masterRank = self.mpiComm.Get_rank()
-        self._workerRank = None
+        self._workerRanks = None
         self._isCollective = False
         if isinstance(workerProcess, MPICollectiveProcess):
             self._isCollective = True
-        else:
-            self._workerRank = workerProcess.rank
+        elif isinstance(workerProcess, MPIRemoteProcess):
+            self._workerRanks = [workerProcess.rank]
+        elif isinstance(workerProcess, MPIRemoteProcesses):
+            self._workerRanks = workerProcess.ranks
         self._localPhysicsDriver = localPhysicsDriver
         self._dataManagersToFree = []
 
     def sendData(self, tag, data=None):
         """! INTERNAL """
         if self._isCollective:
             toSend = (tag,) if data is None else (tag, data)
             self.mpiComm.bcast(toSend, root=self._masterRank)
         else:
             if data is None:
                 data = 0
-            self.mpiComm.send(data, dest=self._workerRank, tag=tag)
+            for workerRank in self._workerRanks:
+                self.mpiComm.send(data, dest=workerRank, tag=tag)
 
     def recvData(self, data, collectiveOperator=MPI.MIN):
         """! INTERNAL """
         if self._isCollective:
             return self.mpiComm.reduce(data, op=collectiveOperator, root=self._masterRank)
-        return collectiveOperator(data, self.mpiComm.recv(source=self._workerRank, tag=MPITag.answer))
+        resu = data
+        for workerRank in self._workerRanks:
+            resu = collectiveOperator(resu, self.mpiComm.recv(source=workerRank, tag=MPITag.answer))
+        return resu
 
     def setDataManagerToFree(self, idDataManager):
         """! INTERNAL """
         self._dataManagersToFree.append(idDataManager)
 
+    def setDataFile(self, datafile):
+        """! See PhysicsDriver.setDataFile(). """
+        self.sendData(MPITag.setDataFile, datafile)
+        if self._localPhysicsDriver is not None:
+            self._localPhysicsDriver.setDataFile(datafile)
+
+    def getMPIComm(self):
+        """! See PhysicsDriver.getMPIComm(). """
+        if self._isCollective and self._localPhysicsDriver is not None:
+            return self.mpiComm
+        raise NotImplementedError
+
     def init(self):
         """! See PhysicsDriver.init(). """
         if self._initNb == 0:
             self.sendData(MPITag.init)
             if self._localPhysicsDriver is not None:
                 self._localPhysicsDriver.init()
         self._initNb += 1
@@ -247,7 +269,63 @@
             self._localPhysicsDriver.setInputIntValue(name, value)
 
     def setInputStringValue(self, name, value):
         """! See c3po.DataAccessor.DataAccessor.setInputStringValue(). """
         self.sendData(MPITag.setInputStringValue, (name, value))
         if self._localPhysicsDriver is not None:
             self._localPhysicsDriver.setInputStringValue(name, value)
+
+    def getInputValuesNames(self):
+        """! See c3po.DataAccessor.DataAccessor.getInputValuesNames(). """
+        self.sendData(MPITag.getInputValuesNames)
+        data = []
+        if self._localPhysicsDriver is not None:
+            data = self._localPhysicsDriver.getInputValuesNames()
+        return self.recvData(data, collectiveOperator=MPI.MAX)
+
+    def getOutputValuesNames(self):
+        """! See c3po.DataAccessor.DataAccessor.getOutputValuesNames(). """
+        self.sendData(MPITag.getOutputValuesNames)
+        data = []
+        if self._localPhysicsDriver is not None:
+            data = self._localPhysicsDriver.getOutputValuesNames()
+        return self.recvData(data, collectiveOperator=MPI.MAX)
+
+    def getValueType(self, name):
+        """! See c3po.DataAccessor.DataAccessor.getValueType(). """
+        self.sendData(MPITag.getValueType, name)
+        data = ""
+        if self._localPhysicsDriver is not None:
+            data = self._localPhysicsDriver.getValueType(name)
+        return self.recvData(data, collectiveOperator=MPI.MAX)
+
+    def getValueUnit(self, name):
+        """! See c3po.DataAccessor.DataAccessor.getValueUnit(). """
+        self.sendData(MPITag.getValueUnit, name)
+        data = ""
+        if self._localPhysicsDriver is not None:
+            data = self._localPhysicsDriver.getValueUnit(name)
+        return self.recvData(data, collectiveOperator=MPI.MAX)
+
+    def getOutputDoubleValue(self, name):
+        """! See c3po.DataAccessor.DataAccessor.getOutputDoubleValue(). """
+        self.sendData(MPITag.getOutputDoubleValue, name)
+        data = -sys.float_info.max
+        if self._localPhysicsDriver is not None:
+            data = self._localPhysicsDriver.getOutputDoubleValue(name)
+        return self.recvData(data, collectiveOperator=MPI.MAX)
+
+    def getOutputIntValue(self, name):
+        """! See c3po.DataAccessor.DataAccessor.getOutputIntValue(). """
+        self.sendData(MPITag.getOutputIntValue, name)
+        data = -sys.float_info.max
+        if self._localPhysicsDriver is not None:
+            data = self._localPhysicsDriver.getOutputIntValue(name)
+        return self.recvData(data, collectiveOperator=MPI.MAX)
+
+    def getOutputStringValue(self, name):
+        """! See c3po.DataAccessor.DataAccessor.getOutputStringValue(). """
+        self.sendData(MPITag.getOutputStringValue, name)
+        data = ""
+        if self._localPhysicsDriver is not None:
+            data = self._localPhysicsDriver.getOutputStringValue(name)
+        return self.recvData(data, collectiveOperator=MPI.MAX)
```

### Comparing `salome-c3po-2.1.1/c3po/mpi/MPIRecipient.py` & `salome-c3po-2.2/sources/c3po/mpi/MPIRecipient.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,22 @@
     def exchange(self):
         """! INTERNAL """
         mpiComm = self._sender.mpiComm
         senderRank = self._sender.rank
         if self._field == 0 or not self._isTemplate:
             medInfo = ()
             if self._isCollective:
+                mpiComm.Barrier()
                 medInfo = mpiComm.bcast(medInfo, root=senderRank)
             else:
+                mpiComm.send(0, dest=senderRank, tag=MPITag.data)
                 medInfo = mpiComm.recv(source=senderRank, tag=MPITag.data)
             self._field = mc.ReadField(*(medInfo[0]))
             self._field.setNature(medInfo[1])
+            self._field.setTime(*(medInfo[2]))
         self._storing.store(self._field)
 
 
 class MPIValueRecipient(object):
     """! INTERNAL """
 
     def __init__(self, sender, storing, isCollective):
```

### Comparing `salome-c3po-2.1.1/c3po/mpi/MPIRemoteProcess.py` & `salome-c3po-2.2/sources/c3po/mpi/MPIRemote.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,44 +4,46 @@
 # All rights reserved.
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # 3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-""" Contain the class MPIRemoteProcess. """
+""" Contain the class MPIRemote. """
 from __future__ import print_function, division
 
 from c3po.PhysicsDriver import PhysicsDriver
 from c3po.DataManager import DataManager
 
 
-class MPIRemoteProcess(PhysicsDriver, DataManager):
-    """! MPIRemoteProcess identifies a remote process.
+class MPIRemote(PhysicsDriver, DataManager):
+    """! MPIRemote replaces a remote PhysicsDriver or a remote DataManager.
 
     Inherits from c3po.PhysicsDriver.PhysicsDriver and c3po.DataManager.DataManager but passes most of the methods: it does nothing.
     """
 
-    def __init__(self, mpiComm, rank):
-        """! Build a MPIRemoteProcess object.
+    def __init__(self, mpiComm):
+        """! Build a MPIRemote object.
 
         @param mpiComm MPI communicator.
-        @param rank Rank of the remote process on mpiComm.
         """
         PhysicsDriver.__init__(self)
         self.mpiComm = mpiComm
-        self.rank = rank
         self._time = 0.
         self._dt = 1.e30
         self._stationaryMode = False
 
     def setMPIComm(self, mpicomm):
         """! pass """
         pass
 
+    def setDataFile(self, datafile):
+        """! pass """
+        pass
+
     def initialize(self):
         """! return True """
         return True
 
     def terminate(self):
         """! pass """
         pass
@@ -89,14 +91,23 @@
         """! reset time. """
         self._time = time_
 
     def iterateTimeStep(self):
         """! return (True, True) """
         return (True, True)
 
+    def save(self, label, method):
+        pass
+
+    def restore(self, label, method):
+        pass
+
+    def forget(self, label, method):
+        pass
+
     def setInputMEDDoubleField(self, name, field):
         """! pass """
         pass
 
     def setInputMEDIntField(self, name, field):
         """! pass """
         pass
@@ -115,9 +126,9 @@
 
     def setInputStringValue(self, name, value):
         """! pass """
         pass
 
     def cloneEmpty(self):
         """! return a clone. """
-        new = MPIRemoteProcess(self.mpiComm, self.rank)
+        new = MPIRemote(self.mpiComm)
         return new
```

### Comparing `salome-c3po-2.1.1/c3po/mpi/MPISender.py` & `salome-c3po-2.2/sources/c3po/mpi/MPISender.py`

 * *Files 27% similar despite different names*

```diff
@@ -60,39 +60,58 @@
 
     def __init__(self, destinations, dataAccess, storing, isTemplate):
         self._destinations = destinations
         self._dataAccess = dataAccess
         self._storing = storing
         self._isTemplate = isTemplate
         self._isFirstSend = True
+        self._fileName = None
 
     def exchange(self):
         """! INTERNAL """
         field = 0
         if self._isTemplate:
             field = self._dataAccess.getFieldTemplate()
         else:
             field = self._dataAccess.get()
 
-        if len(self._destinations) > 0 and (self._isFirstSend or not self._isTemplate):
+        if self._fileName is None:
             num = 0
-            while os.path.exists("ExchangeField_" + str(num) + ".med"):
+            rank = MPI.COMM_WORLD.Get_rank()
+            fileExist = True
+            while fileExist:
+                self._fileName = "ExchangeField_rank" + str(rank) + "_" + str(num) + ".med"
+                fileExist = os.path.exists(self._fileName)
                 num += 1
-            nameFile = "ExchangeField_" + str(num) + ".med"
-            mc.WriteField("ExchangeField_" + str(num) + ".med", field, True)
 
-            _, iteration, order = field.getTime()
-            medInfo = [(field.getTypeOfField(), os.getcwd() + "/" + nameFile, field.getMesh().getName(), 0, field.getName(), iteration, order), field.getNature()]
+        if len(self._destinations) > 0 and (self._isFirstSend or not self._isTemplate):
+            for destination in self._destinations:
+                mpiComm = destination.mpiComm
+                if isinstance(destination, MPICollectiveProcess):
+                    mpiComm.Barrier()
+                else:
+                    mpiComm.recv(source=destination.rank, tag=MPITag.data)
+
+            time, iteration, order = field.getTime()
+            field.setTime(0, 0, 0)
+            if os.path.exists(self._fileName):
+                mc.WriteFieldUsingAlreadyWrittenMesh(self._fileName, field)
+            else:
+                mc.WriteField(self._fileName, field, True)
+
+            medInfo = [(field.getTypeOfField(), os.path.join(os.getcwd(), self._fileName), field.getMesh().getName(), 0, field.getName(), field.getTime()[1], field.getTime()[2]), field.getNature(), (time, iteration, order)]
+            field.setTime(time, iteration, order)
 
             for destination in self._destinations:
                 mpiComm = destination.mpiComm
                 if isinstance(destination, MPICollectiveProcess):
                     mpiComm.bcast(medInfo, root=mpiComm.Get_rank())
                 else:
                     mpiComm.send(medInfo, dest=destination.rank, tag=MPITag.data)
+
         self._isFirstSend = False
         self._storing.store(field)
 
 
 class MPIValueSender(object):
     """! INTERNAL """
```

### Comparing `salome-c3po-2.1.1/c3po/mpi/MPITag.py` & `salome-c3po-2.2/sources/c3po/mpi/MPITag.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,36 +16,44 @@
     """! INTERNAL
 
     MPITag defines tags used in MPI communications.
     """
     answer = 0
     data = 1
 
-    init = 2
-    getInitStatus = 3
-    terminate = 4
-    presentTime = 5
-    computeTimeStep = 6
-    initTimeStep = 7
-    solve = 8
-    getSolveStatus = 9
-    validateTimeStep = 10
-    setStationaryMode = 11
-    getStationaryMode = 12
-    abortTimeStep = 13
-    isStationary = 14
-    resetTime = 15
-    iterate = 16
-    getIterateStatus = 17
-    save = 18
-    restore = 19
-    forget = 20
-    setInputDoubleValue = 21
-    setInputIntValue = 22
-    setInputStringValue = 23
+    setDataFile = 2
+    init = 3
+    getInitStatus = 4
+    terminate = 5
+    presentTime = 6
+    computeTimeStep = 7
+    initTimeStep = 8
+    solve = 9
+    getSolveStatus = 10
+    validateTimeStep = 11
+    setStationaryMode = 12
+    getStationaryMode = 13
+    abortTimeStep = 14
+    isStationary = 15
+    resetTime = 16
+    iterate = 17
+    getIterateStatus = 18
+    save = 19
+    restore = 20
+    forget = 21
+    setInputDoubleValue = 22
+    setInputIntValue = 23
+    setInputStringValue = 24
+    getInputValuesNames = 25
+    getOutputValuesNames = 26
+    getValueType = 27
+    getValueUnit = 28
+    getOutputDoubleValue = 29
+    getOutputIntValue = 30
+    getOutputStringValue = 31
 
     tagBARRIER = 100
 
     deleteDataManager = 101
     cloneEmptyData = 102
     copyData = 103
     normMax = 104
```

### Comparing `salome-c3po-2.1.1/c3po/mpi/MPIWorker.py` & `salome-c3po-2.2/sources/c3po/mpi/MPIWorker.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,15 +83,17 @@
                 tag = data[0]
                 data = data[-1]
             else:
                 data = self.mpiComm.recv(source=self._masterRank, tag=MPI.ANY_TAG, status=status)
                 tag = status.Get_tag()
             # print "rank ", self.mpiComm.Get_rank(), ", tag = ", tag, "*****************************************************************"
             if tag < MPITag.tagBARRIER:
-                if tag == MPITag.init:
+                if tag == MPITag.setDataFile:
+                    self._physicsDriver.setDataFile(data)
+                elif tag == MPITag.init:
                     self._physicsDriver.init()
                 elif tag == MPITag.getInitStatus:
                     self.answer(self._physicsDriver.getInitStatus())
                 elif tag == MPITag.presentTime:
                     self.answer(self._physicsDriver.presentTime())
                 elif tag == MPITag.computeTimeStep:
                     (dt, stop) = self._physicsDriver.computeTimeStep()
@@ -130,14 +132,28 @@
                     self._physicsDriver.forget(*data)
                 elif tag == MPITag.setInputDoubleValue:
                     self._physicsDriver.setInputDoubleValue(*data)
                 elif tag == MPITag.setInputIntValue:
                     self._physicsDriver.setInputIntValue(*data)
                 elif tag == MPITag.setInputStringValue:
                     self._physicsDriver.setInputStringValue(*data)
+                elif tag == MPITag.getInputValuesNames:
+                    self.answer(self._physicsDriver.getInputValuesNames(), collectiveOperator=MPI.MAX)
+                elif tag == MPITag.getOutputValuesNames:
+                    self.answer(self._physicsDriver.getOutputValuesNames(), collectiveOperator=MPI.MAX)
+                elif tag == MPITag.getValueType:
+                    self.answer(self._physicsDriver.getValueType(data), collectiveOperator=MPI.MAX)
+                elif tag == MPITag.getValueUnit:
+                    self.answer(self._physicsDriver.getValueUnit(data), collectiveOperator=MPI.MAX)
+                elif tag == MPITag.getOutputDoubleValue:
+                    self.answer(self._physicsDriver.getOutputDoubleValue(data), collectiveOperator=MPI.MAX)
+                elif tag == MPITag.getOutputIntValue:
+                    self.answer(self._physicsDriver.getOutputIntValue(data), collectiveOperator=MPI.MAX)
+                elif tag == MPITag.getOutputStringValue:
+                    self.answer(self._physicsDriver.getOutputStringValue(data), collectiveOperator=MPI.MAX)
             else:
                 if tag == MPITag.deleteDataManager:
                     self.checkDataID(data)
                     self._idDataFree += data
                 elif tag == MPITag.cloneEmptyData:
                     idNewDataMan = self.getIdNewData()
                     self._dataManagers[idNewDataMan] = self._dataManagers[data].cloneEmpty()
```

### Comparing `salome-c3po-2.1.1/c3po/mpi/__init__.py` & `salome-c3po-2.2/sources/c3po/mpi/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,24 @@
 # 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # 3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """ Import user MPI C3PO objects. """
 
+from .MPIRemote import MPIRemote
 from .MPIRemoteProcess import MPIRemoteProcess
+from .MPIRemoteProcesses import MPIRemoteProcesses
 from .MPICollectiveProcess import MPICollectiveProcess
 from .MPICollectiveDataManager import MPICollectiveDataManager
 from .MPICollaborativeDataManager import MPICollaborativeDataManager
+from .MPIDomainDecompositionDataManager import MPIDomainDecompositionDataManager
 from .MPICollaborativePhysicsDriver import MPICollaborativePhysicsDriver
 from .MPIExchanger import MPIExchanger
 from .MPICoupler import MPICoupler
 from .MPIMasterPhysicsDriver import MPIMasterPhysicsDriver
 from .MPIMasterDataManager import MPIMasterDataManager
 from .MPIMasterExchanger import MPIMasterExchanger
 from .MPIWorker import MPIWorker
+from .mpiExchangeMethods.MPIExchangeMethod import MPIExchangeMethod
+from .mpiExchangeMethods.MPISharedRemapping import MPISharedRemapping, MPIRemapper
+from .mpiExchangeMethods.MPISharedRemappingMulti1D3D import MPISharedRemappingMulti1D3D, MPIMulti1D3DRemapper
```

### Comparing `salome-c3po-2.1.1/c3po/physicsDrivers/ALCYONE2Driver.py` & `salome-c3po-2.2/sources/c3po/physicsDrivers/ALCYONE2Driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # 3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """ Contain the class ALCYONE2Driver. """
 from __future__ import print_function, division
-from ctypes import cdll
 import mpi4py.MPI as mpi
 
 import pleiades
 import pleiadesMPI
 
 from Alcyone2Init import Alcyone2Init
 
@@ -26,15 +25,15 @@
     """! This is the implementation of PhysicsDriver for Alcyone2.
 
     A Alcyone2Init method must be available. It has the internal Alcyone2 object as input.
     """
 
     def __init__(self):
         PhysicsDriver.__init__(self)
-        cdll.LoadLibrary("libALCYONE.so")
+        pleiades.loadLibrary("libALCYONE.so")
         self._alcyone2 = pleiades.createComponent("AlcyoneComponent")
         pleiadesMPI.PleiadesMPIExternalSetting.getInstance().setMPIComm(mpi.COMM_SELF)
         self._dtFactor = 1.
         self._timeShift = 0.
         self._stationaryMode = False
 
     def getMEDCouplingMajorVersion(self):
@@ -46,14 +45,15 @@
     def setMPIComm(self, mpicomm):
         pleiadesMPI.PleiadesMPIExternalSetting.getInstance().setMPIComm(mpicomm)
 
     def initialize(self):
         Alcyone2Init(self._alcyone2)
         self._alcyone2.initialize()
         pleiades.setVerboseLevel(3)
+        return True
 
     def terminate(self):
         self._alcyone2.terminate()
 
     def presentTime(self):
         return self._alcyone2.presentTime() - self._timeShift
 
@@ -113,14 +113,17 @@
         fieldNames = self._alcyone2.getOutputMEDField()
         fieldNames += ["Temperature_FUEL_Rowland"]
         return fieldNames
 
     def getInputMEDDoubleFieldTemplate(self, name):
         return self._alcyone2.getOutputMEDField("Temperature_SCE")
 
+    def getInputMEDIntFieldTemplate(self, name):
+        return self.getInputMEDDoubleFieldTemplate(name)
+
     def setInputMEDDoubleField(self, name, field):
         if name == "LinearPower":
             arrayZ = field.getMesh().getCoordsAt(0)
             arrayDz = mc.DataArrayDouble()
             arrayDz.alloc(arrayZ.getNbOfElems() - 1)
             for i in range(arrayZ.getNbOfElems() - 1):
                 arrayDz.setIJ(i, 0, arrayZ.getIJ(i + 1, 0) - arrayZ.getIJ(i, 0))
@@ -135,7 +138,15 @@
             field *= 4. / 9.
             field2 *= 5. / 9.
             field.getArray().addEqual(field2.getArray())
         else:
             field = self._alcyone2.getOutputMEDField(name)
         field.setNature(mc.IntensiveMaximum)
         return field
+
+    def setInputIntValue(self, name, value):
+        if name == "RampPhase":
+            field = self.getInputMEDIntFieldTemplate(name)
+            field.applyLin(0., value)
+            self._alcyone2.setInputField(name, field)
+        else:
+            raise NotImplementedError
```

### Comparing `salome-c3po-2.1.1/c3po/physicsDrivers/APOLLO3Driver.py` & `salome-c3po-2.2/sources/c3po/physicsDrivers/APOLLO3Driver.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/physicsDrivers/CATHARE3Driver.py` & `salome-c3po-2.2/sources/c3po/physicsDrivers/CATHARE3Driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,22 @@
 
 """ Contain the class CATHARE3Driver. """
 from __future__ import print_function, division
 
 import c3po.medcouplingCompat as mc
 try:
     #import Cathare_opt
-    import Cathare_opt.Problem_Cathare as C3
+    from Cathare_opt import Problem_Cathare as C3
 except ImportError:
-    # importation dans Corpus
-    from CATHARE3SWIG import CATHARE3 as C3
+    try:
+        #import Cathare_opt
+        import Cathare_opt.Problem_Cathare as C3
+    except ImportError:
+        # importation dans Corpus
+        from CATHARE3SWIG import CATHARE3 as C3
 from c3po.PhysicsDriver import PhysicsDriver
 
 
 def shortName(name):
     """! INTERNAL """
     return name.split("__")[1] if (name.startswith("reconstruction") or name.startswith("sommewall__")) else name
```

### Comparing `salome-c3po-2.1.1/c3po/physicsDrivers/CRONOS2Driver.py` & `salome-c3po-2.2/sources/c3po/physicsDrivers/CRONOS2Driver.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/physicsDrivers/FLICA4Driver.py` & `salome-c3po-2.2/sources/c3po/physicsDrivers/FLICA4Driver.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/physicsDrivers/THEDIDriver.py` & `salome-c3po-2.2/sources/c3po/physicsDrivers/THEDIDriver.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/physicsDrivers/TRUSTDriver.py` & `salome-c3po-2.2/sources/c3po/physicsDrivers/TRUSTDriver.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/physicsDrivers/__init__.py` & `salome-c3po-2.2/sources/c3po/couplers/__init__.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/services/ListingWriter.py` & `salome-c3po-2.2/sources/c3po/services/ListingWriter.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/services/NameChanger.py` & `salome-c3po-2.2/sources/c3po/services/NameChanger.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """ Contain the class wrapper nameChanger. """
 from __future__ import print_function, division
 from types import FunctionType
 
 from c3po.PhysicsDriver import PhysicsDriver
+from c3po.services.Printer import warning
 
 
 class NameChanger(PhysicsDriver):
     """! NameChanger wraps a PhysicsDriver object and changes the names of the values and fields quantities that can be get/set through ICoCo methods.
 
     This allows to improve the genericity of coupling scripts by using generic variable names without modifying the PhysicsDriver "by hand".
     """
@@ -33,31 +34,56 @@
             nameChanger will substitute only the preceding part. For example : c3po.NameChanger(nameMappingValue={"newName*" : "oldName*"}, wildcard="*") will substitute
             newNameA05 in oldNameA05 and newNameB9 in oldNameB9.
 
         @note nameMappingValue and nameMappingField are copied.
         """
         PhysicsDriver.__init__(self)
         self._physics = physics
-        self._nameMappingValue = nameMappingValue.copy()
-        self._nameMappingField = nameMappingField.copy()
+        self._nameMappingValue = {}
+        self._nameMappingField = {}
+        self._invertNameMappingValue = {}
+        self._invertNameMappingField = {}
+        self.updateNameMappingValue(nameMappingValue)
+        self.updateNameMappingField(nameMappingField)
+        self._wildcard = wildcard
+        self._value = 0
+        self._field = 1
+
+    def updateNameMappingValue(self, nameMappingValue):
+        """! Update (with the update() method of dict) the dictionary nameMappingValue previously provided.
+
+        @param nameMappingValue the Python dictionary used for the update.
+        """
+        self._nameMappingValue.update(nameMappingValue)
         self._invertNameMappingValue = {}
         for key, val in self._nameMappingValue.items():
             if val not in self._invertNameMappingValue:
                 self._invertNameMappingValue[val] = [key]
             else:
                 self._invertNameMappingValue[val].append(key)
+
+    def updateNameMappingField(self, nameMappingField):
+        """! Update (with the update() method of dict) the dictionary nameMappingField previously provided.
+
+        @param nameMappingField the Python dictionary used for the update.
+        """
+        self._nameMappingField.update(nameMappingField)
         self._invertNameMappingField = {}
         for key, val in self._nameMappingField.items():
             if val not in self._invertNameMappingField:
                 self._invertNameMappingField[val] = [key]
             else:
                 self._invertNameMappingField[val].append(key)
-        self._wildcard = wildcard
-        self._value = 0
-        self._field = 1
+
+    def getPhysicsDriver(self):
+        """! Return the wrapped PhysicsDriver.
+
+        @return the wrapped PhysicsDriver.
+        """
+        return self._physics
 
     def _getNewName(self, name, variableType, inverse):
         """! Return the change name(s).
 
         @param name (string) previous name.
         @param variableType put 0 (self._value) if name is the name of a value, 1 (self._field) if it is the name of a field.
         @param inverse True to inverse research (old -> new), False to direct (new -> old).
@@ -131,14 +157,18 @@
         """! See PhysicsDriver.initTimeStep(). """
         return self._physics.initTimeStep(dt)
 
     def solveTimeStep(self):
         """! See PhysicsDriver.solveTimeStep(). """
         return self._physics.solveTimeStep()
 
+    def iterateTimeStep(self):
+        """! See PhysicsDriver.iterateTimeStep(). """
+        return self._physics.iterateTimeStep()
+
     def validateTimeStep(self):
         """! See PhysicsDriver.validateTimeStep(). """
         self._physics.validateTimeStep()
 
     def setStationaryMode(self, stationaryMode):
         """! See PhysicsDriver.setStationaryMode(). """
         self._physics.setStationaryMode(stationaryMode)
@@ -155,14 +185,26 @@
         """! See PhysicsDriver.isStationary(). """
         return self._physics.isStationary()
 
     def resetTime(self, time_):
         """! See PhysicsDriver.resetTime(). """
         self._physics.resetTime(time_)
 
+    def save(self, label, method):
+        """! See PhysicsDriver.save(). """
+        self._physics.save(label, method)
+
+    def restore(self, label, method):
+        """! See PhysicsDriver.restore(). """
+        self._physics.restore(label, method)
+
+    def forget(self, label, method):
+        """! See PhysicsDriver.forget(). """
+        self._physics.forget(label, method)
+
     def getInputFieldsNames(self):
         """! See c3po.DataAccessor.DataAccessor.getInputFieldsNames(). """
         names = self._physics.getInputFieldsNames()
         newNames = []
         for name in names:
             newNames += self._getNewName(name, variableType=self._field, inverse=True)
         for name in names:
@@ -385,16 +427,16 @@
             Otherwise it will result in TypeError when the daughter class will try to call mother methods (since its mother class does
             not exist anymore!). As a consequence, if nameChanger is to be applied to C3PO classes, it is recommended to change their name
             "(MyNewClass = c3po.nameChanger(...)(MyClass)").
 
     @throw Exception if applied to a class already modified by nameChanger, because it could result in an unexpected behavior.
     """
 
-    print("The class wrapper nameChanger is deprecated and will soon by deleted.\n"
-          + "Please use the class NameChanger (acting on a PhysicsDriver object rather than a class).")
+    warning("The class wrapper nameChanger is deprecated and will soon by deleted. "
+            + "Please use the class NameChanger (acting on a PhysicsDriver object rather than a class).")
 
     def classWrapper(baseclass):
         if hasattr(baseclass, "static_nameMapping"):
             raise Exception("nameChanger: the class " + baseclass.__name__ + " has already been modified by nameChanger. This is not allowed.")
         baseclass.static_nameMapping = nameMapping
         baseclass.static_wildcard = wildcard
         newclass = NameChangerMeta(baseclass.__name__, baseclass.__bases__, baseclass.__dict__)
```

### Comparing `salome-c3po-2.1.1/c3po/services/__init__.py` & `salome-c3po-2.2/sources/c3po/services/__init__.py`

 * *Files identical despite different names*

### Comparing `salome-c3po-2.1.1/c3po/services/tracer.py` & `salome-c3po-2.2/sources/c3po/services/tracer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,28 @@
 # 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # 3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """ Contain the class wrapper tracer. """
 from __future__ import print_function, division
+import re
 from types import FunctionType
 import time
 import sys
 import os
 
 import c3po.medcouplingCompat as mc
 
 
+def getRegularName(name):
+    """! INTERNAL """
+    return re.sub("[^a-zA-Z0-9_]", "_", "_" + name)
+
+
 def getNameFieldInput(name, field):
     """! INTERNAL """
     return (name, field)
 
 
 def getNameInput(name):
     """! INTERNAL """
@@ -108,18 +114,18 @@
                         stringArgs = getArgsString(*args, **kwargs)
                         toWritePython = self.tracerObjectName + " = " + name + stringArgs + "\n"
                     elif method.__name__.startswith("setInputMED"):
                         (nameField, _) = getNameFieldInput(*args, **kwargs)
                         toWritePython = self.tracerObjectName + "." + method.__name__ + "('" + nameField + "', readField)" + "\n"
                     elif method.__name__.startswith("getOutputMED"):
                         nameField = getNameInput(*args, **kwargs)
-                        toWritePython = nameField + "_" + self.tracerObjectName + " = " + self.tracerObjectName + "." + method.__name__ + "('" + nameField + "')" + "\n"
+                        toWritePython = getRegularName(nameField) + "_" + self.tracerObjectName + " = " + self.tracerObjectName + "." + method.__name__ + "('" + nameField + "')" + "\n"
                     elif method.__name__.startswith("updateOutputMED"):
                         (nameField, _) = getNameFieldInput(*args, **kwargs)
-                        toWritePython = self.tracerObjectName + "." + method.__name__ + "('" + nameField + "', " + nameField + "_" + self.tracerObjectName + ")" + "\n"
+                        toWritePython = self.tracerObjectName + "." + method.__name__ + "('" + nameField + "', " + getRegularName(nameField) + "_" + self.tracerObjectName + ")" + "\n"
                     else:
                         stringArgs = getArgsString(*args, **kwargs)
                         toWritePython = self.tracerObjectName + "." + method.__name__ + stringArgs + "\n"
 
                 prevIdstdout = 0
                 prevIdstderr = 0
                 if self.static_stdout is not None:
```

### Comparing `salome-c3po-2.1.1/setup.py` & `salome-c3po-2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 import os
 from setuptools import find_packages, setup
 
 
 def get_version():
     """Extract the package's version number from the ``VERSION`` file."""
-#    filename = os.path.join(os.path.dirname(__file__), "sources", "c3po", "VERSION")
-    filename = os.path.join(os.path.dirname(__file__), "c3po", "VERSION")
+    filename = os.path.join(os.path.dirname(__file__), "sources", "c3po", "VERSION")
     with open(filename) as file:
         return file.read().strip()
 
 
 def check_dependencies(requirements):
     """Check if the dependencies of the package are available in the current
     environment and print a warning message if not.
@@ -64,24 +63,24 @@
     version=get_version(),
     author="CEA",
     author_email="cyril.patricot@cea.fr",
     maintainer="Cyril Patricot",
     maintainer_email="cyril.patricot@cea.fr",
     description="Collaborative Code Coupling PlatfOrm",
     url="https://sourceforge.net/projects/cea-c3po/",
-    packages=find_packages(),
+    packages=find_packages(where="sources"),
     package_data={
         "c3po": [
             "VERSION",
         ],
     },
-    #    package_dir={"": "sources"},
+    package_dir={"": "sources"},
     install_requires=check_dependencies([
         "numpy>=1.9",
         "mpi4py>=1.3",
     ]),
     extras_require={
-        "pytest": ["pytest", "pytest-cov", "pytest-easyMPI", "pytest-html"],
+        "pytest": ["pytest", "pytest-cov", "pytest-html"],
     },
     python_requires=">=2.7, !=3.0.*, !=3.1.*",
     licence="3-Clause BSD"
 )
```

