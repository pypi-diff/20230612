# Comparing `tmp/octoploy-1.2.0.tar.gz` & `tmp/octoploy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoploy-1.2.0.tar", last modified: Tue Jun  6 07:49:27 2023, max compression
+gzip compressed data, was "octoploy-1.2.1.tar", last modified: Mon Jun 12 13:17:16 2023, max compression
```

## Comparing `octoploy-1.2.0.tar` & `octoploy-1.2.1.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 07:49:14.000000 octoploy-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-06 07:49:27.558266 octoploy-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-06-06 07:49:14.000000 octoploy-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/api/Model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/api/Oc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/backup/BackupGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/backup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/AppConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/BaseConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/DeploymentActionConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/DynamicConfigMap.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/YmlConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/deploy/AppDeploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/deploy/DeploymentBundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/deploy/K8sObjectDeployer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/deploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/k8s/BaseObj.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/k8s/SecretObj.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/octoploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy/processing/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/DataPreProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/DecryptionProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/K8sObjectMerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/TreeWalker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/ValueLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/YmlTemplateProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/octoploy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/state/StateTracking.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/octoploy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/Cert.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/DictUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/Encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/Log.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/Yml.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/YmlWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/octoploy/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.554266 octoploy-1.2.0/octoploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-06 07:49:27.000000 octoploy-1.2.0/octoploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-06 07:49:27.000000 octoploy-1.2.0/octoploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:49:27.000000 octoploy-1.2.0/octoploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 07:49:27.000000 octoploy-1.2.0/octoploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-06 07:49:27.000000 octoploy-1.2.0/octoploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-06 07:49:27.000000 octoploy-1.2.0/octoploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 07:49:27.558266 octoploy-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-06 07:49:14.000000 octoploy-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/AppDeploymentTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/DictUtilsTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/OcObjectMergeTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/StateTrackingTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/TestUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/YmlTempalteProcessorTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/config/AppConfigTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/tests/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/processing/ValueLoaderTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:27.558266 octoploy-1.2.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/utils/EncryptionTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/utils/YmlWriterTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:49:14.000000 octoploy-1.2.0/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.505139 octoploy-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 13:17:04.000000 octoploy-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-12 13:17:16.505139 octoploy-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-06-12 13:17:04.000000 octoploy-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.497139 octoploy-1.2.1/octoploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.497139 octoploy-1.2.1/octoploy/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/api/Model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/api/Oc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.497139 octoploy-1.2.1/octoploy/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/backup/BackupGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/backup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.501139 octoploy-1.2.1/octoploy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/AppConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/BaseConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/DeploymentActionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/DynamicConfigMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/YmlConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.501139 octoploy-1.2.1/octoploy/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/deploy/AppDeploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/deploy/DeploymentBundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/deploy/K8sObjectDeployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/deploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.501139 octoploy-1.2.1/octoploy/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/k8s/BaseObj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/k8s/SecretObj.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/octoploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.501139 octoploy-1.2.1/octoploy/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/DataPreProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/DecryptionProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/K8sObjectMerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/NamespaceProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/TreeWalker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/ValueLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/YmlTemplateProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.501139 octoploy-1.2.1/octoploy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/state/StateTracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.501139 octoploy-1.2.1/octoploy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/Cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/DictUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/Encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/Yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/YmlWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.497139 octoploy-1.2.1/octoploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-12 13:17:16.000000 octoploy-1.2.1/octoploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-12 13:17:16.000000 octoploy-1.2.1/octoploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:17:16.000000 octoploy-1.2.1/octoploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 13:17:16.000000 octoploy-1.2.1/octoploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 13:17:16.000000 octoploy-1.2.1/octoploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 13:17:16.000000 octoploy-1.2.1/octoploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 13:17:16.505139 octoploy-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-12 13:17:04.000000 octoploy-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.505139 octoploy-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/AppDeploymentTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/DictUtilsTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/OcObjectMergeTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/StateTrackingTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/TestUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/YmlTempalteProcessorTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.505139 octoploy-1.2.1/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/config/AppConfigTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.505139 octoploy-1.2.1/tests/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/processing/ValueLoaderTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.505139 octoploy-1.2.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/utils/EncryptionTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/utils/YmlWriterTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/utils/__init__.py
```

### Comparing `octoploy-1.2.0/LICENSE` & `octoploy-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/PKG-INFO` & `octoploy-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoploy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Simple kubernetes / openshift templating engine with templating, libraries, state tracking
 Home-page: https://github.com/davidgiga1993/octoploy
 Author: davidgiga1993
 Author-email: david@dev-core.org
 License: UNKNOWN
 Description: # Kubernetes / openshift templating and deployment engine
```

### Comparing `octoploy-1.2.0/README.md` & `octoploy-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/api/Model.py` & `octoploy-1.2.1/octoploy/api/Model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import Dict, Optional
 
+from octoploy.k8s.BaseObj import BaseObj
 from octoploy.utils.DictUtils import DictUtils
 
 
 class NamedItem:
     def __init__(self, data):
         self.data = data
 
