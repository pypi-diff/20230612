# Comparing `tmp/krisi-1.0.1.tar.gz` & `tmp/krisi-1.1.0.tar.gz`

## Comparing `krisi-1.0.1.tar` & `krisi-1.1.0.tar`

### file list

```diff
@@ -1,50 +1,54 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-1.0.1/.flake8
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-1.0.1/.isort.cfg
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 krisi-1.0.1/mkdocs.yaml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-1.0.1/.vscode/launch.json
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 krisi-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 krisi-1.0.1/dev_utils/generate_from_examples.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 krisi-1.0.1/dev_utils/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/analyse/__init__.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/analyse/correlations.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/analyse/dataset.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/analyse/utils.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/assertions.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/compare.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/group.py
--rw-r--r--   0        0        0     8367 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/metric.py
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/score.py
--rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/scorecard.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/type.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/utils.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/library/__init__.py
--rw-r--r--   0        0        0     6642 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/library/default_metrics_classification.py
--rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/library/default_metrics_regression.py
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/library/diagrams.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/evaluate/library/metric_wrappers.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/__init__.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/console.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/graph.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/interactive.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/pdf.py
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/report.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/type.py
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/vizualise.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/library/console/diagrams.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/library/pdf_layouts/scorecard/report.css
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/report/library/pdf_layouts/scorecard/report.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/console_plot.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/data.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/environment.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/io.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/iterable_helpers.py
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/printing.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 krisi-1.0.1/src/krisi/utils/devutils/timing.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-1.0.1/.gitignore
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-1.0.1/LICENSE
--rw-r--r--   0        0        0    61743 2020-02-02 00:00:00.000000 krisi-1.0.1/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 krisi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    66529 2020-02-02 00:00:00.000000 krisi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-1.1.0/.flake8
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-1.1.0/.isort.cfg
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 krisi-1.1.0/mkdocs.yaml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-1.1.0/.vscode/launch.json
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 krisi-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/analyse/__init__.py
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/analyse/correlations.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/analyse/dataset.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/analyse/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/__init__.py
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/assertions.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/compare.py
+-rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/group.py
+-rw-r--r--   0        0        0    13942 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/metric.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/score.py
+-rw-r--r--   0        0        0    23731 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/scorecard.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/type.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/utils.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/library/__init__.py
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/library/benchmarking.py
+-rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/library/default_metrics_classification.py
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/library/default_metrics_regression.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/library/diagrams.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/evaluate/library/metric_wrappers.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/__init__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/console.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/graph.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/interactive.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/pdf.py
+-rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/report.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/type.py
+-rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/vizualise.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/library/console/diagrams.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.css
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.html
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/console_plot.py
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/data.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/enums.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/environment.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/io.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/iterable_helpers.py
+-rw-r--r--   0        0        0     6973 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/printing.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/state.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/devutils/environment_checks.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/devutils/generate_from_examples.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/devutils/timing.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 krisi-1.1.0/src/krisi/utils/devutils/type.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-1.1.0/.gitignore
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-1.1.0/LICENSE
+-rw-r--r--   0        0        0    61727 2020-02-02 00:00:00.000000 krisi-1.1.0/README.md
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 krisi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    66463 2020-02-02 00:00:00.000000 krisi-1.1.0/PKG-INFO
```

### Comparing `krisi-1.0.1/mkdocs.yaml` & `krisi-1.1.0/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `krisi-1.0.1/.vscode/settings.json` & `krisi-1.1.0/.vscode/settings.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'python.testing.pytestArgs'": "{insert: [(1, '-s')]}"}*

```diff
@@ -9,15 +9,16 @@
         "black"
     ],
     "python.analysis.typeCheckingMode": "basic",
     "python.formatting.provider": "black",
     "python.languageServer": "Pylance",
     "python.linting.enabled": true,
     "python.testing.pytestArgs": [
-        "tests"
+        "tests",
+        "-s"
     ],
     "python.testing.pytestEnabled": true,
     "python.testing.unittestEnabled": false,
     "terminal.integrated.env.osx": {
         "PYTHONPATH": "${workspaceFolder}"
     }
 }
```

### Comparing `krisi-1.0.1/src/krisi/analyse/correlations.py` & `krisi-1.1.0/src/krisi/analyse/correlations.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import matplotlib.pyplot as plt
 import pandas as pd
 from typing_extensions import Literal
 
 from krisi.evaluate.type import PathConst
 from krisi.report.graph import create_save_graphs
+from krisi.utils.state import RunType, get_global_state
 
 from .utils import corr_without_symmetry, unroll
 
 
 def get_mean_corr_matrix(df_rolled_corr: List[pd.DataFrame]) -> pd.DataFrame:
     df_rolled_summed = reduce(lambda x, y: x.add(y, fill_value=0), df_rolled_corr)
     df_rolled_mean = df_rolled_summed / len(df_rolled_corr)
@@ -84,15 +85,16 @@
     result.index.name = title
     print(result)
 
     if "save" in save_or_display:
         path_friendly = title.replace(" ", "_")
         plt.savefig(f"{save_location}/{path_friendly}.png", format="PNG")
     if "display" in save_or_display:
-        plt.show()
+        if not get_global_state().run_type == RunType.test:
+            plt.show()
 
 
 def get_rolled_corr_metrics(
     df: pd.DataFrame,
     window: int,
     step: int = 1,
 ) -> Tuple[pd.DataFrame, pd.Series, pd.Series]:
```

### Comparing `krisi-1.0.1/src/krisi/analyse/dataset.py` & `krisi-1.1.0/src/krisi/analyse/dataset.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.1/src/krisi/evaluate/assertions.py` & `krisi-1.1.0/src/krisi/evaluate/assertions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from typing import Any, Iterable, List, Tuple, Union
+from typing import Any, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from typing_extensions import get_args, get_origin
 
-from krisi.evaluate.type import Predictions, Targets
+from krisi.evaluate.metric import Metric
+from krisi.evaluate.type import DatasetType, Predictions, Targets, Weights
 from krisi.utils.iterable_helpers import flatten, isiterable
 
 valid_types = ["int64", "float64", "float32", "float", "int"]
 
 
 def get_bad_types(iterable: Union[Targets, Predictions]) -> Iterable:
     return [x for x in iterable if type(x) not in valid_types]
@@ -25,18 +26,30 @@
         return add_list + [flatten_type(type_) for type_ in get_args(complex_type)]
 
 
 def unpack_type(complex_type: Any) -> Tuple[Any]:
     return tuple(flatten(flatten_type(complex_type)))
 
 
