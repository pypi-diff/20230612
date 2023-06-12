# Comparing `tmp/hiveviewer-0.0.1.tar.gz` & `tmp/hiveviewer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiveviewer-0.0.1.tar", last modified: Wed Jun  7 09:06:09 2023, max compression
+gzip compressed data, was "hiveviewer-0.0.2.tar", last modified: Mon Jun 12 09:03:31 2023, max compression
```

## Comparing `hiveviewer-0.0.1.tar` & `hiveviewer-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-07 09:06:09.619317 hiveviewer-0.0.1/
--rw-r--r--   0 yin        (501) staff       (20)     1066 2023-05-23 06:48:39.000000 hiveviewer-0.0.1/LICENSE
--rw-r--r--   0 yin        (501) staff       (20)      441 2023-06-07 09:06:09.619185 hiveviewer-0.0.1/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)       13 2023-05-23 07:30:53.000000 hiveviewer-0.0.1/README.md
--rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.0.1/pyproject.toml
--rw-r--r--   0 yin        (501) staff       (20)       38 2023-06-07 09:06:09.619375 hiveviewer-0.0.1/setup.cfg
--rw-r--r--   0 yin        (501) staff       (20)     1021 2023-06-07 08:47:41.000000 hiveviewer-0.0.1/setup.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-07 09:06:09.612487 hiveviewer-0.0.1/src/
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-07 09:06:09.613860 hiveviewer-0.0.1/src/hiveviewer/
--rw-r--r--   0 yin        (501) staff       (20)      105 2023-06-01 05:57:50.000000 hiveviewer-0.0.1/src/hiveviewer/__init__.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-07 09:06:09.616008 hiveviewer-0.0.1/src/hiveviewer/dataloader/
--rw-r--r--   0 yin        (501) staff       (20)      108 2023-05-26 07:50:46.000000 hiveviewer-0.0.1/src/hiveviewer/dataloader/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)      544 2023-06-01 03:08:59.000000 hiveviewer-0.0.1/src/hiveviewer/dataloader/base.py
--rw-r--r--   0 yin        (501) staff       (20)     2994 2023-06-01 11:55:05.000000 hiveviewer-0.0.1/src/hiveviewer/dataloader/load_csv.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-07 09:06:09.616533 hiveviewer-0.0.1/src/hiveviewer/evaluation/
--rw-r--r--   0 yin        (501) staff       (20)       70 2023-06-01 05:57:50.000000 hiveviewer-0.0.1/src/hiveviewer/evaluation/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     2781 2023-06-05 12:52:22.000000 hiveviewer-0.0.1/src/hiveviewer/evaluation/calculate_auc.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-07 09:06:09.617572 hiveviewer-0.0.1/src/hiveviewer/sampling/
--rw-r--r--   0 yin        (501) staff       (20)      106 2023-05-25 06:14:02.000000 hiveviewer-0.0.1/src/hiveviewer/sampling/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)      667 2023-06-01 11:26:56.000000 hiveviewer-0.0.1/src/hiveviewer/sampling/base.py
--rw-r--r--   0 yin        (501) staff       (20)     2346 2023-06-01 11:45:32.000000 hiveviewer-0.0.1/src/hiveviewer/sampling/gini_sampler.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-07 09:06:09.618889 hiveviewer-0.0.1/src/hiveviewer/visualization/
--rw-r--r--   0 yin        (501) staff       (20)      173 2023-06-07 08:22:08.000000 hiveviewer-0.0.1/src/hiveviewer/visualization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     8779 2023-06-05 12:59:16.000000 hiveviewer-0.0.1/src/hiveviewer/visualization/lorenz_curve.py
--rw-r--r--   0 yin        (501) staff       (20)     3364 2023-06-07 08:27:13.000000 hiveviewer-0.0.1/src/hiveviewer/visualization/plot_trisurf.py
--rw-r--r--   0 yin        (501) staff       (20)     7857 2023-06-06 02:57:11.000000 hiveviewer-0.0.1/src/hiveviewer/visualization/venn.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-07 09:06:09.614857 hiveviewer-0.0.1/src/hiveviewer.egg-info/
--rw-r--r--   0 yin        (501) staff       (20)      441 2023-06-07 09:06:09.000000 hiveviewer-0.0.1/src/hiveviewer.egg-info/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)      724 2023-06-07 09:06:09.000000 hiveviewer-0.0.1/src/hiveviewer.egg-info/SOURCES.txt
--rw-r--r--   0 yin        (501) staff       (20)        1 2023-06-07 09:06:09.000000 hiveviewer-0.0.1/src/hiveviewer.egg-info/dependency_links.txt
--rw-r--r--   0 yin        (501) staff       (20)      119 2023-06-07 09:06:09.000000 hiveviewer-0.0.1/src/hiveviewer.egg-info/requires.txt
--rw-r--r--   0 yin        (501) staff       (20)       11 2023-06-07 09:06:09.000000 hiveviewer-0.0.1/src/hiveviewer.egg-info/top_level.txt
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.078255 hiveviewer-0.0.2/
+-rw-r--r--   0 yin        (501) staff       (20)     1066 2023-05-23 06:48:39.000000 hiveviewer-0.0.2/LICENSE
+-rw-r--r--   0 yin        (501) staff       (20)     1130 2023-06-12 09:03:31.078126 hiveviewer-0.0.2/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)      702 2023-06-07 09:53:26.000000 hiveviewer-0.0.2/README.md
+-rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.0.2/pyproject.toml
+-rw-r--r--   0 yin        (501) staff       (20)       38 2023-06-12 09:03:31.078307 hiveviewer-0.0.2/setup.cfg
+-rw-r--r--   0 yin        (501) staff       (20)      988 2023-06-12 09:03:28.000000 hiveviewer-0.0.2/setup.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.073349 hiveviewer-0.0.2/src/
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.074495 hiveviewer-0.0.2/src/hiveviewer/
+-rw-r--r--   0 yin        (501) staff       (20)      105 2023-06-01 05:57:50.000000 hiveviewer-0.0.2/src/hiveviewer/__init__.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.075979 hiveviewer-0.0.2/src/hiveviewer/dataloader/
+-rw-r--r--   0 yin        (501) staff       (20)      159 2023-06-08 09:03:04.000000 hiveviewer-0.0.2/src/hiveviewer/dataloader/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     3026 2023-06-08 09:05:52.000000 hiveviewer-0.0.2/src/hiveviewer/dataloader/base.py
+-rw-r--r--   0 yin        (501) staff       (20)      529 2023-06-12 08:50:25.000000 hiveviewer-0.0.2/src/hiveviewer/dataloader/load_csv.py
+-rw-r--r--   0 yin        (501) staff       (20)      522 2023-06-08 09:04:37.000000 hiveviewer-0.0.2/src/hiveviewer/dataloader/load_excel.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.076501 hiveviewer-0.0.2/src/hiveviewer/evaluation/
+-rw-r--r--   0 yin        (501) staff       (20)       70 2023-06-01 05:57:50.000000 hiveviewer-0.0.2/src/hiveviewer/evaluation/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     2781 2023-06-05 12:52:22.000000 hiveviewer-0.0.2/src/hiveviewer/evaluation/calculate_auc.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.077019 hiveviewer-0.0.2/src/hiveviewer/sampling/
+-rw-r--r--   0 yin        (501) staff       (20)      106 2023-05-25 06:14:02.000000 hiveviewer-0.0.2/src/hiveviewer/sampling/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)      667 2023-06-01 11:26:56.000000 hiveviewer-0.0.2/src/hiveviewer/sampling/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     2346 2023-06-01 11:45:32.000000 hiveviewer-0.0.2/src/hiveviewer/sampling/gini_sampler.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.077891 hiveviewer-0.0.2/src/hiveviewer/visualization/
+-rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.0.2/src/hiveviewer/visualization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     8779 2023-06-12 09:02:43.000000 hiveviewer-0.0.2/src/hiveviewer/visualization/lorenz_curve.py
+-rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.0.2/src/hiveviewer/visualization/plot_trisurf.py
+-rw-r--r--   0 yin        (501) staff       (20)     3929 2023-06-08 08:44:36.000000 hiveviewer-0.0.2/src/hiveviewer/visualization/venn2.py
+-rw-r--r--   0 yin        (501) staff       (20)     6601 2023-06-12 09:00:24.000000 hiveviewer-0.0.2/src/hiveviewer/visualization/venn3.py
+-rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.0.2/src/hiveviewer/visualization/venn_base.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-06-12 09:03:31.075258 hiveviewer-0.0.2/src/hiveviewer.egg-info/
+-rw-r--r--   0 yin        (501) staff       (20)     1130 2023-06-12 09:03:31.000000 hiveviewer-0.0.2/src/hiveviewer.egg-info/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)      845 2023-06-12 09:03:31.000000 hiveviewer-0.0.2/src/hiveviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yin        (501) staff       (20)        1 2023-06-12 09:03:31.000000 hiveviewer-0.0.2/src/hiveviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yin        (501) staff       (20)       75 2023-06-12 09:03:31.000000 hiveviewer-0.0.2/src/hiveviewer.egg-info/requires.txt
+-rw-r--r--   0 yin        (501) staff       (20)       11 2023-06-12 09:03:31.000000 hiveviewer-0.0.2/src/hiveviewer.egg-info/top_level.txt
```

### Comparing `hiveviewer-0.0.1/LICENSE` & `hiveviewer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.0.1/setup.py` & `hiveviewer-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 SETUP_DIRECTORY = Path(__file__).resolve().parent
 
 with (SETUP_DIRECTORY / "README.md").open() as ifs:
     LONG_DESCRIPTION = ifs.read()
 
 install_requires = (
     [
-        "pandas==2.0.1",
-        "numpy==1.24.3",
-        "matplotlib==3.7.1",
-        "imageio==2.29.0",
-        "tqdm==4.65.0",
-        "scikit-learn==1.2.2",
-        "matplotlib_venn==0.11.9",
+        "pandas",
+        "numpy",
+        "matplotlib",
+        "imageio",
+        "tqdm",
+        "scikit-learn",
+        "matplotlib_venn",
+        "openpyxl",
     ],
 )
 
 setup(
     name="hiveviewer",
-    version="0.0.1",
+    version="0.0.2",
     author="Yin Cheng",
     author_email="yin.sjtu@gmail.com",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/yinsn/hiveviewer",
     python_requires=">=3.7",
-    description='Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.',
+    description="Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=install_requires,
     include_package_data=True,
 )