@@ -34,17 +35,17 @@
         Name of the associated deployment config
         """
 
     def set_labels(self, labels):
         self.deployment_config = labels.get('deploymentconfig')
 
 
-class DeploymentConfig:
-    def __init__(self, data):
-        self.data = data
+class DeploymentConfig(BaseObj):
+    def __init__(self, data: BaseObj):
+        super().__init__(data.data)
 
     def get_template(self) -> Optional[dict]:
         """
         Returns the template object
         """
         return DictUtils.get(self.data, 'spec.template')
 
@@ -61,16 +62,16 @@
         """
         return DictUtils.get(self.get_template(), 'metadata.labels.name')
 
     def get_containers(self) -> Dict[str, DeploymentConfigContainer]:
         items = self.get_template_spec().get('containers', [])
         out = {}
         for data in items:
-            volume = DeploymentConfigContainer(data)
-            out[volume.get_name()] = volume
+            container = DeploymentConfigContainer(data)
+            out[container.get_name()] = container
         return out
 
     def get_volumes(self) -> Dict[str, DeploymentConfigVolume]:
         items = self.get_template_spec().get('volumes', [])
         out = {}
         for data in items:
             volume = DeploymentConfigVolume(data)
```

### Comparing `octoploy-1.2.0/octoploy/api/Oc.py` & `octoploy-1.2.1/octoploy/api/Oc.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/backup/BackupGenerator.py` & `octoploy-1.2.1/octoploy/backup/BackupGenerator.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/config/AppConfig.py` & `octoploy-1.2.1/octoploy/config/AppConfig.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/config/BaseConfig.py` & `octoploy-1.2.1/octoploy/config/BaseConfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,21 +28,14 @@
         Returns the path to a file inside the dir of the app/project
         :param path: Relative path
         :return: Path
         """
         base = os.path.dirname(os.path.abspath(self._path))
         return os.path.abspath(os.path.join(base, path))
 
-    def get_yml_processors(self) -> List[TreeProcessor]:
-        """
-        Returns all yml processors which should be applied
-        :return: Processors
-        """
-        return [DecryptionProcessor()]
-
     def get_template_processor(self) -> YmlTemplateProcessor:
         return YmlTemplateProcessor(self)
 
     def get_replacements(self) -> Dict[str, any]:
         """
         Returns all variables which are available for the yml files
```

### Comparing `octoploy-1.2.0/octoploy/config/Config.py` & `octoploy-1.2.1/octoploy/config/Config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import os
 from typing import Optional, Dict, List
 
 from octoploy.api.Oc import Oc, K8, K8sApi
 from octoploy.config.AppConfig import AppConfig
 from octoploy.config.BaseConfig import BaseConfig
 from octoploy.processing.DataPreProcessor import DataPreProcessor, OcToK8PreProcessor
+from octoploy.processing.DecryptionProcessor import DecryptionProcessor
+from octoploy.processing.NamespaceProcessor import NamespaceProcessor
+from octoploy.processing.TreeWalker import TreeProcessor
 from octoploy.processing.YmlTemplateProcessor import YmlTemplateProcessor
 from octoploy.state.StateTracking import StateTracking
 from octoploy.utils.Errors import ConfigError
 
 
 class RunMode:
     def __init__(self):
@@ -77,23 +80,14 @@
 
     def is_library(self) -> bool:
         """
         Indicates if this collection is a library
         """
         return self.data.get('type', '') == 'library'
 
