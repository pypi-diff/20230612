# Comparing `tmp/agsi-1.8.tar.gz` & `tmp/agsi-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-1.8.tar", last modified: Mon Jun 12 10:15:33 2023, max compression
+gzip compressed data, was "agsi-1.9.tar", last modified: Mon Jun 12 10:27:21 2023, max compression
```

## Comparing `agsi-1.8.tar` & `agsi-1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:15:33.143444 agsi-1.8/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-1.8/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-12 10:15:33.143444 agsi-1.8/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-1.8/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:15:33.143444 agsi-1.8/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-1.8/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:15:33.143444 agsi-1.8/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    15761 2023-06-12 08:25:13.000000 agsi-1.8/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-1.8/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     8953 2023-06-12 10:08:03.000000 agsi-1.8/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)  1075103 2023-06-12 08:02:57.000000 agsi-1.8/agsi/demo_V2.ipynb
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-1.8/agsi/main.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-1.8/agsi/requirements.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:15:33.143444 agsi-1.8/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-12 10:15:33.000000 agsi-1.8/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-12 10:15:33.000000 agsi-1.8/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-12 10:15:33.000000 agsi-1.8/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-12 10:15:33.000000 agsi-1.8/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-12 10:15:33.000000 agsi-1.8/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-12 10:15:33.143444 agsi-1.8/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-12 10:15:25.000000 agsi-1.8/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:27:21.172641 agsi-1.9/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-1.9/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-12 10:27:21.172641 agsi-1.9/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-1.9/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:27:21.172641 agsi-1.9/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-1.9/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:27:21.172641 agsi-1.9/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    15761 2023-06-12 10:27:05.000000 agsi-1.9/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-1.9/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     8953 2023-06-12 10:08:03.000000 agsi-1.9/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)  1079849 2023-06-12 10:26:58.000000 agsi-1.9/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-1.9/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-1.9/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:27:21.172641 agsi-1.9/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-12 10:27:21.000000 agsi-1.9/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-12 10:27:21.000000 agsi-1.9/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-12 10:27:21.000000 agsi-1.9/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-12 10:27:21.000000 agsi-1.9/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-12 10:27:21.000000 agsi-1.9/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-12 10:27:21.172641 agsi-1.9/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-12 10:27:17.000000 agsi-1.9/setup.py
```

### Comparing `agsi-1.8/agsi/data/FarmData.py` & `agsi-1.9/agsi/data/FarmData.py`

 * *Files identical despite different names*

### Comparing `agsi-1.8/agsi/data/utils.py` & `agsi-1.9/agsi/data/utils.py`

 * *Files identical despite different names*

### Comparing `agsi-1.8/agsi/demo_V2.ipynb` & `agsi-1.9/agsi/demo_V2.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891176621510673%*

 * *Differences: {"'cells'": "{1: {'source': ['from data.utils import ndvi']}, 5: {'execution_count': 5}, 8: "*

 * *            '{\'execution_count\': 4, \'outputs\': {0: {\'text\': {insert: [(14, "4 {\'block_id\': '*

 * *            "'4', 'farm_id': '5', 'block_name': 'block_3a', 'vegetation_type': 'plant', "*

 * *            "'crop_name': '', 'yield': '', 'shp': "*

 * *            "'./assets/DroneAssets/dronedata/block_files/AllShapeFiles/block3A.shp', 'data_path': "*

 * *            "{'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': "*

 * *   […]*

```diff
@@ -1,26 +1,35 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
                 "import os, sys\n",
                 "#from agsi import FarmData\n",
                 "from data.FarmData import FarmData\n",
                 "from rasterio.plot import show\n",
                 "import rasterio\n",
                 "from data.utils import convert_path\n",
                 "from pprint import pprint"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from data.utils import ndvi"
+            ]
+        },
+        {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Tutorial on using the agse library"
             ]
         },
@@ -52,39 +61,95 @@
             "metadata": {},
             "source": [
                 "Now let us load this data into a python object"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "farm_csv_path = \"./assets/DroneAssets/dronedata/farm.csv\"\n",
                 "block_csv_path = \"./assets/DroneAssets/dronedata/block.csv\"\n",
                 "\n",
                 "if os.name == \"nt\":\n",
                 "    farm_csv_path = convert_path(farm_csv_path)\n",
                 "    block_csv_path = convert_path(block_csv_path)\n",
                 "\n",
                 "all_data = FarmData(farm_csv_path,block_csv_path)"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": 8,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "{'block_id': '12', 'farm_id': '1', 'block_name': 'Block_26a', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block26.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 26A_75m-21Feb2023.tif'}}, 'timestamps': ['23/02/23']}\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/home/sambal/Desktop/agri-sensing-india/agsi/data/utils.py:259: RuntimeWarning: invalid value encountered in divide\n",
+                        "  ndvi = (nir_band.astype(float)-red_band.astype(float))/(nir_band.astype(float)+red_band.astype(float))\n"
+                    ]
+                },
+                {
+                    "ename": "AttributeError",
+                    "evalue": "'NoneType' object has no attribute 'set_xlabel'",
+                    "output_type": "error",
+                    "traceback": [
+                        "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
+                        "\u001b[0;31mAttributeError\u001b[0m                            Traceback (most recent call last)",
+                        "\u001b[0;32m/tmp/ipykernel_32004/1599852738.py\u001b[0m in \u001b[0;36m<module>\u001b[0;34m\u001b[0m\n\u001b[1;32m      6\u001b[0m                                timestamp ='23/02/23')\n\u001b[1;32m      7\u001b[0m \u001b[0mblock_obj\u001b[0m\u001b[0;34m=\u001b[0m\u001b[0mndvi\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0mblock_image\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n\u001b[0;32m----> 8\u001b[0;31m \u001b[0mblock_obj\u001b[0m\u001b[0;34m.\u001b[0m\u001b[0mget_histogram\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n\u001b[0m",
+                        "\u001b[0;32m~/Desktop/agri-sensing-india/agsi/data/utils.py\u001b[0m in \u001b[0;36mget_histogram\u001b[0;34m(self, ax)\u001b[0m\n\u001b[1;32m    220\u001b[0m           \u001b[0mplt\u001b[0m\u001b[0;34m.\u001b[0m\u001b[0mhist\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0marray_flat\u001b[0m\u001b[0;34m,\u001b[0m \u001b[0mbins\u001b[0m\u001b[0;34m=\u001b[0m\u001b[0;36m50\u001b[0m\u001b[0;34m,\u001b[0m \u001b[0mcolor\u001b[0m\u001b[0;34m=\u001b[0m\u001b[0;34m'green'\u001b[0m\u001b[0;34m,\u001b[0m \u001b[0malpha\u001b[0m\u001b[0;34m=\u001b[0m\u001b[0;36m0.8\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n\u001b[1;32m    221\u001b[0m \u001b[0;34m\u001b[0m\u001b[0m\n\u001b[0;32m--> 222\u001b[0;31m         \u001b[0max\u001b[0m\u001b[0;34m.\u001b[0m\u001b[0mset_xlabel\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;34m'NDVI'\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n\u001b[0m\u001b[1;32m    223\u001b[0m         \u001b[0max\u001b[0m\u001b[0;34m.\u001b[0m\u001b[0mset_ylabel\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;34m'Frequency'\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n\u001b[1;32m    224\u001b[0m         \u001b[0max\u001b[0m\u001b[0;34m.\u001b[0m\u001b[0mset_title\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;34m'NDVI Histogram'\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n",
+                        "\u001b[0;31mAttributeError\u001b[0m: 'NoneType' object has no attribute 'set_xlabel'"
+                    ]
+                },
+                {
+                    "data": {
+                        "image/png": "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",
+                        "text/plain": [
+                            "<Figure size 432x288 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "#Extract a sample block from vikram farm\n",
+                "sample_block = all_data.blocks['12'] #Accessing a block by id\n",
+                "print(sample_block.info)\n",
+                "#Visualize the block\n",
+                "block_image=sample_block.get_modality(modality_type='drone_75', \n",
+                "                               timestamp ='23/02/23')\n",
+                "block_obj=ndvi(block_image)\n",
+                "block_obj.get_histogram()"
+            ]
+        },
+        {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The `all_data` object now provides information about the entire dataset and specifically provides access to farms and blocks which are exposed as dictionaries."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "1 {'owner': 'vikram_farm_1', 'area': None, 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 26A_75m-21Feb2023.tif'}}, 'farm_id': '1', 'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'}\n",
@@ -97,21 +162,21 @@
                         "8 {'owner': 'vikram_farm_8', 'area': None, 'data_path': {'29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block 3b_75m_29March2023.tif'}}, 'farm_id': '8', 'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'}\n",
                         "9 {'owner': 'vikram_farm_9', 'area': None, 'data_path': {'19/04/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block3a_75m19April2023.tif'}}, 'farm_id': '9', 'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'}\n",
                         "10 {'owner': 'vikram_farm_10', 'area': None, 'data_path': {'19/04/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block_15_16_17_18_75m_19April.tif'}}, 'farm_id': '10', 'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'}\n",
                         "11 {'owner': 'vikram_farm_11', 'area': None, 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 17b_18_37.8m_21feb2023.tif', 'drone_75': ''}}, 'farm_id': '11', 'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'}\n",
                         "1 {'block_id': '1', 'farm_id': '3', 'block_name': 'block_11', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block11.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 11_12_13_21Feb2023_75m.tif'}}, 'timestamps': ['23/02/23']}\n",
                         "2 {'block_id': '2', 'farm_id': '3', 'block_name': 'block_12', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block12.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 11_12_13_21Feb2023_75m.tif'}}, 'timestamps': ['23/02/23']}\n",
                         "3 {'block_id': '3', 'farm_id': '3', 'block_name': 'block_13', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block13.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 11_12_13_21Feb2023_75m.tif'}}, 'timestamps': ['23/02/23']}\n",
-                        "4 {'block_id': '4', 'farm_id': '5', 'block_name': 'block_3a', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block3A.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 3a_3b_75.6m_21Feb2023.tif'}, '29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block3a_75m_29March2023.tif'}, '19/04/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block3a_75m19April2023.tif'}}, 'timestamps': ['29/03/23', '19/04/23', '23/02/23']}\n",
+                        "4 {'block_id': '4', 'farm_id': '5', 'block_name': 'block_3a', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block3A.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 3a_3b_75.6m_21Feb2023.tif'}, '29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block3a_75m_29March2023.tif'}, '19/04/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block3a_75m19April2023.tif'}}, 'timestamps': ['19/04/23', '29/03/23', '23/02/23']}\n",
                         "5 {'block_id': '5', 'farm_id': '5', 'block_name': 'block_3b', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block3B.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 3a_3b_75.6m_21Feb2023.tif'}, '29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block 3b_75m_29March2023.tif'}}, 'timestamps': ['29/03/23', '23/02/23']}\n",
                         "6 {'block_id': '6', 'farm_id': '4', 'block_name': 'block_19', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block19.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block19_20_75.6m_21Feb2023.tif'}, '29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block15b_partof16_18_17b_19_20_30March2023.tif'}}, 'timestamps': ['29/03/23', '23/02/23']}\n",
-                        "7 {'block_id': '7', 'farm_id': '2', 'block_name': 'Block_15b', 'vegetation_type': 'ratoon', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block15B.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/block 15b_16b_17b_18_21feb2023_75m.tif'}, '29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block15b_partof16_18_17b_19_20_30March2023.tif'}, '19/04/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block_15_16_17_18_75m_19April.tif'}}, 'timestamps': ['29/03/23', '19/04/23', '23/02/23']}\n",
-                        "8 {'block_id': '8', 'farm_id': '2', 'block_name': 'Block_16b', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block16b.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/block 15b_16b_17b_18_21feb2023_75m.tif'}, '29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block15b_partof16_18_17b_19_20_30March2023.tif'}, '19/04/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block_15_16_17_18_75m_19April.tif'}}, 'timestamps': ['29/03/23', '19/04/23', '23/02/23']}\n",
-                        "9 {'block_id': '9', 'farm_id': '2', 'block_name': 'Block_17b', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block17b.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/block 15b_16b_17b_18_21feb2023_75m.tif'}, '29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block15b_partof16_18_17b_19_20_30March2023.tif'}, '19/04/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block_15_16_17_18_75m_19April.tif'}}, 'timestamps': ['29/03/23', '19/04/23', '23/02/23']}\n",
-                        "10 {'block_id': '10', 'farm_id': '2', 'block_name': 'Block_18', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block18.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/block 15b_16b_17b_18_21feb2023_75m.tif'}, '29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block15b_partof16_18_17b_19_20_30March2023.tif'}, '19/04/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block_15_16_17_18_75m_19April.tif'}}, 'timestamps': ['29/03/23', '19/04/23', '23/02/23']}\n",
+                        "7 {'block_id': '7', 'farm_id': '2', 'block_name': 'Block_15b', 'vegetation_type': 'ratoon', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block15B.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/block 15b_16b_17b_18_21feb2023_75m.tif'}, '29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block15b_partof16_18_17b_19_20_30March2023.tif'}, '19/04/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block_15_16_17_18_75m_19April.tif'}}, 'timestamps': ['19/04/23', '29/03/23', '23/02/23']}\n",
+                        "8 {'block_id': '8', 'farm_id': '2', 'block_name': 'Block_16b', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block16b.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/block 15b_16b_17b_18_21feb2023_75m.tif'}, '29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block15b_partof16_18_17b_19_20_30March2023.tif'}, '19/04/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block_15_16_17_18_75m_19April.tif'}}, 'timestamps': ['19/04/23', '29/03/23', '23/02/23']}\n",
+                        "9 {'block_id': '9', 'farm_id': '2', 'block_name': 'Block_17b', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block17b.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/block 15b_16b_17b_18_21feb2023_75m.tif'}, '29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block15b_partof16_18_17b_19_20_30March2023.tif'}, '19/04/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block_15_16_17_18_75m_19April.tif'}}, 'timestamps': ['19/04/23', '29/03/23', '23/02/23']}\n",
+                        "10 {'block_id': '10', 'farm_id': '2', 'block_name': 'Block_18', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block18.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/block 15b_16b_17b_18_21feb2023_75m.tif'}, '29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block15b_partof16_18_17b_19_20_30March2023.tif'}, '19/04/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block_15_16_17_18_75m_19April.tif'}}, 'timestamps': ['19/04/23', '29/03/23', '23/02/23']}\n",
                         "11 {'block_id': '11', 'farm_id': '4', 'block_name': 'Block_20', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block20.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block19_20_75.6m_21Feb2023.tif'}, '29/03/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block15b_partof16_18_17b_19_20_30March2023.tif'}}, 'timestamps': ['29/03/23', '23/02/23']}\n",
                         "12 {'block_id': '12', 'farm_id': '1', 'block_name': 'Block_26a', 'vegetation_type': 'plant', 'crop_name': '', 'yield': '', 'shp': './assets/DroneAssets/dronedata/block_files/AllShapeFiles/block26.shp', 'data_path': {'23/02/23': {'drone_18': '', 'drone_37': '', 'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 26A_75m-21Feb2023.tif'}}, 'timestamps': ['23/02/23']}\n"
                     ]
                 }
             ],
             "source": [
                 "#Iterating through all the farms\n",
@@ -121,106 +186,30 @@
                 "#Iterating through all the blocks\n",
                 "for block_id, block in all_data.blocks.items():\n",
                 "    print(block_id, block.info)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'1': {'owner': 'vikram_farm_1',\n",
-                            "  'area': None,\n",
-                            "  'data_path': {'23/02/23': {'drone_18': '',\n",
-                            "    'drone_37': '',\n",
-                            "    'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 26A_75m-21Feb2023.tif'}},\n",
-                            "  'farm_id': '1',\n",
-                            "  'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'},\n",
-                            " '2': {'owner': 'vikram_farm_2',\n",
-                            "  'area': None,\n",
-                            "  'data_path': {'23/02/23': {'drone_18': '',\n",
-                            "    'drone_37': '',\n",
-                            "    'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/block 15b_16b_17b_18_21feb2023_75m.tif'}},\n",
-                            "  'farm_id': '2',\n",
-                            "  'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'},\n",
-                            " '3': {'owner': 'vikram_farm_3',\n",
-                            "  'area': None,\n",
-                            "  'data_path': {'23/02/23': {'drone_18': '',\n",
-                            "    'drone_37': '',\n",
-                            "    'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 11_12_13_21Feb2023_75m.tif'}},\n",
-                            "  'farm_id': '3',\n",
-                            "  'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'},\n",
-                            " '4': {'owner': 'vikram_farm_4',\n",
-                            "  'area': None,\n",
-                            "  'data_path': {'23/02/23': {'drone_18': '',\n",
-                            "    'drone_37': '',\n",
-                            "    'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block19_20_75.6m_21Feb2023.tif'}},\n",
-                            "  'farm_id': '4',\n",
-                            "  'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'},\n",
-                            " '5': {'owner': 'vikram_farm_5',\n",
-                            "  'area': None,\n",
-                            "  'data_path': {'23/02/23': {'drone_18': '',\n",
-                            "    'drone_37': '',\n",
-                            "    'drone_75': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 3a_3b_75.6m_21Feb2023.tif'}},\n",
-                            "  'farm_id': '5',\n",
-                            "  'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'},\n",
-                            " '6': {'owner': 'vikram_farm_6',\n",
-                            "  'area': None,\n",
-                            "  'data_path': {'29/03/23': {'drone_18': '',\n",
-                            "    'drone_37': '',\n",
-                            "    'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block15b_partof16_18_17b_19_20_30March2023.tif'}},\n",
-                            "  'farm_id': '6',\n",
-                            "  'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'},\n",
-                            " '7': {'owner': 'vikram_farm_7',\n",
-                            "  'area': None,\n",
-                            "  'data_path': {'29/03/23': {'drone_18': '',\n",
-                            "    'drone_37': '',\n",
-                            "    'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block3a_75m_29March2023.tif'}},\n",
-                            "  'farm_id': '7',\n",
-                            "  'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'},\n",
-                            " '8': {'owner': 'vikram_farm_8',\n",
-                            "  'area': None,\n",
-                            "  'data_path': {'29/03/23': {'drone_18': '',\n",
-                            "    'drone_37': '',\n",
-                            "    'drone_75': './assets/DroneAssets/dronedata/farm_files/images/29_march_2023/Block 3b_75m_29March2023.tif'}},\n",
-                            "  'farm_id': '8',\n",
-                            "  'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'},\n",
-                            " '9': {'owner': 'vikram_farm_9',\n",
-                            "  'area': None,\n",
-                            "  'data_path': {'19/04/23': {'drone_18': '',\n",
-                            "    'drone_37': '',\n",
-                            "    'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block3a_75m19April2023.tif'}},\n",
-                            "  'farm_id': '9',\n",
-                            "  'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'},\n",
-                            " '10': {'owner': 'vikram_farm_10',\n",
-                            "  'area': None,\n",
-                            "  'data_path': {'19/04/23': {'drone_18': '',\n",
-                            "    'drone_37': '',\n",
-                            "    'drone_75': './assets/DroneAssets/dronedata/farm_files/images/19_april_2023/Block_15_16_17_18_75m_19April.tif'}},\n",
-                            "  'farm_id': '10',\n",
-                            "  'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'},\n",
-                            " '11': {'owner': 'vikram_farm_11',\n",
-                            "  'area': None,\n",
-                            "  'data_path': {'23/02/23': {'drone_18': '',\n",
-                            "    'drone_37': './assets/DroneAssets/dronedata/farm_files/images/21_feb_2023/Block 17b_18_37.8m_21feb2023.tif',\n",
-                            "    'drone_75': ''}},\n",
-                            "  'farm_id': '11',\n",
-                            "  'shp': './assets/DroneAssets/satellitedata/farm_files/shp_files/Vikram_Farm_CNH.shp'}}"
+                            "['drone_75']"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "all_data.farms_info"
+                "all_data.blocks['1'].get_modalities_for_times('23/02/23')"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

