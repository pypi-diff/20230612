# Comparing `tmp/KapoorLabs-Lightning-5.2.2.tar.gz` & `tmp/KapoorLabs-Lightning-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/KapoorLabs-Lightning/dist/.tmp-72hynfqm/KapoorLabs-Lightning-5.2.2.tar", last modified: Sun Jun 11 12:21:41 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/KapoorLabs-Lightning/dist/.tmp-0bwmghag/KapoorLabs-Lightning-5.2.3.tar", last modified: Sun Jun 11 21:21:06 2023, max compression
```

## Comparing `KapoorLabs-Lightning-5.2.2.tar` & `KapoorLabs-Lightning-5.2.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:21:41.291835 KapoorLabs-Lightning-5.2.2/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:21:40.418537 KapoorLabs-Lightning-5.2.2/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:21:40.572237 KapoorLabs-Lightning-5.2.2/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2795 2023-05-15 12:36:30.000000 KapoorLabs-Lightning-5.2.2/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      991 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.2/.gitignore
--rwxrwxrwx   0 debian    (1000) debian    (1000)      864 2023-05-15 12:16:19.000000 KapoorLabs-Lightning-5.2.2/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.2/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.2/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-11 12:21:41.292840 KapoorLabs-Lightning-5.2.2/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2435 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.2/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:21:40.699211 KapoorLabs-Lightning-5.2.2/licenses/
--rwxrwxrwx   0 debian    (1000) debian    (1000)    11358 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.2/licenses/Apache-2
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.2/licenses/BSD-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)    35148 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.2/licenses/GPL-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)     7653 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.2/licenses/LGPL-3
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1080 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.2/licenses/MIT
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16726 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.2/licenses/MPL-2
--rwxrwxrwx   0 debian    (1000) debian    (1000)      270 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.2/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1734 2023-06-11 12:21:41.300292 KapoorLabs-Lightning-5.2.2/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:21:40.435172 KapoorLabs-Lightning-5.2.2/src/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:21:40.864541 KapoorLabs-Lightning-5.2.2/src/KapoorLabs_Lightning.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-11 12:21:39.000000 KapoorLabs-Lightning-5.2.2/src/KapoorLabs_Lightning.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1157 2023-06-11 12:21:40.000000 KapoorLabs-Lightning-5.2.2/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 12:21:39.000000 KapoorLabs-Lightning-5.2.2/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       72 2023-06-11 12:21:39.000000 KapoorLabs-Lightning-5.2.2/src/KapoorLabs_Lightning.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       87 2023-06-11 12:21:39.000000 KapoorLabs-Lightning-5.2.2/src/KapoorLabs_Lightning.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       21 2023-06-11 12:21:39.000000 KapoorLabs-Lightning-5.2.2/src/KapoorLabs_Lightning.egg-info/top_level.txt
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:21:41.199980 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      859 2023-05-26 19:51:02.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/__init__.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 12:21:41.262726 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3106 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-11 12:21:39.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/caped.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2065 2023-05-15 12:33:19.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/graph_functions.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       68 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/kapoorlabs.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)    35027 2023-06-11 12:21:06.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/lightning_trainer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3537 2023-05-26 19:09:09.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/optimizers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    15688 2023-06-05 14:50:17.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/pytorch_datasets.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3801 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/pytorch_loggers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      762 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/pytorch_losses.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16569 2023-06-02 16:45:22.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/pytorch_models.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1809 2023-06-03 13:57:05.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/pytorch_transforms.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3123 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/schedulers.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      615 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.2/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 21:21:05.988090 KapoorLabs-Lightning-5.2.3/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 21:21:04.884511 KapoorLabs-Lightning-5.2.3/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 21:21:05.063176 KapoorLabs-Lightning-5.2.3/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2795 2023-05-15 12:36:30.000000 KapoorLabs-Lightning-5.2.3/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      991 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.3/.gitignore
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      864 2023-05-15 12:16:19.000000 KapoorLabs-Lightning-5.2.3/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.3/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.3/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-11 21:21:05.990492 KapoorLabs-Lightning-5.2.3/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2435 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.3/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 21:21:05.232400 KapoorLabs-Lightning-5.2.3/licenses/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11358 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.3/licenses/Apache-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.3/licenses/BSD-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    35148 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.3/licenses/GPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     7653 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.3/licenses/LGPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1080 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.3/licenses/MIT
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16726 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.3/licenses/MPL-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      270 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.3/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1734 2023-06-11 21:21:06.003011 KapoorLabs-Lightning-5.2.3/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 21:21:04.900056 KapoorLabs-Lightning-5.2.3/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 21:21:05.443593 KapoorLabs-Lightning-5.2.3/src/KapoorLabs_Lightning.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3746 2023-06-11 21:21:03.000000 KapoorLabs-Lightning-5.2.3/src/KapoorLabs_Lightning.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1157 2023-06-11 21:21:04.000000 KapoorLabs-Lightning-5.2.3/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 21:21:03.000000 KapoorLabs-Lightning-5.2.3/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       72 2023-06-11 21:21:03.000000 KapoorLabs-Lightning-5.2.3/src/KapoorLabs_Lightning.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       87 2023-06-11 21:21:03.000000 KapoorLabs-Lightning-5.2.3/src/KapoorLabs_Lightning.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       21 2023-06-11 21:21:03.000000 KapoorLabs-Lightning-5.2.3/src/KapoorLabs_Lightning.egg-info/top_level.txt
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 21:21:05.880024 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      859 2023-05-26 19:51:02.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/__init__.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 21:21:05.950066 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3106 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-11 21:21:03.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2023-05-15 12:16:04.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/caped.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2065 2023-05-15 12:33:19.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/graph_functions.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       68 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/kapoorlabs.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    35081 2023-06-11 21:19:42.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/lightning_trainer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3537 2023-05-26 19:09:09.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/optimizers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    15688 2023-06-05 14:50:17.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/pytorch_datasets.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3801 2023-05-26 14:17:53.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/pytorch_loggers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      762 2023-05-15 12:20:06.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/pytorch_losses.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16569 2023-06-02 16:45:22.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/pytorch_models.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1809 2023-06-03 13:57:05.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/pytorch_transforms.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3123 2023-05-15 12:33:24.000000 KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/schedulers.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      615 2023-05-15 12:16:03.000000 KapoorLabs-Lightning-5.2.3/tox.ini
```

### Comparing `KapoorLabs-Lightning-5.2.2/.github/workflows/test_and_deploy.yml` & `KapoorLabs-Lightning-5.2.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/.gitignore` & `KapoorLabs-Lightning-5.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/.pre-commit-config.yaml` & `KapoorLabs-Lightning-5.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/LICENSE` & `KapoorLabs-Lightning-5.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/PKG-INFO` & `KapoorLabs-Lightning-5.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.2.2
+Version: 5.2.3
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.2.2/README.md` & `KapoorLabs-Lightning-5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/licenses/Apache-2` & `KapoorLabs-Lightning-5.2.3/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/licenses/BSD-3` & `KapoorLabs-Lightning-5.2.3/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/licenses/GPL-3` & `KapoorLabs-Lightning-5.2.3/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/licenses/LGPL-3` & `KapoorLabs-Lightning-5.2.3/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/licenses/MIT` & `KapoorLabs-Lightning-5.2.3/licenses/MIT`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/licenses/MPL-2` & `KapoorLabs-Lightning-5.2.3/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/setup.cfg` & `KapoorLabs-Lightning-5.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/src/KapoorLabs_Lightning.egg-info/PKG-INFO` & `KapoorLabs-Lightning-5.2.3/src/KapoorLabs_Lightning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.2.2
+Version: 5.2.3
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.2.2/src/KapoorLabs_Lightning.egg-info/SOURCES.txt` & `KapoorLabs-Lightning-5.2.3/src/KapoorLabs_Lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/__init__.py` & `KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/_tests/test_pytorch_models.py` & `KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/_tests/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/graph_functions.py` & `KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/graph_functions.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/lightning_trainer.py` & `KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/lightning_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,16 +269,18 @@
     def loss(self, y_hat, y):
         return self.loss_func(y_hat, y)
 
     def predict_step(self, batch: Any, batch_idx: int) -> Any:
         if isinstance(batch, (list, tuple)):
             batch = batch[0]
 
-        mean = torch.mean(batch, 0)
-        scale = torch.tensor([[self.scale_z, self.scale_xy, self.scale_xy]])
+        mean = torch.mean(batch, 0).to(self.device)
+        scale = torch.tensor(
+            [[self.scale_z, self.scale_xy, self.scale_xy]]
+        ).to(self.device)
 
         outputs, features = self(batch)
 
         outputs = outputs * scale + mean
 
         return outputs
```

### Comparing `KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/optimizers.py` & `KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/optimizers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/pytorch_datasets.py` & `KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/pytorch_loggers.py` & `KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/pytorch_loggers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/pytorch_losses.py` & `KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/pytorch_losses.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/pytorch_models.py` & `KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/pytorch_models.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/pytorch_transforms.py` & `KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/pytorch_transforms.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/src/kapoorlabs_lightning/schedulers.py` & `KapoorLabs-Lightning-5.2.3/src/kapoorlabs_lightning/schedulers.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.2.2/tox.ini` & `KapoorLabs-Lightning-5.2.3/tox.ini`

 * *Files identical despite different names*