-    def get_pre_processor(self) -> DataPreProcessor:
-        """
-        Returns the pre processor for the current config
-        """
-        mode = self._get_mode()
-        if mode == 'k8s' or mode == 'k8s':
-            return OcToK8PreProcessor()
-        return DataPreProcessor()
-
     def _get_mode(self) -> str:
         return self.data.get('mode', 'k8s')
 
     def create_api(self) -> K8sApi:
         """
         Creates a new openshift / k8s client
         :return: Client
@@ -122,14 +116,23 @@
     def get_kubectl_context(self) -> Optional[str]:
         """
         Returns the configuration context name
         :return: Name or null if the current context should be used
         """
         return self.data.get('context')
 
+    def get_pre_processor(self) -> DataPreProcessor:
+        """
+        Returns the pre processor for the current config
+        """
+        mode = self._get_mode()
+        if mode == 'k8s' or mode == 'k8s':
+            return OcToK8PreProcessor()
+        return DataPreProcessor()
+
     def get_template_processor(self) -> YmlTemplateProcessor:
         root_processor = super().get_template_processor()
         if self._library is not None:
             processor = self._library.get_template_processor()
             root_processor.parent(processor)
         return root_processor
 
@@ -143,14 +146,21 @@
         if name is not None:
             items.update({
                 'OC_PROJECT': name,
                 'NAMESPACE': name
             })
         return items
 
+    def get_yml_processors(self) -> List[TreeProcessor]:
+        """
+        Returns all yml processors which should be applied
+        :return: Processors
+        """
+        return [DecryptionProcessor(), NamespaceProcessor(self)]
+
     def load_app_configs(self) -> List[AppConfig]:
         """
         Loads all app configurations available in this project
         :return:
         """
         items = []
         names = set()
```

### Comparing `octoploy-1.2.0/octoploy/config/DeploymentActionConfig.py` & `octoploy-1.2.1/octoploy/config/DeploymentActionConfig.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/config/DynamicConfigMap.py` & `octoploy-1.2.1/octoploy/config/DynamicConfigMap.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/deploy/AppDeploy.py` & `octoploy-1.2.1/octoploy/deploy/AppDeploy.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,21 +87,27 @@
         self._apply_templates(self._app_config.get_pre_template_refs(), template_processor)
         self._load_files(self._app_config.get_config_root(), template_processor)
         self._load_extra_configmaps(template_processor)
         self._apply_templates(self._app_config.get_post_template_refs(), template_processor)
 
         # Additional processing
         tree_processors = self._root_config.get_yml_processors()
+        skipped_objects = []
         for processor in tree_processors:
-            for data in list(self._bundle.objects):
+            for k8s_object in self._bundle.objects:
                 try:
-                    processor.process(data)
+                    processor.process(k8s_object)
                 except SkipObject as e:
                     self.log.warning(f'Skipping object: {e}')
-                    self._bundle.objects.remove(data)
+                    skipped_objects.append(k8s_object)
+
+        for k8s_object in skipped_objects:
+            # Mark in state as "visited" so the object doesn't get deleted on k8s side
+            self._root_config.get_state().visit(self._app_config.get_name(), k8s_object, k8s_object.get_hash())
+            self._bundle.objects.remove(k8s_object)
 
         api = self._root_config.create_api()
         if self._mode.out_file is not None:
             self._bundle.dump_objects(self._mode.out_file)
 
         if self._mode.dry_run:
             return
```

### Comparing `octoploy-1.2.0/octoploy/deploy/DeploymentBundle.py` & `octoploy-1.2.1/octoploy/deploy/DeploymentBundle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from __future__ import annotations
 
-import base64
 import os
-from typing import List, Dict
+from typing import List
 
 import yaml
 
 from octoploy.deploy.K8sObjectDeployer import K8sObjectDeployer
 from octoploy.k8s.BaseObj import BaseObj
 from octoploy.processing.DataPreProcessor import DataPreProcessor
-from octoploy.processing.DecryptionProcessor import DecryptionProcessor
 from octoploy.processing.K8sObjectMerge import K8sObjectMerge
 from octoploy.processing.YmlTemplateProcessor import YmlTemplateProcessor
 from octoploy.utils.Log import Log
 from octoploy.utils.YmlWriter import YmlWriter
 
 
 class DeploymentBundle(Log):
     """
     Holds all objects of a single deployment (aka everything inside one folder)
     """
-    objects: List[Dict[str, any]]
+    objects: List[BaseObj]
 
     def __init__(self, pre_processor: DataPreProcessor):
         super().__init__()
         self.objects = []  # All objects which should be deployed
         self._pre_processor = pre_processor
 
     def add_object(self, data: dict, template_processor: YmlTemplateProcessor):
@@ -36,40 +34,37 @@
         k8s_object = BaseObj(data)
         if k8s_object.kind is None:
             self.log.info('Unknown object kind: ' + str(data))
             return
 
         # Pre-process any variables
         if template_processor is not None:
-            template_processor.process(data)
+            template_processor.process(k8s_object)
 
         merger = K8sObjectMerge()
         # Check if the new data can be merged into any existing objects
         for item in self.objects:
-            if merger.merge(item, data):
+            if merger.merge(item, k8s_object):
                 # Data has been merged
                 return
 
         self._pre_processor.process(data)
-        self.objects.append(data)
+        self.objects.append(k8s_object)
 
     def deploy(self, deploy_runner: K8sObjectDeployer):
         """
         Deploys all objects in this bundle
         :param deploy_runner: Deployment runner which should be used
         """
         deploy_runner.select_context()
 
         # First sort the objects, we want "deployments" to be the last object type
         # so all prerequisites are available
-        def sorting(x):
-            k8s_object = BaseObj(x)
-            object_kind = k8s_object.kind.lower()
-            if object_kind == 'DeploymentConfig'.lower() or \
-                    object_kind == 'Deployment'.lower():
+        def sorting(x: BaseObj):
+            if x.is_kind('DeploymentConfig') or x.is_kind('Deployment'):
                 return 1
             return 0
 
         self.objects.sort(key=sorting)
         for item in self.objects:
             deploy_runner.deploy_object(item)
 
@@ -84,10 +79,10 @@
         all_objects = []
         if os.path.isfile(path):
             with open(path) as f:
                 data = yaml.load_all(f, Loader=yaml.FullLoader)
                 for doc in data:
                     all_objects.append(doc)
 
-        all_objects.extend(self.objects)
+        all_objects.extend([x.data for x in self.objects])
         with open(path, 'w') as file:
             YmlWriter.dump_all(all_objects, file)
```

### Comparing `octoploy-1.2.0/octoploy/deploy/K8sObjectDeployer.py` & `octoploy-1.2.1/octoploy/deploy/K8sObjectDeployer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import hashlib
-
 from octoploy.api.Oc import K8sApi
 from octoploy.config.Config import RootConfig, AppConfig, RunMode
 from octoploy.k8s.BaseObj import BaseObj
 from octoploy.state.StateTracking import StateTracking
 from octoploy.utils.Log import Log
-from octoploy.utils.YmlWriter import YmlWriter
 
 
 class K8sObjectDeployer(Log):
     """
     Deploys k9s object
     """
 
@@ -34,34 +31,26 @@
         """
         Selects the cluster context
         """
         context = self._root_config.get_kubectl_context()
         if context is not None:
             self._api.switch_context(context)
 
-    def deploy_object(self, data: dict):
+    def deploy_object(self, k8s_object: BaseObj):
         """
         Deploy the given object (if a deployment required, otherwise does nothing)