```

### Comparing `hiveviewer-0.0.1/src/hiveviewer/dataloader/load_csv.py` & `hiveviewer-0.0.2/src/hiveviewer/dataloader/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import os
-from typing import Optional
+from abc import ABC, abstractmethod
+from typing import Optional, Tuple
 
 import pandas as pd
 
-from .base import BaseDataLoader
 
+class BaseDataLoader(ABC):
+    """Base class for data loaders."""
 
-class CSVLoader(BaseDataLoader):
-    "CSVLoader class for loading CSV files"
-
-    def __init__(self, file_path: str, **kwargs: str):
-        super().__init__(file_path, **kwargs)
-        self.column_name_spliting()
-
-    def load_data(self) -> Optional[pd.DataFrame]:
-        """Load data from CSV file."""
-        file_url = os.path.join(self.file_path, self.file_name) + ".csv"
-        return pd.read_csv(file_url, low_memory=False)
+    def __init__(self, file_path: str, file_name: str, file_type: str = "csv") -> None:
+        self.file_path = file_path
+        self.file_type = file_type
+        self.file_name = file_name
+        self.df = self.load_data()
+
+    @abstractmethod
+    def load_data(self) -> pd.DataFrame:
+        """Load data from file."""
+        raise NotImplementedError("load_data() not implemented")
 
     def column_name_spliting(self, delimiter: str = ".") -> None:
         """Split column names by delimiter."""
         columns = []
         if self.df is not None:
             for column in self.df.columns:
                 columns.append(column.split(delimiter)[-1])
