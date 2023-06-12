# Comparing `tmp/KapoorLabs-Lightning-5.2.6.tar.gz` & `tmp/KapoorLabs-Lightning-5.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/KapoorLabs-Lightning/dist/.tmp-5hw6fww3/KapoorLabs-Lightning-5.2.6.tar", last modified: Sun Jun 11 23:23:41 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/KapoorLabs-Lightning/dist/.tmp-dzvvd_5p/KapoorLabs-Lightning-5.2.7.tar", last modified: Mon Jun 12 07:18:06 2023, max compression
```

## Comparing `KapoorLabs-Lightning-5.2.6.tar` & `KapoorLabs-Lightning-5.2.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 23:23:41.889688 KapoorLabs-Lightning-5.2.6/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 23:23:41.083796 KapoorLabs-Lightning-5.2.6/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 23:23:41.240905 KapoorLabs-Lightning-5.2.6/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2795 2023-05-15 12:36:30.000000 KapoorLabs-Lightning-5.2.6/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      991 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.6/.gitignore
--rwxrwxrwx   0 debian    (1000) debian    (1000)      864 2023-05-15 12:16:19.000000 KapoorLabs-Lightning-5.2.6/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.6/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.6/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-11 23:23:41.890259 KapoorLabs-Lightning-5.2.6/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2435 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.6/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 23:23:41.353117 KapoorLabs-Lightning-5.2.6/licenses/
--rwxrwxrwx   0 debian    (1000) debian    (1000)    11358 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.6/licenses/Apache-2
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.6/licenses/BSD-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)    35148 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.6/licenses/GPL-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)     7653 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.6/licenses/LGPL-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1080 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.6/licenses/MIT
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16726 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.6/licenses/MPL-2
--rwxrwxrwx   0 debian    (1000) debian    (1000)      270 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.6/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1734 2023-06-11 23:23:41.895778 KapoorLabs-Lightning-5.2.6/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 23:23:41.098639 KapoorLabs-Lightning-5.2.6/src/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 23:23:41.503170 KapoorLabs-Lightning-5.2.6/src/KapoorLabs_Lightning.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-11 23:23:39.000000 KapoorLabs-Lightning-5.2.6/src/KapoorLabs_Lightning.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1157 2023-06-11 23:23:41.000000 KapoorLabs-Lightning-5.2.6/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 23:23:39.000000 KapoorLabs-Lightning-5.2.6/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       72 2023-06-11 23:23:39.000000 KapoorLabs-Lightning-5.2.6/src/KapoorLabs_Lightning.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       87 2023-06-11 23:23:39.000000 KapoorLabs-Lightning-5.2.6/src/KapoorLabs_Lightning.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       21 2023-06-11 23:23:39.000000 KapoorLabs-Lightning-5.2.6/src/KapoorLabs_Lightning.egg-info/top_level.txt
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 23:23:41.807039 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      859 2023-05-26 19:51:02.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/__init__.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 23:23:41.864600 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3106 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-11 23:23:39.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/caped.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2065 2023-05-15 12:33:19.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/graph_functions.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       68 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/kapoorlabs.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)    35081 2023-06-11 23:23:02.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/lightning_trainer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3537 2023-05-26 19:09:09.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/optimizers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    15688 2023-06-05 14:50:17.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/pytorch_datasets.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3801 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/pytorch_loggers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      762 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/pytorch_losses.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16569 2023-06-02 16:45:22.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/pytorch_models.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1809 2023-06-03 13:57:05.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/pytorch_transforms.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3123 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/schedulers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      615 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.6/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 07:18:05.989688 KapoorLabs-Lightning-5.2.7/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 07:18:05.110512 KapoorLabs-Lightning-5.2.7/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 07:18:05.270366 KapoorLabs-Lightning-5.2.7/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2795 2023-05-15 12:36:30.000000 KapoorLabs-Lightning-5.2.7/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      991 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.7/.gitignore
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      864 2023-05-15 12:16:19.000000 KapoorLabs-Lightning-5.2.7/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.7/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.7/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-12 07:18:05.990696 KapoorLabs-Lightning-5.2.7/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2435 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.7/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 07:18:05.418115 KapoorLabs-Lightning-5.2.7/licenses/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11358 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.7/licenses/Apache-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.7/licenses/BSD-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    35148 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.7/licenses/GPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     7653 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.7/licenses/LGPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1080 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.7/licenses/MIT
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16726 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.7/licenses/MPL-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      270 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.7/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1734 2023-06-12 07:18:05.996856 KapoorLabs-Lightning-5.2.7/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 07:18:05.124693 KapoorLabs-Lightning-5.2.7/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 07:18:05.544484 KapoorLabs-Lightning-5.2.7/src/KapoorLabs_Lightning.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-12 07:18:04.000000 KapoorLabs-Lightning-5.2.7/src/KapoorLabs_Lightning.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1157 2023-06-12 07:18:05.000000 KapoorLabs-Lightning-5.2.7/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-12 07:18:04.000000 KapoorLabs-Lightning-5.2.7/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       72 2023-06-12 07:18:04.000000 KapoorLabs-Lightning-5.2.7/src/KapoorLabs_Lightning.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       87 2023-06-12 07:18:04.000000 KapoorLabs-Lightning-5.2.7/src/KapoorLabs_Lightning.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       21 2023-06-12 07:18:04.000000 KapoorLabs-Lightning-5.2.7/src/KapoorLabs_Lightning.egg-info/top_level.txt
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 07:18:05.895224 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      859 2023-05-26 19:51:02.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/__init__.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 07:18:05.961333 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3106 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-12 07:18:04.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/caped.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2065 2023-05-15 12:33:19.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/graph_functions.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       68 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/kapoorlabs.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    35200 2023-06-12 07:17:24.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/lightning_trainer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3537 2023-05-26 19:09:09.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/optimizers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    15688 2023-06-05 14:50:17.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/pytorch_datasets.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3801 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/pytorch_loggers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      762 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/pytorch_losses.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16569 2023-06-02 16:45:22.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/pytorch_models.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1809 2023-06-03 13:57:05.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/pytorch_transforms.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3123 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/schedulers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      615 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.7/tox.ini
```

### Comparing `KapoorLabs-Lightning-5.2.6/.github/workflows/test_and_deploy.yml` & `KapoorLabs-Lightning-5.2.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/.gitignore` & `KapoorLabs-Lightning-5.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/.pre-commit-config.yaml` & `KapoorLabs-Lightning-5.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/LICENSE` & `KapoorLabs-Lightning-5.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/PKG-INFO` & `KapoorLabs-Lightning-5.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.2.6
+Version: 5.2.7
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.2.6/README.md` & `KapoorLabs-Lightning-5.2.7/README.md`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/licenses/Apache-2` & `KapoorLabs-Lightning-5.2.7/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/licenses/BSD-3` & `KapoorLabs-Lightning-5.2.7/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/licenses/GPL-3` & `KapoorLabs-Lightning-5.2.7/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/licenses/LGPL-3` & `KapoorLabs-Lightning-5.2.7/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/licenses/MIT` & `KapoorLabs-Lightning-5.2.7/licenses/MIT`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/licenses/MPL-2` & `KapoorLabs-Lightning-5.2.7/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/setup.cfg` & `KapoorLabs-Lightning-5.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/src/KapoorLabs_Lightning.egg-info/PKG-INFO` & `KapoorLabs-Lightning-5.2.7/src/KapoorLabs_Lightning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.2.6
+Version: 5.2.7
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.2.6/src/KapoorLabs_Lightning.egg-info/SOURCES.txt` & `KapoorLabs-Lightning-5.2.7/src/KapoorLabs_Lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/__init__.py` & `KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/_tests/test_pytorch_models.py` & `KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/_tests/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/graph_functions.py` & `KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/graph_functions.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/lightning_trainer.py` & `KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/lightning_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,16 +275,18 @@
 
         mean = torch.mean(batch, 1).to(self.device)
         scale = torch.tensor(
             [[self.scale_z, self.scale_xy, self.scale_xy]]
         ).to(self.device)
 
         outputs, features = self(batch)
-
-        outputs = outputs * scale + mean
+        batch_size = batch.shape[0]
+        outputs = outputs * scale
+        for i in range(batch_size):
+            outputs[i, :] = outputs[i, :] + mean[i, :]
 
         return outputs
 
     def training_step(self, batch, batch_idx):
         inputs = batch
         outputs, features = self(inputs)
```

### Comparing `KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/optimizers.py` & `KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/optimizers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/pytorch_datasets.py` & `KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/pytorch_loggers.py` & `KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/pytorch_loggers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/pytorch_losses.py` & `KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/pytorch_losses.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/pytorch_models.py` & `KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/pytorch_models.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/pytorch_transforms.py` & `KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/pytorch_transforms.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/src/kapoorlabs_lightning/schedulers.py` & `KapoorLabs-Lightning-5.2.7/src/kapoorlabs_lightning/schedulers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.6/tox.ini` & `KapoorLabs-Lightning-5.2.7/tox.ini`

 * *Files identical despite different names*