-        :param data: Data which should be deployed
+        :param k8s_object: Object which should be deployed
         """
-        # Sort the content so it's always reproducible
-        str_repr = YmlWriter.dump(data)
-        hash_val = hashlib.md5(str_repr.encode('utf-8')).hexdigest()
-
-        k8s_object = BaseObj(data)
-        # An object might be in a different namespace than the current context
+        hash_val = k8s_object.get_hash()
+        item_path = k8s_object.get_fqn()
         namespace = k8s_object.namespace
-        if namespace is None:
-            namespace = self._root_config.get_namespace_name()
-        k8s_object.namespace = namespace  # Make sure the object points to the correct namespace
 
-        item_path = k8s_object.get_fqn()
         current_object = self._api.get(item_path, namespace=namespace)
         if current_object is None:
-            self.log.info(f'{item_path} will be created')
+            self._log_create(item_path)
 
         current_hash = None
         if current_object is not None:
             obj_state = self._state.get_state(self._app_config.get_name(), k8s_object)
             if obj_state is not None and obj_state.hash != '':
                 current_hash = obj_state.hash
             else:  # Fallback to old hash location
@@ -75,21 +64,21 @@
 
         if current_hash == hash_val:
             self._state.visit(self._app_config.get_name(), k8s_object, hash_val)
             self.log.debug(f"{item_path} hasn't changed")
             return
 
         if current_object is not None:
-            self.log.info(f'{item_path} will be updated')
+            self._log_update(item_path)
 
         if self._mode.plan:
             self._state.visit(self._app_config.get_name(), k8s_object, hash_val)
             return
 
-        self._api.apply(str_repr, namespace=namespace)
+        self._api.apply(k8s_object.as_string(), namespace=namespace)
         self._state.visit(self._app_config.get_name(), k8s_object, hash_val)
 
         if k8s_object.is_kind('ConfigMap'):
             self._reload_config()
 
     def delete_abandoned_objects(self):
         """
@@ -98,21 +87,36 @@
         """
         abandoned = self._state.get_not_visited(self._app_config.get_name())
         for item in abandoned:
             namespace = item.namespace
             if namespace is None:
                 namespace = self._root_config.get_namespace_name()
             item_path = item.kind + '/' + item.name
-            self.log.info(f'{item_path} will be deleted')
+            self._log_delete(item_path)
             if self._mode.plan:
                 continue
 
             self._api.delete(item_path, namespace=namespace)
             self._state.remove(item)
 
     def _reload_config(self):
         """
         Tries to reload the configuration for the app
         """
         reload_actions = self._app_config.get_reload_actions()
         for action in reload_actions:
             action.run(self._api)
+
+    def _log_create(self, item_path: str):
+        self._log_verb(item_path, 'created', 'creating')
+
+    def _log_delete(self, item_path: str):
+        self._log_verb(item_path, 'deleted', 'deleting')
+
+    def _log_update(self, item_path: str):
+        self._log_verb(item_path, 'updated', 'updating')
+
+    def _log_verb(self, item_path: str, past_verb: str, progressive_verb: str):
+        if self._mode.plan or self._mode.dry_run:
+            self.log.info(f'{item_path} will be {past_verb}')
+            return
+        self.log.info(f'{progressive_verb} {item_path}')
```

### Comparing `octoploy-1.2.0/octoploy/octoploy.py` & `octoploy-1.2.1/octoploy/octoploy.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/processing/DataPreProcessor.py` & `octoploy-1.2.1/octoploy/processing/DataPreProcessor.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/processing/DecryptionProcessor.py` & `octoploy-1.2.1/octoploy/processing/DecryptionProcessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Dict, Optional
 
+from octoploy.k8s.BaseObj import BaseObj
+
 from octoploy.k8s.SecretObj import SecretObj
 from octoploy.processing.TreeWalker import TreeProcessor, TreeWalker
 from octoploy.utils import Utils
 from octoploy.utils.Encryption import Encryption
 from octoploy.utils.Errors import SkipObject
 from octoploy.utils.Log import Log
 
@@ -26,22 +28,22 @@
 
     _secret_obj: Optional[SecretObj]
 
     def __init__(self):
         super().__init__(__name__)
         self.encryption = Encryption()
 
-    def process(self, root: Dict[str, any]):
+    def process(self, k8s_object: BaseObj):
         try:
-            self._secret_obj = SecretObj(root)
+            self._secret_obj = SecretObj(k8s_object.data)
         except ValueError:
             self._secret_obj = None
 
         walker = TreeWalker(self)
-        walker.walk(root)
+        walker.walk(k8s_object.data)
 
     def process_str(self, value: str, parent: Dict[str, any], key: str) -> str:
         if not value.startswith(Encryption.CRYPT_PREFIX):
             if self._secret_obj is None:
                 # Not a secret object, simply pass through
                 return value
```

### Comparing `octoploy-1.2.0/octoploy/processing/K8sObjectMerge.py` & `octoploy-1.2.1/octoploy/processing/K8sObjectMerge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 from typing import Dict
 
 from octoploy.api.Model import DeploymentConfig, NamedItem
-from octoploy.utils.DictUtils import DictUtils
+from octoploy.k8s.BaseObj import BaseObj
 from octoploy.utils.Log import Log
 
 
 class K8sObjectMerge(Log):
     """
     Merges kubernetes objects
     """
     NAME_PATH = 'metadata.name'
 
     def __init__(self):
         super().__init__()
         self._existing_dc = None  # type: DeploymentConfig
         self._new_dc = None  # type: DeploymentConfig
 
-    def merge(self, existing, to_add) -> bool:
+    def merge(self, existing: BaseObj, to_add: BaseObj) -> bool:
         """
         Merges the given openshift object into one.
         :param existing: Existing where the data should be added to
         :param to_add: New data
         :return: True if the data has been merged, false otherwise
         """
-        expected_type = existing['kind'].lower()
-        type_str = to_add['kind'].lower()
-        if expected_type != type_str:
+        if existing.get_fqn() != to_add.get_fqn():
             return False
 
-        expected_name = DictUtils.get(existing, self.NAME_PATH)
-        name = DictUtils.get(to_add, self.NAME_PATH)
-        if name is not None and expected_name is not None and expected_name != name:
-            return False
-
-        if expected_type == 'DeploymentConfig'.lower() or expected_type == 'Deployment'.lower():
+        if existing.is_kind('DeploymentConfig') or existing.is_kind('Deployment'):
             self._merge_dc(DeploymentConfig(existing), DeploymentConfig(to_add))
             return True
 
-        self.log.warning('Don\'t know how to merge ' + expected_type)
+        self.log.warning('Don\'t know how to merge ' + existing.kind)
 
     def _merge_dc(self, existing: DeploymentConfig, to_add: DeploymentConfig):
         """
         Merges the given deployment configs if their name match
         :param existing: Deployment config where the data should be added
         :param to_add: New data
         """
```

### Comparing `octoploy-1.2.0/octoploy/processing/TreeWalker.py` & `octoploy-1.2.1/octoploy/processing/TreeWalker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from abc import abstractmethod
 from typing import Dict, Optional
 
+from octoploy.k8s.BaseObj import BaseObj
+
 
 class TreeProcessor:
     @abstractmethod
-    def process(self, root: dict):
+    def process(self, k8s_object: BaseObj):
         """
         Processes the tree
 