-def check_valid_pred_target(y: Targets, predictions: Predictions):
+def check_no_duplicate_metrics(metrics: List[Metric]):
+    assert len(metrics) == len(
+        set([metric.key for metric in metrics])
+    ), f"Duplicate metric key found in {metrics}. Please remove the duplicates."
+
+
+def check_valid_pred_target(
+    y: Targets, predictions: Predictions, sample_weights: Optional[Weights]
+):
     assert len(y) == len(
         predictions
     ), f"Target length {len(y)} should match predictions length {len(predictions)}"
+    if sample_weights is not None:
+        assert len(y) == len(
+            sample_weights
+        ), f"Target length {len(y)} should match sample_weights length {len(sample_weights)}"
 
     assert isinstance(
         y, unpack_type(Targets)
     ), f"Targets: {type(y)} are not of a valid type."
     assert isinstance(
         predictions, unpack_type(Predictions)
     ), f"Predictions: {type(predictions)} are not of a valid type."
@@ -54,20 +67,31 @@
             dtype_name = list(types)[0]
 
         assert (
             dtype_name in valid_types
         ), f"{iterable} contains at least one invalid type. {get_bad_types(iterable)}"
 
 
-def is_dataset_classification_like(y: Targets):
+def infer_dataset_type(y: Targets) -> DatasetType:
     # TODO: Should work with booleans
-    # TODO: Create multilabel heuristic to be passed on to ScoreCard
+    def infer_exact_type(is_classification: bool, y: Targets) -> DatasetType:
+        if is_classification is False:
+            return DatasetType.regression
+        if len(set(y)) == 2:
+            return DatasetType.classification_binary
+        else:
+            return DatasetType.classification_multiclass
+
     if isinstance(y, pd.Series):
-        return pd.api.types.is_integer_dtype(y)
-    elif isinstance(y, np.ndarray):
+        y = y.to_numpy()
+    if isinstance(y, np.ndarray):
         if hasattr(y[0], "is_integer"):
             # Using this is faster, if available use this.
-            return all([i.is_integer() for i in y if i is not None])
+            return infer_exact_type(
+                all([i.is_integer() for i in y if i is not None]), y
+            )
         else:
-            return np.all(np.mod(y, 1) == 0)
+            return infer_exact_type(np.all(np.mod(y, 1) == 0), y)
     else:
-        return all([isinstance(i, int) for i in y if i is not None])
+        return infer_exact_type(
+            all([isinstance(i, int) for i in y if i is not None]), y
+        )
```

### Comparing `krisi-1.0.1/src/krisi/evaluate/compare.py` & `krisi-1.1.0/src/krisi/evaluate/compare.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.1/src/krisi/evaluate/score.py` & `krisi-1.1.0/src/krisi/evaluate/score.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-from typing import Any, Dict, List, Optional, Tuple, Union
-
-import pandas as pd
+from typing import Any, Dict, List, Optional, Union
 
 from krisi.evaluate.metric import Metric
 from krisi.evaluate.scorecard import ScoreCard
 from krisi.evaluate.type import (
     Calculation,
+    DatasetType,
     Predictions,
     Probabilities,
     SampleTypes,
     Targets,
+    Weights,
 )
 
 
 def score(
     y: Targets,
     predictions: Predictions,
     probabilities: Optional[Probabilities] = None,
+    sample_weight: Optional[Weights] = None,
     model_name: Optional[str] = None,
     dataset_name: Optional[str] = None,
     project_name: Optional[str] = None,
     default_metrics: Optional[List[Metric]] = None,
     custom_metrics: Optional[List[Metric]] = None,
-    classification: Optional[bool] = None,
+    dataset_type: Optional[Union[DatasetType, str]] = None,
     sample_type: SampleTypes = SampleTypes.outofsample,
     calculation: Union[Calculation, str] = Calculation.single,
     rolling_args: Optional[Dict[str, Any]] = None,
+    surpress_warnings: bool = False,
     **kwargs,
 ) -> ScoreCard:
     """
     Creates a ScoreCard based on the passed in arguments, evaluates and then returns the ScoreCard.
 
     Parameters
     ----------
@@ -44,16 +46,16 @@
     project_name: Optional[str]
         The name of the project. Used for reporting and saving to a directory (eg.: multiple scorecards)
     default_metrics: Optional[List[Metric]]
         Default metrics that get evaluated. See `library`.
     custom_metrics: Optional[List[Metric]]
         Custom metrics that get evaluated. If specified it will evaluate these after `default_metric`
         See `library`.
-    classification: Optional[bool]
-        Whether the task was classifiction of regression. If set to `None` it will guess from the targets.
+    dataset_type: Optional[Union[DatasetType, str]]
+        Whether the task was a binar/multi-label classifiction of regression. If set to `None` it will infer from the target.
     sample_type: SampleTypes = SampleTypes.outofsample
         Whether we should evaluate it on insample or out of sample.
 
             - `SampleTypes.outofsample`
             - `SampleTypes.insample`
     calculation : Union[Calculation, str], optional
         Whether it should evaluate `Metrics` on a rolling basis or on the whole prediction or both, by default Calculation.single
@@ -74,77 +76,38 @@
         The ScoreCard Evaluated
 
     Raises
     ------
     ValueError
         If Calculation type is incorrectly specified.
     """