@@ -73,22 +73,22 @@
         valid_df = df[df[user_column].isin(valid_users)].copy()
         valid_df.reset_index(drop=True, inplace=True)
         return valid_df
 
     @staticmethod
     def clip_clean_count_with_group(
         df: pd.DataFrame, groupby: str, clip_column: str, label_column: str
-    ) -> tuple:
+    ) -> Tuple:
         """Clip and count with group.
 
         :param df: dataframe
         :param groupby: groupby column
         :param clip_column: column to clip
         :param label_column: label column
         """
-        df_clean = CSVLoader.clean_one_label_users(
+        df_clean = BaseDataLoader.clean_one_label_users(
             df=df, user_column=groupby, label_column=label_column
         )
-        counts_df = CSVLoader.clip_and_sum_with_group(
+        counts_df = BaseDataLoader.clip_and_sum_with_group(
             df=df_clean, groupby=groupby, clip_column=clip_column
         )
         return df_clean, counts_df
```

### Comparing `hiveviewer-0.0.1/src/hiveviewer/evaluation/calculate_auc.py` & `hiveviewer-0.0.2/src/hiveviewer/evaluation/calculate_auc.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.0.1/src/hiveviewer/sampling/base.py` & `hiveviewer-0.0.2/src/hiveviewer/sampling/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.0.1/src/hiveviewer/sampling/gini_sampler.py` & `hiveviewer-0.0.2/src/hiveviewer/sampling/gini_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.0.1/src/hiveviewer/visualization/lorenz_curve.py` & `hiveviewer-0.0.2/src/hiveviewer/visualization/lorenz_curve.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.0.1/src/hiveviewer/visualization/plot_trisurf.py` & `hiveviewer-0.0.2/src/hiveviewer/visualization/plot_trisurf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 import matplotlib.patches as mpatches
 import numpy as np
 from matplotlib import pyplot as plt
 
 
 class TrisurfPloter:
     """TrisurfPloter class for plotting trisurf."""
 
     def __init__(
         self,
-        surf_data_group: List[tuple[np.ndarray, np.ndarray, np.ndarray]],
+        surf_data_group: List[Tuple[np.ndarray, np.ndarray, np.ndarray]],
         surf_labels: List[str],
         xyz_labels: List[str],
         cmap_colors: List[str] = ["Blues", "Greens", "Oranges"],
         alphas: List[float] = [0.5, 0.6, 0.7],
         legend_loc: str = "lower center",
-        view_init: tuple[float, float] = (10, 35),
+        view_init: Tuple[float, float] = (10, 35),
         save_fig: bool = False,
         file_tag: Optional[float] = None,
         file_type: str = "pdf",
     ) -> None:
         """Initialize TrisurfPloter.
 
         :param surf_data_group: surf data group
```

### Comparing `hiveviewer-0.0.1/src/hiveviewer/visualization/venn.py` & `hiveviewer-0.0.2/src/hiveviewer/visualization/venn3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,39 @@
 import os
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 import imageio
 import matplotlib.pyplot as plt
 import pandas as pd
 from matplotlib_venn import venn3
 
+from .venn_base import BaseVennPloter
 
-class VennPloter:
+
+class Venn3Ploter(BaseVennPloter):
     """
-    Class to plot venn diagrams
+    Class to plot a venn diagram with 4 groups
     """
 
     def __init__(
         self, dataframe: pd.DataFrame, column1_name: str, column2_name: str
     ) -> None:
-        """
-        dataframe: dataframe to plot
-        column1_name: name of the first column
-        column2_name: name of the second column
-        """
-        self.df = dataframe
-        self.column1_name = column1_name
-        self.column2_name = column2_name
-        self.column1_data = dataframe[column1_name]
-        self.column2_data = dataframe[column2_name]
-        self.df_len = len(dataframe)
+        super().__init__(dataframe, column1_name, column2_name)
 
-    def get_conditions(self) -> tuple:
+    def get_conditions(self) -> Tuple:
         """
         Returns the conditions for the venn diagram
         """
         both0 = (self.column1_data == 0) & (self.column2_data == 0)
         only_column1 = (self.column1_data == 1) & (self.column2_data == 0)
         only_column2 = (self.column1_data == 0) & (self.column2_data == 1)
         both1 = (self.column1_data == 1) & (self.column2_data == 1)
         return (both0, only_column1, only_column2, both1)
 
-    def get_group_count_ratios(self) -> tuple:
+    def get_group_count_ratios(self) -> Tuple:
         """
         Returns the ratios of the groups based on the count
         """
         both0, only_column1, only_column2, both1 = self.get_conditions()
         both0_ratio = sum(both0) / self.df_len
         only_column1_ratio = sum(only_column1) / self.df_len
         only_column2_ratio = sum(only_column2) / self.df_len
@@ -49,15 +41,15 @@
         return (both0_ratio, only_column1_ratio, only_column2_ratio, both1_ratio)
 
     def get_group_value_ratios(
         self,
         value_column_name: str,
         lower_bound: Optional[float] = None,
         upper_bound: Optional[float] = None,
-    ) -> tuple:
+    ) -> Tuple:
         """
         Returns the ratios of the groups based on the value
 
         value_column_name: name of the column with the values
         lower_bound: lower bound of the values
         upper_bound: upper bound of the values
         """
@@ -149,45 +141,14 @@
                     transform=plt.gca().transAxes,
                     fontsize=10,
                     verticalalignment="top",
                 )
                 file_name = f"ratio_venn_{file_tag}.{file_type}"
             plt.savefig(file_name, format=file_type)
 
-    def plot_count_ratio_venn(self) -> None:
-        """
-        Plots the venn diagram with the count ratios
-        """
-        ratios = self.get_group_count_ratios()
-        self.plot_ratio_venn(ratios)
-
-    def plot_value_ratio_venn(
-        self,
-        value_column_name: str,
-        lower_bound: Optional[float] = None,
-        upper_bound: Optional[float] = None,
-        save_fig: bool = False,
-        file_type: str = "pdf",
-    ) -> None:
-        """
-        Plots the venn diagram with the value ratios
-
-        value_column_name: name of the column with the values
-        lower_bound: lower bound of the values
-        upper_bound: upper bound of the values
-        save_fig: whether to save the figure
-        """
-
-        ratios = self.get_group_value_ratios(
-            value_column_name, lower_bound=lower_bound, upper_bound=upper_bound
-        )
-        self.plot_ratio_venn(
-            ratios, save_fig=save_fig, file_tag=upper_bound, file_type=file_type
-        )
-
     def plot_value_ratio_venn_with_upper_bounds(
         self,
         value_column_name: str,
         upper_bounds: List[float],
         duration: Optional[int] = 300,
     ) -> None:
         filenames: List[str] = []
```

### Comparing `hiveviewer-0.0.1/src/hiveviewer.egg-info/SOURCES.txt` & `hiveviewer-0.0.2/src/hiveviewer.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 src/hiveviewer.egg-info/SOURCES.txt
 src/hiveviewer.egg-info/dependency_links.txt
 src/hiveviewer.egg-info/requires.txt
 src/hiveviewer.egg-info/top_level.txt
 src/hiveviewer/dataloader/__init__.py
 src/hiveviewer/dataloader/base.py
 src/hiveviewer/dataloader/load_csv.py
+src/hiveviewer/dataloader/load_excel.py
 src/hiveviewer/evaluation/__init__.py
 src/hiveviewer/evaluation/calculate_auc.py
 src/hiveviewer/sampling/__init__.py
 src/hiveviewer/sampling/base.py
 src/hiveviewer/sampling/gini_sampler.py
 src/hiveviewer/visualization/__init__.py
 src/hiveviewer/visualization/lorenz_curve.py
 src/hiveviewer/visualization/plot_trisurf.py
-src/hiveviewer/visualization/venn.py
+src/hiveviewer/visualization/venn2.py
+src/hiveviewer/visualization/venn3.py
+src/hiveviewer/visualization/venn_base.py
```