-        :param root: Root of the tree
-        :raises: SkipObject: The tree should be skipped
+        :param k8s_object: K8s object
+        :raises: SkipObject: The object should be skipped
         """
         pass
 
     def process_object(self, data: Dict[str, any], parent: Dict[str, any], key: str) -> Optional[Dict[str, any]]:
         """
        Processes a node of the tree
        :param data: Object
```

### Comparing `octoploy-1.2.0/octoploy/processing/ValueLoader.py` & `octoploy-1.2.1/octoploy/processing/ValueLoader.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/processing/YmlTemplateProcessor.py` & `octoploy-1.2.1/octoploy/processing/YmlTemplateProcessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import re
 from typing import Optional, Dict, List, Set
 from typing import TYPE_CHECKING
 
+from octoploy.k8s.BaseObj import BaseObj
 from octoploy.processing.TreeWalker import TreeWalker, TreeProcessor
 from octoploy.utils.Log import Log
 
 if TYPE_CHECKING:
     from octoploy.config.BaseConfig import BaseConfig
 from octoploy.utils.Errors import MissingParam
 
@@ -55,28 +56,27 @@
 
         :param template_processor: Child processor
         """
         if self._child is not None:
             raise ValueError('Child processor already defined')
         self._child = template_processor
 
-    def process(self, data: dict):
+    def process(self, k8s_object: BaseObj):
         """
         Processes the app data
 