-    if rolling_args is None:
-        rolling_args = dict(window=len(y) // 100, step=len(y) // 100)
+
+    calculation = Calculation.from_str(calculation)
 
     sc = ScoreCard(
         y=y,
         predictions=predictions,
         probabilities=probabilities,
+        sample_weight=sample_weight,
         model_name=model_name,
         dataset_name=dataset_name,
         project_name=project_name,
         sample_type=sample_type,
-        classification=classification,
+        dataset_type=dataset_type,
         default_metrics=default_metrics,
         custom_metrics=custom_metrics,
         rolling_args=rolling_args,
+        surpress_warnings=surpress_warnings,
         **kwargs,
     )
 
-    if calculation == Calculation.single or calculation == Calculation.single.value:
+    if calculation == Calculation.single:
         sc.evaluate()
-    elif calculation == Calculation.rolling or calculation == Calculation.rolling.value:
+    elif calculation == Calculation.rolling:
         sc.evaluate_over_time()
-    elif calculation == Calculation.both or calculation == Calculation.both.value:
+    elif calculation == Calculation.both:
         sc.evaluate()
         sc.evaluate_over_time()
     else:
         raise ValueError(f"Calculation type {calculation} not recognized.")
 
     return sc
-
-
-def score_in_out_of_sample(
-    y_insample: pd.Series,
-    insample_predictions: pd.Series,
-    y_outsample: pd.Series,
-    outsample_predictions: pd.Series,
-    model_name: Optional[str] = None,
-    dataset_name: Optional[str] = None,
-    project_name: Optional[str] = None,
-    default_metrics: Optional[List[Metric]] = None,
-    custom_metrics: Optional[List[Metric]] = None,
-    classification: Optional[bool] = None,
-    calculation: Union[Calculation, str] = Calculation.single,
-) -> Tuple[ScoreCard, ScoreCard]:
-    insample_summary = score(
-        y_insample,
-        insample_predictions,
-        model_name,
-        dataset_name,
-        project_name,
-        default_metrics,
-        custom_metrics,
-        classification,
-        SampleTypes.insample,
-        calculation,
-    )
-    outsample_summary = score(
-        y_outsample,
-        outsample_predictions,
-        model_name,
-        dataset_name,
-        project_name,
-        default_metrics,
-        custom_metrics,
-        classification,
-        SampleTypes.outofsample,
-        calculation,
-    )
-
-    return insample_summary, outsample_summary
```

### Comparing `krisi-1.0.1/src/krisi/evaluate/scorecard.py` & `krisi-1.1.0/src/krisi/evaluate/scorecard.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 import datetime
+import logging
 import os
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Union
 
 import pandas as pd
 from rich import print
 from typing_extensions import Literal
 
 from krisi.evaluate.assertions import (
+    check_no_duplicate_metrics,
     check_valid_pred_target,
-    is_dataset_classification_like,
+    infer_dataset_type,
 )
 from krisi.evaluate.group import Group
-from krisi.evaluate.library.default_metrics_classification import (
-    all_classification_metrics,
-)
-from krisi.evaluate.library.default_metrics_regression import all_regression_metrics
+from krisi.evaluate.library import get_default_metrics_for_dataset_type
 from krisi.evaluate.metric import Metric
 from krisi.evaluate.type import (
+    DatasetType,
     MetricCategories,
     PathConst,
     Predictions,
     PredictionsDS,
     PrintMode,
     Probabilities,
+    ProbabilitiesDF,
     SampleTypes,
     SaveModes,
     ScoreCardMetadata,
     Targets,
     TargetsDS,
+    Weights,
+    WeightsDS,
 )
 from krisi.evaluate.utils import (
     convert_to_series,
     ensure_df,
     get_save_path,
     handle_unnamed,
+    rename_probs_columns,
 )
 from krisi.report.console import (
     get_large_metric_summary,
     get_minimal_summary,
     get_summary,
 )
 from krisi.report.report import create_report_from_scorecard
 from krisi.report.type import DisplayModes, InteractiveFigure
 from krisi.utils.environment import is_notebook
 from krisi.utils.io import ensure_path, save_console, save_minimal_summary, save_object
 from krisi.utils.iterable_helpers import (
+    empty_if_None,
     flatten,
     map_newdict_on_olddict,
     remove_nans,
     replace_if_None,
     strip_builtin_functions,
     wrap_in_list,
 )
+from krisi.utils.state import RunType, get_global_state, set_global_state
+
+logger = logging.getLogger("krisi")
 
 
 class ScoreCard:
     """
     ScoreCard Object.
 
     Krisi's main object holding and evaluating metrics.
@@ -78,16 +86,16 @@
         The name of the dataset from which the `y` (targets) orginate from. Used for reporting.
     dataset_description: str = ""
         A description of the dataset from which the `y` (targets) orginate from. Used for reporting.
     project_name: Optional[str]
         The name of the project. Used for reporting and saving to a directory (eg.: multiple scorecards)
     project_description: str = ""
         A description of the project. Used for reporting.
-    classification: Optional[bool]
-        Whether the task was classifiction of regression. If set to `None` it will guess from the targets.
+    dataset_type: Optional[Union[DatasetType, str]]
+        Whether the task was a binar/multi-label classifiction of regression. If set to `None` it will infer from the target.
     sample_type: SampleTypes = SampleTypes.outofsample
         Whether we should evaluate it on insample or out of sample.
 
             - `SampleTypes.outofsample`
             - `SampleTypes.insample`
     default_metrics: Optional[List[Metric]]
         Default metrics that get evaluated. See `library`.
@@ -109,55 +117,91 @@
     ... sc.evaluate(y_pred, y_true, defaults=True) # Calculate predefined metrics
     ... sc["own_metric"] = (y_pred - y_true).mean() # Add a metric result directly
     ... sc.print()
     """
 
     y: TargetsDS
     predictions: PredictionsDS
-    probabilities: Optional[Probabilities]
+    probabilities: Optional[ProbabilitiesDF]
+    sample_weight: Optional[WeightsDS]
     sample_type: SampleTypes
     default_metrics_keys: List[str]
     custom_metrics_keys: List[str]
-    classification: bool  # TODO: Support multilabel classification
+    dataset_type: DatasetType
     metadata: ScoreCardMetadata
     rolling_args: Dict[str, Any]
 
     def __init__(
         self,
         y: Targets,
         predictions: Predictions,
         probabilities: Optional[Probabilities] = None,
+        sample_weight: Optional[Weights] = None,
         model_name: Optional[str] = None,
         model_description: str = "",
         dataset_name: Optional[str] = None,
         dataset_description: str = "",
         project_name: Optional[str] = None,
         project_description: str = "",
-        classification: Optional[bool] = None,
+        dataset_type: Optional[Union[DatasetType, str]] = None,
         sample_type: SampleTypes = SampleTypes.outofsample,
         default_metrics: Optional[List[Metric]] = None,
         custom_metrics: Optional[List[Metric]] = None,
         rolling_args: Optional[Dict[str, Any]] = None,
+        surpress_warnings: bool = False,
     ) -> None:
-        check_valid_pred_target(y, predictions)
+        if surpress_warnings:
+            state = get_global_state()
+            state.run_type = RunType.dev
+            set_global_state(state)
+
+        dataset_type = DatasetType.from_str(dataset_type) if dataset_type else None
+        check_valid_pred_target(y, predictions, sample_weight)
+        default_metrics = (
+            wrap_in_list(default_metrics) if default_metrics is not None else None
+        )
+        custom_metrics = (
+            wrap_in_list(custom_metrics) if custom_metrics is not None else None
+        )
+
+        check_no_duplicate_metrics(
+            empty_if_None(default_metrics) + empty_if_None(custom_metrics)
+        )
         self.__dict__["y"] = convert_to_series(y, "y")
         self.__dict__["predictions"] = convert_to_series(predictions, "predictions")
         self.__dict__["probabilities"] = (
-            ensure_df(probabilities, "probabilities")
+            rename_probs_columns(ensure_df(probabilities, "probabilities"))
             if probabilities is not None
             else None
         )
+        self.__dict__["sample_weight"] = (
+            convert_to_series(
+                sample_weight,  # pd.Series([1.0] * len(y))
+                "sample_weight",
+            )
+            if sample_weight is not None
+            else None
+        )
+
         self.__dict__["sample_type"] = sample_type
+        if rolling_args is None:
+            window_size = len(y) // 20  # 5% of the data
+            rolling_args = dict(
+                window=window_size,
+                step=window_size,
+                min_periods=window_size,
+                closed="left",
+            )
+            logger.info(f"rolling_args not specified, using default: {rolling_args}")
+
         self.__dict__["rolling_args"] = (
             rolling_args if rolling_args is not None else dict(window=len(y) // 100)
         )
-        self.__dict__["classification"] = (
-            is_dataset_classification_like(y)
-            if classification is None
-            else classification
+        self.__dict__["dataset_type"] = (
+            infer_dataset_type(y) if dataset_type is None else dataset_type
         )
         model_name_, dataset_name_, project_name_ = handle_unnamed(
             y, predictions, model_name, dataset_name, project_name
         )
 
         self.__dict__["metadata"] = ScoreCardMetadata(
             get_save_path(project_name_),
@@ -166,19 +210,16 @@
             model_name_,
             model_description,
             dataset_name_,
             dataset_description,
         )
 
         if default_metrics is None:
-            default_metrics = (
-                all_classification_metrics
-                if self.classification
-                else all_regression_metrics
-            )
+            self.__dict__["dataset_type"] = infer_dataset_type(y)
+            default_metrics = get_default_metrics_for_dataset_type(self.dataset_type)
 
         self.__dict__["default_metrics_keys"] = [
             metric.key for metric in default_metrics
         ]
         if custom_metrics is None:
             custom_metrics = []
 
@@ -381,47 +422,55 @@
         rolling_args: Optional[Dict[str, Any]] = dict(),
     ):
         for metric in self.get_all_metrics(defaults=defaults):
             if metric.restrict_to_sample is not self.sample_type:
                 if isinstance(metric, Group):
                     group = metric
                     for metric_in_group in getattr(group, func_key_evaluate)(
-                        self.y, self.predictions, self.probabilities, **rolling_args
+                        self.y,
+                        self.predictions,
+                        self.probabilities,
+                        self.sample_weight,
+                        **rolling_args,
                     ):
                         if metric_in_group.key not in self.__dict__:
                             metric_in_group._from_group = True
                             self[metric_in_group.key] = metric_in_group
                         else:
                             self[metric_in_group.key] = {
                                 result_key: metric_in_group.result,
                                 "_from_group": True,
                             }
                 else:
                     getattr(metric, func_key_evaluate)(
-                        self.y, self.predictions, self.probabilities, **rolling_args
+                        self.y,
+                        self.predictions,
+                        self.probabilities,
+                        self.sample_weight,
+                        **rolling_args,
                     )
+            if func_key_evaluate == "evaluate_over_time":
+                metric.evaluate_rolling_properties()
 
-    def evaluate(self, defaults: bool = True) -> "ScoreCard":
+    def evaluate(self, defaults: bool = True) -> None:
         """
         Evaluates `Metric`s present on the `ScoreCard`
 
         Parameters
         ----------
         defaults: boolean
             Wether the default `Metric`s should be evaluated or not.
 
         Returns
         -------
-        ScoreCard
+        None
         """
         self.__evaluate("evaluate", "result", defaults=defaults)
 
-        return self
-
-    def evaluate_over_time(self, defaults: bool = True) -> "ScoreCard":
+    def evaluate_over_time(self, defaults: bool = True) -> None:
         """
         Evaluates `Metric`s present on the `ScoreCard` over time, either with expanding
         or fixed sized window. Assigns list of results to `results_over_time`.
 
         Parameters
         ----------
         y: Targets = Union[np.ndarray, pd.Series, List[Union[int, float]]]
@@ -432,28 +481,29 @@
             Wether the default ``Metric``s should be evaluated or not. Default value = True
         window: int
             Size of window. If number is provided then evaluation happens on a fixed window size,
             otherwise it evaluates it on an expanding window basis.
 
         Returns
         -------
-        ScoreCard
+        None
         """
         self.__evaluate(
             "evaluate_over_time",
             "result_rolling",
             defaults=defaults,
             rolling_args={"rolling_args": self.rolling_args},
         )
-        return self
 
     def print(
         self,
         mode: Union[str, PrintMode, List[PrintMode], List[str]] = PrintMode.extended,
         with_info: bool = False,
+        with_parameters: bool = True,
+        with_diagnostics: bool = False,
         input_analysis: bool = True,
         title: Optional[str] = None,
         frame_or_series: bool = True,
     ) -> None:
         """
         Prints the ScoreCard to the console.
 
@@ -477,31 +527,41 @@
         for mode in modes:
             if mode is PrintMode.extended:
                 to_display = get_summary(
                     self,
                     repr=True,
                     categories=[el.value for el in MetricCategories],
                     with_info=with_info,
+                    with_parameters=with_parameters,
+                    with_diagnostics=with_diagnostics,
                     input_analysis=input_analysis,
                 )
 
             elif mode is PrintMode.minimal:
                 to_display = get_minimal_summary(self, dataframe=frame_or_series)
             elif mode is PrintMode.minimal_table:
-                to_display = get_large_metric_summary(self, title)
+                to_display = get_large_metric_summary(
+                    self,
+                    title,
+                    with_info=with_info,
+                    with_parameters=with_parameters,
+                    with_diagnostics=with_diagnostics,
+                )
             if isinstance(to_display, (pd.DataFrame, pd.Series)) and is_notebook():
                 from IPython.display import display
 
                 display(to_display)
             else:
                 print(to_display)
 
     def save(
         self,
         with_info: bool = False,
+        with_parameters: bool = True,
+        with_diagnostics: bool = False,
         save_modes: List[Union[SaveModes, str]] = [
             SaveModes.minimal,
             SaveModes.obj,
             SaveModes.text,
         ],
         override_base_path: Optional[Path] = None,
         timestamp_no_overwrite: bool = False,
@@ -524,15 +584,22 @@
         )
         ensure_path(path)
 
         if SaveModes.minimal in save_modes or SaveModes.minimal.value in save_modes:
             save_minimal_summary(self, path)
         if SaveModes.obj in save_modes or SaveModes.obj.value in save_modes:
             save_object(self, path)
-        save_console(self, path, with_info, save_modes)
+        save_console(
+            self,
+            path,
+            with_info,
+            with_parameters=with_parameters,
+            with_diagnostics=with_diagnostics,
+            save_modes=save_modes,
+        )
 
         return self
 
     def get_diagram_dictionary(self) -> Dict[str, InteractiveFigure]:
         diagrams = flatten(
             remove_nans([metric.get_diagrams() for metric in self.get_all_metrics()])
         )
```

### Comparing `krisi-1.0.1/src/krisi/evaluate/type.py` & `krisi-1.1.0/src/krisi/evaluate/type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,78 @@
+from __future__ import annotations
+
 import os
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from typing import Any, Callable, List, Tuple, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 
+from krisi.utils.enums import ParsableEnum
+
 MetricResult = TypeVar(
     "MetricResult", bound=Union[float, int, str, List, Tuple, pd.DataFrame, pd.Series]
 )
 
 
 Predictions = Union[np.ndarray, pd.Series, List[Union[int, float]]]
 Targets = Union[np.ndarray, pd.Series, List[Union[int, float]]]
 Probabilities = Union[np.ndarray, pd.Series, pd.DataFrame, List[Union[int, float]]]
+Weights = Union[np.ndarray, pd.Series, List[Union[int, float]]]
 PredictionsDS = pd.Series
-ProbabilitiesDS = pd.DataFrame
+ProbabilitiesDF = pd.DataFrame
 TargetsDS = pd.Series
-MetricFunctionProb = Callable[[PredictionsDS, TargetsDS, ProbabilitiesDS], MetricResult]
-MetricFunctionNoProb = Callable[
-    [PredictionsDS, TargetsDS, ProbabilitiesDS], MetricResult
+WeightsDS = pd.Series
+MetricFunctionProb = Callable[[PredictionsDS, TargetsDS, ProbabilitiesDF], MetricResult]
+MetricFunctionProbWeights = Callable[
+    [PredictionsDS, TargetsDS, ProbabilitiesDF, WeightsDS], MetricResult
+]
+MetricFunctionNoProb = Callable[[PredictionsDS, TargetsDS], MetricResult]
+MetricFunctionNoProbWeights = Callable[
+    [PredictionsDS, TargetsDS, WeightsDS], MetricResult
+]
+MetricFunction = Union[
+    MetricFunctionNoProb,
+    MetricFunctionProb,
+    MetricFunctionProbWeights,
+    MetricFunctionNoProbWeights,
 ]
-MetricFunction = Union[MetricFunctionNoProb, MetricFunctionProb]
 
 
 class MetricCategories(Enum):
     residual = "Residual Diagnostics"
     entropy = "Information Entropy"
     class_err = "Forecast Errors - Classification"
     reg_err = "Forecast Errors - Regression"
+    stats = "General Statistics"
     unknown = "Unknown"
 
 
 class SampleTypes(Enum):
     insample = "insample"
     outofsample = "outofsample"
 
 
 class Calculation(Enum):
     single = "single"
     rolling = "rolling"
     both = "both"
 
+    @staticmethod
+    def from_str(value: Union[str, Calculation]) -> Calculation:
+        if isinstance(value, Calculation):
+            return value
+        for calc in Calculation:
+            if calc.value == value:
+                return calc
+        else:
+            raise ValueError(f"Unknown Calculation: {value}")
+
 
 class SaveModes(Enum):
     svg = "svg"
     html = "html"
     text = "text"
     obj = "obj"
     minimal = "minimal"
@@ -87,21 +113,50 @@
 
 class PrintMode(Enum):
     extended = "extended"
     minimal = "minimal"
     minimal_table = "minimal_table"
 
     @staticmethod
-    def from_str(value: Union[str, "PrintMode"]) -> "PrintMode":
+    def from_str(value: Union[str, PrintMode]) -> PrintMode:
         if isinstance(value, PrintMode):
             return value
         for strategy in PrintMode:
             if strategy.value == value:
                 return strategy
         else:
             raise ValueError(f"Unknown PrintMode: {value}")
 
 
 class NamingPrefixes:
     model = "Model_"
     dataset = "Dataset_"
     project = "Project_"
+
+
+class DatasetType(Enum):
+    regression = "regression"
+    classification_binary = "classification_binary"
+    classification_multiclass = "classification_multiclass"
+
+    @staticmethod
+    def from_str(value: Union[str, DatasetType]) -> DatasetType:
+        if isinstance(value, DatasetType):
+            return value
+        for strategy in DatasetType:
+            if strategy.value == value:
+                return strategy
+        else:
+            raise ValueError(f"Unknown DatasetType: {value}")
+
+    def is_classification(self):
+        return self in [
+            DatasetType.classification_binary,
+            DatasetType.classification_multiclass,
+        ]
+
+
+class Purpose(ParsableEnum):
+    objective = "objective"
+    loss = "loss"
+    diagram = "diagram"
+    group = "group"
```

### Comparing `krisi-1.0.1/src/krisi/evaluate/utils.py` & `krisi-1.1.0/src/krisi/evaluate/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -139,7 +139,19 @@
         return df
     elif isinstance(data, list):
         df = pd.DataFrame(data)
         df.index.name = name
         return df
     else:
         raise ValueError(f"Data type {type(data)} not supported.")
+
+
+def rename_probs_columns(df: pd.DataFrame) -> pd.DataFrame:
+    if all(
+        [
+            col if isinstance(col, int) else is_int(col.split("_")[-1])
+            for col in df.columns
+        ]
+    ):
+        return df.rename(columns={col: int(col.split("_")[-1]) for col in df.columns})
+    else:
+        return df.rename(columns={col: i for i, col in enumerate(df.columns)})
```

### Comparing `krisi-1.0.1/src/krisi/evaluate/library/diagrams.py` & `krisi-1.1.0/src/krisi/evaluate/library/diagrams.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, List, Tuple
 
 import numpy as np
 import pandas as pd
+from sklearn.calibration import calibration_curve
 
 if TYPE_CHECKING:
     import plotly.graph_objects as go
 
 from statsmodels.tsa.stattools import acf, pacf
 
 from krisi.evaluate.type import MetricResult
@@ -100,33 +101,42 @@
     if not isinstance(data, pd.Series):
         data = pd.Series(data)
     fig = px.histogram(data, marginal="box")  # or violin, rug
 
     return fig
 
 
-def callibration_plot(
-    data: MetricResult, bin_size: float = 0.1, **kwargs
-) -> "go.Figure":
-    import plotly.graph_objects as go
-
+def calculate_calibration_bins(
+    data: MetricResult, n_bins: int = 10, **kwargs
+) -> Tuple[np.ndarray, np.ndarray]:
     y_true = data["y"]
     y_prob = data["probs"]
 
-    # sort probabilities and corresponding true labels in ascending order
-    order = np.argsort(y_prob)
-    y_true = y_true[order]
-    y_prob = y_prob[order]
-
-    # calculate fraction of positives at each probability bin
-    bins = np.arange(0, 1.1, bin_size)
-    bin_indices = np.digitize(y_prob, bins)
-    bin_counts = np.bincount(bin_indices, minlength=len(bins) + 1)
-    fraction_positives = np.cumsum(bin_counts[:-1]) / np.sum(y_true)
+    prob_true, prob_pred = calibration_curve(y_true, y_prob, n_bins=n_bins)
+    return prob_true, prob_pred
+    # # sort probabilities and corresponding true labels in ascending order
+    # order = np.argsort(y_prob)
+    # y_true = y_true[order]
+    # y_prob = y_prob[order]
+
+    # # calculate fraction of positives at each probability bin
+    # bins = np.arange(0, 1.1, bin_size)
+    # bin_indices = np.digitize(y_prob, bins)
+    # bin_counts = np.bincount(bin_indices, minlength=len(bins) + 1)
+
+    # num_positives = np.cumsum(bin_counts[:-1])
+    # fraction_positives = num_positives / (num_positives + np.sum(y_true))
+
+    # return fraction_positives, bins
+
+
+def callibration_plot(data: MetricResult, n_bins: int = 10, **kwargs) -> "go.Figure":
+    import plotly.graph_objects as go
 
+    fraction_positives, bins = calculate_calibration_bins(data, n_bins)
     scatter = go.Scatter(
         x=bins, y=fraction_positives, mode="lines+markers", name="Data Points"
     )
 
     perfect_calibration = go.Scatter(
         x=[0, 1],
         y=[0, 1],
```

### Comparing `krisi-1.0.1/src/krisi/report/console.py` & `krisi-1.1.0/src/krisi/report/console.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,44 +65,59 @@
             f"{metric.name:>40s} - {metric.result:<15.5}"
             for metric in obj.get_all_metrics()
             if isinstance(metric.result, (float, int))
         ]
     )
 
 
-def get_large_metric_summary(obj: "ScoreCard", title: str) -> Table:
+def get_large_metric_summary(
+    obj: "ScoreCard",
+    title: str,
+    with_info: bool,
+    with_parameters: bool,
+    with_diagnostics: bool,
+) -> Table:
     return create_metric_table(
         title=title,
         metrics=obj.get_all_metrics(),
-        with_info=False,
-        with_parameters=False,
+        with_info=with_info,
+        with_parameters=with_parameters,
+        with_diagnostics=with_diagnostics,
     )
 
 
 def get_summary(
     obj: "ScoreCard",
     categories: List[str],
     repr: bool = True,
     with_info: bool = False,
+    with_parameters: bool = True,
+    with_diagnostics: bool = False,
     input_analysis: bool = True,
 ) -> Union[Panel, Layout]:
     category_groups = group_by_categories(list(vars(obj).values()), categories)
     input_analysis_table = (
-        [create_y_pred_table(obj.classification, obj.y, obj.predictions)]
+        [
+            create_y_pred_table(
+                obj.dataset_type.is_classification(), obj.y, obj.predictions
+            )
+        ]
         if input_analysis
         else []
     )
 
     metric_tables = Group(
         *input_analysis_table
         + [
             create_metric_table(
                 f"{category if category is not None else 'Unknown Category':>15s}",
                 metrics,
-                with_info,
+                with_info=with_info,
+                with_parameters=with_parameters,
+                with_diagnostics=with_diagnostics,
                 show_header=True if index == 0 else False,
             )
             for index, (category, metrics) in enumerate(category_groups.items())
             if not metrics_empty_in_category(metrics)
         ],
     )
```

### Comparing `krisi-1.0.1/src/krisi/report/graph.py` & `krisi-1.1.0/src/krisi/report/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import networkx as nx
 import numpy as np
 import pandas as pd
 from typing_extensions import Literal
 
 from krisi.evaluate.type import PathConst
 from krisi.utils.io import ensure_path
+from krisi.utils.state import RunType, get_global_state
 
 
 def create_save_graphs(
     df_rolled_corr: List[pd.DataFrame],
     save_or_display: List[Literal["save", "display"]] = ["save", "display"],
     corr_direction: Literal["positive", "negative"] = "positive",
     min_correlation: float = 0.01,
@@ -138,15 +139,16 @@
     )
 
     plt.axis("off")
 
     if "save" in save_or_display:
         plt.savefig(f"{save_location}/{file_name}_{corr_direction}.png", format="PNG")
     if "display" in save_or_display:
-        plt.show()
+        if not get_global_state().run_type == RunType.test:
+            plt.show()
 
 
 def create_animation(
     path: str = "structured_data/plots", file_suffix: str = "positive"
 ):
     import os
```

### Comparing `krisi-1.0.1/src/krisi/report/interactive.py` & `krisi-1.1.0/src/krisi/report/interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 from krisi.evaluate.type import ScoreCardMetadata
 from krisi.report.type import InteractiveFigure, PlotlyInput
 from krisi.utils.environment import is_notebook
 from krisi.utils.iterable_helpers import del_dict_keys, flatten
+from krisi.utils.state import RunType, get_global_state
 
 if TYPE_CHECKING:
     from dash import dcc, html
 
 
 external_script = ["https://tailwindcss.com/", {"src": "https://cdn.tailwindcss.com"}]
 
@@ -183,11 +184,12 @@
         if len(component.inputs) > 0 or len(component.global_input_ids) > 0:
             app.callback(
                 Output(component.id, "figure"),
                 [Input(input_.id, input_.value_name) for input_ in component.inputs]
                 + [Input(input_id, "value") for input_id in component.global_input_ids],
             )(component.get_figure)
 
-    if isnotebook:
-        app.run_server(mode="inline", debug=False, threaded=True)
-    else:
-        app.run(debug=False, threaded=True)
+    if get_global_state().run_type != RunType.test:
+        if isnotebook:
+            app.run_server(mode="inline", debug=False, threaded=True)
+        else:
+            app.run(debug=False, threaded=True)
```

### Comparing `krisi-1.0.1/src/krisi/report/pdf.py` & `krisi-1.1.0/src/krisi/report/pdf.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.1/src/krisi/report/report.py` & `krisi-1.1.0/src/krisi/report/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from krisi.utils.iterable_helpers import (
     flatten,
     group_by_categories,
     remove_nans,
     replace_if_None,
     wrap_in_list,
 )
+from krisi.utils.state import RunType, get_global_state
 
 if TYPE_CHECKING:
     from krisi.evaluate.metric import Metric
     from krisi.evaluate.scorecard import ScoreCard
 
 
 class Report:
@@ -75,26 +76,33 @@
                 css_template_url=self.css_template_url,
                 html_elements_to_inject=self.get_html_elements()
                 if self.get_html_elements is not None
                 else dict(),
             )
 
         if DisplayModes.direct in self.modes:
-            [figure.get_figure(**figure.plot_args).show() for figure in self.figures]
+            if not get_global_state().run_type == RunType.test:
+                [
+                    figure.get_figure(**figure.plot_args).show()
+                    for figure in self.figures
+                ]
 
         if DisplayModes.direct_save in self.modes:
             diagram_path = Path(os.path.join(self.save_path, Path("diagrams")))
             ensure_path(diagram_path)
             for i, figure in enumerate(self.figures):
                 figure.get_figure(**figure.plot_args).write_image(
                     os.path.join(diagram_path, f"{i}_{figure.title}.svg")
                 )
 
         if DisplayModes.direct_one_subplot in self.modes:
-            create_subplots_from_mutiple_plots(self.figures, title=self.title).show()
+            if not get_global_state().run_type == RunType.test:
+                create_subplots_from_mutiple_plots(
+                    self.figures, title=self.title
+                ).show()
 
         if DisplayModes.interactive in self.modes:
             run_app(
                 figures_by_category,
                 self.global_controllers,
                 self.title,
                 self.general_description,
```

### Comparing `krisi-1.0.1/src/krisi/report/type.py` & `krisi-1.1.0/src/krisi/report/type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 from typing_extensions import Literal
 
 if TYPE_CHECKING:
     import plotly.graph_objects as go
 
 from krisi.evaluate.type import MetricCategories, MetricResult
 
 PlotFunction = Callable[
     [List[MetricResult], str, Optional[float]],
     "go.Figure",
 ]
+PlotDefinition = Tuple[PlotFunction, Optional[Dict[str, Any]]]
 
 
 @dataclass
 class PlotlyInput:
     type: Literal[
         "dcc.Dropdown", "dcc.Input", "dcc.Checklist", "dcc.Slider", "dcc.RangeSlider"
     ]
```

### Comparing `krisi-1.0.1/src/krisi/report/vizualise.py` & `krisi-1.1.0/src/krisi/report/vizualise.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from enum import Enum
 from typing import TYPE_CHECKING, List, Optional, Union
 
 import pandas as pd
 
 from krisi.report.type import InteractiveFigure
 from krisi.utils.iterable_helpers import wrap_in_list
+from krisi.utils.state import RunType, get_global_state
 
 if TYPE_CHECKING:
     import plotly.graph_objects as go
 
 
 class VizualisationMethod(Enum):
     overlap = "overlap"
@@ -155,15 +156,16 @@
     fig.update_layout(
         title=title,
         autosize=True,
         height=350.0 * num_plots,
         margin=dict(l=75, r=75, b=50, t=75, pad=0),
         hovermode="x unified",
     )
-    fig.show()
+    if not get_global_state().run_type == RunType.test:
+        fig.show()
 
 
 def plot_y_predictions(
     y: pd.Series,
     preds: Union[List[pd.Series], pd.DataFrame],
     title: Optional[str] = "",
     x_name: str = "index",
```

### Comparing `krisi-1.0.1/src/krisi/report/library/pdf_layouts/scorecard/report.css` & `krisi-1.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.css`

 * *Files identical despite different names*

### Comparing `krisi-1.0.1/src/krisi/report/library/pdf_layouts/scorecard/report.html` & `krisi-1.1.0/src/krisi/report/library/pdf_layouts/scorecard/report.html`

 * *Files identical despite different names*

### Comparing `krisi-1.0.1/src/krisi/utils/console_plot.py` & `krisi-1.1.0/src/krisi/utils/console_plot.py`

 * *Files identical despite different names*

### Comparing `krisi-1.0.1/src/krisi/utils/environment.py` & `krisi-1.1.0/src/krisi/utils/environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 def is_notebook() -> bool:
+    if "get_ipython" not in globals():
+        return False
     try:
         shell = get_ipython().__class__.__name__
         if shell == "ZMQInteractiveShell":
             return True  # Jupyter notebook or qtconsole
         elif shell == "google.colab._shell":
             return True  # Terminal running IPython
         elif shell == "TerminalInteractiveShell":
             return False  # Terminal running IPython
         else:
             return False  # Other type (?)
+
     except NameError:
         return False  # Probably standard Python interpreter
```

### Comparing `krisi-1.0.1/src/krisi/utils/io.py` & `krisi-1.1.0/src/krisi/utils/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,25 @@
         dill.dump(obj, file)
 
 
 def save_console(
     obj: "ScoreCard",
     path: Path,
     with_info: bool,
+    with_parameters: bool,
+    with_diagnostics: bool,
     save_modes: List[Union[SaveModes, str]],
 ) -> None:
     summary = get_summary(
         obj,
         repr=True,
         categories=[el.value for el in MetricCategories],
         with_info=with_info,
+        with_parameters=with_parameters,
+        with_diagnostics=with_diagnostics,
     )
 
     console = Console(record=True, width=120)
     with console.capture():
         console.print(summary)
 
     if SaveModes.text in save_modes or SaveModes.text.value in save_modes:
```

### Comparing `krisi-1.0.1/src/krisi/utils/iterable_helpers.py` & `krisi-1.1.0/src/krisi/utils/iterable_helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,18 @@
-from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, List, TypeVar, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    TypeVar,
+    Union,
+)
 
 import numpy as np
 import pandas as pd
 
 from krisi.evaluate.type import Predictions, Targets
 
 if TYPE_CHECKING:
@@ -69,14 +79,31 @@
 def isiterable(obj: Any) -> bool:
     if isinstance(obj, Iterable) and not isinstance(obj, str):
         return True
     else:
         return False
 
 
+def isnumber(obj: Any) -> bool:
+    if isinstance(obj, (int, float, np.number)):
+        return True
+    else:
+        return False
+
+
+def check_iterable_with_number(iterable: Any):
+    if isinstance(iterable, Exception) or iterable is None:
+        return False
+
+    if isiterable(iterable) and len(iterable) > 0:
+        if isnumber(iterable[0]):
+            return True
+    return False
+
+
 def strip_builtin_functions(dict_to_strip: dict) -> dict:
     return {key_: value_ for key_, value_ in dict_to_strip.items() if key_[:2] != "__"}
 
 
 def __flatten(xs: Iterable[Any]) -> Any:
     for x in xs:
         if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
@@ -108,18 +135,28 @@
 
 
 def replace_if_None(input: Any, replacement: Any) -> Any:
     return replacement if input is None else input
 
 
 def is_int(s: Any):
+    if isinstance(s, str) and "." in s:
+        return False
     try:
         int(s)
     except ValueError:
         return False
     else:
         return True
 
 
 def del_dict_keys(d: dict, keys: Union[str, List[str]]) -> dict:
     keys = wrap_in_list(keys)
     return {k: v for k, v in d.items() if k not in keys}
+
+
+def empty_if_None(metrics: Optional[List]) -> List:
+    return metrics if metrics is not None else []
+
+
+def filter_none(list: List) -> List:
+    return [el for el in list if el is not None]
```

### Comparing `krisi-1.0.1/src/krisi/utils/devutils/timing.py` & `krisi-1.1.0/src/krisi/utils/devutils/timing.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,11 +66,11 @@
     )
 
 
 # res1 = timeingit(func1)
 # res2 = timeingit(func2)
 # # res3 = timeingit(func3)
 # res4 = timeingit(func4)
-timeingit(func_actual)
+# timeingit(func_actual)
 
 # assert res1 == res2 == res4
 # assert res1 == res2 == res3 == res4
```

### Comparing `krisi-1.0.1/.gitignore` & `krisi-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `krisi-1.0.1/LICENSE` & `krisi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `krisi-1.0.1/README.md` & `krisi-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 ## Installation
 
 
 The project was entirely built in ``python``. 
 
 Prerequisites
 
-* ``python >= 3.7`` and ``pip``
+* ``python >= 3.8`` and ``pip``
 
 
 Then run:
 
 *  ``pip install krisi``
 
 If you'd like to also use interactive plotting (html) and pdf generation then run:
@@ -111,16 +111,16 @@
 
 
 ```python
 import numpy as np
 from krisi import score
 
 sc = score(
-    y=np.random.normal(0, 0.1, 1000),
-    predictions=np.random.normal(0, 0.1, 1000),
+    y=np.random.random(1000),
+    predictions=np.random.random(1000),
 ).print()
 ```
 <details>
 <summary>
 Outputs:
 </summary>
```

#### html2text {}

```diff
@@ -26,29 +26,29 @@
 extensive library of predefined metrics.** - Too many dependencies.
 **â Krisi has few hard dependencies (only core libaries, eg.: sklearn and
 plotting libraries).** - Visualisation results are too basic.
 **â With Krisi you can decide to share and interactive web, a static PDF,
 each metric diagram displayed inline or quickly look at the ScoreCard pretty
 printed to the console.**
 ## Installation The project was entirely built in ``python``. Prerequisites *
-``python >= 3.7`` and ``pip`` Then run: * ``pip install krisi`` If you'd like
+``python >= 3.8`` and ``pip`` Then run: * ``pip install krisi`` If you'd like
 to also use interactive plotting (html) and pdf generation then run: * ``pip
 install krisi "krisi[plotting]"``
 ## Quickstart You can quickly evaluate your predictions by running: ```python
 import numpy as np from krisi.evaluate import score print(score
 (y=np.random.rand(100), predictions=np.random.rand(100))) ```   Outputs:  ```
 Model_20230505-15094466243320 <- you can add your name here Mean Absolute Error
 0.115402 Mean Absolute Percentage Error 3.272862 Symmetric Mean Absolute
 Percentage Error 0.718754 Mean Squared Error 0.020945 Root Mean Squared Error
 0.144723 R-squared -1.108832 Mean of the Residuals -0.002094 Standard Deviation
 of the Residuals 0.144781 ```  ----- Krisi's main object is the ``ScoreCard``
 that contains predefined ``Metric``s and which you can add further ``Metric``s
 to. ```python import numpy as np from krisi import score sc = score
-( y=np.random.normal(0, 0.1, 1000), predictions=np.random.normal(0, 0.1, 1000),
-).print() ```   Outputs:  ``` ââ Result of Model_20230505-130632d68aefea on
+( y=np.random.random(1000), predictions=np.random.random(1000), ).print() ```
+Outputs:  ``` ââ Result of Model_20230505-130632d68aefea on
 Dataset_20230505-130632d4167ca4 tested on outofsamââ â â â Targets
 and Predictions Analysis â â
 â­ââââââââââââââââââ¬âââââââââââââââââââââââââââââââââââââââââââââââââ¬âââââââââââââ¬âââââââââââââ®
 â â â Series Type â Histogram â Types â Indicies â â â
 âââââââââââââââââââ¼âââââââââââââââââââââââââââââââââââââââââââââââââ¼âââââââââââââ¼âââââââââââââ¤
 â â â Targets â
 ââââââââââââââââââââââââââââââââââââââââââ
```

### Comparing `krisi-1.0.1/pyproject.toml` & `krisi-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "krisi"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="Mark Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 description = "Testing and Reporting framework for Time Series Analysis"
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
 ]
 
@@ -135,15 +134,15 @@
   "src",
   ".",
 ]
 testpaths = ["tests"] 
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "1.0.1"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `krisi-1.0.1/PKG-INFO` & `krisi-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krisi
-Version: 1.0.1
+Version: 1.1.0
 Summary: Testing and Reporting framework for Time Series Analysis
 Project-URL: Documentation, https://dream-faster.github.io/krisi
 Project-URL: Issues, https://github.com/dream-faster/krisi/issues
 Project-URL: Source, https://github.com/dream-faster/krisi
 Author-email: Mark Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License: MIT License
         
@@ -45,19 +45,18 @@
         Licensor: Myalo UG (haftungsbeschränkt), Berlin, Germany
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: dill
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: plotext
 Requires-Dist: pytest
 Requires-Dist: rich
 Requires-Dist: scikit-learn
@@ -152,15 +151,15 @@
 ## Installation
 
 
 The project was entirely built in ``python``. 
 
 Prerequisites
 
-* ``python >= 3.7`` and ``pip``
+* ``python >= 3.8`` and ``pip``
 
 
 Then run:
 
 *  ``pip install krisi``
 
 If you'd like to also use interactive plotting (html) and pdf generation then run:
@@ -205,16 +204,16 @@
 
 
 ```python
 import numpy as np
 from krisi import score
 
 sc = score(
-    y=np.random.normal(0, 0.1, 1000),
-    predictions=np.random.normal(0, 0.1, 1000),
+    y=np.random.random(1000),
+    predictions=np.random.random(1000),
 ).print()
 ```
 <details>
 <summary>
 Outputs:
 </summary>
```