-        :param data: Data of the app, the data will be modified in place
+        :param k8s_object: Data of the app, the data will be modified in place
         :raise MissingParam: Gets raised if at least one parameter is not defined
         """
         self._load_replacements()
 
         # Now replace any placeholders in the actual data tree
         walker = TreeWalker(self)
-        walker.walk(data)
-
-        # self._walk_dict(replacements, data)
+        walker.walk(k8s_object.data)
+        k8s_object.refresh()
 
         # Check if any of the missing vars are declared as "params"
         # (aka are required)
         if len(self._missing_vars) > 0:
             missing_params = []
             params = self._get_params()
             for missing in self._missing_vars:
```

### Comparing `octoploy-1.2.0/octoploy/state/StateTracking.py` & `octoploy-1.2.1/octoploy/state/StateTracking.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/utils/Cert.py` & `octoploy-1.2.1/octoploy/utils/Cert.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/utils/DictUtils.py` & `octoploy-1.2.1/octoploy/utils/DictUtils.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/utils/Encryption.py` & `octoploy-1.2.1/octoploy/utils/Encryption.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/utils/Log.py` & `octoploy-1.2.1/octoploy/utils/Log.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy/utils/YmlWriter.py` & `octoploy-1.2.1/octoploy/utils/YmlWriter.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/octoploy.egg-info/PKG-INFO` & `octoploy-1.2.1/octoploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoploy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Simple kubernetes / openshift templating engine with templating, libraries, state tracking
 Home-page: https://github.com/davidgiga1993/octoploy
 Author: davidgiga1993
 Author-email: david@dev-core.org
 License: UNKNOWN
 Description: # Kubernetes / openshift templating and deployment engine
```

### Comparing `octoploy-1.2.0/octoploy.egg-info/SOURCES.txt` & `octoploy-1.2.1/octoploy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 octoploy/deploy/__init__.py
 octoploy/k8s/BaseObj.py
 octoploy/k8s/SecretObj.py
 octoploy/k8s/__init__.py
 octoploy/processing/DataPreProcessor.py
 octoploy/processing/DecryptionProcessor.py
 octoploy/processing/K8sObjectMerge.py
+octoploy/processing/NamespaceProcessor.py
 octoploy/processing/TreeWalker.py
 octoploy/processing/ValueLoader.py
 octoploy/processing/YmlTemplateProcessor.py
 octoploy/processing/__init__.py
 octoploy/state/StateTracking.py
 octoploy/state/__init__.py
 octoploy/utils/Cert.py
```

### Comparing `octoploy-1.2.0/setup.py` & `octoploy-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/tests/AppDeploymentTest.py` & `octoploy-1.2.1/tests/AppDeploymentTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/tests/DictUtilsTest.py` & `octoploy-1.2.1/tests/DictUtilsTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/tests/OcObjectMergeTest.py` & `octoploy-1.2.1/tests/OcObjectMergeTest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,96 @@
 from unittest import TestCase
 
 import yaml
+from octoploy.k8s.BaseObj import BaseObj
 
 from octoploy.processing.K8sObjectMerge import K8sObjectMerge
 
 
 class K8sObjectMergeTest(TestCase):
 
     def test_append_sidecar_container(self):
         existing = '''kind: Deployment
 apiVersion: v1
 metadata:
-  name: "${DC_NAME}"
+  name: "${APP_NAME}"
 
 spec:
   replicas: 1
   selector:
-    name: "${DC_NAME}"
+    name: "${APP_NAME}"
   strategy:
      type: Rolling
 
   template:
     metadata:
       labels:
-        name: "${DC_NAME}"
+        name: "${APP_NAME}"
 
     spec:
       containers:
-        - name: "${DC_NAME}"
+        - name: "${APP_NAME}"
           volumeMounts:
             - name: java-cacerts-volume
               mountPath: /java/java-cacerts
 '''
         new = '''
+apiVersion: v1
 kind: Deployment
+metadata:
+  name: "${APP_NAME}"
 spec:
   template:
     spec:
       containers:
         - name: "sidecar-container"
 '''
         merge = K8sObjectMerge()
         data = yaml.safe_load(existing)
-        merge.merge(data, yaml.safe_load(new))
+        merge.merge(BaseObj(data), BaseObj(yaml.safe_load(new)))
 
         def validate(data):
             self.assertEqual('v1', data['apiVersion'])
             containers = data['spec']['template']['spec']['containers']
             self.assertEqual(2, len(containers))
 
             for container in containers:
-                if container['name'] == '${DC_NAME}':
+                if container['name'] == '${APP_NAME}':
                     self.assertEqual(1, len(container['volumeMounts']))
                 else:
                     self.assertEqual('sidecar-container', container['name'])
 
         validate(data)
 
         # Now invert the inputs, the result should be the same
         new_data = yaml.safe_load(new)
-        merge.merge(new_data, yaml.safe_load(existing))
+        merge.merge(BaseObj(new_data), BaseObj(yaml.safe_load(existing)))
         validate(new_data)
 
     def test_merge_same_container(self):
         existing = '''kind: Deployment
 apiVersion: v1
 metadata:
-  name: "${DC_NAME}"
+  name: "${APP_NAME}"
 
 spec:
   replicas: 1
   selector:
-    name: "${DC_NAME}"
+    name: "${APP_NAME}"
   strategy:
      type: Rolling
 
   template:
     metadata:
       labels:
-        name: "${DC_NAME}"
+        name: "${APP_NAME}"
 
     spec:
       containers:
-        - name: "${DC_NAME}"
+        - name: "${APP_NAME}"
           imagePullPolicy: Always
           resources:
             requests:
               cpu: "20m"
               memory: "10Mi"
             limits:
               memory: "300Mi"
@@ -107,45 +111,46 @@
 
   triggers:
     - type: ConfigChange
     - type: ImageChange
       imageChangeParams:
         automatic: true
         containerNames:
-          - "${DC_NAME}"
+          - "${APP_NAME}"
         from:
           kind: ImageStreamTag
-          name: '${DC_NAME}:prod'
+          name: '${APP_NAME}:prod'
 '''
         new = '''
+apiVersion: v1
 kind: Deployment
 metadata:
-  name: "${DC_NAME}"
+  name: "${APP_NAME}"
 
 spec:
   template:
     metadata:
       labels:
-        name: "${DC_NAME}"
+        name: "${APP_NAME}"
 
     spec:
       containers:
-        - name: "${DC_NAME}"
+        - name: "${APP_NAME}"
           volumeMounts:
             - name: crawler-packages-volume
               mountPath: /packages
 
       volumes:
         - name: crawler-packages-volume
           persistentVolumeClaim:
             claimName: "pvc-crawler-packages"'''
 
         merge = K8sObjectMerge()
         data = yaml.safe_load(existing)
-        merge.merge(data, yaml.safe_load(new))
+        merge.merge(BaseObj(data), BaseObj(yaml.safe_load(new)))
 
         containers = data['spec']['template']['spec']['containers']
         self.assertEqual(1, len(containers))
 
         container = containers[0]
         self.assertEqual(2, len(container['volumeMounts']))
```

### Comparing `octoploy-1.2.0/tests/StateTrackingTest.py` & `octoploy-1.2.1/tests/StateTrackingTest.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         octoploy.octoploy._run_app_deploy('app_deploy_test', 'app', self._mode)
 
         self.assertEqual(4, len(self._dummy_api.commands))
         self.assertEqual(['get', 'ConfigMap/octoploy-state', '-o', 'json'], self._dummy_api.commands[0].args)
         state_update = self._dummy_api.commands[-1]
         self.assertEqual(['apply', '-f', '-'], state_update.args)
         self.assertStateEqual([{"context": "ABC",
-                                "hash": "d7e628adce4fa1b75b861be76920b6dc",
+                                "hash": "e2e4634c5cd31a1b58da917e8b181b28",
                                 "kind": "Deployment",
                                 "name": "ABC",
                                 "namespace": "oc-project",
                                 }], state_update.stdin)
 
     def test_deploy_all_then_app(self):
         """
@@ -119,40 +119,45 @@
         self.assertEqual(14, len(self._dummy_api.commands))
         self.assertEqual(['get', 'ConfigMap/octoploy-state', '-o', 'json'], self._dummy_api.commands[0].args)
 
         state_update = self._dummy_api.commands[-1]
         self.assertEqual(['apply', '-f', '-'], state_update.args)
         self.assertStateEqual([
             {"context": "ABC",
-             "hash": "d7e628adce4fa1b75b861be76920b6dc",
+             "hash": "e2e4634c5cd31a1b58da917e8b181b28",
              "kind": "Deployment",
              "name": "ABC",
              "namespace": "oc-project"},
             {"context": "entity-compare-api",
-             "hash": "8b3e2f9b6499582cc3e4fe66681a7850",
+             "hash": "644921ab79abf165d8fb8304913ff1c7",
              "kind": "Deployment",
              "name": "8080",
              "namespace": "oc-project"},
             {"context": "favorite-api",
-             "hash": "96204a555b80b50b3cf49e5684f3daa9",
+             "hash": "3005876d55a8c9af38a58a4227a377fc",
              "kind": "Deployment",
              "name": "8081",
              "namespace": "oc-project"},
             {"context": "cm-types",
-             "hash": "a48eadd6d347e2591a3929df077aead7",
+             "hash": "1f4d778af0ea594402e656fd6139c584",
              "kind": "ConfigMap",
              "name": "config",
              "namespace": "oc-project"},
             {"context": "ABC2",
-             "hash": "ea23b547bb9a06ca79d3dc23c3d1d0dd",
+             "hash": "d6e8e8f4b59b77117ec4ad267be8dcae",
              "kind": "Secret",
              "name": "secret",
              "namespace": "oc-project"},
+            {"context": "ABC2",
+             "hash": "178859f1aa21598384610f352d314ae6",
+             "kind": "Secret",
+             "name": "plain-secret",
+             "namespace": "oc-project"},
             {"context": "var-append",
-             "hash": "e19d6902d55e14e99213b1d112acbde0",
+             "hash": "24d921e38f585e26cdc247d8fddc260e",
              "kind": "ConfigMap",
              "name": "config",
              "namespace": "oc-project"},
         ], state_update.stdin)
 
         # Now deploy a single app
         current_state = yaml.safe_load(state_update.stdin)
@@ -177,43 +182,48 @@
 
         self.assertEqual(14, len(self._dummy_api.commands))
         self.assertEqual(['get', 'ConfigMap/octoploy-state', '-o', 'json'], self._dummy_api.commands[0].args)
 
         state_update = self._dummy_api.commands[-1]
         self.assertEqual(['apply', '-f', '-'], state_update.args)
         self.assertStateEqual([{"context": "ABC",
-                                "hash": "d7e628adce4fa1b75b861be76920b6dc",
+                                "hash": "e2e4634c5cd31a1b58da917e8b181b28",
                                 "kind": "Deployment",
                                 "name": "ABC",
                                 "namespace": "oc-project"},
                                {"context": "entity-compare-api",
-                                "hash": "8b3e2f9b6499582cc3e4fe66681a7850",
+                                "hash": "644921ab79abf165d8fb8304913ff1c7",
                                 "kind": "Deployment",
                                 "name": "8080",
                                 "namespace": "oc-project"},
                                {"context": "favorite-api",
-                                "hash": "96204a555b80b50b3cf49e5684f3daa9",
+                                "hash": "3005876d55a8c9af38a58a4227a377fc",
                                 "kind": "Deployment",
                                 "name": "8081",
                                 "namespace": "oc-project"},
                                {"context": "cm-types",
-                                "hash": "a48eadd6d347e2591a3929df077aead7",
+                                "hash": "1f4d778af0ea594402e656fd6139c584",
                                 "kind": "ConfigMap",
                                 "name": "config",
                                 "namespace": "oc-project"},
                                {"context": "ABC2",
-                                "hash": "ea23b547bb9a06ca79d3dc23c3d1d0dd",
+                                "hash": "d6e8e8f4b59b77117ec4ad267be8dcae",
                                 "kind": "Secret",
                                 "name": "secret",
                                 "namespace": "oc-project"},
                                {"context": "var-append",
-                                "hash": "e19d6902d55e14e99213b1d112acbde0",
+                                "hash": "24d921e38f585e26cdc247d8fddc260e",
                                 "kind": "ConfigMap",
                                 "name": "config",
                                 "namespace": "oc-project"},
+                               {"context": "ABC2",
+                                "hash": "178859f1aa21598384610f352d314ae6",
+                                "kind": "Secret",
+                                "name": "plain-secret",
+                                "namespace": "oc-project"},
                                ], state_update.stdin)
         # Now deploy a single app
         current_state = yaml.safe_load(state_update.stdin)
         self._dummy_api.respond(['get', 'ConfigMap/octoploy-state', '-o', 'json'], json.dumps(current_state))
         self._dummy_api.respond(['get', 'Deployment/ABC', '-o', 'json'], '{}')
         self._dummy_api.respond(['get', 'Deployment/8080', '-o', 'json'], '{}')
         self._dummy_api.respond(['get', 'Deployment/8081', '-o', 'json'], '{}')
```

### Comparing `octoploy-1.2.0/tests/TestUtils.py` & `octoploy-1.2.1/tests/TestUtils.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/tests/YmlTempalteProcessorTest.py` & `octoploy-1.2.1/tests/YmlTempalteProcessorTest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from unittest import TestCase, mock
 
 from octoploy.config.Config import AppConfig
+from octoploy.k8s.BaseObj import BaseObj
 from octoploy.processing.YmlTemplateProcessor import YmlTemplateProcessor
 
 
 class YmlTemplateProcessorTest(TestCase):
 
     def test_replace(self):
         with mock.patch('builtins.open', mock.mock_open(read_data='''
@@ -15,25 +16,28 @@
     MY_OBJECT:
         someItem: 1
         someOtherItem: 2
 ''')):
             app_config = AppConfig('', '')
 
         proc = YmlTemplateProcessor(app_config)
-        data = {'root': {
-            'item': '${DC_NAME}',
-            'object': '${MY_OBJECT}',
-            'list': [{
-                'other': '${DC_NAME}/${IMAGE_NAME}'
-            }],
-            'sub': {
-                'item2': '${MY_VAR}'
-            }
-        }}
-        proc.process(data)
+        data = {
+            'kind': 'Test',
+            'apiVersion': 'v1',
+            'root': {
+                'item': '${APP_NAME}',
+                'object': '${MY_OBJECT}',
+                'list': [{
+                    'other': '${APP_NAME}/${IMAGE_NAME}'
+                }],
+                'sub': {
+                    'item2': '${MY_VAR}'
+                }
+            }}
+        proc.process(BaseObj(data))
         self.assertEqual('hello', data['root']['item'])
         self.assertEqual('hello/image', data['root']['list'][0]['other'])
         self.assertEqual('testVal', data['root']['sub']['item2'])
         self.assertEqual({
             'someItem': 1,
             'someOtherItem': 2
         }, data['root']['object'])
@@ -43,55 +47,64 @@
 name: hello
 vars:
     MY_VAR: testVal
 ''')):
             app_config = AppConfig('', '')
 
         proc = YmlTemplateProcessor(app_config)
-        data = {'root': {
-            'item': '${DC_NAME}',
-            'list': [{
-                'other': '${DC_NAME}'
-            }],
-            'sub': {
-                'item2': '${MY_VAR}'
-            }
-        }}
-        proc.process(data)
+        data = {
+            'kind': 'Test',
+            'apiVersion': 'v1',
+            'root': {
+                'item': '${APP_NAME}',
+                'list': [{
+                    'other': '${APP_NAME}'
+                }],
+                'sub': {
+                    'item2': '${MY_VAR}'
+                }
+            }}
+        proc.process(BaseObj(data))
         self.assertEqual('hello', data['root']['item'])
         self.assertEqual('hello', data['root']['list'][0]['other'])
         self.assertEqual('testVal', data['root']['sub']['item2'])
 
     def test_merge_var_inline(self):
         with mock.patch('builtins.open', mock.mock_open(read_data='''
 name: hello
 vars:
     MERGE_OBJ: 
         someKey: value
 ''')):
             app_config = AppConfig('', '')
 
         proc = YmlTemplateProcessor(app_config)
-        data = {'root': {
-            'item': '${DC_NAME}',
-            '_merge': '${MERGE_OBJ}',
-        }}
-        proc.process(data)
+        data = {
+            'kind': 'Test',
+            'apiVersion': 'v1',
+            'root': {
+                'item': '${APP_NAME}',
+                '_merge': '${MERGE_OBJ}',
+            }}
+        proc.process(BaseObj(data))
         self.assertEqual('hello', data['root']['item'])
         self.assertEqual('value', data['root']['someKey'])
 
     def test_merge_object_inline(self):
         with mock.patch('builtins.open', mock.mock_open(read_data='''
 name: hello
 ''')):
             app_config = AppConfig('', '')
 
         proc = YmlTemplateProcessor(app_config)
-        data = {'root': {
-            'item': '${DC_NAME}',
-            '_merge': {
-                'someKey': 'value',
-            },
-        }}
-        proc.process(data)
+        data = {
+            'kind': 'Test',
+            'apiVersion': 'v1',
+            'root': {
+                'item': '${APP_NAME}',
+                '_merge': {
+                    'someKey': 'value',
+                },
+            }}
+        proc.process(BaseObj(data))
         self.assertEqual('hello', data['root']['item'])
-        self.assertEqual('value', data['root']['someKey'])
+        self.assertEqual('value', data['root']['someKey'])
```

### Comparing `octoploy-1.2.0/tests/processing/ValueLoaderTest.py` & `octoploy-1.2.1/tests/processing/ValueLoaderTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.0/tests/utils/EncryptionTest.py` & `octoploy-1.2.1/tests/utils/EncryptionTest.py`

 * *Files identical despite different names*

