# Comparing `tmp/benchtemp-1.0.0.tar.gz` & `tmp/benchtemp-1.1.0.tar.gz`

## Comparing `benchtemp-1.0.0.tar` & `benchtemp-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,28 @@
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 benchtemp-1.0.0/LICENSE
--rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 benchtemp-1.0.0/README-github.md
--rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 benchtemp-1.0.0/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 benchtemp-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 benchtemp-1.0.0/src/benchtemp/__init__.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 benchtemp-1.0.0/src/benchtemp/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchtemp-1.0.0/src/benchtemp/lp/__init__.py
--rw-r--r--   0        0        0     8308 2020-02-02 00:00:00.000000 benchtemp-1.0.0/src/benchtemp/lp/readers.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 benchtemp-1.0.0/src/benchtemp/lp/sampler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchtemp-1.0.0/src/benchtemp/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchtemp-1.0.0/src/benchtemp/nc/__init__.py
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 benchtemp-1.0.0/src/benchtemp/nc/readers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchtemp-1.0.0/src/benchtemp/preprocessing/__init__.py
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 benchtemp-1.0.0/src/benchtemp/preprocessing/data.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 benchtemp-1.0.0/tests/test.html
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 benchtemp-1.0.0/tests/test.py
--rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 benchtemp-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 benchtemp-1.1.0/LICENSE
+-rw-r--r--   0        0        0    11732 2020-02-02 00:00:00.000000 benchtemp-1.1.0/README-github.md
+-rw-r--r--   0        0        0    11251 2020-02-02 00:00:00.000000 benchtemp-1.1.0/README.md
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 benchtemp-1.1.0/img.png
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 benchtemp-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0   216464 2020-02-02 00:00:00.000000 benchtemp-1.1.0/img/framework.png
+-rw-r--r--   0        0        0   127427 2020-02-02 00:00:00.000000 benchtemp-1.1.0/img/pipeline.png
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/core/__init__.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/core/api.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/lp/__init__.py
+-rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/lp/dataloader.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/lp/edgesampler.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/nc/__init__.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/nc/dataloader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/optimization/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/optimization/loss.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/optimization/optimizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/preprocess/__init__.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/preprocess/preprocessing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/utils/__init__.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/utils/earlystop_monitor.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/utils/evaluator.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 benchtemp-1.1.0/src/benchtemp/utils/temporal_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchtemp-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 benchtemp-1.1.0/tests/test.html
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 benchtemp-1.1.0/tests/test.py
+-rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 benchtemp-1.1.0/PKG-INFO
```

### Comparing `benchtemp-1.0.0/LICENSE` & `benchtemp-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `benchtemp-1.0.0/README-github.md` & `benchtemp-1.1.0/README-github.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,17 @@
 
 Returns:
 - **ml_{data_name}.csv** - the csv file of the Temporal Graph.
 - **ml_{data_name}.npy** - the edge features of the Temporal Graph.
 - **ml_{data_name}_node.npy** - the node features of the Temporal Graph.
 
 Example:
-```python
-from benchtemp.preprocessing.data import data_preprocess
 
+```python
+from benchtemp.data.preprocessing import data_preprocess
 
 # If the dataset is bipartite graph, i.e. the user (source nodes) and the item (destination nodes) are of the same type.
 data_preprocess("data_name", bipartite=True)
 
 # non-bipartite graph.
 data_preprocess("data_name", bipartite=False)
 ```
@@ -152,18 +152,20 @@
 - **new_old_node_val_data <font color='lightblue'>: benchtemp.Data</font>** - The **inductive [new-old]** setting validation Temporal Graph dataset.
 - **new_old_node_test_data <font color='lightblue'>: benchtemp.Data</font>** - The **inductive [new-old]** setting test Temporal Graph dataset.
 - **new_new_node_val_data <font color='lightblue'>: benchtemp.Data</font>** - The **inductive [new-new]** setting validation Temporal Graph dataset.
 - **new_new_node_test_data <font color='lightblue'>: benchtemp.Data</font>** - The **inductive [new-new]** setting test Temporal Graph dataset.
 - **unseen_nodes_num <font color='lightblue'>: int</font>** - The number of unseen nodes of inductive setting.
 
 Example:
+
 ```python
-from benchtemp.lp.readers import get_data
+from benchtemp.lp.dataloader import get_data
 
-node_features, edge_features, full_data, train_data, val_data, test_data, new_node_val_data, new_node_test_data, new_old_node_val_data, new_old_node_test_data, new_new_node_val_data, new_new_node_test_data, unseen_nodes_num = get_data(dataset_name, different_new_nodes_between_val_and_test=False, randomize_features=False)
+node_features, edge_features, full_data, train_data, val_data, test_data, new_node_val_data, new_node_test_data, new_old_node_val_data, new_old_node_test_data, new_new_node_val_data, new_new_node_test_data, unseen_nodes_num = get_data(
+    dataset_name, different_new_nodes_between_val_and_test=False, randomize_features=False)
 ```
 
 ### EdgeSampler
 BenchTeMP provides the unified
 negative edge sampler with **seed** for Link Prediction task to  sample an equal amount of negatives to the positive interactions.
 
 Class:
@@ -176,16 +178,17 @@
 - **seed <font color='lightblue'>: numpy.ndarray</font>** - seed of random.
 
 Returns: 
 
 - **<font color='lightblue'> benchtemp.RandEdgeSampler</font>**
 
 Example:
+
 ```python
-from benchtemp.lp.sampler import RandEdgeSampler
+from benchtemp.lp.edgesampler import RandEdgeSampler
 
 # For example, if you are training , you should create a training  RandEdgeSampler based on the training dataset.
 train_rand_sampler = RandEdgeSampler(train_data.sources, train_data.destinations)
 
 ...
 for epoch in range(args.epochs):
     ...
```

### Comparing `benchtemp-1.0.0/README.md` & `benchtemp-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,649 +1,704 @@
-00000000: 2320 4265 6e63 6854 654d 503a 2041 2047  # BenchTeMP: A G
+00000000: 2320 4265 6e63 6854 656d 703a 2041 2047  # BenchTemp: A G
 00000010: 656e 6572 616c 2042 656e 6368 6d61 726b  eneral Benchmark
-00000020: 204c 6962 7261 7279 2066 6f72 2045 7661   Library for Eva
-00000030: 6c75 6174 696e 6720 5465 6d70 6f72 616c  luating Temporal
-00000040: 2047 7261 7068 204d 6f64 656c 730a 0a23   Graph Models..#
-00000050: 2320 4f76 6572 7669 6577 0a2a 2a42 656e  # Overview.**Ben
-00000060: 6368 5465 4d50 2a2a 2069 7320 6120 6765  chTeMP** is a ge
-00000070: 6e65 7261 6c20 4265 6e63 686d 6172 6b20  neral Benchmark 
-00000080: 5079 7468 6f6e 204c 6962 7261 7279 2066  Python Library f
-00000090: 6f72 2075 7365 7273 2074 6f20 6372 6561  or users to crea
-000000a0: 7465 2061 6e64 2065 7661 6c75 6174 6520  te and evaluate 
-000000b0: 5465 6d70 6f72 616c 2047 7261 7068 206d  Temporal Graph m
-000000c0: 6f64 656c 7320 7175 6963 6b6c 7920 616e  odels quickly an
-000000d0: 6420 6566 6669 6369 656e 746c 792e 200a  d efficiently. .
-000000e0: 2a2a 4265 6e63 6854 654d 502a 2a20 7072  **BenchTeMP** pr
-000000f0: 6f76 6964 6573 2075 7365 7273 2077 6974  ovides users wit
-00000100: 6820 7468 6520 756e 6966 6965 6420 2a2a  h the unified **
-00000110: 6f72 6967 696e 616c 2064 6174 6173 6574  original dataset
-00000120: 2070 7265 7072 6f63 6573 7320 6675 6e63   preprocess func
-00000130: 7469 6f6e 2c20 4461 7461 2043 6c61 7373  tion, Data Class
-00000140: 2c20 4461 7461 4c6f 6164 6572 2c20 4564  , DataLoader, Ed
-00000150: 6765 5361 6d70 6c65 722c 2061 6e64 2045  geSampler, and E
-00000160: 7661 6c75 6174 6f72 2a2a 2066 6f72 2063  valuator** for c
-00000170: 7265 6174 696e 6720 616e 6420 6576 616c  reating and eval
-00000180: 7561 7469 6e67 2079 6f75 7220 5465 6d70  uating your Temp
-00000190: 6f72 616c 2047 7261 7068 206d 6f64 656c  oral Graph model
-000001a0: 2e0a 0a2d 2054 6865 206f 7269 6769 6e61  ...- The origina
-000001b0: 6c20 6461 7461 7365 7473 2061 7265 205b  l datasets are [
-000001c0: 4865 7265 5d28 2920 616e 6420 7468 6520  Here]() and the 
-000001d0: 6461 7461 7365 7473 2070 7265 7072 6f63  datasets preproc
-000001e0: 6573 7365 6420 6279 2042 656e 6368 5465  essed by BenchTe
-000001f0: 4d50 2061 7265 205b 4865 7265 5d28 292e  MP are [Here]().
-00000200: 0a2d 2054 6865 2047 6974 4875 6220 6f66  .- The GitHub of
-00000210: 2042 656e 6368 5465 4d50 2070 726f 6a65   BenchTeMP proje
-00000220: 6374 2069 7320 5b48 6572 655d 2829 2e0a  ct is [Here]()..
-00000230: 2d20 5468 6520 736f 7572 6365 2063 6f64  - The source cod
-00000240: 6573 2066 6f72 2065 7661 6c75 6174 696e  es for evaluatin
-00000250: 6720 6578 6973 7469 6e67 2054 656d 706f  g existing Tempo
-00000260: 7261 6c20 4772 6170 6820 6d6f 6465 6c73  ral Graph models
-00000270: 2062 6173 6564 206f 6e20 4265 6e63 6854   based on BenchT
-00000280: 654d 5020 6172 6520 5b48 6572 655d 2829  eMP are [Here]()
-00000290: 2e20 0a2d 2054 6865 206c 6561 6465 7262  . .- The leaderb
-000002a0: 6f61 7264 7320 7765 6273 6974 6520 6372  oards website cr
-000002b0: 6561 7465 6420 6279 206f 7572 2074 6561  eated by our tea
-000002c0: 6d20 666f 7220 5465 6d70 6f72 616c 2047  m for Temporal G
-000002d0: 7261 7068 206d 6f64 656c 7320 6973 205b  raph models is [
-000002e0: 4865 7265 5d28 292e 0a0a 2323 2049 6e73  Here]()...## Ins
-000002f0: 7461 6c6c 6174 696f 6e0a 2323 2320 5265  tallation.### Re
-00000300: 7175 6972 656d 656e 7473 0a50 6c65 6173  quirements.Pleas
-00000310: 6520 656e 7375 7265 2074 6861 7420 796f  e ensure that yo
-00000320: 7520 6861 7665 2069 6e73 7461 6c6c 6564  u have installed
-00000330: 2074 6865 2066 6f6c 6c6f 7769 6e67 2064   the following d
-00000340: 6570 656e 6465 6e63 6965 733a 0a0a 2d20  ependencies:..- 
-00000350: 6e75 6d70 7920 3e3d 2031 2e31 382e 300a  numpy >= 1.18.0.
-00000360: 2d20 7061 6e64 6173 203e 3d20 312e 322e  - pandas >= 1.2.
-00000370: 300a 2d20 736b 6c65 6172 6e20 3e3d 2030  0.- sklearn >= 0
-00000380: 2e32 302e 300a 0a23 2323 2050 7950 4920  .20.0..### PyPI 
-00000390: 696e 7374 616c 6c0a 6060 6062 6173 680a  install.```bash.
-000003a0: 7069 7033 2069 6e73 7461 6c6c 2062 656e  pip3 install ben
-000003b0: 6368 7465 6d70 200a 6060 600a 0a23 2320  chtemp .```..## 
-000003c0: 5061 636b 6167 6520 5573 6167 650a 2323  Package Usage.##
-000003d0: 2320 4461 7461 7365 7473 0a54 6865 2064  # Datasets.The d
-000003e0: 6174 6173 6574 7320 7468 6174 2068 6176  atasets that hav
-000003f0: 6520 6265 656e 2070 7265 7072 6f63 6573  e been preproces
-00000400: 7365 6420 6279 2042 656e 6368 5465 4d50  sed by BenchTeMP
-00000410: 2061 7265 205b 4865 7265 5d28 292e 0a59   are [Here]()..Y
-00000420: 6f75 2063 616e 2064 6972 6563 746c 7920  ou can directly 
-00000430: 646f 776e 6c6f 6164 2074 6865 2064 6174  download the dat
-00000440: 6173 6574 7320 616e 6420 7468 656e 2070  asets and then p
-00000450: 7574 2074 6865 6d20 696e 746f 2074 6865  ut them into the
-00000460: 2064 6972 6563 746f 7279 2027 2e2f 6461   directory './da
-00000470: 7461 272e 0a0a 496e 2061 6464 6974 696f  ta'...In additio
-00000480: 6e2c 2042 656e 6368 5465 4d50 2070 726f  n, BenchTeMP pro
-00000490: 7669 6465 7320 6461 7461 2070 726f 6365  vides data proce
-000004a0: 7373 696e 6720 6675 6e63 7469 6f6e 732e  ssing functions.
-000004b0: 2079 6f75 2063 616e 2064 6f77 6e6c 6f61   you can downloa
-000004c0: 6420 7468 6520 6f72 6967 696e 616c 2064  d the original d
-000004d0: 6174 6173 6574 7320 5b48 6572 655d 2829  atasets [Here]()
-000004e0: 2061 6e64 2074 6865 6e20 0a75 7365 2074   and then .use t
-000004f0: 6865 2066 756e 6374 696f 6e73 2070 726f  he functions pro
-00000500: 7669 6465 6420 6279 2042 656e 6368 5465  vided by BenchTe
-00000510: 4d50 2066 6f72 2064 6174 6120 7072 6570  MP for data prep
-00000520: 726f 6365 7373 696e 672e 0a0a 4675 6e63  rocessing...Func
-00000530: 7469 6f6e 3a0a 2a2a 6265 6e63 6874 656d  tion:.**benchtem
-00000540: 702e 7072 6570 726f 6365 7373 696e 672e  p.preprocessing.
-00000550: 6461 7461 2e64 6174 615f 7072 6570 726f  data.data_prepro
-00000560: 6365 7373 2864 6174 615f 6e61 6d65 203a  cess(data_name :
-00000570: 2073 7472 2c20 6269 7061 7274 6974 6520   str, bipartite 
-00000580: 3a20 626f 6f6c 3d54 7275 6529 2a2a 0a0a  : bool=True)**..
-00000590: 5061 7261 6d65 7465 7273 3a0a 2d20 2a2a  Parameters:.- **
-000005a0: 6461 7461 5f6e 616d 6520 3a20 7374 722a  data_name : str*
-000005b0: 2a20 2d20 7468 6520 6e61 6d65 206f 6620  * - the name of 
-000005c0: 7468 6520 6461 7461 7365 742e 0a2d 202a  the dataset..- *
-000005d0: 2a62 6970 6172 7469 7465 203a 2062 6f6f  *bipartite : boo
-000005e0: 6c2a 2a20 2d20 5768 6574 6865 7220 7468  l** - Whether th
-000005f0: 6520 5465 6d70 6f72 616c 2047 7261 7068  e Temporal Graph
-00000600: 2069 7320 6269 7061 7274 6974 6520 6772   is bipartite gr
-00000610: 6170 682e 0a0a 5265 7475 726e 733a 0a2d  aph...Returns:.-
-00000620: 202a 2a6d 6c5f 7b64 6174 615f 6e61 6d65   **ml_{data_name
-00000630: 7d2e 6373 762a 2a20 2d20 7468 6520 6373  }.csv** - the cs
-00000640: 7620 6669 6c65 206f 6620 7468 6520 5465  v file of the Te
-00000650: 6d70 6f72 616c 2047 7261 7068 2e0a 2d20  mporal Graph..- 
-00000660: 2a2a 6d6c 5f7b 6461 7461 5f6e 616d 657d  **ml_{data_name}
-00000670: 2e6e 7079 2a2a 202d 2074 6865 2065 6467  .npy** - the edg
-00000680: 6520 6665 6174 7572 6573 206f 6620 7468  e features of th
-00000690: 6520 5465 6d70 6f72 616c 2047 7261 7068  e Temporal Graph
-000006a0: 2e0a 2d20 2a2a 6d6c 5f7b 6461 7461 5f6e  ..- **ml_{data_n
-000006b0: 616d 657d 5f6e 6f64 652e 6e70 792a 2a20  ame}_node.npy** 
-000006c0: 2d20 7468 6520 6e6f 6465 2066 6561 7475  - the node featu
-000006d0: 7265 7320 6f66 2074 6865 2054 656d 706f  res of the Tempo
-000006e0: 7261 6c20 4772 6170 682e 0a0a 4578 616d  ral Graph...Exam
-000006f0: 706c 653a 0a60 6060 7079 7468 6f6e 0a66  ple:.```python.f
-00000700: 726f 6d20 6265 6e63 6874 656d 702e 7072  rom benchtemp.pr
-00000710: 6570 726f 6365 7373 696e 672e 6461 7461  eprocessing.data
-00000720: 2069 6d70 6f72 7420 6461 7461 5f70 7265   import data_pre
-00000730: 7072 6f63 6573 730a 0a0a 2320 4966 2074  process...# If t
-00000740: 6865 2064 6174 6173 6574 2069 7320 6269  he dataset is bi
-00000750: 7061 7274 6974 6520 6772 6170 682c 2069  partite graph, i
-00000760: 2e65 2e20 7468 6520 7573 6572 2028 736f  .e. the user (so
-00000770: 7572 6365 206e 6f64 6573 2920 616e 6420  urce nodes) and 
-00000780: 7468 6520 6974 656d 2028 6465 7374 696e  the item (destin
-00000790: 6174 696f 6e20 6e6f 6465 7329 2061 7265  ation nodes) are
-000007a0: 206f 6620 7468 6520 7361 6d65 2074 7970   of the same typ
-000007b0: 652e 0a64 6174 615f 7072 6570 726f 6365  e..data_preproce
-000007c0: 7373 2822 6461 7461 5f6e 616d 6522 2c20  ss("data_name", 
-000007d0: 6269 7061 7274 6974 653d 5472 7565 290a  bipartite=True).
-000007e0: 0a23 206e 6f6e 2d62 6970 6172 7469 7465  .# non-bipartite
-000007f0: 2067 7261 7068 2e0a 6461 7461 5f70 7265   graph..data_pre
-00000800: 7072 6f63 6573 7328 2264 6174 615f 6e61  process("data_na
-00000810: 6d65 222c 2062 6970 6172 7469 7465 3d46  me", bipartite=F
-00000820: 616c 7365 290a 6060 600a 0a4e 6f74 6573  alse).```..Notes
-00000830: 3a0a 0a46 6f72 2062 6970 6172 7469 7465  :..For bipartite
-00000840: 2067 7261 7068 2c20 4265 6e63 6854 654d   graph, BenchTeM
-00000850: 5020 7769 6c6c 2066 6163 746f 7269 7a65  P will factorize
-00000860: 2074 6865 2073 6f75 7263 6520 6e6f 6465   the source node
-00000870: 2069 6e64 6578 2061 6e64 200a 7468 6520   index and .the 
-00000880: 6465 7374 696e 6174 696f 6e20 6e6f 6465  destination node
-00000890: 2069 6e64 6578 2c20 7265 7370 6563 7469   index, respecti
-000008a0: 7665 6c79 2e20 0a60 6060 7079 7468 6f6e  vely. .```python
-000008b0: 0a69 6d70 6f72 7420 7061 6e64 6173 2061  .import pandas a
-000008c0: 7320 7064 0a0a 6173 7365 7274 206c 656e  s pd..assert len
-000008d0: 2873 6f75 7263 6573 2920 3d3d 206c 656e  (sources) == len
-000008e0: 2864 6573 7469 6e61 7469 6f6e 7329 0a0a  (destinations)..
-000008f0: 2320 6269 7061 7274 6974 6520 6772 6170  # bipartite grap
-00000900: 680a 736f 7572 6365 732c 205f 203d 2070  h.sources, _ = p
-00000910: 642e 6661 6374 6f72 697a 6528 736f 7572  d.factorize(sour
-00000920: 6365 7329 0a64 6573 7469 6e61 7469 6f6e  ces).destination
-00000930: 732c 205f 203d 2070 642e 6661 6374 6f72  s, _ = pd.factor
-00000940: 697a 6528 6465 7374 696e 6174 696f 6e73  ize(destinations
-00000950: 290a 0a75 7070 6572 5f75 203d 2073 6f75  )..upper_u = sou
-00000960: 7263 6573 2e6d 6178 202b 2031 0a64 6573  rces.max + 1.des
-00000970: 7469 6e61 7469 6f6e 7320 3d20 6465 7374  tinations = dest
-00000980: 696e 6174 696f 6e73 202b 2075 7070 6572  inations + upper
-00000990: 5f75 0a60 6060 0a46 6f72 206e 6f6e 2d62  _u.```.For non-b
-000009a0: 6970 6172 7469 7465 2067 7261 7068 2c20  ipartite graph, 
-000009b0: 4265 6e63 6854 654d 5020 7769 6c6c 2066  BenchTeMP will f
-000009c0: 6163 746f 7269 7a65 2074 6865 2063 6f6e  actorize the con
-000009d0: 6361 7465 6e61 7469 6f6e 206f 6620 736f  catenation of so
-000009e0: 7572 6365 206e 6f64 6520 6172 7261 7920  urce node array 
-000009f0: 616e 6420 0a74 6865 2064 6573 7469 6e61  and .the destina
-00000a00: 7469 6f6e 206e 6f64 6520 6172 7261 792e  tion node array.
-00000a10: 200a 0a60 6060 7079 7468 6f6e 0a69 6d70   ..```python.imp
-00000a20: 6f72 7420 7061 6e64 6173 2061 7320 7064  ort pandas as pd
-00000a30: 0a69 6d70 6f72 7420 6e75 6d70 7920 6173  .import numpy as
-00000a40: 206e 700a 0a61 7373 6572 7420 6c65 6e28   np..assert len(
-00000a50: 736f 7572 6365 7329 203d 3d20 6c65 6e28  sources) == len(
-00000a60: 6465 7374 696e 6174 696f 6e73 290a 696e  destinations).in
-00000a70: 7465 7261 6374 696f 6e5f 6e75 6d20 3d20  teraction_num = 
-00000a80: 6c65 6e28 736f 7572 6365 7329 0a0a 2320  len(sources)..# 
-00000a90: 6e6f 6e2d 6269 7061 7274 6974 6520 6772  non-bipartite gr
-00000aa0: 6170 680a 6e6f 6465 5f69 6e64 6578 2c20  aph.node_index, 
-00000ab0: 5f20 3d20 7064 2e66 6163 746f 7269 7a65  _ = pd.factorize
-00000ac0: 286e 702e 636f 6e63 6174 656e 6174 6528  (np.concatenate(
-00000ad0: 2873 6f75 7263 6573 2c20 6465 7374 696e  (sources, destin
-00000ae0: 6174 696f 6e73 292c 2061 7869 733d 3029  ations), axis=0)
-00000af0: 290a 0a73 6f75 7263 6573 203d 206e 6f64  )..sources = nod
-00000b00: 655f 696e 6465 785b 5b30 3a69 6e74 6572  e_index[[0:inter
-00000b10: 6163 7469 6f6e 5f6e 756d 5d5d 0a64 6573  action_num]].des
-00000b20: 7469 6e61 7469 6f6e 7320 3d20 6e6f 6465  tinations = node
-00000b30: 5f69 6e64 6578 5b5b 696e 7465 7261 6374  _index[[interact
-00000b40: 696f 6e5f 6e75 6d3a 696e 7465 7261 6374  ion_num:interact
-00000b50: 696f 6e5f 6e75 6d20 2b20 696e 7465 7261  ion_num + intera
-00000b60: 6374 696f 6e5f 6e75 6d5d 5d0a 6060 600a  ction_num]].```.
-00000b70: 0a0a 2323 2320 5465 6d70 6f72 616c 4461  ..### TemporalDa
-00000b80: 7461 2043 6c61 7373 0a43 6c61 7373 3a0a  ta Class.Class:.
-00000b90: 0a2a 2a44 6174 6128 736f 7572 6365 7320  .**Data(sources 
-00000ba0: 3a20 6e75 6d70 792e 6e64 6172 7261 792c  : numpy.ndarray,
-00000bb0: 0a64 6573 7469 6e61 7469 6f6e 7320 3a20  .destinations : 
-00000bc0: 6e75 6d70 792e 6e64 6172 7261 792c 0a74  numpy.ndarray,.t
-00000bd0: 696d 6573 7461 6d70 7320 3a20 6e75 6d70  imestamps : nump
-00000be0: 792e 6e64 6172 7261 792c 0a65 6467 655f  y.ndarray,.edge_
-00000bf0: 6964 7873 203a 206e 756d 7079 2e6e 6461  idxs : numpy.nda
-00000c00: 7272 6179 2c0a 6c61 6265 6c73 203a 206e  rray,.labels : n
-00000c10: 756d 7079 2e6e 6461 7272 6179 292a 2a0a  umpy.ndarray)**.
-00000c20: 0a50 6172 616d 6574 6572 733a 0a2d 202a  .Parameters:.- *
-00000c30: 2a73 6f75 7263 6573 203a 206e 756d 7079  *sources : numpy
-00000c40: 2e6e 6461 7272 6179 2a2a 202d 2041 7272  .ndarray** - Arr
-00000c50: 6179 206f 6620 736f 7572 6365 7320 6f66  ay of sources of
-00000c60: 2054 656d 706f 7261 6c20 4772 6170 6820   Temporal Graph 
-00000c70: 6564 6765 732e 0a2d 202a 2a64 6573 7469  edges..- **desti
-00000c80: 6e61 7469 6f6e 7320 3a20 6e75 6d70 792e  nations : numpy.
-00000c90: 6e64 6172 7261 792a 2a20 2d20 4172 7261  ndarray** - Arra
-00000ca0: 7920 6f66 2064 6573 7469 6e61 7469 6f6e  y of destination
-00000cb0: 7320 6f66 2054 656d 706f 7261 6c20 4772  s of Temporal Gr
-00000cc0: 6170 6820 6564 6765 732e 0a2d 202a 2a74  aph edges..- **t
-00000cd0: 696d 6573 7461 6d70 7320 3a20 6e75 6d70  imestamps : nump
-00000ce0: 792e 6e64 6172 7261 792a 2a20 2d20 4172  y.ndarray** - Ar
-00000cf0: 7261 7920 6f66 2074 696d 6573 7461 6d70  ray of timestamp
-00000d00: 7320 6f66 2054 656d 706f 7261 6c20 4772  s of Temporal Gr
-00000d10: 6170 6820 6564 6765 732e 0a2d 202a 2a65  aph edges..- **e
-00000d20: 6467 655f 6964 7873 203a 206e 756d 7079  dge_idxs : numpy
-00000d30: 2e6e 6461 7272 6179 2a2a 202d 2041 7272  .ndarray** - Arr
-00000d40: 6179 206f 6620 6564 6765 2049 4473 206f  ay of edge IDs o
-00000d50: 6620 5465 6d70 6f72 616c 2047 7261 7068  f Temporal Graph
-00000d60: 2065 6467 6573 2e0a 2d20 2a2a 6c61 6265   edges..- **labe
-00000d70: 6c73 203a 206e 756d 7079 2e6e 6461 7272  ls : numpy.ndarr
-00000d80: 6179 2a2a 202d 2041 7272 6179 206f 6620  ay** - Array of 
-00000d90: 6c61 6265 6c73 206f 6620 5465 6d70 6f72  labels of Tempor
-00000da0: 616c 2047 7261 7068 6520 6467 6573 2e0a  al Graphe dges..
-00000db0: 0a52 6574 7572 6e73 3a20 0a2d 202a 2a62  .Returns: .- **b
-00000dc0: 656e 6368 7465 6d70 2e44 6174 612a 2a2e  enchtemp.Data**.
-00000dd0: 2041 2054 656d 706f 7261 6c20 4772 6170   A Temporal Grap
-00000de0: 682e 0a0a 0a0a 0a45 7861 6d70 6c65 3a0a  h......Example:.
-00000df0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
-00000e00: 2070 616e 6461 7320 6173 2070 640a 696d   pandas as pd.im
-00000e10: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
-00000e20: 0a66 726f 6d20 6265 6e63 6874 656d 702e  .from benchtemp.
-00000e30: 7574 696c 7320 696d 706f 7274 2044 6174  utils import Dat
-00000e40: 610a 0a67 7261 7068 5f64 6620 3d20 7064  a..graph_df = pd
-00000e50: 2e72 6561 645f 6373 7628 2264 6174 6173  .read_csv("datas
-00000e60: 6574 5f70 6174 6822 290a 0a73 6f75 7263  et_path")..sourc
-00000e70: 6573 203d 2067 7261 7068 5f64 662e 752e  es = graph_df.u.
-00000e80: 7661 6c75 6573 0a64 6573 7469 6e61 7469  values.destinati
-00000e90: 6f6e 7320 3d20 6772 6170 685f 6466 2e69  ons = graph_df.i
-00000ea0: 2e76 616c 7565 730a 6564 6765 5f69 6478  .values.edge_idx
-00000eb0: 7320 3d20 6772 6170 685f 6466 2e69 6478  s = graph_df.idx
-00000ec0: 2e76 616c 7565 730a 6c61 6265 6c73 203d  .values.labels =
-00000ed0: 2067 7261 7068 5f64 662e 6c61 6265 6c2e   graph_df.label.
-00000ee0: 7661 6c75 6573 0a74 696d 6573 7461 6d70  values.timestamp
-00000ef0: 7320 3d20 6772 6170 685f 6466 2e74 732e  s = graph_df.ts.
-00000f00: 7661 6c75 6573 0a0a 2320 466f 7220 6578  values..# For ex
-00000f10: 616d 706c 652c 2074 6865 2066 756c 6c20  ample, the full 
-00000f20: 5465 6d70 6f72 616c 2047 7261 7068 206f  Temporal Graph o
-00000f30: 6620 7468 6520 6461 7461 7365 7420 6973  f the dataset is
-00000f40: 2066 756c 6c5f 6461 7461 2e0a 6675 6c6c   full_data..full
-00000f50: 5f64 6174 6120 3d20 4461 7461 2873 6f75  _data = Data(sou
-00000f60: 7263 6573 2c20 6465 7374 696e 6174 696f  rces, destinatio
-00000f70: 6e73 2c20 7469 6d65 7374 616d 7073 2c20  ns, timestamps, 
-00000f80: 6564 6765 5f69 6478 732c 206c 6162 656c  edge_idxs, label
-00000f90: 7329 0a60 6060 0a0a 0a23 2323 2044 6174  s).```...### Dat
-00000fa0: 614c 6f61 6465 720a 2323 2320 2831 2920  aLoader.### (1) 
-00000fb0: 4c69 6e6b 2050 7265 6469 6374 696f 6e20  Link Prediction 
-00000fc0: 7461 736b 0a46 756e 6374 696f 6e3a 0a0a  task.Function:..
-00000fd0: 2a2a 6265 6e63 6874 656d 702e 6c70 2e72  **benchtemp.lp.r
-00000fe0: 6561 6465 7273 2e67 6574 5f64 6174 6128  eaders.get_data(
-00000ff0: 6461 7461 7365 745f 6e61 6d65 203a 2073  dataset_name : s
-00001000: 7472 2c20 6469 6666 6572 656e 745f 6e65  tr, different_ne
-00001010: 775f 6e6f 6465 735f 6265 7477 6565 6e5f  w_nodes_between_
-00001020: 7661 6c5f 616e 645f 7465 7374 3d46 616c  val_and_test=Fal
-00001030: 7365 2c20 7261 6e64 6f6d 697a 655f 6665  se, randomize_fe
-00001040: 6174 7572 6573 3d46 616c 7365 292a 2a0a  atures=False)**.
-00001050: 200a 5061 7261 6d65 7465 7273 3a0a 2d20   .Parameters:.- 
-00001060: 2a2a 6461 7461 7365 745f 6e61 6d65 203a  **dataset_name :
-00001070: 2073 7472 2a2a 202d 2054 6865 206e 616d   str** - The nam
-00001080: 6520 6f66 2074 6865 2064 6174 6173 6574  e of the dataset
-00001090: 2e20 5468 6520 6461 7461 7365 7420 6669  . The dataset fi
-000010a0: 6c65 2028 2e63 7376 2066 696c 6520 6f66  le (.csv file of
-000010b0: 2074 6865 2054 656d 706f 7261 6c20 4772   the Temporal Gr
-000010c0: 6170 682c 202e 6e70 7920 6669 6c65 206f  aph, .npy file o
-000010d0: 6620 7468 6520 6e6f 6465 2066 6561 7475  f the node featu
-000010e0: 7265 7320 616e 6420 2e6e 7079 2066 696c  res and .npy fil
-000010f0: 6520 6f66 2074 6865 2065 6467 6520 6665  e of the edge fe
-00001100: 6174 7572 6573 2920 7368 6f75 6c64 2062  atures) should b
-00001110: 6520 696e 2022 2e2f 6461 7461 2220 6469  e in "./data" di
-00001120: 7265 6374 6f72 792e 0a2d 202a 2a64 6966  rectory..- **dif
-00001130: 6665 7265 6e74 5f6e 6577 5f6e 6f64 6573  ferent_new_nodes
-00001140: 5f62 6574 7765 656e 5f76 616c 5f61 6e64  _between_val_and
-00001150: 5f74 6573 7420 3a20 626f 6f6c 2a2a 202d  _test : bool** -
-00001160: 2044 6966 6665 7265 6e74 206e 6577 206e   Different new n
-00001170: 6f64 6573 2062 6574 7765 656e 2020 7468  odes between  th
-00001180: 6520 7661 6c69 6461 7469 6f6e 2061 6e64  e validation and
-00001190: 2074 6573 7420 6461 7461 7365 742e 0a2d   test dataset..-
-000011a0: 202a 2a72 616e 646f 6d69 7a65 5f66 6561   **randomize_fea
-000011b0: 7475 7265 7320 3a20 626f 6f6c 2a2a 202d  tures : bool** -
-000011c0: 2052 616e 646f 6d20 696e 6974 6961 6c69   Random initiali
-000011d0: 7a61 7469 6f6e 206f 6620 6e6f 6465 2046  zation of node F
-000011e0: 6561 7475 7265 732e 200a 0a52 6574 7572  eatures. ..Retur
-000011f0: 6e73 3a0a 2d20 2a2a 6e6f 6465 5f66 6561  ns:.- **node_fea
-00001200: 7475 7265 7320 3a20 6e75 6d70 792e 6e64  tures : numpy.nd
-00001210: 6172 7261 792a 2a20 2d20 4172 7261 7920  array** - Array 
-00001220: 6f66 2074 6865 204e 6f64 6520 4665 6174  of the Node Feat
-00001230: 7572 6573 206f 6620 7468 6520 5465 6d70  ures of the Temp
-00001240: 6f72 616c 2047 7261 7068 2e20 0a2d 202a  oral Graph. .- *
-00001250: 2a65 6467 655f 6665 6174 7572 6573 203a  *edge_features :
-00001260: 206e 756d 7079 2e6e 6461 7272 6179 2a2a   numpy.ndarray**
-00001270: 202d 2041 7272 6179 206f 6620 7468 6520   - Array of the 
-00001280: 4564 6765 2046 6561 7475 7265 7320 6f66  Edge Features of
-00001290: 2074 6865 2054 656d 706f 7261 6c20 4772   the Temporal Gr
-000012a0: 6170 682e 0a2d 202a 2a66 756c 6c5f 6461  aph..- **full_da
-000012b0: 7461 203a 2062 656e 6368 7465 6d70 2e44  ta : benchtemp.D
-000012c0: 6174 612a 2a20 2d20 4675 6c6c 2054 656d  ata** - Full Tem
-000012d0: 706f 7261 6c20 4772 6170 6820 6461 7461  poral Graph data
-000012e0: 7365 742e 200a 2d20 2a2a 7472 6169 6e5f  set. .- **train_
-000012f0: 6461 7461 203a 2062 656e 6368 7465 6d70  data : benchtemp
-00001300: 2e44 6174 612a 2a20 2d20 5468 6520 7472  .Data** - The tr
-00001310: 6169 6e69 6e67 2054 656d 706f 7261 6c20  aining Temporal 
-00001320: 4772 6170 6820 6461 7461 7365 742e 200a  Graph dataset. .
-00001330: 2d20 2a2a 7661 6c5f 6461 7461 203a 2062  - **val_data : b
-00001340: 656e 6368 7465 6d70 2e44 6174 612a 2a20  enchtemp.Data** 
-00001350: 2d20 5468 6520 7661 6c69 6461 7469 6f6e  - The validation
-00001360: 2054 656d 706f 7261 6c20 4772 6170 6820   Temporal Graph 
-00001370: 6461 7461 7365 742e 0a2d 202a 2a74 6573  dataset..- **tes
-00001380: 745f 6461 7461 203a 2062 656e 6368 7465  t_data : benchte
-00001390: 6d70 2e44 6174 612a 2a20 202d 2054 6865  mp.Data**  - The
-000013a0: 202a 2a74 7261 6e73 6475 6374 6976 652a   **transductive*
-000013b0: 2a20 7465 7374 2054 656d 706f 7261 6c20  * test Temporal 
-000013c0: 4772 6170 6820 6461 7461 7365 742e 0a2d  Graph dataset..-
-000013d0: 202a 2a6e 6577 5f6e 6f64 655f 7661 6c5f   **new_node_val_
-000013e0: 6461 7461 203a 2062 656e 6368 7465 6d70  data : benchtemp
-000013f0: 2e44 6174 612a 2a20 2d20 5468 6520 2a2a  .Data** - The **
-00001400: 696e 6475 6374 6976 6520 5b6e 6577 2d5d  inductive [new-]
-00001410: 2a2a 2073 6574 7469 6e67 2076 616c 6964  ** setting valid
-00001420: 6174 696f 6e20 5465 6d70 6f72 616c 2047  ation Temporal G
-00001430: 7261 7068 2064 6174 6173 6574 2e0a 2d20  raph dataset..- 
-00001440: 2a2a 6e65 775f 6e6f 6465 5f74 6573 745f  **new_node_test_
-00001450: 6461 7461 203a 2062 656e 6368 7465 6d70  data : benchtemp
-00001460: 2e44 6174 612a 2a20 2d20 5468 6520 2a2a  .Data** - The **
-00001470: 696e 6475 6374 6976 6520 5b6e 6577 2d5d  inductive [new-]
-00001480: 2a2a 2073 6574 7469 6e67 2074 6573 7420  ** setting test 
-00001490: 5465 6d70 6f72 616c 2047 7261 7068 2064  Temporal Graph d
-000014a0: 6174 6173 6574 2e0a 2d20 2a2a 6e65 775f  ataset..- **new_
-000014b0: 6f6c 645f 6e6f 6465 5f76 616c 5f64 6174  old_node_val_dat
-000014c0: 6120 3a20 6265 6e63 6874 656d 702e 4461  a : benchtemp.Da
-000014d0: 7461 2a2a 202d 2054 6865 202a 2a69 6e64  ta** - The **ind
-000014e0: 7563 7469 7665 205b 6e65 772d 6f6c 645d  uctive [new-old]
-000014f0: 2a2a 2073 6574 7469 6e67 2076 616c 6964  ** setting valid
-00001500: 6174 696f 6e20 5465 6d70 6f72 616c 2047  ation Temporal G
-00001510: 7261 7068 2064 6174 6173 6574 2e0a 2d20  raph dataset..- 
-00001520: 2a2a 6e65 775f 6f6c 645f 6e6f 6465 5f74  **new_old_node_t
-00001530: 6573 745f 6461 7461 203a 2062 656e 6368  est_data : bench
-00001540: 7465 6d70 2e44 6174 612a 2a20 2d20 5468  temp.Data** - Th
-00001550: 6520 2a2a 696e 6475 6374 6976 6520 5b6e  e **inductive [n
-00001560: 6577 2d6f 6c64 5d2a 2a20 7365 7474 696e  ew-old]** settin
-00001570: 6720 7465 7374 2054 656d 706f 7261 6c20  g test Temporal 
-00001580: 4772 6170 6820 6461 7461 7365 742e 0a2d  Graph dataset..-
-00001590: 202a 2a6e 6577 5f6e 6577 5f6e 6f64 655f   **new_new_node_
-000015a0: 7661 6c5f 6461 7461 203a 2062 656e 6368  val_data : bench
-000015b0: 7465 6d70 2e44 6174 612a 2a20 2d20 5468  temp.Data** - Th
-000015c0: 6520 2a2a 696e 6475 6374 6976 6520 5b6e  e **inductive [n
-000015d0: 6577 2d6e 6577 5d2a 2a20 7365 7474 696e  ew-new]** settin
-000015e0: 6720 7661 6c69 6461 7469 6f6e 2054 656d  g validation Tem
-000015f0: 706f 7261 6c20 4772 6170 6820 6461 7461  poral Graph data
-00001600: 7365 742e 0a2d 202a 2a6e 6577 5f6e 6577  set..- **new_new
-00001610: 5f6e 6f64 655f 7465 7374 5f64 6174 6120  _node_test_data 
-00001620: 3a20 6265 6e63 6874 656d 702e 4461 7461  : benchtemp.Data
-00001630: 2a2a 202d 2054 6865 202a 2a69 6e64 7563  ** - The **induc
-00001640: 7469 7665 205b 6e65 772d 6e65 775d 2a2a  tive [new-new]**
-00001650: 2073 6574 7469 6e67 2074 6573 7420 5465   setting test Te
-00001660: 6d70 6f72 616c 2047 7261 7068 2064 6174  mporal Graph dat
-00001670: 6173 6574 2e0a 2d20 2a2a 756e 7365 656e  aset..- **unseen
-00001680: 5f6e 6f64 6573 5f6e 756d 203a 2069 6e74  _nodes_num : int
-00001690: 2a2a 202d 2054 6865 206e 756d 6265 7220  ** - The number 
-000016a0: 6f66 2075 6e73 6565 6e20 6e6f 6465 7320  of unseen nodes 
-000016b0: 6f66 2069 6e64 7563 7469 7665 2073 6574  of inductive set
-000016c0: 7469 6e67 2e0a 0a45 7861 6d70 6c65 3a0a  ting...Example:.
-000016d0: 6060 6070 7974 686f 6e0a 6672 6f6d 2062  ```python.from b
-000016e0: 656e 6368 7465 6d70 2e6c 702e 7265 6164  enchtemp.lp.read
-000016f0: 6572 7320 696d 706f 7274 2067 6574 5f64  ers import get_d
-00001700: 6174 610a 0a6e 6f64 655f 6665 6174 7572  ata..node_featur
-00001710: 6573 2c20 6564 6765 5f66 6561 7475 7265  es, edge_feature
-00001720: 732c 2066 756c 6c5f 6461 7461 2c20 7472  s, full_data, tr
-00001730: 6169 6e5f 6461 7461 2c20 7661 6c5f 6461  ain_data, val_da
-00001740: 7461 2c20 7465 7374 5f64 6174 612c 206e  ta, test_data, n
-00001750: 6577 5f6e 6f64 655f 7661 6c5f 6461 7461  ew_node_val_data
-00001760: 2c20 6e65 775f 6e6f 6465 5f74 6573 745f  , new_node_test_
-00001770: 6461 7461 2c20 6e65 775f 6f6c 645f 6e6f  data, new_old_no
-00001780: 6465 5f76 616c 5f64 6174 612c 206e 6577  de_val_data, new
-00001790: 5f6f 6c64 5f6e 6f64 655f 7465 7374 5f64  _old_node_test_d
-000017a0: 6174 612c 206e 6577 5f6e 6577 5f6e 6f64  ata, new_new_nod
-000017b0: 655f 7661 6c5f 6461 7461 2c20 6e65 775f  e_val_data, new_
-000017c0: 6e65 775f 6e6f 6465 5f74 6573 745f 6461  new_node_test_da
-000017d0: 7461 2c20 756e 7365 656e 5f6e 6f64 6573  ta, unseen_nodes
-000017e0: 5f6e 756d 203d 2067 6574 5f64 6174 6128  _num = get_data(
-000017f0: 6461 7461 7365 745f 6e61 6d65 2c20 6469  dataset_name, di
-00001800: 6666 6572 656e 745f 6e65 775f 6e6f 6465  fferent_new_node
-00001810: 735f 6265 7477 6565 6e5f 7661 6c5f 616e  s_between_val_an
-00001820: 645f 7465 7374 3d46 616c 7365 2c20 7261  d_test=False, ra
-00001830: 6e64 6f6d 697a 655f 6665 6174 7572 6573  ndomize_features
-00001840: 3d46 616c 7365 290a 6060 600a 0a23 2323  =False).```..###
-00001850: 2045 6467 6553 616d 706c 6572 0a42 656e   EdgeSampler.Ben
-00001860: 6368 5465 4d50 2070 726f 7669 6465 7320  chTeMP provides 
-00001870: 7468 6520 756e 6966 6965 640a 6e65 6761  the unified.nega
-00001880: 7469 7665 2065 6467 6520 7361 6d70 6c65  tive edge sample
-00001890: 7220 7769 7468 202a 2a73 6565 642a 2a20  r with **seed** 
-000018a0: 666f 7220 4c69 6e6b 2050 7265 6469 6374  for Link Predict
-000018b0: 696f 6e20 7461 736b 2074 6f20 2073 616d  ion task to  sam
-000018c0: 706c 6520 616e 2065 7175 616c 2061 6d6f  ple an equal amo
-000018d0: 756e 7420 6f66 206e 6567 6174 6976 6573  unt of negatives
-000018e0: 2074 6f20 7468 6520 706f 7369 7469 7665   to the positive
-000018f0: 2069 6e74 6572 6163 7469 6f6e 732e 0a0a   interactions...
-00001900: 436c 6173 733a 0a0a 2a2a 5261 6e64 4564  Class:..**RandEd
-00001910: 6765 5361 6d70 6c65 7228 7372 635f 6c69  geSampler(src_li
-00001920: 7374 203a 206e 756d 7079 2e6e 6461 7272  st : numpy.ndarr
-00001930: 6179 2c20 6473 745f 6c69 7374 203a 206e  ay, dst_list : n
-00001940: 756d 7079 2e6e 6461 7272 6179 2c20 7365  umpy.ndarray, se
-00001950: 6564 203a 2069 6e74 203d 4e6f 6e65 292a  ed : int =None)*
-00001960: 2a0a 0a50 6172 616d 6574 6572 733a 0a2d  *..Parameters:.-
-00001970: 202a 2a73 7263 5f6c 6973 7420 3a20 6e75   **src_list : nu
-00001980: 6d70 792e 6e64 6172 7261 792a 2a20 2d20  mpy.ndarray** - 
-00001990: 7468 6520 6c69 7374 206f 6620 736f 7572  the list of sour
-000019a0: 6365 206e 6f64 6573 2e0a 2d20 2a2a 6473  ce nodes..- **ds
-000019b0: 745f 6c69 7374 203a 206e 756d 7079 2e6e  t_list : numpy.n
-000019c0: 6461 7272 6179 2a2a 202d 2074 6865 206c  darray** - the l
-000019d0: 6973 7420 6f66 2064 6573 7469 6e61 7469  ist of destinati
-000019e0: 6f6e 206e 6f64 6573 2e0a 2d20 2a2a 7365  on nodes..- **se
-000019f0: 6564 203a 206e 756d 7079 2e6e 6461 7272  ed : numpy.ndarr
-00001a00: 6179 2a2a 202d 2073 6565 6420 6f66 2072  ay** - seed of r
-00001a10: 616e 646f 6d2e 0a0a 5265 7475 726e 733a  andom...Returns:
-00001a20: 200a 0a2d 202a 2a62 656e 6368 7465 6d70   ..- **benchtemp
-00001a30: 2e52 616e 6445 6467 6553 616d 706c 6572  .RandEdgeSampler
-00001a40: 2a2a 0a0a 4578 616d 706c 653a 0a60 6060  **..Example:.```
-00001a50: 7079 7468 6f6e 0a66 726f 6d20 6265 6e63  python.from benc
-00001a60: 6874 656d 702e 6c70 2e73 616d 706c 6572  htemp.lp.sampler
-00001a70: 2069 6d70 6f72 7420 5261 6e64 4564 6765   import RandEdge
-00001a80: 5361 6d70 6c65 720a 0a23 2046 6f72 2065  Sampler..# For e
-00001a90: 7861 6d70 6c65 2c20 6966 2079 6f75 2061  xample, if you a
-00001aa0: 7265 2074 7261 696e 696e 6720 2c20 796f  re training , yo
-00001ab0: 7520 7368 6f75 6c64 2063 7265 6174 6520  u should create 
-00001ac0: 6120 7472 6169 6e69 6e67 2020 5261 6e64  a training  Rand
-00001ad0: 4564 6765 5361 6d70 6c65 7220 6261 7365  EdgeSampler base
-00001ae0: 6420 6f6e 2074 6865 2074 7261 696e 696e  d on the trainin
-00001af0: 6720 6461 7461 7365 742e 0a74 7261 696e  g dataset..train
-00001b00: 5f72 616e 645f 7361 6d70 6c65 7220 3d20  _rand_sampler = 
-00001b10: 5261 6e64 4564 6765 5361 6d70 6c65 7228  RandEdgeSampler(
-00001b20: 7472 6169 6e5f 6461 7461 2e73 6f75 7263  train_data.sourc
-00001b30: 6573 2c20 7472 6169 6e5f 6461 7461 2e64  es, train_data.d
-00001b40: 6573 7469 6e61 7469 6f6e 7329 0a0a 2e2e  estinations)....
-00001b50: 2e0a 666f 7220 6570 6f63 6820 696e 2072  ..for epoch in r
-00001b60: 616e 6765 2861 7267 732e 6570 6f63 6873  ange(args.epochs
-00001b70: 293a 0a20 2020 202e 2e2e 0a20 2020 2023  ):.    ....    #
-00001b80: 2073 616d 706c 6520 616e 2065 7175 616c   sample an equal
-00001b90: 2061 6d6f 756e 7420 6f66 206e 6567 6174   amount of negat
-00001ba0: 6976 6573 2074 6f20 7468 6520 706f 7369  ives to the posi
-00001bb0: 7469 7665 2069 6e74 6572 6163 7469 6f6e  tive interaction
-00001bc0: 732e 0a20 2020 205f 2c20 6e65 6761 7469  s..    _, negati
-00001bd0: 7665 735f 6261 7463 6820 3d20 7472 6169  ves_batch = trai
-00001be0: 6e5f 7261 6e64 5f73 616d 706c 6572 2e73  n_rand_sampler.s
-00001bf0: 616d 706c 6528 7369 7a65 290a 2020 2020  ample(size).    
-00001c00: 2e2e 2e0a 2e2e 2e0a 6060 600a 2323 2320  ........```.### 
-00001c10: 2832 2920 4e6f 6465 2043 6c61 7373 6966  (2) Node Classif
-00001c20: 6963 6174 696f 6e20 7461 736b 0a46 756e  ication task.Fun
-00001c30: 6374 696f 6e3a 0a0a 0a0a 2a2a 6265 6e63  ction:....**benc
-00001c40: 6874 656d 702e 6e63 2e72 6561 6465 7273  htemp.nc.readers
-00001c50: 2e67 6574 5f64 6174 615f 6e6f 6465 5f63  .get_data_node_c
-00001c60: 6c61 7373 6966 6963 6174 696f 6e28 2864  lassification((d
-00001c70: 6174 6173 6574 5f6e 616d 6520 3a20 7374  ataset_name : st
-00001c80: 722c 2075 7365 5f76 616c 6964 6174 696f  r, use_validatio
-00001c90: 6e20 3a20 626f 6f6c 3d46 616c 7365 2929  n : bool=False))
-00001ca0: 2a2a 200a 0a50 6172 616d 6574 6572 733a  ** ..Parameters:
-00001cb0: 0a2d 2064 6174 6173 6574 5f6e 616d 6520  .- dataset_name 
-00001cc0: 3a20 7374 7220 2d20 5468 6520 6e61 6d65  : str - The name
-00001cd0: 206f 6620 7468 6520 6461 7461 7365 742e   of the dataset.
-00001ce0: 2054 6865 2064 6174 6173 6574 2066 696c   The dataset fil
-00001cf0: 6520 282e 6373 7620 6669 6c65 206f 6620  e (.csv file of 
-00001d00: 7468 6520 5465 6d70 6f72 616c 2047 7261  the Temporal Gra
-00001d10: 7068 2c20 2e6e 7079 2066 696c 6520 6f66  ph, .npy file of
-00001d20: 2074 6865 206e 6f64 6520 6665 6174 7572   the node featur
-00001d30: 6573 2061 6e64 202e 6e70 7920 6669 6c65  es and .npy file
-00001d40: 206f 6620 7468 6520 6564 6765 2066 6561   of the edge fea
-00001d50: 7475 7265 7329 2073 686f 756c 6420 6265  tures) should be
-00001d60: 2069 6e20 222e 2f64 6174 6122 2064 6972   in "./data" dir
-00001d70: 6563 746f 7279 2e0a 2d20 7573 655f 7661  ectory..- use_va
-00001d80: 6c69 6461 7469 6f6e 203a 2062 6f6f 6c20  lidation : bool 
-00001d90: 2d20 5768 6574 6865 7220 7573 6520 7661  - Whether use va
-00001da0: 6c69 6461 7469 6f6e 2064 6174 6173 6574  lidation dataset
-00001db0: 206f 7220 6e6f 742e 0a0a 5265 7475 726e   or not...Return
-00001dc0: 733a 0a2d 202a 2a6e 6f64 655f 6665 6174  s:.- **node_feat
-00001dd0: 7572 6573 203a 206e 756d 7079 2e6e 6461  ures : numpy.nda
-00001de0: 7272 6179 2a2a 202d 2041 7272 6179 206f  rray** - Array o
-00001df0: 6620 7468 6520 4e6f 6465 2046 6561 7475  f the Node Featu
-00001e00: 7265 7320 6f66 2074 6865 2054 656d 706f  res of the Tempo
-00001e10: 7261 6c20 4772 6170 682e 200a 2d20 2a2a  ral Graph. .- **
-00001e20: 6564 6765 5f66 6561 7475 7265 7320 3a20  edge_features : 
-00001e30: 6e75 6d70 792e 6e64 6172 7261 792a 2a20  numpy.ndarray** 
-00001e40: 2d20 4172 7261 7920 6f66 2074 6865 2045  - Array of the E
-00001e50: 6467 6520 4665 6174 7572 6573 206f 6620  dge Features of 
-00001e60: 7468 6520 5465 6d70 6f72 616c 2047 7261  the Temporal Gra
-00001e70: 7068 2e0a 2d20 2a2a 6675 6c6c 5f64 6174  ph..- **full_dat
-00001e80: 6120 3a20 6265 6e63 6874 656d 702e 4461  a : benchtemp.Da
-00001e90: 7461 2a2a 202d 2046 756c 6c20 5465 6d70  ta** - Full Temp
-00001ea0: 6f72 616c 2047 7261 7068 2064 6174 6173  oral Graph datas
-00001eb0: 6574 2066 6f72 204e 6f64 6520 436c 6173  et for Node Clas
-00001ec0: 7369 6669 6361 7469 6f6e 2074 6173 6b2e  sification task.
-00001ed0: 200a 2d20 2a2a 7472 6169 6e5f 6461 7461   .- **train_data
-00001ee0: 203a 2062 656e 6368 7465 6d70 2e44 6174   : benchtemp.Dat
-00001ef0: 612a 2a20 2d20 5468 6520 7472 6169 6e69  a** - The traini
-00001f00: 6e67 2054 656d 706f 7261 6c20 4772 6170  ng Temporal Grap
-00001f10: 6820 6461 7461 7365 7420 666f 7220 4e6f  h dataset for No
-00001f20: 6465 2043 6c61 7373 6966 6963 6174 696f  de Classificatio
-00001f30: 6e20 7461 736b 2e20 0a2d 202a 2a76 616c  n task. .- **val
-00001f40: 5f64 6174 6120 3a20 6265 6e63 6874 656d  _data : benchtem
-00001f50: 702e 4461 7461 2a2a 202d 2054 6865 2076  p.Data** - The v
-00001f60: 616c 6964 6174 696f 6e20 5465 6d70 6f72  alidation Tempor
-00001f70: 616c 2047 7261 7068 2064 6174 6173 6574  al Graph dataset
-00001f80: 2066 6f72 204e 6f64 6520 436c 6173 7369   for Node Classi
-00001f90: 6669 6361 7469 6f6e 2074 6173 6b2e 0a2d  fication task..-
-00001fa0: 202a 2a74 6573 745f 6461 7461 203a 2062   **test_data : b
-00001fb0: 656e 6368 7465 6d70 2e44 6174 612a 2a20  enchtemp.Data** 
-00001fc0: 202d 2054 6865 2074 6573 7420 5465 6d70   - The test Temp
-00001fd0: 6f72 616c 2047 7261 7068 2064 6174 6173  oral Graph datas
-00001fe0: 6574 2066 6f72 204e 6f64 6520 436c 6173  et for Node Clas
-00001ff0: 7369 6669 6361 7469 6f6e 2074 6173 6b2e  sification task.
-00002000: 0a0a 0a0a 2323 2320 4561 726c 7953 746f  ....### EarlySto
-00002010: 704d 6f6e 6974 6f72 0a43 6c61 7373 3a0a  pMonitor.Class:.
-00002020: 0a2a 2a45 6172 6c79 5374 6f70 4d6f 6e69  .**EarlyStopMoni
-00002030: 746f 7228 6d61 785f 726f 756e 643d 332c  tor(max_round=3,
-00002040: 2068 6967 6865 725f 6265 7474 6572 3d54   higher_better=T
-00002050: 7275 652c 2074 6f6c 6572 616e 6365 3d31  rue, tolerance=1
-00002060: 652d 3130 292a 2a0a 0a50 6172 616d 6574  e-10)**..Paramet
-00002070: 6572 733a 0a2d 202a 2a6d 6178 5f72 6f75  ers:.- **max_rou
-00002080: 6e64 203a 2069 6e74 2a2a 202d 2074 6865  nd : int** - the
-00002090: 206d 6178 696d 756d 206e 756d 6265 7220   maximum number 
-000020a0: 6f66 2072 6f75 6e64 7320 6f66 2045 6172  of rounds of Ear
-000020b0: 6c79 5374 6f70 4d6f 6e69 746f 722e 0a2d  lyStopMonitor..-
-000020c0: 202a 2a68 6967 6865 725f 6265 7474 6572   **higher_better
-000020d0: 203a 2062 6f6f 6c2a 2a20 2d20 6265 7474   : bool** - bett
-000020e0: 6572 2074 6865 2070 6572 666f 726d 616e  er the performan
-000020f0: 6365 2e0a 2d20 2a2a 746f 6c65 7261 6e63  ce..- **toleranc
-00002100: 6520 3a20 666c 6f61 742a 2a20 2d20 7468  e : float** - th
-00002110: 6520 746f 6c65 7261 6e63 6520 6f66 2074  e tolerance of t
-00002120: 6865 2045 6172 6c79 5374 6f70 4d6f 6e69  he EarlyStopMoni
-00002130: 746f 722e 0a0a 5265 7475 726e 733a 0a2d  tor...Returns:.-
-00002140: 202a 2a62 656e 6368 7465 6d70 2e45 6172   **benchtemp.Ear
-00002150: 6c79 5374 6f70 4d6f 6e69 746f 722a 2a0a  lyStopMonitor**.
-00002160: 0a45 7861 6d70 6c65 3a0a 6060 6070 7974  .Example:.```pyt
-00002170: 686f 6e0a 6672 6f6d 2062 656e 6368 7465  hon.from benchte
-00002180: 6d70 2e75 7469 6c73 2069 6d70 6f72 7420  mp.utils import 
-00002190: 4561 726c 7953 746f 704d 6f6e 6974 6f72  EarlyStopMonitor
-000021a0: 0a0a 2e2e 2e0a 6561 726c 795f 7374 6f70  ......early_stop
-000021b0: 7065 7220 3d20 4561 726c 7953 746f 704d  per = EarlyStopM
-000021c0: 6f6e 6974 6f72 286d 6178 5f72 6f75 6e64  onitor(max_round
-000021d0: 3d61 7267 732e 7061 7469 656e 6365 290a  =args.patience).
-000021e0: 666f 7220 6570 6f63 6820 696e 2072 616e  for epoch in ran
-000021f0: 6765 2861 7267 732e 6570 6f63 6873 293a  ge(args.epochs):
-00002200: 0a20 2020 202e 2e2e 0a20 2020 2076 616c  .    ....    val
-00002210: 5f61 7020 3d20 6d6f 6465 6c28 7661 6c5f  _ap = model(val_
-00002220: 6461 7461 7365 7473 290a 2020 2020 6966  datasets).    if
-00002230: 2065 6172 6c79 5f73 746f 7070 6572 2e65   early_stopper.e
-00002240: 6172 6c79 5f73 746f 705f 6368 6563 6b28  arly_stop_check(
-00002250: 7661 6c5f 6170 293a 0a20 2020 2020 2020  val_ap):.       
-00002260: 2062 7265 616b 0a20 2020 202e 2e2e 0a2e   break.    .....
-00002270: 2e2e 0a60 6060 0a0a 2323 2320 4576 616c  ...```..### Eval
-00002280: 7561 746f 720a 0a2a 2a4c 696e 6b20 5072  uator..**Link Pr
-00002290: 6564 6963 7469 6f6e 2a2a 2045 7661 6c75  ediction** Evalu
-000022a0: 6174 696f 6e20 4d65 7472 6963 7320 2061  ation Metrics  a
-000022b0: 7265 202a 2a41 7265 6120 556e 6465 7220  re **Area Under 
-000022c0: 7468 6520 5265 6365 6976 6572 204f 7065  the Receiver Ope
-000022d0: 7261 7469 6e67 2043 6861 7261 6374 6572  rating Character
-000022e0: 6973 7469 6320 4375 7276 6520 2852 4f43  istic Curve (ROC
-000022f0: 2041 5543 292a 2a20 616e 6420 2a2a 6176   AUC)** and **av
-00002300: 6572 6167 6520 7072 6563 6973 696f 6e20  erage precision 
-00002310: 2841 5029 2a2a 0a0a 2a2a 4e6f 6465 2043  (AP)**..**Node C
-00002320: 6c61 7373 6966 6963 6174 696f 6e2a 2a20  lassification** 
-00002330: 4576 616c 7561 7469 6f6e 204d 6574 7269  Evaluation Metri
-00002340: 6320 6973 202a 2a41 7265 6120 556e 6465  c is **Area Unde
-00002350: 7220 7468 6520 5265 6365 6976 6572 204f  r the Receiver O
-00002360: 7065 7261 7469 6e67 2043 6861 7261 6374  perating Charact
-00002370: 6572 6973 7469 6320 4375 7276 6520 2852  eristic Curve (R
-00002380: 4f43 2041 5543 292a 2a0a 0a43 6c61 7373  OC AUC)**..Class
-00002390: 3a20 0a0a 2a2a 4576 616c 7561 746f 7228  : ..**Evaluator(
-000023a0: 7461 736b 5f6e 616d 653a 2073 7472 203d  task_name: str =
-000023b0: 2022 4c50 2229 2a2a 0a0a 5061 7261 6d65   "LP")**..Parame
-000023c0: 7465 7273 3a0a 2d20 7461 736b 5f6e 616d  ters:.- task_nam
-000023d0: 6520 3a20 7374 7220 202d 2074 6865 206e  e : str  - the n
-000023e0: 616d 6520 6f66 2074 6865 2074 6173 6b2c  ame of the task,
-000023f0: 2063 686f 6963 6520 696e 202a 2a5b 224c   choice in **["L
-00002400: 5022 2c20 224e 4322 5d2a 2a2e 0a0a 5265  P", "NC"]**...Re
-00002410: 7475 726e 733a 0a2d 202a 2a62 656e 6368  turns:.- **bench
-00002420: 7465 6d70 2e45 7661 6c75 6174 6f72 2a2a  temp.Evaluator**
-00002430: 0a0a 4578 616d 706c 653a 0a0a 6060 6070  ..Example:..```p
-00002440: 7974 686f 6e0a 6672 6f6d 2062 656e 6368  ython.from bench
-00002450: 7465 6d70 2e75 7469 6c73 2069 6d70 6f72  temp.utils impor
-00002460: 7420 4576 616c 7561 746f 720a 0a23 2046  t Evaluator..# F
-00002470: 6f72 2065 7861 6d70 6c65 2c20 4c69 6e6b  or example, Link
-00002480: 2070 7265 6469 6374 696f 6e20 7461 736b   prediction task
-00002490: 2e20 4576 616c 7561 7469 6f6e 204d 6574  . Evaluation Met
-000024a0: 7269 6373 3a20 4155 432c 2041 502e 0a65  rics: AUC, AP..e
-000024b0: 7661 6c75 6174 6f72 203d 2045 7661 6c75  valuator = Evalu
-000024c0: 6174 6f72 2822 4c50 2229 0a0a 2e2e 2e0a  ator("LP")......
-000024d0: 2320 7465 7374 2064 6174 610a 7072 6564  # test data.pred
-000024e0: 5f73 636f 7265 203d 206d 6f64 656c 2874  _score = model(t
-000024f0: 6573 745f 6461 7461 290a 7465 7374 5f61  est_data).test_a
-00002500: 7563 2c20 7465 7374 5f61 7020 3d20 4576  uc, test_ap = Ev
-00002510: 616c 7561 746f 722e 6576 616c 2870 7265  aluator.eval(pre
-00002520: 645f 7363 6f72 652c 2074 7275 655f 6c61  d_score, true_la
-00002530: 6265 6c29 0a2e 2e2e 0a60 6060 0a0a 6060  bel).....```..``
-00002540: 6070 7974 686f 6e0a 6672 6f6d 2062 656e  `python.from ben
-00002550: 6368 7465 6d70 2e75 7469 6c73 2069 6d70  chtemp.utils imp
-00002560: 6f72 7420 4576 616c 7561 746f 720a 0a23  ort Evaluator..#
-00002570: 2046 6f72 2065 7861 6d70 6c65 2c20 4e6f   For example, No
-00002580: 6465 2043 6c61 7373 6966 6963 6174 696f  de Classificatio
-00002590: 6e20 7461 736b 2e20 4576 616c 7561 7469  n task. Evaluati
-000025a0: 6f6e 204d 6574 7269 6373 3a20 4155 432e  on Metrics: AUC.
-000025b0: 0a65 7661 6c75 6174 6f72 203d 2045 7661  .evaluator = Eva
-000025c0: 6c75 6174 6f72 2822 4e43 2229 0a0a 2e2e  luator("NC")....
-000025d0: 2e0a 2320 7465 7374 2064 6174 610a 7072  ..# test data.pr
-000025e0: 6564 5f73 636f 7265 203d 206d 6f64 656c  ed_score = model
-000025f0: 2874 6573 745f 6461 7461 290a 7465 7374  (test_data).test
-00002600: 5f61 7563 203d 2045 7661 6c75 6174 6f72  _auc = Evaluator
-00002610: 2e65 7661 6c28 7072 6564 5f73 636f 7265  .eval(pred_score
-00002620: 2c20 7472 7565 5f6c 6162 656c 290a 2e2e  , true_label)...
-00002630: 2e0a 6060 600a 0a23 2320 4361 6c6c 2066  ..```..## Call f
-00002640: 6f72 2043 6f6e 7472 6962 7574 696f 6e73  or Contributions
-00002650: 0a0a 2a2a 4265 6e63 6854 654d 502a 2a20  ..**BenchTeMP** 
-00002660: 7072 6f6a 6563 7420 6973 206c 6f6f 6b69  project is looki
-00002670: 6e67 2066 6f72 2063 6f6e 7472 6962 7574  ng for contribut
-00002680: 6f72 7320 7769 7468 200a 6578 7065 7274  ors with .expert
-00002690: 6973 6520 616e 6420 656e 7468 7573 6961  ise and enthusia
-000026a0: 736d 2120 4966 2079 6f75 2068 6176 6520  sm! If you have 
-000026b0: 6120 6465 7369 7265 2074 6f20 636f 6e74  a desire to cont
-000026c0: 7269 6275 7465 2074 6f20 2a2a 4265 6e63  ribute to **Benc
-000026d0: 6854 654d 502a 2a2c 200a 706c 6561 7365  hTeMP**, .please
-000026e0: 2063 6f6e 7461 6374 205b 4265 6e63 6854   contact [BenchT
-000026f0: 654d 5020 7465 616d 5d28 6d61 696c 746f  eMP team](mailto
-00002700: 3a6a 6f6e 6e79 6875 616e 6768 6e75 4067  :jonnyhuanghnu@g
-00002710: 6d61 696c 2e63 6f6d 292e 0a0a 5c69 7465  mail.com)...\ite
-00002720: 6d20 5765 2072 656c 6561 7365 205c 7379  m We release \sy
-00002730: 732c 2061 2067 656e 6572 616c 2062 656e  s, a general ben
-00002740: 6368 6d61 726b 206c 6962 7261 7279 2066  chmark library f
-00002750: 6f72 2065 7661 6c75 6174 696e 6720 7465  or evaluating te
-00002760: 6d70 6f72 616c 2067 7261 7068 206d 6f64  mporal graph mod
-00002770: 656c 733b 0a0a 5c69 7465 6d20 5765 2070  els;..\item We p
-00002780: 726f 7669 6465 7320 756e 6966 6965 6420  rovides unified 
-00002790: 6265 6e63 6b6d 6172 6b20 7465 6d70 6f72  benckmark tempor
-000027a0: 616c 2067 7261 7068 2064 6174 6173 6574  al graph dataset
-000027b0: 7320 7072 6f63 6573 7365 6420 6279 205c  s processed by \
-000027c0: 7379 733b 0a0a 5c69 7465 6d20 5765 2062  sys;..\item We b
-000027d0: 656e 6368 6d61 726b 2065 7869 7374 696e  enchmark existin
-000027e0: 6720 7465 6d70 6f72 616c 2067 7261 7068  g temporal graph
-000027f0: 206d 6f64 656c 7320 6261 7365 6420 6f6e   models based on
-00002800: 205c 7379 7320 2066 6f72 2072 6f62 7573   \sys  for robus
-00002810: 7420 6465 7665 6c6f 706d 656e 7473 2061  t developments a
-00002820: 6e64 2061 6e61 6c79 7369 7320 7468 6520  nd analysis the 
-00002830: 7065 7266 6f72 6d61 6e63 6520 6f66 206d  performance of m
-00002840: 6f64 656c 7320 696e 2064 6574 6169 6c3b  odels in detail;
-00002850: 0a0a 5c69 7465 6d20 5765 2072 656c 7365  ..\item We relse
-00002860: 6420 7468 6520 6c65 6164 6572 626f 6172  d the leaderboar
-00002870: 6473 2066 6f72 2074 656d 706f 7261 6c20  ds for temporal 
-00002880: 6772 6170 6820 6d6f 6465 6c73 2e0a 0a    graph models...
+00000020: 2066 6f72 2045 7661 6c75 6174 696e 6720   for Evaluating 
+00000030: 5465 6d70 6f72 616c 2047 7261 7068 204e  Temporal Graph N
+00000040: 6575 7261 6c20 4e65 7477 6f72 6b73 0a0a  eural Networks..
+00000050: 2323 2042 656e 6368 5465 6d70 2046 7261  ## BenchTemp Fra
+00000060: 6d65 776f 726b 0a3c 696d 6720 7372 633d  mework.<img src=
+00000070: 2269 6d67 2f66 7261 6d65 776f 726b 2e70  "img/framework.p
+00000080: 6e67 2220 616c 743d 224f 7665 7276 6965  ng" alt="Overvie
+00000090: 7720 6f66 2042 656e 6368 5465 6d70 2220  w of BenchTemp" 
+000000a0: 7374 796c 653d 2277 6964 7468 3a31 3030  style="width:100
+000000b0: 253b 2220 2f3e 0a0a 2323 2042 656e 6368  %;" />..## Bench
+000000c0: 5465 6d70 2050 6970 656c 696e 650a 3c69  Temp Pipeline.<i
+000000d0: 6d67 2073 7263 3d22 696d 672f 7069 7065  mg src="img/pipe
+000000e0: 6c69 6e65 2e70 6e67 2220 616c 743d 2242  line.png" alt="B
+000000f0: 656e 6368 5465 6d70 2050 6970 656c 696e  enchTemp Pipelin
+00000100: 6522 2073 7479 6c65 3d22 7769 6474 683a  e" style="width:
+00000110: 3130 3025 3b22 202f 3e0a 0a23 2320 4f76  100%;" />..## Ov
+00000120: 6572 7669 6577 0a2a 2a42 656e 6368 5465  erview.**BenchTe
+00000130: 6d70 2a2a 2069 7320 6120 6765 6e65 7261  mp** is a genera
+00000140: 6c20 4265 6e63 686d 6172 6b20 5079 7468  l Benchmark Pyth
+00000150: 6f6e 204c 6962 7261 7279 2066 6f72 2075  on Library for u
+00000160: 7365 7273 2074 6f20 6576 616c 7561 7465  sers to evaluate
+00000170: 2054 656d 706f 7261 6c20 4772 6170 6820   Temporal Graph 
+00000180: 4e65 7572 616c 204e 6574 776f 726b 7320  Neural Networks 
+00000190: 2854 474e 4e73 2920 7175 6963 6b6c 7920  (TGNNs) quickly 
+000001a0: 616e 6420 6566 6669 6369 656e 746c 7920  and efficiently 
+000001b0: 6f6e 2076 6172 696f 7573 2077 6f72 6b6c  on various workl
+000001c0: 6f61 6473 2e20 0a2a 2a42 656e 6368 5465  oads. .**BenchTe
+000001d0: 6d70 2a2a 2070 726f 7669 6465 7320 2a2a  mp** provides **
+000001e0: 4265 6e63 686d 6172 6b20 4461 7461 7365  Benchmark Datase
+000001f0: 7473 2a2a 2c20 616e 6420 756e 6966 6965  ts**, and unifie
+00000200: 6420 7069 7065 6c69 6e65 7320 282a 2a44  d pipelines (**D
+00000210: 6174 6150 7265 7072 6f63 6573 736f 722c  ataPreprocessor,
+00000220: 2044 6174 614c 6f61 6465 7220 4564 6765   DataLoader Edge
+00000230: 5361 6d70 6c65 722c 2045 7661 6c75 6174  Sampler, Evaluat
+00000240: 6f72 2c20 4561 726c 7953 746f 704d 6f6e  or, EarlyStopMon
+00000250: 6974 6f72 2c20 4243 454c 6f73 732c 204f  itor, BCELoss, O
+00000260: 7074 696d 697a 6572 2c61 6e64 204c 6561  ptimizer,and Lea
+00000270: 6465 7262 6f61 7264 2a2a 2029 2066 6f72  derboard** ) for
+00000280: 2065 7661 6c75 6174 696e 6720 5465 6d70   evaluating Temp
+00000290: 6f72 616c 2047 7261 7068 204e 6575 7261  oral Graph Neura
+000002a0: 6c20 4e65 7477 6f72 6b73 206f 6e20 626f  l Networks on bo
+000002b0: 7468 206c 696e 6b20 7072 6564 6963 7469  th link predicti
+000002c0: 6f6e 2061 6e64 206e 6f64 6520 636c 6173  on and node clas
+000002d0: 7369 6669 6361 7469 6f6e 2074 6173 6b73  sification tasks
+000002e0: 2e0a 0a2d 2054 6865 2042 656e 6368 5465  ...- The BenchTe
+000002f0: 6d70 2050 7950 4920 5765 6273 6974 6520  mp PyPI Website 
+00000300: 6973 203c 6120 6872 6566 3d22 6874 7470  is <a href="http
+00000310: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000320: 6a65 6374 2f62 656e 6368 7465 6d70 2f22  ject/benchtemp/"
+00000330: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000340: 3e48 6572 653c 2f61 3e2e 0a0a 2d20 5468  >Here</a>...- Th
+00000350: 6520 4769 7448 7562 206f 6620 4265 6e63  e GitHub of Benc
+00000360: 6854 656d 7020 7072 6f6a 6563 7420 6973  hTemp project is
+00000370: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000380: 2f2f 6769 7468 7562 2e63 6f6d 2f71 6961  //github.com/qia
+00000390: 6e67 6875 616e 6777 6875 2f62 656e 6368  nghuangwhu/bench
+000003a0: 7465 6d70 2220 7461 7267 6574 3d22 5f62  temp" target="_b
+000003b0: 6c61 6e6b 223e 4865 7265 3c2f 613e 2e20  lank">Here</a>. 
+000003c0: 0a0a 2d20 5468 6520 6461 7461 7365 7473  ..- The datasets
+000003d0: 2061 7265 203c 6120 6872 6566 3d22 6874   are <a href="ht
+000003e0: 7470 733a 2f2f 6472 6976 652e 676f 6f67  tps://drive.goog
+000003f0: 6c65 2e63 6f6d 2f64 7269 7665 2f66 6f6c  le.com/drive/fol
+00000400: 6465 7273 2f31 484b 5346 4745 6678 4844  ders/1HKSFGEfxHD
+00000410: 6c48 7551 5a36 6e4b 3453 4c43 454d 4651  lHuQZ6nK4SLCEMFQ
+00000420: 494f 747a 707a 3f75 7370 3d73 6861 7269  IOtzpz?usp=shari
+00000430: 6e67 2220 7461 7267 6574 3d22 5f62 6c61  ng" target="_bla
+00000440: 6e6b 223e 4865 7265 3c2f 613e 2e20 0a0a  nk">Here</a>. ..
+00000450: 2d20 5468 6520 6c65 6164 6572 626f 6172  - The leaderboar
+00000460: 6473 2077 6562 7369 7465 2066 6f72 2054  ds website for T
+00000470: 656d 706f 7261 6c20 4772 6170 6820 4e65  emporal Graph Ne
+00000480: 7572 616c 204e 6574 776f 726b 7320 6f6e  ural Networks on
+00000490: 2062 6f74 6820 4c69 6e6b 2050 7265 6469   both Link Predi
+000004a0: 6374 696f 6e20 616e 6420 4e6f 6465 2043  ction and Node C
+000004b0: 6c61 7373 6966 6963 6174 696f 6e20 7461  lassification ta
+000004c0: 736b 7320 6973 203c 6120 6872 6566 3d22  sks is <a href="
+000004d0: 6874 7470 733a 2f2f 6d79 2d77 6562 7369  https://my-websi
+000004e0: 7465 2d36 676e 7069 6179 6d30 3839 3137  te-6gnpiaym08917
+000004f0: 3032 622d 3132 3537 3235 3932 3534 2e74  02b-1257259254.t
+00000500: 636c 6f75 6462 6173 6561 7070 2e63 6f6d  cloudbaseapp.com
+00000510: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
+00000520: 6b22 3e48 6572 653c 2f61 3e2e 0a2d 2054  k">Here</a>..- T
+00000530: 6865 2073 6f75 7263 6520 636f 6465 7320  he source codes 
+00000540: 666f 7220 6576 616c 7561 7469 6e67 2065  for evaluating e
+00000550: 7869 7374 696e 6720 5465 6d70 6f72 616c  xisting Temporal
+00000560: 2047 7261 7068 204e 6575 7261 6c20 4e65   Graph Neural Ne
+00000570: 7477 6f72 6b73 2062 6173 6564 206f 6e20  tworks based on 
+00000580: 4265 6e63 6854 656d 7020 6172 6520 3c61  BenchTemp are <a
+00000590: 2068 7265 663d 2268 7474 7073 3a2f 2f6d   href="https://m
+000005a0: 792d 7765 6273 6974 652d 3667 6e70 6961  y-website-6gnpia
+000005b0: 796d 3038 3931 3730 3262 2d31 3235 3732  ym0891702b-12572
+000005c0: 3539 3235 342e 7463 6c6f 7564 6261 7365  59254.tcloudbase
+000005d0: 6170 702e 636f 6d2f 2220 7461 7267 6574  app.com/" target
+000005e0: 3d22 5f62 6c61 6e6b 223e 636f 6d69 6e67  ="_blank">coming
+000005f0: 2073 6f6f 6e3c 2f61 3e2e 0a0a 0a23 2320   soon</a>....## 
+00000600: 496e 7374 616c 6c61 7469 6f6e 0a23 2323  Installation.###
+00000610: 2052 6571 7569 7265 6d65 6e74 730a 506c   Requirements.Pl
+00000620: 6561 7365 2065 6e73 7572 6520 7468 6174  ease ensure that
+00000630: 2079 6f75 2068 6176 6520 696e 7374 616c   you have instal
+00000640: 6c65 6420 7468 6520 666f 6c6c 6f77 696e  led the followin
+00000650: 6720 6465 7065 6e64 656e 6369 6573 3a0a  g dependencies:.
+00000660: 0a2d 206e 756d 7079 203e 3d20 312e 3138  .- numpy >= 1.18
+00000670: 2e30 0a2d 2070 616e 6461 7320 3e3d 2031  .0.- pandas >= 1
+00000680: 2e32 2e30 0a2d 2073 6b6c 6561 726e 203e  .2.0.- sklearn >
+00000690: 3d20 302e 3230 2e30 0a0a 2323 2320 4265  = 0.20.0..### Be
+000006a0: 6e63 6854 656d 7020 5079 5049 2069 6e73  nchTemp PyPI ins
+000006b0: 7461 6c6c 0a0a 6060 6062 6173 680a 7069  tall..```bash.pi
+000006c0: 7033 2069 6e73 7461 6c6c 2062 656e 6368  p3 install bench
+000006d0: 7465 6d70 200a 6060 600a 0a0a 2323 2050  temp .```...## P
+000006e0: 6163 6b61 6765 2055 7361 6765 0a0a 0a23  ackage Usage...#
+000006f0: 2323 2044 6174 6173 6574 730a 5468 6520  ## Datasets.The 
+00000700: 6461 7461 7365 7473 2074 6861 7420 6861  datasets that ha
+00000710: 7665 2062 6565 6e20 7072 6570 726f 6365  ve been preproce
+00000720: 7373 6564 2062 7920 4265 6e63 6854 656d  ssed by BenchTem
+00000730: 7020 6172 6520 5b48 6572 655d 2868 7474  p are [Here](htt
+00000740: 7073 3a2f 2f64 7269 7665 2e67 6f6f 676c  ps://drive.googl
+00000750: 652e 636f 6d2f 6472 6976 652f 666f 6c64  e.com/drive/fold
+00000760: 6572 732f 3148 4b53 4647 4566 7848 446c  ers/1HKSFGEfxHDl
+00000770: 4875 515a 366e 4b34 534c 4345 4d46 5149  HuQZ6nK4SLCEMFQI
+00000780: 4f74 7a70 7a3f 7573 703d 7368 6172 696e  Otzpz?usp=sharin
+00000790: 6729 2e0a 596f 7520 6361 6e20 6469 7265  g)..You can dire
+000007a0: 6374 6c79 2064 6f77 6e6c 6f61 6420 7468  ctly download th
+000007b0: 6520 6461 7461 7365 7473 2061 6e64 2074  e datasets and t
+000007c0: 6865 6e20 7075 7420 7468 656d 2069 6e74  hen put them int
+000007d0: 6f20 7468 6520 6469 7265 6374 6f72 7920  o the directory 
+000007e0: 272e 2f64 6174 6127 2e0a 0a49 6e20 6164  './data'...In ad
+000007f0: 6469 7469 6f6e 2c20 4265 6e63 6854 656d  dition, BenchTem
+00000800: 7020 7072 6f76 6964 6573 2064 6174 6120  p provides data 
+00000810: 7072 6f63 6573 7369 6e67 2066 756e 6374  processing funct
+00000820: 696f 6e73 2066 6f72 2079 6f75 2074 6f20  ions for you to 
+00000830: 7072 6570 726f 6365 7373 2079 6f75 7273  preprocess yours
+00000840: 2054 474e 4e73 2064 6174 6173 6574 732e   TGNNs datasets.
+00000850: 200a 3c21 2d2d 2079 6f75 2063 616e 2064   .<!-- you can d
+00000860: 6f77 6e6c 6f61 6420 7468 6520 6f72 6967  ownload the orig
+00000870: 696e 616c 2064 6174 6173 6574 7320 5b48  inal datasets [H
+00000880: 6572 655d 2829 2061 6e64 2074 6865 6e20  ere]() and then 
+00000890: 202d 2d3e 0a3c 212d 2d20 7573 6520 7468   -->.<!-- use th
+000008a0: 6520 6675 6e63 7469 6f6e 7320 7072 6f76  e functions prov
+000008b0: 6964 6564 2062 7920 4265 6e63 6854 656d  ided by BenchTem
+000008c0: 7020 666f 7220 6461 7461 2064 6174 612e  p for data data.
+000008d0: 202d 2d3e 0a0a 4675 6e63 7469 6f6e 3a0a   -->..Function:.
+000008e0: 2a2a 6265 6e63 6874 656d 702e 7072 6570  **benchtemp.prep
+000008f0: 726f 6365 7373 696e 672e 6461 7461 2e64  rocessing.data.d
+00000900: 6174 615f 7072 6570 726f 6365 7373 2864  ata_preprocess(d
+00000910: 6174 615f 6e61 6d65 203a 2073 7472 2c20  ata_name : str, 
+00000920: 6269 7061 7274 6974 6520 3a20 626f 6f6c  bipartite : bool
+00000930: 3d54 7275 6529 2a2a 0a0a 5061 7261 6d65  =True)**..Parame
+00000940: 7465 7273 3a0a 2d20 2a2a 6461 7461 5f6e  ters:.- **data_n
+00000950: 616d 6520 3a20 7374 722a 2a20 2d20 7468  ame : str** - th
+00000960: 6520 6e61 6d65 206f 6620 7468 6520 6461  e name of the da
+00000970: 7461 7365 742e 0a2d 202a 2a62 6970 6172  taset..- **bipar
+00000980: 7469 7465 203a 2062 6f6f 6c2a 2a20 2d20  tite : bool** - 
+00000990: 5768 6574 6865 7220 7468 6520 5465 6d70  Whether the Temp
+000009a0: 6f72 616c 2047 7261 7068 2069 7320 6269  oral Graph is bi
+000009b0: 7061 7274 6974 6520 6772 6170 682e 0a0a  partite graph...
+000009c0: 5265 7475 726e 733a 0a2d 202a 2a6d 6c5f  Returns:.- **ml_
+000009d0: 7b64 6174 615f 6e61 6d65 7d2e 6373 762a  {data_name}.csv*
+000009e0: 2a20 2d20 7468 6520 6373 7620 6669 6c65  * - the csv file
+000009f0: 206f 6620 7468 6520 5465 6d70 6f72 616c   of the Temporal
+00000a00: 2047 7261 7068 2e0a 2d20 2a2a 6d6c 5f7b   Graph..- **ml_{
+00000a10: 6461 7461 5f6e 616d 657d 2e6e 7079 2a2a  data_name}.npy**
+00000a20: 202d 2074 6865 2065 6467 6520 6665 6174   - the edge feat
+00000a30: 7572 6573 206f 6620 7468 6520 5465 6d70  ures of the Temp
+00000a40: 6f72 616c 2047 7261 7068 2e0a 2d20 2a2a  oral Graph..- **
+00000a50: 6d6c 5f7b 6461 7461 5f6e 616d 657d 5f6e  ml_{data_name}_n
+00000a60: 6f64 652e 6e70 792a 2a20 2d20 7468 6520  ode.npy** - the 
+00000a70: 6e6f 6465 2066 6561 7475 7265 7320 6f66  node features of
+00000a80: 2074 6865 2054 656d 706f 7261 6c20 4772   the Temporal Gr
+00000a90: 6170 682e 0a0a 4578 616d 706c 653a 0a0a  aph...Example:..
+00000aa0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00000ab0: 2062 656e 6368 7465 6d70 2061 7320 6274   benchtemp as bt
+00000ac0: 0a0a 7072 6f63 6573 736f 7220 3d20 6274  ..processor = bt
+00000ad0: 2e44 6174 6150 7265 7072 6f63 6573 736f  .DataPreprocesso
+00000ae0: 7228 6461 7461 5f70 6174 683d 222e 2f64  r(data_path="./d
+00000af0: 6174 612f 222c 2064 6174 615f 6e61 6d65  ata/", data_name
+00000b00: 3d22 6d6f 6f63 2229 0a23 2049 6620 7468  ="mooc").# If th
+00000b10: 6520 6461 7461 7365 7420 6973 2062 6970  e dataset is bip
+00000b20: 6172 7469 7465 2067 7261 7068 2c20 692e  artite graph, i.
+00000b30: 652e 2074 6865 2075 7365 7220 2873 6f75  e. the user (sou
+00000b40: 7263 6520 6e6f 6465 7329 2061 6e64 2074  rce nodes) and t
+00000b50: 6865 2069 7465 6d20 2864 6573 7469 6e61  he item (destina
+00000b60: 7469 6f6e 206e 6f64 6573 2920 6172 6520  tion nodes) are 
+00000b70: 6f66 2074 6865 2073 616d 6520 7479 7065  of the same type
+00000b80: 2e0a 7072 6f63 6573 736f 722e 6461 7461  ..processor.data
+00000b90: 5f70 7265 7072 6f63 6573 7328 6269 7061  _preprocess(bipa
+00000ba0: 7274 6974 653d 5472 7565 290a 0a23 206e  rtite=True)..# n
+00000bb0: 6f6e 2d62 6970 6172 7469 7465 2067 7261  on-bipartite gra
+00000bc0: 7068 2e0a 7072 6f63 6573 736f 722e 6461  ph..processor.da
+00000bd0: 7461 5f70 7265 7072 6f63 6573 7328 6269  ta_preprocess(bi
+00000be0: 7061 7274 6974 653d 4661 6c73 6529 0a60  partite=False).`
+00000bf0: 6060 0a0a 4e6f 7465 733a 0a0a 466f 7220  ``..Notes:..For 
+00000c00: 6269 7061 7274 6974 6520 6772 6170 682c  bipartite graph,
+00000c10: 2042 656e 6368 5465 6d70 2077 696c 6c20   BenchTemp will 
+00000c20: 6661 6374 6f72 697a 6520 7468 6520 736f  factorize the so
+00000c30: 7572 6365 206e 6f64 6520 696e 6465 7820  urce node index 
+00000c40: 616e 6420 0a74 6865 2064 6573 7469 6e61  and .the destina
+00000c50: 7469 6f6e 206e 6f64 6520 696e 6465 782c  tion node index,
+00000c60: 2072 6573 7065 6374 6976 656c 792e 200a   respectively. .
+00000c70: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00000c80: 2070 616e 6461 7320 6173 2070 640a 0a61   pandas as pd..a
+00000c90: 7373 6572 7420 6c65 6e28 736f 7572 6365  ssert len(source
+00000ca0: 7329 203d 3d20 6c65 6e28 6465 7374 696e  s) == len(destin
+00000cb0: 6174 696f 6e73 290a 0a23 2062 6970 6172  ations)..# bipar
+00000cc0: 7469 7465 2067 7261 7068 0a73 6f75 7263  tite graph.sourc
+00000cd0: 6573 2c20 5f20 3d20 7064 2e66 6163 746f  es, _ = pd.facto
+00000ce0: 7269 7a65 2873 6f75 7263 6573 290a 6465  rize(sources).de
+00000cf0: 7374 696e 6174 696f 6e73 2c20 5f20 3d20  stinations, _ = 
+00000d00: 7064 2e66 6163 746f 7269 7a65 2864 6573  pd.factorize(des
+00000d10: 7469 6e61 7469 6f6e 7329 0a0a 7570 7065  tinations)..uppe
+00000d20: 725f 7520 3d20 736f 7572 6365 732e 6d61  r_u = sources.ma
+00000d30: 7820 2b20 310a 6465 7374 696e 6174 696f  x + 1.destinatio
+00000d40: 6e73 203d 2064 6573 7469 6e61 7469 6f6e  ns = destination
+00000d50: 7320 2b20 7570 7065 725f 750a 6060 600a  s + upper_u.```.
+00000d60: 466f 7220 6e6f 6e2d 6269 7061 7274 6974  For non-bipartit
+00000d70: 6520 6772 6170 682c 2042 656e 6368 5465  e graph, BenchTe
+00000d80: 6d70 2077 696c 6c20 6661 6374 6f72 697a  mp will factoriz
+00000d90: 6520 7468 6520 636f 6e63 6174 656e 6174  e the concatenat
+00000da0: 696f 6e20 6f66 2073 6f75 7263 6520 6e6f  ion of source no
+00000db0: 6465 2061 7272 6179 2061 6e64 200a 7468  de array and .th
+00000dc0: 6520 6465 7374 696e 6174 696f 6e20 6e6f  e destination no
+00000dd0: 6465 2061 7272 6179 2e20 0a0a 6060 6070  de array. ..```p
+00000de0: 7974 686f 6e0a 696d 706f 7274 2070 616e  ython.import pan
+00000df0: 6461 7320 6173 2070 640a 696d 706f 7274  das as pd.import
+00000e00: 206e 756d 7079 2061 7320 6e70 0a0a 6173   numpy as np..as
+00000e10: 7365 7274 206c 656e 2873 6f75 7263 6573  sert len(sources
+00000e20: 2920 3d3d 206c 656e 2864 6573 7469 6e61  ) == len(destina
+00000e30: 7469 6f6e 7329 0a69 6e74 6572 6163 7469  tions).interacti
+00000e40: 6f6e 5f6e 756d 203d 206c 656e 2873 6f75  on_num = len(sou
+00000e50: 7263 6573 290a 0a23 206e 6f6e 2d62 6970  rces)..# non-bip
+00000e60: 6172 7469 7465 2067 7261 7068 0a6e 6f64  artite graph.nod
+00000e70: 655f 696e 6465 782c 205f 203d 2070 642e  e_index, _ = pd.
+00000e80: 6661 6374 6f72 697a 6528 6e70 2e63 6f6e  factorize(np.con
+00000e90: 6361 7465 6e61 7465 2828 736f 7572 6365  catenate((source
+00000ea0: 732c 2064 6573 7469 6e61 7469 6f6e 7329  s, destinations)
+00000eb0: 2c20 6178 6973 3d30 2929 0a0a 736f 7572  , axis=0))..sour
+00000ec0: 6365 7320 3d20 6e6f 6465 5f69 6e64 6578  ces = node_index
+00000ed0: 5b5b 303a 696e 7465 7261 6374 696f 6e5f  [[0:interaction_
+00000ee0: 6e75 6d5d 5d0a 6465 7374 696e 6174 696f  num]].destinatio
+00000ef0: 6e73 203d 206e 6f64 655f 696e 6465 785b  ns = node_index[
+00000f00: 5b69 6e74 6572 6163 7469 6f6e 5f6e 756d  [interaction_num
+00000f10: 3a69 6e74 6572 6163 7469 6f6e 5f6e 756d  :interaction_num
+00000f20: 202b 2069 6e74 6572 6163 7469 6f6e 5f6e   + interaction_n
+00000f30: 756d 5d5d 0a60 6060 0a0a 0a23 2323 2054  um]].```...### T
+00000f40: 656d 706f 7261 6c44 6174 6120 436c 6173  emporalData Clas
+00000f50: 730a 436c 6173 733a 0a0a 2a2a 4461 7461  s.Class:..**Data
+00000f60: 2873 6f75 7263 6573 203a 206e 756d 7079  (sources : numpy
+00000f70: 2e6e 6461 7272 6179 2c0a 6465 7374 696e  .ndarray,.destin
+00000f80: 6174 696f 6e73 203a 206e 756d 7079 2e6e  ations : numpy.n
+00000f90: 6461 7272 6179 2c0a 7469 6d65 7374 616d  darray,.timestam
+00000fa0: 7073 203a 206e 756d 7079 2e6e 6461 7272  ps : numpy.ndarr
+00000fb0: 6179 2c0a 6564 6765 5f69 6478 7320 3a20  ay,.edge_idxs : 
+00000fc0: 6e75 6d70 792e 6e64 6172 7261 792c 0a6c  numpy.ndarray,.l
+00000fd0: 6162 656c 7320 3a20 6e75 6d70 792e 6e64  abels : numpy.nd
+00000fe0: 6172 7261 7929 2a2a 0a0a 5061 7261 6d65  array)**..Parame
+00000ff0: 7465 7273 3a0a 2d20 2a2a 736f 7572 6365  ters:.- **source
+00001000: 7320 3a20 6e75 6d70 792e 6e64 6172 7261  s : numpy.ndarra
+00001010: 792a 2a20 2d20 4172 7261 7920 6f66 2073  y** - Array of s
+00001020: 6f75 7263 6573 206f 6620 5465 6d70 6f72  ources of Tempor
+00001030: 616c 2047 7261 7068 2065 6467 6573 2e0a  al Graph edges..
+00001040: 2d20 2a2a 6465 7374 696e 6174 696f 6e73  - **destinations
+00001050: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
+00001060: 2a2a 202d 2041 7272 6179 206f 6620 6465  ** - Array of de
+00001070: 7374 696e 6174 696f 6e73 206f 6620 5465  stinations of Te
+00001080: 6d70 6f72 616c 2047 7261 7068 2065 6467  mporal Graph edg
+00001090: 6573 2e0a 2d20 2a2a 7469 6d65 7374 616d  es..- **timestam
+000010a0: 7073 203a 206e 756d 7079 2e6e 6461 7272  ps : numpy.ndarr
+000010b0: 6179 2a2a 202d 2041 7272 6179 206f 6620  ay** - Array of 
+000010c0: 7469 6d65 7374 616d 7073 206f 6620 5465  timestamps of Te
+000010d0: 6d70 6f72 616c 2047 7261 7068 2065 6467  mporal Graph edg
+000010e0: 6573 2e0a 2d20 2a2a 6564 6765 5f69 6478  es..- **edge_idx
+000010f0: 7320 3a20 6e75 6d70 792e 6e64 6172 7261  s : numpy.ndarra
+00001100: 792a 2a20 2d20 4172 7261 7920 6f66 2065  y** - Array of e
+00001110: 6467 6520 4944 7320 6f66 2054 656d 706f  dge IDs of Tempo
+00001120: 7261 6c20 4772 6170 6820 6564 6765 732e  ral Graph edges.
+00001130: 0a2d 202a 2a6c 6162 656c 7320 3a20 6e75  .- **labels : nu
+00001140: 6d70 792e 6e64 6172 7261 792a 2a20 2d20  mpy.ndarray** - 
+00001150: 4172 7261 7920 6f66 206c 6162 656c 7320  Array of labels 
+00001160: 6f66 2054 656d 706f 7261 6c20 4772 6170  of Temporal Grap
+00001170: 6865 2064 6765 732e 0a0a 5265 7475 726e  he dges...Return
+00001180: 733a 200a 2d20 2a2a 6265 6e63 6874 656d  s: .- **benchtem
+00001190: 702e 4461 7461 2a2a 2e20 4120 5465 6d70  p.Data**. A Temp
+000011a0: 6f72 616c 2047 7261 7068 2e0a 0a0a 0a0a  oral Graph......
+000011b0: 4578 616d 706c 653a 0a60 6060 7079 7468  Example:.```pyth
+000011c0: 6f6e 0a69 6d70 6f72 7420 7061 6e64 6173  on.import pandas
+000011d0: 2061 7320 7064 0a69 6d70 6f72 7420 6e75   as pd.import nu
+000011e0: 6d70 7920 6173 206e 700a 696d 706f 7274  mpy as np.import
+000011f0: 2062 656e 6368 7465 6d70 2061 7320 6274   benchtemp as bt
+00001200: 0a0a 0a67 7261 7068 5f64 6620 3d20 7064  ...graph_df = pd
+00001210: 2e72 6561 645f 6373 7628 2264 6174 6173  .read_csv("datas
+00001220: 6574 5f70 6174 6822 290a 0a73 6f75 7263  et_path")..sourc
+00001230: 6573 203d 2067 7261 7068 5f64 662e 752e  es = graph_df.u.
+00001240: 7661 6c75 6573 0a64 6573 7469 6e61 7469  values.destinati
+00001250: 6f6e 7320 3d20 6772 6170 685f 6466 2e69  ons = graph_df.i
+00001260: 2e76 616c 7565 730a 6564 6765 5f69 6478  .values.edge_idx
+00001270: 7320 3d20 6772 6170 685f 6466 2e69 6478  s = graph_df.idx
+00001280: 2e76 616c 7565 730a 6c61 6265 6c73 203d  .values.labels =
+00001290: 2067 7261 7068 5f64 662e 6c61 6265 6c2e   graph_df.label.
+000012a0: 7661 6c75 6573 0a74 696d 6573 7461 6d70  values.timestamp
+000012b0: 7320 3d20 6772 6170 685f 6466 2e74 732e  s = graph_df.ts.
+000012c0: 7661 6c75 6573 0a0a 2320 466f 7220 6578  values..# For ex
+000012d0: 616d 706c 652c 2074 6865 2066 756c 6c20  ample, the full 
+000012e0: 5465 6d70 6f72 616c 2047 7261 7068 206f  Temporal Graph o
+000012f0: 6620 7468 6520 6461 7461 7365 7420 6973  f the dataset is
+00001300: 2066 756c 6c5f 6461 7461 2e0a 6675 6c6c   full_data..full
+00001310: 5f64 6174 6120 3d20 6274 2e44 6174 6128  _data = bt.Data(
+00001320: 736f 7572 6365 732c 2064 6573 7469 6e61  sources, destina
+00001330: 7469 6f6e 732c 2074 696d 6573 7461 6d70  tions, timestamp
+00001340: 732c 2065 6467 655f 6964 7873 2c20 6c61  s, edge_idxs, la
+00001350: 6265 6c73 290a 6060 600a 0a0a 2323 2320  bels).```...### 
+00001360: 4461 7461 4c6f 6164 6572 0a23 2323 2028  DataLoader.### (
+00001370: 3129 204c 696e 6b20 5072 6564 6963 7469  1) Link Predicti
+00001380: 6f6e 2074 6173 6b0a 4675 6e63 7469 6f6e  on task.Function
+00001390: 3a0a 0a2a 2a62 656e 6368 7465 6d70 2e6c  :..**benchtemp.l
+000013a0: 702e 7265 6164 6572 732e 6765 745f 6461  p.readers.get_da
+000013b0: 7461 2864 6174 6173 6574 5f6e 616d 6520  ta(dataset_name 
+000013c0: 3a20 7374 722c 2064 6966 6665 7265 6e74  : str, different
+000013d0: 5f6e 6577 5f6e 6f64 6573 5f62 6574 7765  _new_nodes_betwe
+000013e0: 656e 5f76 616c 5f61 6e64 5f74 6573 743d  en_val_and_test=
+000013f0: 4661 6c73 652c 2072 616e 646f 6d69 7a65  False, randomize
+00001400: 5f66 6561 7475 7265 733d 4661 6c73 6529  _features=False)
+00001410: 2a2a 0a20 0a50 6172 616d 6574 6572 733a  **. .Parameters:
+00001420: 0a2d 202a 2a64 6174 6173 6574 5f6e 616d  .- **dataset_nam
+00001430: 6520 3a20 7374 722a 2a20 2d20 5468 6520  e : str** - The 
+00001440: 6e61 6d65 206f 6620 7468 6520 6461 7461  name of the data
+00001450: 7365 742e 2054 6865 2064 6174 6173 6574  set. The dataset
+00001460: 2066 696c 6520 282e 6373 7620 6669 6c65   file (.csv file
+00001470: 206f 6620 7468 6520 5465 6d70 6f72 616c   of the Temporal
+00001480: 2047 7261 7068 2c20 2e6e 7079 2066 696c   Graph, .npy fil
+00001490: 6520 6f66 2074 6865 206e 6f64 6520 6665  e of the node fe
+000014a0: 6174 7572 6573 2061 6e64 202e 6e70 7920  atures and .npy 
+000014b0: 6669 6c65 206f 6620 7468 6520 6564 6765  file of the edge
+000014c0: 2066 6561 7475 7265 7329 2073 686f 756c   features) shoul
+000014d0: 6420 6265 2069 6e20 222e 2f64 6174 6122  d be in "./data"
+000014e0: 2064 6972 6563 746f 7279 2e0a 2d20 2a2a   directory..- **
+000014f0: 6469 6666 6572 656e 745f 6e65 775f 6e6f  different_new_no
+00001500: 6465 735f 6265 7477 6565 6e5f 7661 6c5f  des_between_val_
+00001510: 616e 645f 7465 7374 203a 2062 6f6f 6c2a  and_test : bool*
+00001520: 2a20 2d20 4469 6666 6572 656e 7420 6e65  * - Different ne
+00001530: 7720 6e6f 6465 7320 6265 7477 6565 6e20  w nodes between 
+00001540: 2074 6865 2076 616c 6964 6174 696f 6e20   the validation 
+00001550: 616e 6420 7465 7374 2064 6174 6173 6574  and test dataset
+00001560: 2e0a 2d20 2a2a 7261 6e64 6f6d 697a 655f  ..- **randomize_
+00001570: 6665 6174 7572 6573 203a 2062 6f6f 6c2a  features : bool*
+00001580: 2a20 2d20 5261 6e64 6f6d 2069 6e69 7469  * - Random initi
+00001590: 616c 697a 6174 696f 6e20 6f66 206e 6f64  alization of nod
+000015a0: 6520 4665 6174 7572 6573 2e20 0a0a 5265  e Features. ..Re
+000015b0: 7475 726e 733a 0a2d 202a 2a6e 6f64 655f  turns:.- **node_
+000015c0: 6665 6174 7572 6573 203a 206e 756d 7079  features : numpy
+000015d0: 2e6e 6461 7272 6179 2a2a 202d 2041 7272  .ndarray** - Arr
+000015e0: 6179 206f 6620 7468 6520 4e6f 6465 2046  ay of the Node F
+000015f0: 6561 7475 7265 7320 6f66 2074 6865 2054  eatures of the T
+00001600: 656d 706f 7261 6c20 4772 6170 682e 200a  emporal Graph. .
+00001610: 2d20 2a2a 6564 6765 5f66 6561 7475 7265  - **edge_feature
+00001620: 7320 3a20 6e75 6d70 792e 6e64 6172 7261  s : numpy.ndarra
+00001630: 792a 2a20 2d20 4172 7261 7920 6f66 2074  y** - Array of t
+00001640: 6865 2045 6467 6520 4665 6174 7572 6573  he Edge Features
+00001650: 206f 6620 7468 6520 5465 6d70 6f72 616c   of the Temporal
+00001660: 2047 7261 7068 2e0a 2d20 2a2a 6675 6c6c   Graph..- **full
+00001670: 5f64 6174 6120 3a20 6265 6e63 6874 656d  _data : benchtem
+00001680: 702e 4461 7461 2a2a 202d 2046 756c 6c20  p.Data** - Full 
+00001690: 5465 6d70 6f72 616c 2047 7261 7068 2064  Temporal Graph d
+000016a0: 6174 6173 6574 2e20 0a2d 202a 2a74 7261  ataset. .- **tra
+000016b0: 696e 5f64 6174 6120 3a20 6265 6e63 6874  in_data : bencht
+000016c0: 656d 702e 4461 7461 2a2a 202d 2054 6865  emp.Data** - The
+000016d0: 2074 7261 696e 696e 6720 5465 6d70 6f72   training Tempor
+000016e0: 616c 2047 7261 7068 2064 6174 6173 6574  al Graph dataset
+000016f0: 2e20 0a2d 202a 2a76 616c 5f64 6174 6120  . .- **val_data 
+00001700: 3a20 6265 6e63 6874 656d 702e 4461 7461  : benchtemp.Data
+00001710: 2a2a 202d 2054 6865 2076 616c 6964 6174  ** - The validat
+00001720: 696f 6e20 5465 6d70 6f72 616c 2047 7261  ion Temporal Gra
+00001730: 7068 2064 6174 6173 6574 2e0a 2d20 2a2a  ph dataset..- **
+00001740: 7465 7374 5f64 6174 6120 3a20 6265 6e63  test_data : benc
+00001750: 6874 656d 702e 4461 7461 2a2a 2020 2d20  htemp.Data**  - 
+00001760: 5468 6520 2a2a 7472 616e 7364 7563 7469  The **transducti
+00001770: 7665 2a2a 2074 6573 7420 5465 6d70 6f72  ve** test Tempor
+00001780: 616c 2047 7261 7068 2064 6174 6173 6574  al Graph dataset
+00001790: 2e0a 2d20 2a2a 6e65 775f 6e6f 6465 5f76  ..- **new_node_v
+000017a0: 616c 5f64 6174 6120 3a20 6265 6e63 6874  al_data : bencht
+000017b0: 656d 702e 4461 7461 2a2a 202d 2054 6865  emp.Data** - The
+000017c0: 202a 2a69 6e64 7563 7469 7665 205b 6e65   **inductive [ne
+000017d0: 772d 5d2a 2a20 7365 7474 696e 6720 7661  w-]** setting va
+000017e0: 6c69 6461 7469 6f6e 2054 656d 706f 7261  lidation Tempora
+000017f0: 6c20 4772 6170 6820 6461 7461 7365 742e  l Graph dataset.
+00001800: 0a2d 202a 2a6e 6577 5f6e 6f64 655f 7465  .- **new_node_te
+00001810: 7374 5f64 6174 6120 3a20 6265 6e63 6874  st_data : bencht
+00001820: 656d 702e 4461 7461 2a2a 202d 2054 6865  emp.Data** - The
+00001830: 202a 2a69 6e64 7563 7469 7665 205b 6e65   **inductive [ne
+00001840: 772d 5d2a 2a20 7365 7474 696e 6720 7465  w-]** setting te
+00001850: 7374 2054 656d 706f 7261 6c20 4772 6170  st Temporal Grap
+00001860: 6820 6461 7461 7365 742e 0a2d 202a 2a6e  h dataset..- **n
+00001870: 6577 5f6f 6c64 5f6e 6f64 655f 7661 6c5f  ew_old_node_val_
+00001880: 6461 7461 203a 2062 656e 6368 7465 6d70  data : benchtemp
+00001890: 2e44 6174 612a 2a20 2d20 5468 6520 2a2a  .Data** - The **
+000018a0: 696e 6475 6374 6976 6520 5b6e 6577 2d6f  inductive [new-o
+000018b0: 6c64 5d2a 2a20 7365 7474 696e 6720 7661  ld]** setting va
+000018c0: 6c69 6461 7469 6f6e 2054 656d 706f 7261  lidation Tempora
+000018d0: 6c20 4772 6170 6820 6461 7461 7365 742e  l Graph dataset.
+000018e0: 0a2d 202a 2a6e 6577 5f6f 6c64 5f6e 6f64  .- **new_old_nod
+000018f0: 655f 7465 7374 5f64 6174 6120 3a20 6265  e_test_data : be
+00001900: 6e63 6874 656d 702e 4461 7461 2a2a 202d  nchtemp.Data** -
+00001910: 2054 6865 202a 2a69 6e64 7563 7469 7665   The **inductive
+00001920: 205b 6e65 772d 6f6c 645d 2a2a 2073 6574   [new-old]** set
+00001930: 7469 6e67 2074 6573 7420 5465 6d70 6f72  ting test Tempor
+00001940: 616c 2047 7261 7068 2064 6174 6173 6574  al Graph dataset
+00001950: 2e0a 2d20 2a2a 6e65 775f 6e65 775f 6e6f  ..- **new_new_no
+00001960: 6465 5f76 616c 5f64 6174 6120 3a20 6265  de_val_data : be
+00001970: 6e63 6874 656d 702e 4461 7461 2a2a 202d  nchtemp.Data** -
+00001980: 2054 6865 202a 2a69 6e64 7563 7469 7665   The **inductive
+00001990: 205b 6e65 772d 6e65 775d 2a2a 2073 6574   [new-new]** set
+000019a0: 7469 6e67 2076 616c 6964 6174 696f 6e20  ting validation 
+000019b0: 5465 6d70 6f72 616c 2047 7261 7068 2064  Temporal Graph d
+000019c0: 6174 6173 6574 2e0a 2d20 2a2a 6e65 775f  ataset..- **new_
+000019d0: 6e65 775f 6e6f 6465 5f74 6573 745f 6461  new_node_test_da
+000019e0: 7461 203a 2062 656e 6368 7465 6d70 2e44  ta : benchtemp.D
+000019f0: 6174 612a 2a20 2d20 5468 6520 2a2a 696e  ata** - The **in
+00001a00: 6475 6374 6976 6520 5b6e 6577 2d6e 6577  ductive [new-new
+00001a10: 5d2a 2a20 7365 7474 696e 6720 7465 7374  ]** setting test
+00001a20: 2054 656d 706f 7261 6c20 4772 6170 6820   Temporal Graph 
+00001a30: 6461 7461 7365 742e 0a2d 202a 2a75 6e73  dataset..- **uns
+00001a40: 6565 6e5f 6e6f 6465 735f 6e75 6d20 3a20  een_nodes_num : 
+00001a50: 696e 742a 2a20 2d20 5468 6520 6e75 6d62  int** - The numb
+00001a60: 6572 206f 6620 756e 7365 656e 206e 6f64  er of unseen nod
+00001a70: 6573 206f 6620 696e 6475 6374 6976 6520  es of inductive 
+00001a80: 7365 7474 696e 672e 0a0a 4578 616d 706c  setting...Exampl
+00001a90: 653a 0a0a 6060 6070 7974 686f 6e0a 696d  e:..```python.im
+00001aa0: 706f 7274 2062 656e 6368 7465 6d70 2061  port benchtemp a
+00001ab0: 7320 6274 0a0a 6461 7461 203d 2062 742e  s bt..data = bt.
+00001ac0: 6c70 2e44 6174 614c 6f61 6465 7228 6461  lp.DataLoader(da
+00001ad0: 7461 7365 745f 7061 7468 3d22 2e2f 6461  taset_path="./da
+00001ae0: 7461 2f22 2c20 6461 7461 7365 745f 6e61  ta/", dataset_na
+00001af0: 6d65 3d27 6d6f 6f63 2729 0a0a 6e6f 6465  me='mooc')..node
+00001b00: 5f66 6561 7475 7265 732c 2065 6467 655f  _features, edge_
+00001b10: 6665 6174 7572 6573 2c20 6675 6c6c 5f64  features, full_d
+00001b20: 6174 612c 2074 7261 696e 5f64 6174 612c  ata, train_data,
+00001b30: 2076 616c 5f64 6174 612c 2074 6573 745f   val_data, test_
+00001b40: 6461 7461 2c20 6e65 775f 6e6f 6465 5f76  data, new_node_v
+00001b50: 616c 5f64 6174 612c 206e 6577 5f6e 6f64  al_data, new_nod
+00001b60: 655f 7465 7374 5f64 6174 612c 206e 6577  e_test_data, new
+00001b70: 5f6f 6c64 5f6e 6f64 655f 7661 6c5f 6461  _old_node_val_da
+00001b80: 7461 2c20 6e65 775f 6f6c 645f 6e6f 6465  ta, new_old_node
+00001b90: 5f74 6573 745f 6461 7461 2c20 6e65 775f  _test_data, new_
+00001ba0: 6e65 775f 6e6f 6465 5f76 616c 5f64 6174  new_node_val_dat
+00001bb0: 612c 206e 6577 5f6e 6577 5f6e 6f64 655f  a, new_new_node_
+00001bc0: 7465 7374 5f64 6174 612c 2075 6e73 6565  test_data, unsee
+00001bd0: 6e5f 6e6f 6465 735f 6e75 6d20 3d20 6461  n_nodes_num = da
+00001be0: 7461 2e6c 6f61 6428 290a 6060 600a 0a23  ta.load().```..#
+00001bf0: 2323 2045 6467 6553 616d 706c 6572 0a42  ## EdgeSampler.B
+00001c00: 656e 6368 5465 6d70 2070 726f 7669 6465  enchTemp provide
+00001c10: 7320 7468 6520 756e 6966 6965 640a 6e65  s the unified.ne
+00001c20: 6761 7469 7665 2065 6467 6520 7361 6d70  gative edge samp
+00001c30: 6c65 7220 7769 7468 202a 2a73 6565 642a  ler with **seed*
+00001c40: 2a20 666f 7220 4c69 6e6b 2050 7265 6469  * for Link Predi
+00001c50: 6374 696f 6e20 7461 736b 2074 6f20 2073  ction task to  s
+00001c60: 616d 706c 6520 616e 2065 7175 616c 2061  ample an equal a
+00001c70: 6d6f 756e 7420 6f66 206e 6567 6174 6976  mount of negativ
+00001c80: 6573 2074 6f20 7468 6520 706f 7369 7469  es to the positi
+00001c90: 7665 2069 6e74 6572 6163 7469 6f6e 732e  ve interactions.
+00001ca0: 0a0a 436c 6173 733a 0a0a 2a2a 5261 6e64  ..Class:..**Rand
+00001cb0: 4564 6765 5361 6d70 6c65 7228 7372 635f  EdgeSampler(src_
+00001cc0: 6c69 7374 203a 206e 756d 7079 2e6e 6461  list : numpy.nda
+00001cd0: 7272 6179 2c20 6473 745f 6c69 7374 203a  rray, dst_list :
+00001ce0: 206e 756d 7079 2e6e 6461 7272 6179 2c20   numpy.ndarray, 
+00001cf0: 7365 6564 203a 2069 6e74 203d 4e6f 6e65  seed : int =None
+00001d00: 292a 2a0a 0a50 6172 616d 6574 6572 733a  )**..Parameters:
+00001d10: 0a2d 202a 2a73 7263 5f6c 6973 7420 3a20  .- **src_list : 
+00001d20: 6e75 6d70 792e 6e64 6172 7261 792a 2a20  numpy.ndarray** 
+00001d30: 2d20 7468 6520 6c69 7374 206f 6620 736f  - the list of so
+00001d40: 7572 6365 206e 6f64 6573 2e0a 2d20 2a2a  urce nodes..- **
+00001d50: 6473 745f 6c69 7374 203a 206e 756d 7079  dst_list : numpy
+00001d60: 2e6e 6461 7272 6179 2a2a 202d 2074 6865  .ndarray** - the
+00001d70: 206c 6973 7420 6f66 2064 6573 7469 6e61   list of destina
+00001d80: 7469 6f6e 206e 6f64 6573 2e0a 2d20 2a2a  tion nodes..- **
+00001d90: 7365 6564 203a 206e 756d 7079 2e6e 6461  seed : numpy.nda
+00001da0: 7272 6179 2a2a 202d 2073 6565 6420 6f66  rray** - seed of
+00001db0: 2072 616e 646f 6d2e 0a0a 5265 7475 726e   random...Return
+00001dc0: 733a 200a 0a2d 202a 2a62 656e 6368 7465  s: ..- **benchte
+00001dd0: 6d70 2e52 616e 6445 6467 6553 616d 706c  mp.RandEdgeSampl
+00001de0: 6572 2a2a 0a0a 4578 616d 706c 653a 0a0a  er**..Example:..
+00001df0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00001e00: 2062 656e 6368 7465 6d70 2061 7320 6274   benchtemp as bt
+00001e10: 0a0a 2320 466f 7220 6578 616d 706c 652c  ..# For example,
+00001e20: 2069 6620 796f 7520 6172 6520 7472 6169   if you are trai
+00001e30: 6e69 6e67 202c 2079 6f75 2073 686f 756c  ning , you shoul
+00001e40: 6420 6372 6561 7465 2061 2074 7261 696e  d create a train
+00001e50: 696e 6720 2052 616e 6445 6467 6553 616d  ing  RandEdgeSam
+00001e60: 706c 6572 2062 6173 6564 206f 6e20 7468  pler based on th
+00001e70: 6520 7472 6169 6e69 6e67 2064 6174 6173  e training datas
+00001e80: 6574 2e0a 7472 6169 6e5f 7261 6e64 5f73  et..train_rand_s
+00001e90: 616d 706c 6572 203d 2062 742e 6c70 2e52  ampler = bt.lp.R
+00001ea0: 616e 6445 6467 6553 616d 706c 6572 2874  andEdgeSampler(t
+00001eb0: 7261 696e 5f64 6174 612e 736f 7572 6365  rain_data.source
+00001ec0: 732c 2074 7261 696e 5f64 6174 612e 6465  s, train_data.de
+00001ed0: 7374 696e 6174 696f 6e73 290a 0a2e 2e2e  stinations).....
+00001ee0: 0a66 6f72 2065 706f 6368 2069 6e20 7261  .for epoch in ra
+00001ef0: 6e67 6528 6172 6773 2e65 706f 6368 7329  nge(args.epochs)
+00001f00: 3a0a 2020 2020 2e2e 2e0a 2020 2020 2320  :.    ....    # 
+00001f10: 7361 6d70 6c65 2061 6e20 6571 7561 6c20  sample an equal 
+00001f20: 616d 6f75 6e74 206f 6620 6e65 6761 7469  amount of negati
+00001f30: 7665 7320 746f 2074 6865 2070 6f73 6974  ves to the posit
+00001f40: 6976 6520 696e 7465 7261 6374 696f 6e73  ive interactions
+00001f50: 2e0a 2020 2020 5f2c 206e 6567 6174 6976  ..    _, negativ
+00001f60: 6573 5f62 6174 6368 203d 2074 7261 696e  es_batch = train
+00001f70: 5f72 616e 645f 7361 6d70 6c65 722e 7361  _rand_sampler.sa
+00001f80: 6d70 6c65 2873 697a 6529 0a20 2020 202e  mple(size).    .
+00001f90: 2e2e 0a2e 2e2e 0a60 6060 0a23 2323 2028  .......```.### (
+00001fa0: 3229 204e 6f64 6520 436c 6173 7369 6669  2) Node Classifi
+00001fb0: 6361 7469 6f6e 2074 6173 6b0a 4675 6e63  cation task.Func
+00001fc0: 7469 6f6e 3a0a 0a0a 0a2a 2a62 656e 6368  tion:....**bench
+00001fd0: 7465 6d70 2e6e 632e 7265 6164 6572 732e  temp.nc.readers.
+00001fe0: 6765 745f 6461 7461 5f6e 6f64 655f 636c  get_data_node_cl
+00001ff0: 6173 7369 6669 6361 7469 6f6e 2828 6461  assification((da
+00002000: 7461 7365 745f 6e61 6d65 203a 2073 7472  taset_name : str
+00002010: 2c20 7573 655f 7661 6c69 6461 7469 6f6e  , use_validation
+00002020: 203a 2062 6f6f 6c3d 4661 6c73 6529 292a   : bool=False))*
+00002030: 2a20 0a0a 5061 7261 6d65 7465 7273 3a0a  * ..Parameters:.
+00002040: 2d20 6461 7461 7365 745f 6e61 6d65 203a  - dataset_name :
+00002050: 2073 7472 202d 2054 6865 206e 616d 6520   str - The name 
+00002060: 6f66 2074 6865 2064 6174 6173 6574 2e20  of the dataset. 
+00002070: 5468 6520 6461 7461 7365 7420 6669 6c65  The dataset file
+00002080: 2028 2e63 7376 2066 696c 6520 6f66 2074   (.csv file of t
+00002090: 6865 2054 656d 706f 7261 6c20 4772 6170  he Temporal Grap
+000020a0: 682c 202e 6e70 7920 6669 6c65 206f 6620  h, .npy file of 
+000020b0: 7468 6520 6e6f 6465 2066 6561 7475 7265  the node feature
+000020c0: 7320 616e 6420 2e6e 7079 2066 696c 6520  s and .npy file 
+000020d0: 6f66 2074 6865 2065 6467 6520 6665 6174  of the edge feat
+000020e0: 7572 6573 2920 7368 6f75 6c64 2062 6520  ures) should be 
+000020f0: 696e 2022 2e2f 6461 7461 2220 6469 7265  in "./data" dire
+00002100: 6374 6f72 792e 0a2d 2075 7365 5f76 616c  ctory..- use_val
+00002110: 6964 6174 696f 6e20 3a20 626f 6f6c 202d  idation : bool -
+00002120: 2057 6865 7468 6572 2075 7365 2076 616c   Whether use val
+00002130: 6964 6174 696f 6e20 6461 7461 7365 7420  idation dataset 
+00002140: 6f72 206e 6f74 2e0a 0a52 6574 7572 6e73  or not...Returns
+00002150: 3a0a 2d20 2a2a 6e6f 6465 5f66 6561 7475  :.- **node_featu
+00002160: 7265 7320 3a20 6e75 6d70 792e 6e64 6172  res : numpy.ndar
+00002170: 7261 792a 2a20 2d20 4172 7261 7920 6f66  ray** - Array of
+00002180: 2074 6865 204e 6f64 6520 4665 6174 7572   the Node Featur
+00002190: 6573 206f 6620 7468 6520 5465 6d70 6f72  es of the Tempor
+000021a0: 616c 2047 7261 7068 2e20 0a2d 202a 2a65  al Graph. .- **e
+000021b0: 6467 655f 6665 6174 7572 6573 203a 206e  dge_features : n
+000021c0: 756d 7079 2e6e 6461 7272 6179 2a2a 202d  umpy.ndarray** -
+000021d0: 2041 7272 6179 206f 6620 7468 6520 4564   Array of the Ed
+000021e0: 6765 2046 6561 7475 7265 7320 6f66 2074  ge Features of t
+000021f0: 6865 2054 656d 706f 7261 6c20 4772 6170  he Temporal Grap
+00002200: 682e 0a2d 202a 2a66 756c 6c5f 6461 7461  h..- **full_data
+00002210: 203a 2062 656e 6368 7465 6d70 2e44 6174   : benchtemp.Dat
+00002220: 612a 2a20 2d20 4675 6c6c 2054 656d 706f  a** - Full Tempo
+00002230: 7261 6c20 4772 6170 6820 6461 7461 7365  ral Graph datase
+00002240: 7420 666f 7220 4e6f 6465 2043 6c61 7373  t for Node Class
+00002250: 6966 6963 6174 696f 6e20 7461 736b 2e20  ification task. 
+00002260: 0a2d 202a 2a74 7261 696e 5f64 6174 6120  .- **train_data 
+00002270: 3a20 6265 6e63 6874 656d 702e 4461 7461  : benchtemp.Data
+00002280: 2a2a 202d 2054 6865 2074 7261 696e 696e  ** - The trainin
+00002290: 6720 5465 6d70 6f72 616c 2047 7261 7068  g Temporal Graph
+000022a0: 2064 6174 6173 6574 2066 6f72 204e 6f64   dataset for Nod
+000022b0: 6520 436c 6173 7369 6669 6361 7469 6f6e  e Classification
+000022c0: 2074 6173 6b2e 200a 2d20 2a2a 7661 6c5f   task. .- **val_
+000022d0: 6461 7461 203a 2062 656e 6368 7465 6d70  data : benchtemp
+000022e0: 2e44 6174 612a 2a20 2d20 5468 6520 7661  .Data** - The va
+000022f0: 6c69 6461 7469 6f6e 2054 656d 706f 7261  lidation Tempora
+00002300: 6c20 4772 6170 6820 6461 7461 7365 7420  l Graph dataset 
+00002310: 666f 7220 4e6f 6465 2043 6c61 7373 6966  for Node Classif
+00002320: 6963 6174 696f 6e20 7461 736b 2e0a 2d20  ication task..- 
+00002330: 2a2a 7465 7374 5f64 6174 6120 3a20 6265  **test_data : be
+00002340: 6e63 6874 656d 702e 4461 7461 2a2a 2020  nchtemp.Data**  
+00002350: 2d20 5468 6520 7465 7374 2054 656d 706f  - The test Tempo
+00002360: 7261 6c20 4772 6170 6820 6461 7461 7365  ral Graph datase
+00002370: 7420 666f 7220 4e6f 6465 2043 6c61 7373  t for Node Class
+00002380: 6966 6963 6174 696f 6e20 7461 736b 2e0a  ification task..
+00002390: 0a0a 0a23 2323 2045 6172 6c79 5374 6f70  ...### EarlyStop
+000023a0: 4d6f 6e69 746f 720a 436c 6173 733a 0a0a  Monitor.Class:..
+000023b0: 2a2a 4561 726c 7953 746f 704d 6f6e 6974  **EarlyStopMonit
+000023c0: 6f72 286d 6178 5f72 6f75 6e64 3d33 2c20  or(max_round=3, 
+000023d0: 6869 6768 6572 5f62 6574 7465 723d 5472  higher_better=Tr
+000023e0: 7565 2c20 746f 6c65 7261 6e63 653d 3165  ue, tolerance=1e
+000023f0: 2d31 3029 2a2a 0a0a 5061 7261 6d65 7465  -10)**..Paramete
+00002400: 7273 3a0a 2d20 2a2a 6d61 785f 726f 756e  rs:.- **max_roun
+00002410: 6420 3a20 696e 742a 2a20 2d20 7468 6520  d : int** - the 
+00002420: 6d61 7869 6d75 6d20 6e75 6d62 6572 206f  maximum number o
+00002430: 6620 726f 756e 6473 206f 6620 4561 726c  f rounds of Earl
+00002440: 7953 746f 704d 6f6e 6974 6f72 2e0a 2d20  yStopMonitor..- 
+00002450: 2a2a 6869 6768 6572 5f62 6574 7465 7220  **higher_better 
+00002460: 3a20 626f 6f6c 2a2a 202d 2062 6574 7465  : bool** - bette
+00002470: 7220 7468 6520 7065 7266 6f72 6d61 6e63  r the performanc
+00002480: 652e 0a2d 202a 2a74 6f6c 6572 616e 6365  e..- **tolerance
+00002490: 203a 2066 6c6f 6174 2a2a 202d 2074 6865   : float** - the
+000024a0: 2074 6f6c 6572 616e 6365 206f 6620 7468   tolerance of th
+000024b0: 6520 4561 726c 7953 746f 704d 6f6e 6974  e EarlyStopMonit
+000024c0: 6f72 2e0a 0a52 6574 7572 6e73 3a0a 2d20  or...Returns:.- 
+000024d0: 2a2a 6265 6e63 6874 656d 702e 4561 726c  **benchtemp.Earl
+000024e0: 7953 746f 704d 6f6e 6974 6f72 2a2a 0a0a  yStopMonitor**..
+000024f0: 4578 616d 706c 653a 0a60 6060 7079 7468  Example:.```pyth
+00002500: 6f6e 0a69 6d70 6f72 7420 6265 6e63 6874  on.import bencht
+00002510: 656d 7020 6173 2062 740a 0a2e 2e2e 0a65  emp as bt......e
+00002520: 6172 6c79 5f73 746f 7070 6572 203d 2062  arly_stopper = b
+00002530: 742e 4561 726c 7953 746f 704d 6f6e 6974  t.EarlyStopMonit
+00002540: 6f72 286d 6178 5f72 6f75 6e64 3d61 7267  or(max_round=arg
+00002550: 732e 7061 7469 656e 6365 290a 666f 7220  s.patience).for 
+00002560: 6570 6f63 6820 696e 2072 616e 6765 2861  epoch in range(a
+00002570: 7267 732e 6570 6f63 6873 293a 0a20 2020  rgs.epochs):.   
+00002580: 202e 2e2e 0a20 2020 2076 616c 5f61 7020   ....    val_ap 
+00002590: 3d20 6d6f 6465 6c28 7661 6c5f 6461 7461  = model(val_data
+000025a0: 7365 7473 290a 2020 2020 6966 2065 6172  sets).    if ear
+000025b0: 6c79 5f73 746f 7070 6572 2e65 6172 6c79  ly_stopper.early
+000025c0: 5f73 746f 705f 6368 6563 6b28 7661 6c5f  _stop_check(val_
+000025d0: 6170 293a 0a20 2020 2020 2020 2062 7265  ap):.        bre
+000025e0: 616b 0a20 2020 202e 2e2e 0a2e 2e2e 0a60  ak.    ........`
+000025f0: 6060 0a0a 2323 2320 4576 616c 7561 746f  ``..### Evaluato
+00002600: 720a 0a2a 2a4c 696e 6b20 5072 6564 6963  r..**Link Predic
+00002610: 7469 6f6e 2a2a 2045 7661 6c75 6174 696f  tion** Evaluatio
+00002620: 6e20 4d65 7472 6963 7320 2061 7265 202a  n Metrics  are *
+00002630: 2a41 7265 6120 556e 6465 7220 7468 6520  *Area Under the 
+00002640: 5265 6365 6976 6572 204f 7065 7261 7469  Receiver Operati
+00002650: 6e67 2043 6861 7261 6374 6572 6973 7469  ng Characteristi
+00002660: 6320 4375 7276 6520 2852 4f43 2041 5543  c Curve (ROC AUC
+00002670: 292a 2a20 616e 6420 2a2a 6176 6572 6167  )** and **averag
+00002680: 6520 7072 6563 6973 696f 6e20 2841 5029  e precision (AP)
+00002690: 2a2a 0a0a 2a2a 4e6f 6465 2043 6c61 7373  **..**Node Class
+000026a0: 6966 6963 6174 696f 6e2a 2a20 4576 616c  ification** Eval
+000026b0: 7561 7469 6f6e 204d 6574 7269 6320 6973  uation Metric is
+000026c0: 202a 2a41 7265 6120 556e 6465 7220 7468   **Area Under th
+000026d0: 6520 5265 6365 6976 6572 204f 7065 7261  e Receiver Opera
+000026e0: 7469 6e67 2043 6861 7261 6374 6572 6973  ting Characteris
+000026f0: 7469 6320 4375 7276 6520 2852 4f43 2041  tic Curve (ROC A
+00002700: 5543 292a 2a0a 0a43 6c61 7373 3a20 0a0a  UC)**..Class: ..
+00002710: 2a2a 4576 616c 7561 746f 7228 7461 736b  **Evaluator(task
+00002720: 5f6e 616d 653a 2073 7472 203d 2022 4c50  _name: str = "LP
+00002730: 2229 2a2a 0a0a 5061 7261 6d65 7465 7273  ")**..Parameters
+00002740: 3a0a 2d20 7461 736b 5f6e 616d 6520 3a20  :.- task_name : 
+00002750: 7374 7220 202d 2074 6865 206e 616d 6520  str  - the name 
+00002760: 6f66 2074 6865 2074 6173 6b2c 2063 686f  of the task, cho
+00002770: 6963 6520 696e 202a 2a5b 224c 5022 2c20  ice in **["LP", 
+00002780: 224e 4322 5d2a 2a2e 0a0a 5265 7475 726e  "NC"]**...Return
+00002790: 733a 0a2d 202a 2a62 656e 6368 7465 6d70  s:.- **benchtemp
+000027a0: 2e45 7661 6c75 6174 6f72 2a2a 0a0a 4578  .Evaluator**..Ex
+000027b0: 616d 706c 653a 0a0a 6060 6070 7974 686f  ample:..```pytho
+000027c0: 6e0a 696d 706f 7274 2062 656e 6368 7465  n.import benchte
+000027d0: 6d70 2061 7320 6274 0a0a 2320 466f 7220  mp as bt..# For 
+000027e0: 6578 616d 706c 652c 204c 696e 6b20 7072  example, Link pr
+000027f0: 6564 6963 7469 6f6e 2074 6173 6b2e 2045  ediction task. E
+00002800: 7661 6c75 6174 696f 6e20 4d65 7472 6963  valuation Metric
+00002810: 733a 2041 5543 2c20 4150 2e0a 6576 616c  s: AUC, AP..eval
+00002820: 7561 746f 7220 3d20 6274 2e45 7661 6c75  uator = bt.Evalu
+00002830: 6174 6f72 2822 4c50 2229 0a0a 2e2e 2e0a  ator("LP")......
+00002840: 2320 7465 7374 2064 6174 610a 7072 6564  # test data.pred
+00002850: 5f73 636f 7265 203d 206d 6f64 656c 2874  _score = model(t
+00002860: 6573 745f 6461 7461 290a 7465 7374 5f61  est_data).test_a
+00002870: 7563 2c20 7465 7374 5f61 7020 3d20 6576  uc, test_ap = ev
+00002880: 616c 7561 746f 722e 6576 616c 2870 7265  aluator.eval(pre
+00002890: 645f 7363 6f72 652c 2074 7275 655f 6c61  d_score, true_la
+000028a0: 6265 6c29 0a2e 2e2e 0a60 6060 0a0a 6060  bel).....```..``
+000028b0: 6070 7974 686f 6e0a 696d 706f 7274 2062  `python.import b
+000028c0: 656e 6368 7465 6d70 2061 7320 6274 0a0a  enchtemp as bt..
+000028d0: 2320 466f 7220 6578 616d 706c 652c 204e  # For example, N
+000028e0: 6f64 6520 436c 6173 7369 6669 6361 7469  ode Classificati
+000028f0: 6f6e 2074 6173 6b2e 2045 7661 6c75 6174  on task. Evaluat
+00002900: 696f 6e20 4d65 7472 6963 733a 2041 5543  ion Metrics: AUC
+00002910: 2e0a 6576 616c 7561 746f 7220 3d20 6274  ..evaluator = bt
+00002920: 2e45 7661 6c75 6174 6f72 2822 4e43 2229  .Evaluator("NC")
+00002930: 0a0a 2e2e 2e0a 2320 7465 7374 2064 6174  ......# test dat
+00002940: 610a 7072 6564 5f73 636f 7265 203d 206d  a.pred_score = m
+00002950: 6f64 656c 2874 6573 745f 6461 7461 290a  odel(test_data).
+00002960: 7465 7374 5f61 7563 203d 2065 7661 6c75  test_auc = evalu
+00002970: 6174 6f72 2e65 7661 6c28 7072 6564 5f73  ator.eval(pred_s
+00002980: 636f 7265 2c20 7472 7565 5f6c 6162 656c  core, true_label
+00002990: 290a 2e2e 2e0a 6060 600a 0a23 2320 4361  ).....```..## Ca
+000029a0: 6c6c 2066 6f72 2043 6f6e 7472 6962 7574  ll for Contribut
+000029b0: 696f 6e73 0a0a 2a2a 4265 6e63 6854 656d  ions..**BenchTem
+000029c0: 702a 2a20 7072 6f6a 6563 7420 6973 206c  p** project is l
+000029d0: 6f6f 6b69 6e67 2066 6f72 2063 6f6e 7472  ooking for contr
+000029e0: 6962 7574 6f72 7320 7769 7468 200a 6578  ibutors with .ex
+000029f0: 7065 7274 6973 6520 616e 6420 656e 7468  pertise and enth
+00002a00: 7573 6961 736d 2120 4966 2079 6f75 2068  usiasm! If you h
+00002a10: 6176 6520 6120 6465 7369 7265 2074 6f20  ave a desire to 
+00002a20: 636f 6e74 7269 6275 7465 2074 6f20 2a2a  contribute to **
+00002a30: 4265 6e63 6854 656d 702a 2a2c 200a 706c  BenchTemp**, .pl
+00002a40: 6561 7365 2063 6f6e 7461 6374 205b 4265  ease contact [Be
+00002a50: 6e63 6854 656d 7020 7465 616d 5d28 6d61  nchTemp team](ma
+00002a60: 696c 746f 3a6a 6f6e 6e79 6875 616e 6768  ilto:jonnyhuangh
+00002a70: 6e75 4067 6d61 696c 2e63 6f6d 292e 0a0a  nu@gmail.com)...
+00002a80: 5c69 7465 6d20 5765 2072 656c 6561 7365  \item We release
+00002a90: 205c 7379 732c 2061 2067 656e 6572 616c   \sys, a general
+00002aa0: 2062 656e 6368 6d61 726b 206c 6962 7261   benchmark libra
+00002ab0: 7279 2066 6f72 2065 7661 6c75 6174 696e  ry for evaluatin
+00002ac0: 6720 7465 6d70 6f72 616c 2067 7261 7068  g temporal graph
+00002ad0: 206d 6f64 656c 733b 0a0a 5c69 7465 6d20   models;..\item 
+00002ae0: 5765 2070 726f 7669 6465 7320 756e 6966  We provides unif
+00002af0: 6965 6420 6265 6e63 6b6d 6172 6b20 7465  ied benckmark te
+00002b00: 6d70 6f72 616c 2067 7261 7068 2064 6174  mporal graph dat
+00002b10: 6173 6574 7320 7072 6f63 6573 7365 6420  asets processed 
+00002b20: 6279 205c 7379 733b 0a0a 5c69 7465 6d20  by \sys;..\item 
+00002b30: 5765 2062 656e 6368 6d61 726b 2065 7869  We benchmark exi
+00002b40: 7374 696e 6720 7465 6d70 6f72 616c 2067  sting temporal g
+00002b50: 7261 7068 206d 6f64 656c 7320 6261 7365  raph models base
+00002b60: 6420 6f6e 205c 7379 7320 2066 6f72 2072  d on \sys  for r
+00002b70: 6f62 7573 7420 6465 7665 6c6f 706d 656e  obust developmen
+00002b80: 7473 2061 6e64 2061 6e61 6c79 7369 7320  ts and analysis 
+00002b90: 7468 6520 7065 7266 6f72 6d61 6e63 6520  the performance 
+00002ba0: 6f66 206d 6f64 656c 7320 696e 2064 6574  of models in det
+00002bb0: 6169 6c3b 0a0a 5c69 7465 6d20 5765 2072  ail;..\item We r
+00002bc0: 656c 7365 6420 7468 6520 6c65 6164 6572  elsed the leader
+00002bd0: 626f 6172 6473 2066 6f72 2074 656d 706f  boards for tempo
+00002be0: 7261 6c20 6772 6170 6820 6d6f 6465 6c73  ral graph models
+00002bf0: 2e0a 0a                                  ...
```

### Comparing `benchtemp-1.0.0/pyproject.toml` & `benchtemp-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "benchtemp"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   {name="Qiang Huang", email="jonnyhuanghnu@gmail.com"},
 ]
-description = "BenchTeMP: A General Benchmark Library for Evaluating Temporal Graph Models"
+description = "BenchTemp: A General Benchmark for Evaluating Temporal Graph Neural Networks"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `benchtemp-1.0.0/src/benchtemp/lp/readers.py` & `benchtemp-1.1.0/src/benchtemp/lp/dataloader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,154 +1,147 @@
 import numpy as np
 import pandas as pd
 import random
 
-from benchtemp.utils import Data
+from benchtemp.utils.temporal_data import Data
 
 
-def get_data(dataset_name, different_new_nodes_between_val_and_test=False, randomize_features=False):
-    # Load data and train val test split
-    graph_df = pd.read_csv('./data/ml_{}.csv'.format(dataset_name))
-    edge_features = np.load('./data/ml_{}.npy'.format(dataset_name))
-    node_features = np.load('./data/ml_{}_node.npy'.format(dataset_name))
-
-    if randomize_features:
-        node_features = np.random.rand(node_features.shape[0], node_features.shape[1])
-
-    val_time, test_time = list(np.quantile(graph_df.ts, [0.70, 0.85]))
-
-    sources = graph_df.u.values
-    destinations = graph_df.i.values
-    edge_idxs = graph_df.idx.values
-    labels = graph_df.label.values
-    timestamps = graph_df.ts.values
-
-    full_data = Data(sources, destinations, timestamps, edge_idxs, labels)
-
-    random.seed(2020)
-
-    node_set = set(sources) | set(destinations)
-    n_total_unique_nodes = len(node_set)
-
-    # Compute nodes which appear at test time
-    test_node_set = set(sources[timestamps > val_time]).union(
-        set(destinations[timestamps > val_time]))
-    # Sample nodes which we keep as new nodes (to test inductiveness), so than we have to remove all
-    # their edges from training
-    new_test_node_set = set(random.sample(test_node_set, int(0.1 * n_total_unique_nodes)))
-
-    # Mask saying for each source and destination whether they are new test nodes
-    new_test_source_mask = graph_df.u.map(lambda x: x in new_test_node_set).values
-    new_test_destination_mask = graph_df.i.map(lambda x: x in new_test_node_set).values
-
-    # Mask which is true for edges with both destination and source not being new test nodes (because
-    # we want to remove all edges involving any new test node)
-    observed_edges_mask = np.logical_and(~new_test_source_mask, ~new_test_destination_mask)
-
-    # For train we keep edges happening before the validation time which do not involve any new node
-    # used for inductiveness
-    train_mask = np.logical_and(timestamps <= val_time, observed_edges_mask)
-
-    train_data = Data(sources[train_mask], destinations[train_mask], timestamps[train_mask],
-                      edge_idxs[train_mask], labels[train_mask])
-
-    # define the new nodes sets for testing inductiveness of the model
-    train_node_set = set(train_data.sources).union(train_data.destinations)
-    assert len(train_node_set & new_test_node_set) == 0
-    new_node_set = node_set - train_node_set
-
-    val_mask = np.logical_and(timestamps <= test_time, timestamps > val_time)
-    test_mask = timestamps > test_time
-
-    if different_new_nodes_between_val_and_test:
-        n_new_nodes = len(new_test_node_set) // 2
-        val_new_node_set = set(list(new_test_node_set)[:n_new_nodes])
-        test_new_node_set = set(list(new_test_node_set)[n_new_nodes:])
-
-        edge_contains_new_val_node_mask = np.array(
-            [(a in val_new_node_set or b in val_new_node_set) for a, b in zip(sources, destinations)])
-        edge_contains_new_test_node_mask = np.array(
-            [(a in test_new_node_set or b in test_new_node_set) for a, b in zip(sources, destinations)])
-        new_node_val_mask = np.logical_and(val_mask, edge_contains_new_val_node_mask)
-        new_node_test_mask = np.logical_and(test_mask, edge_contains_new_test_node_mask)
-
-    else:
-        # edge: new-
-        edge_contains_new_node_mask = np.array(
-            [(a in new_node_set or b in new_node_set) for a, b in zip(sources, destinations)])
-        new_node_val_mask = np.logical_and(val_mask, edge_contains_new_node_mask)
-        new_node_test_mask = np.logical_and(test_mask, edge_contains_new_node_mask)
-
-        # edge: new-new
-        edge_contains_new_new_node_mask = np.array(
-            [(a in new_node_set and b in new_node_set) for a, b in zip(sources, destinations)])
-        new_new_node_val_mask = np.logical_and(val_mask, edge_contains_new_new_node_mask)
-        new_new_node_test_mask = np.logical_and(test_mask, edge_contains_new_new_node_mask)
-        # way 2: anther way of constructing egde: new-old
-        '''
-        new- | new-new | new-old
-        True | True    | False 
-        True | False   | True 
-        False| False   | False
-        i.e. 
-        new-old = new- && !new-new
-        new-new = new- && !new-old
-        new- = new-new || new-old
-        '''
-        edge_contains_new_old_node_mask = np.logical_and(edge_contains_new_node_mask,
-                                                         np.logical_not(edge_contains_new_new_node_mask))
-        new_old_node_val_mask = np.logical_and(val_mask, edge_contains_new_old_node_mask)
-        new_old_node_test_mask = np.logical_and(test_mask, edge_contains_new_old_node_mask)
-
-    # validation and test with all edges
-    val_data = Data(sources[val_mask], destinations[val_mask], timestamps[val_mask],
-                    edge_idxs[val_mask], labels[val_mask])
-
-    test_data = Data(sources[test_mask], destinations[test_mask], timestamps[test_mask],
-                     edge_idxs[test_mask], labels[test_mask])
-
-    # validation and test with edges that at least has one new node (not in training set)
-    new_node_val_data = Data(sources[new_node_val_mask], destinations[new_node_val_mask],
-                             timestamps[new_node_val_mask],
-                             edge_idxs[new_node_val_mask], labels[new_node_val_mask])
-
-    new_node_test_data = Data(sources[new_node_test_mask], destinations[new_node_test_mask],
-                              timestamps[new_node_test_mask], edge_idxs[new_node_test_mask],
-                              labels[new_node_test_mask])
-
-    # dataset:  new-old
-    new_old_node_val_data = Data(sources[new_old_node_val_mask], destinations[new_old_node_val_mask],
-                                 timestamps[new_old_node_val_mask],
-                                 edge_idxs[new_old_node_val_mask], labels[new_old_node_val_mask])
-
-    new_old_node_test_data = Data(sources[new_old_node_test_mask], destinations[new_old_node_test_mask],
-                                  timestamps[new_old_node_test_mask], edge_idxs[new_old_node_test_mask],
-                                  labels[new_old_node_test_mask])
-    # dataset:  new-new
-    new_new_node_val_data = Data(sources[new_new_node_val_mask], destinations[new_new_node_val_mask],
-                                 timestamps[new_new_node_val_mask],
-                                 edge_idxs[new_new_node_val_mask], labels[new_new_node_val_mask])
-
-    new_new_node_test_data = Data(sources[new_new_node_test_mask], destinations[new_new_node_test_mask],
-                                  timestamps[new_new_node_test_mask], edge_idxs[new_new_node_test_mask],
-                                  labels[new_new_node_test_mask])
-
-    # print("The dataset has {} interactions, involving {} different nodes".format(full_data.n_interactions,
-    #                                                                              full_data.n_unique_nodes))
-    # print("The training dataset has {} interactions, involving {} different nodes".format(
-    #     train_data.n_interactions, train_data.n_unique_nodes))
-    # print("The validation dataset has {} interactions, involving {} different nodes".format(
-    #     val_data.n_interactions, val_data.n_unique_nodes))
-    # print("The test dataset has {} interactions, involving {} different nodes".format(
-    #     test_data.n_interactions, test_data.n_unique_nodes))
-    # print("The new node validation dataset has {} interactions, involving {} different nodes".format(
-    #     new_node_val_data.n_interactions, new_node_val_data.n_unique_nodes))
-    # print("The new node test dataset has {} interactions, involving {} different nodes".format(
-    #     new_node_test_data.n_interactions, new_node_test_data.n_unique_nodes))
-    # unseen nodes num
-    unseen_nodes_num = len(new_test_node_set)
-    # print("{} nodes were used for the inductive testing, i.e. are never seen during training".format(
-    #     unseen_nodes_num))
-
-    return node_features, edge_features, full_data, train_data, val_data, test_data, \
-        new_node_val_data, new_node_test_data, new_old_node_val_data, new_old_node_test_data, new_new_node_val_data, \
-        new_new_node_test_data, unseen_nodes_num
+class DataLoader:
+    def __init__(self, dataset_path="./data/", dataset_name='mooc', different_new_nodes_between_val_and_test=False,
+                 randomize_features=False):
+        self.dataset_path = dataset_path
+        self.dataset_name = dataset_name
+        self.different_new_nodes_between_val_and_test = different_new_nodes_between_val_and_test
+        self.randomize_features = randomize_features
+
+    def load(self):
+        # Load data and train val test split
+        graph_df = pd.read_csv(self.dataset_path + 'ml_{}.csv'.format(self.dataset_name))
+        edge_features = np.load(self.dataset_path + 'ml_{}.npy'.format(self.dataset_name))
+        node_features = np.load(self.dataset_path + 'ml_{}_node.npy'.format(self.dataset_name))
+
+        if self.randomize_features:
+            node_features = np.random.rand(node_features.shape[0], node_features.shape[1])
+
+        val_time, test_time = list(np.quantile(graph_df.ts, [0.70, 0.85]))
+
+        sources = graph_df.u.values
+        destinations = graph_df.i.values
+        edge_idxs = graph_df.idx.values
+        labels = graph_df.label.values
+        timestamps = graph_df.ts.values
+
+        full_data = Data(sources, destinations, timestamps, edge_idxs, labels)
+
+        random.seed(2020)
+
+        node_set = set(sources) | set(destinations)
+        n_total_unique_nodes = len(node_set)
+
+        # Compute nodes which appear at test time
+        test_node_set = set(sources[timestamps > val_time]).union(
+            set(destinations[timestamps > val_time]))
+        # Sample nodes which we keep as new nodes (to test inductiveness), so than we have to remove all
+        # their edges from training
+        new_test_node_set = set(random.sample(test_node_set, int(0.1 * n_total_unique_nodes)))
+
+        # Mask saying for each source and destination whether they are new test nodes
+        new_test_source_mask = graph_df.u.map(lambda x: x in new_test_node_set).values
+        new_test_destination_mask = graph_df.i.map(lambda x: x in new_test_node_set).values
+
+        # Mask which is true for edges with both destination and source not being new test nodes (because
+        # we want to remove all edges involving any new test node)
+        observed_edges_mask = np.logical_and(~new_test_source_mask, ~new_test_destination_mask)
+
+        # For train we keep edges happening before the validation time which do not involve any new node
+        # used for inductiveness
+        train_mask = np.logical_and(timestamps <= val_time, observed_edges_mask)
+
+        train_data = Data(sources[train_mask], destinations[train_mask], timestamps[train_mask],
+                          edge_idxs[train_mask], labels[train_mask])
+
+        # define the new nodes sets for testing inductiveness of the model
+        train_node_set = set(train_data.sources).union(train_data.destinations)
+        assert len(train_node_set & new_test_node_set) == 0
+        new_node_set = node_set - train_node_set
+
+        val_mask = np.logical_and(timestamps <= test_time, timestamps > val_time)
+        test_mask = timestamps > test_time
+
+        if self.different_new_nodes_between_val_and_test:
+            n_new_nodes = len(new_test_node_set) // 2
+            val_new_node_set = set(list(new_test_node_set)[:n_new_nodes])
+            test_new_node_set = set(list(new_test_node_set)[n_new_nodes:])
+
+            edge_contains_new_val_node_mask = np.array(
+                [(a in val_new_node_set or b in val_new_node_set) for a, b in zip(sources, destinations)])
+            edge_contains_new_test_node_mask = np.array(
+                [(a in test_new_node_set or b in test_new_node_set) for a, b in zip(sources, destinations)])
+            new_node_val_mask = np.logical_and(val_mask, edge_contains_new_val_node_mask)
+            new_node_test_mask = np.logical_and(test_mask, edge_contains_new_test_node_mask)
+
+        else:
+            # edge: new-
+            edge_contains_new_node_mask = np.array(
+                [(a in new_node_set or b in new_node_set) for a, b in zip(sources, destinations)])
+            new_node_val_mask = np.logical_and(val_mask, edge_contains_new_node_mask)
+            new_node_test_mask = np.logical_and(test_mask, edge_contains_new_node_mask)
+
+            # edge: new-new
+            edge_contains_new_new_node_mask = np.array(
+                [(a in new_node_set and b in new_node_set) for a, b in zip(sources, destinations)])
+            new_new_node_val_mask = np.logical_and(val_mask, edge_contains_new_new_node_mask)
+            new_new_node_test_mask = np.logical_and(test_mask, edge_contains_new_new_node_mask)
+            # way 2: anther way of constructing egde: new-old
+            '''
+            new- | new-new | new-old
+            True | True    | False 
+            True | False   | True 
+            False| False   | False
+            i.e. 
+            new-old = new- && !new-new
+            new-new = new- && !new-old
+            new- = new-new || new-old
+            '''
+            edge_contains_new_old_node_mask = np.logical_and(edge_contains_new_node_mask,
+                                                             np.logical_not(edge_contains_new_new_node_mask))
+            new_old_node_val_mask = np.logical_and(val_mask, edge_contains_new_old_node_mask)
+            new_old_node_test_mask = np.logical_and(test_mask, edge_contains_new_old_node_mask)
+
+        # validation and test with all edges
+        val_data = Data(sources[val_mask], destinations[val_mask], timestamps[val_mask],
+                        edge_idxs[val_mask], labels[val_mask])
+
+        test_data = Data(sources[test_mask], destinations[test_mask], timestamps[test_mask],
+                         edge_idxs[test_mask], labels[test_mask])
+
+        # validation and test with edges that at least has one new node (not in training set)
+        new_node_val_data = Data(sources[new_node_val_mask], destinations[new_node_val_mask],
+                                 timestamps[new_node_val_mask],
+                                 edge_idxs[new_node_val_mask], labels[new_node_val_mask])
+
+        new_node_test_data = Data(sources[new_node_test_mask], destinations[new_node_test_mask],
+                                  timestamps[new_node_test_mask], edge_idxs[new_node_test_mask],
+                                  labels[new_node_test_mask])
+
+        # dataset:  new-old
+        new_old_node_val_data = Data(sources[new_old_node_val_mask], destinations[new_old_node_val_mask],
+                                     timestamps[new_old_node_val_mask],
+                                     edge_idxs[new_old_node_val_mask], labels[new_old_node_val_mask])
+
+        new_old_node_test_data = Data(sources[new_old_node_test_mask], destinations[new_old_node_test_mask],
+                                      timestamps[new_old_node_test_mask], edge_idxs[new_old_node_test_mask],
+                                      labels[new_old_node_test_mask])
+        # dataset:  new-new
+        new_new_node_val_data = Data(sources[new_new_node_val_mask], destinations[new_new_node_val_mask],
+                                     timestamps[new_new_node_val_mask],
+                                     edge_idxs[new_new_node_val_mask], labels[new_new_node_val_mask])
+
+        new_new_node_test_data = Data(sources[new_new_node_test_mask], destinations[new_new_node_test_mask],
+                                      timestamps[new_new_node_test_mask], edge_idxs[new_new_node_test_mask],
+                                      labels[new_new_node_test_mask])
+
+        unseen_nodes_num = len(new_test_node_set)
+
+        return node_features, edge_features, full_data, train_data, val_data, test_data, \
+            new_node_val_data, new_node_test_data, new_old_node_val_data, new_old_node_test_data, new_new_node_val_data, \
+            new_new_node_test_data, unseen_nodes_num
```

### Comparing `benchtemp-1.0.0/src/benchtemp/lp/sampler.py` & `benchtemp-1.1.0/src/benchtemp/lp/edgesampler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 
-class RandEdgeSampler(object):
+class RandEdgeSampler:
     def __init__(self, src_list, dst_list, seed=None):
         self.seed = None
         self.src_list = np.unique(src_list)
         self.dst_list = np.unique(dst_list)
 
         if seed is not None:
             self.seed = seed
```

### Comparing `benchtemp-1.0.0/src/benchtemp/preprocessing/data.py` & `benchtemp-1.1.0/src/benchtemp/preprocess/preprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,41 @@
 import json
 import numpy as np
 import pandas as pd
 from pathlib import Path
 import argparse
 
 
+class DataPreprocessor:
+    def __init__(self, data_path="./data/", data_name="mooc"):
+        self.data_path = data_path
+        self.data_name = data_name
+
+    def data_preprocess(self, bipartite=True):
+        PATH = self.data_path + '{}.csv'.format(self.data_name)
+        OUT_DF = self.data_path + 'ml_{}.csv'.format(self.data_name)
+        OUT_FEAT = self.data_path + 'ml_{}.npy'.format(self.data_name)
+        OUT_NODE_FEAT = './data/ml_{}_node.npy'.format(self.data_name)
+
+        df, feat = preprocess(PATH)
+        new_df = reindex(df, bipartite)
+
+        empty = np.zeros(feat.shape[1])[np.newaxis, :]
+        feat = np.vstack([empty, feat])
+
+        max_idx = max(new_df.u.max(), new_df.i.max())
+        rand_feat = np.zeros((max_idx + 1, 172))
+
+        new_df.to_csv(OUT_DF)
+        np.save(OUT_FEAT, feat)
+        np.save(OUT_NODE_FEAT, rand_feat)
+        print(feat.shape)
+        print(rand_feat.shape)
+
+
 def preprocess(data_name):
     u_list, i_list, ts_list, label_list = [], [], [], []
     feat_l = []
     idx_list = []
 
     with open(data_name) as f:
         s = next(f)
@@ -67,47 +94,25 @@
         new_df.u += 1
         new_df.i += 1
         new_df.idx += 1
 
     return new_df
 
 
-def data_preprocess(data_name, bipartite=True):
-    Path("data/").mkdir(parents=True, exist_ok=True)
-    PATH = './data/{}.csv'.format(data_name)
-    OUT_DF = './data/ml_{}.csv'.format(data_name)
-    OUT_FEAT = './data/ml_{}.npy'.format(data_name)
-    OUT_NODE_FEAT = './data/ml_{}_node.npy'.format(data_name)
-
-    df, feat = preprocess(PATH)
-    new_df = reindex(df, bipartite)
-
-    empty = np.zeros(feat.shape[1])[np.newaxis, :]
-    feat = np.vstack([empty, feat])
-
-    max_idx = max(new_df.u.max(), new_df.i.max())
-    rand_feat = np.zeros((max_idx + 1, 172))
-
-    new_df.to_csv(OUT_DF)
-    np.save(OUT_FEAT, feat)
-    np.save(OUT_NODE_FEAT, rand_feat)
-    print(feat.shape)
-    print(rand_feat.shape)
-
-
-def run_without_source(data_name, bipartite=True):
-    Path("data/").mkdir(parents=True, exist_ok=True)
-    # PATH = './{}.csv'.format(data_name)
-    OUT_DF = './data/ml_{}.csv'.format(data_name)
-    # OUT_FEAT = './ml_{}.npy'.format(data_name)
-    OUT_NODE_FEAT = './data/ml_{}_node.npy'.format(data_name)
-
-    df = pd.read_csv('./ml_{}.csv'.format(data_name))
-    edge_features = np.load('./ml_{}.npy'.format(data_name))
-    node_features = np.load('./ml_{}_node.npy'.format(data_name))
+
+
+
+def data_preprocess_nosource(data_path="./data/", data_name="mooc", bipartite=True):
+    OUT_DF = data_path + 'ml_{}.csv'.format(data_name)
+    OUT_NODE_FEAT = data_path + 'ml_{}_node.npy'.format(data_name)
+
+    Path("./nosource/").mkdir(parents=True, exist_ok=True)
+    df = pd.read_csv('./nosource/ml_{}.csv'.format(data_name))
+    edge_features = np.load('./nosource/ml_{}.npy'.format(data_name))
+    node_features = np.load('./nosource/ml_{}_node.npy'.format(data_name))
 
     # df, feat = preprocess(PATH)
     print(edge_features.shape)
     print(node_features.shape)
     # new_df = reindex(graph_df, bipartite)
 
     print(str(max(df.u)))
```

### Comparing `benchtemp-1.0.0/tests/test.html` & `benchtemp-1.1.0/tests/test.html`

 * *Files identical despite different names*

### Comparing `benchtemp-1.0.0/PKG-INFO` & `benchtemp-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,683 +1,738 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6265 6e63  : 2.1.Name: benc
 00000020: 6874 656d 700a 5665 7273 696f 6e3a 2031  htemp.Version: 1
-00000030: 2e30 2e30 0a53 756d 6d61 7279 3a20 4265  .0.0.Summary: Be
-00000040: 6e63 6854 654d 503a 2041 2047 656e 6572  nchTeMP: A Gener
-00000050: 616c 2042 656e 6368 6d61 726b 204c 6962  al Benchmark Lib
-00000060: 7261 7279 2066 6f72 2045 7661 6c75 6174  rary for Evaluat
-00000070: 696e 6720 5465 6d70 6f72 616c 2047 7261  ing Temporal Gra
-00000080: 7068 204d 6f64 656c 730a 5072 6f6a 6563  ph Models.Projec
-00000090: 742d 5552 4c3a 2042 7567 2054 7261 636b  t-URL: Bug Track
-000000a0: 6572 2c20 6874 7470 733a 2f2f 6769 7468  er, https://gith
-000000b0: 7562 2e63 6f6d 2f71 6961 6e67 6875 616e  ub.com/qianghuan
-000000c0: 6777 6875 2f62 656e 6368 7465 6d70 2f69  gwhu/benchtemp/i
-000000d0: 7373 7565 730a 5072 6f6a 6563 742d 5552  ssues.Project-UR
-000000e0: 4c3a 2048 6f6d 6570 6167 652c 2068 7474  L: Homepage, htt
-000000f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000100: 7169 616e 6768 7561 6e67 7768 752f 6265  qianghuangwhu/be
-00000110: 6e63 6874 656d 700a 4175 7468 6f72 2d65  nchtemp.Author-e
-00000120: 6d61 696c 3a20 5169 616e 6720 4875 616e  mail: Qiang Huan
-00000130: 6720 3c6a 6f6e 6e79 6875 616e 6768 6e75  g <jonnyhuanghnu
-00000140: 4067 6d61 696c 2e63 6f6d 3e0a 436c 6173  @gmail.com>.Clas
-00000150: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-00000160: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000170: 3a3a 204d 4954 204c 6963 656e 7365 0a43  :: MIT License.C
-00000180: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
-00000190: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-000001a0: 5320 496e 6465 7065 6e64 656e 740a 436c  S Independent.Cl
-000001b0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000001c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001d0: 3a20 5079 7468 6f6e 203a 3a20 330a 5265  : Python :: 3.Re
-000001e0: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
-000001f0: 3d33 2e36 0a44 6573 6372 6970 7469 6f6e  =3.6.Description
-00000200: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
-00000210: 6578 742f 6d61 726b 646f 776e 0a0a 2320  ext/markdown..# 
-00000220: 4265 6e63 6854 654d 503a 2041 2047 656e  BenchTeMP: A Gen
-00000230: 6572 616c 2042 656e 6368 6d61 726b 204c  eral Benchmark L
-00000240: 6962 7261 7279 2066 6f72 2045 7661 6c75  ibrary for Evalu
-00000250: 6174 696e 6720 5465 6d70 6f72 616c 2047  ating Temporal G
-00000260: 7261 7068 204d 6f64 656c 730a 0a23 2320  raph Models..## 
-00000270: 4f76 6572 7669 6577 0a2a 2a42 656e 6368  Overview.**Bench
-00000280: 5465 4d50 2a2a 2069 7320 6120 6765 6e65  TeMP** is a gene
-00000290: 7261 6c20 4265 6e63 686d 6172 6b20 5079  ral Benchmark Py
-000002a0: 7468 6f6e 204c 6962 7261 7279 2066 6f72  thon Library for
-000002b0: 2075 7365 7273 2074 6f20 6372 6561 7465   users to create
-000002c0: 2061 6e64 2065 7661 6c75 6174 6520 5465   and evaluate Te
-000002d0: 6d70 6f72 616c 2047 7261 7068 206d 6f64  mporal Graph mod
-000002e0: 656c 7320 7175 6963 6b6c 7920 616e 6420  els quickly and 
-000002f0: 6566 6669 6369 656e 746c 792e 200a 2a2a  efficiently. .**
-00000300: 4265 6e63 6854 654d 502a 2a20 7072 6f76  BenchTeMP** prov
-00000310: 6964 6573 2075 7365 7273 2077 6974 6820  ides users with 
-00000320: 7468 6520 756e 6966 6965 6420 2a2a 6f72  the unified **or
-00000330: 6967 696e 616c 2064 6174 6173 6574 2070  iginal dataset p
-00000340: 7265 7072 6f63 6573 7320 6675 6e63 7469  reprocess functi
-00000350: 6f6e 2c20 4461 7461 2043 6c61 7373 2c20  on, Data Class, 
-00000360: 4461 7461 4c6f 6164 6572 2c20 4564 6765  DataLoader, Edge
-00000370: 5361 6d70 6c65 722c 2061 6e64 2045 7661  Sampler, and Eva
-00000380: 6c75 6174 6f72 2a2a 2066 6f72 2063 7265  luator** for cre
-00000390: 6174 696e 6720 616e 6420 6576 616c 7561  ating and evalua
-000003a0: 7469 6e67 2079 6f75 7220 5465 6d70 6f72  ting your Tempor
-000003b0: 616c 2047 7261 7068 206d 6f64 656c 2e0a  al Graph model..
-000003c0: 0a2d 2054 6865 206f 7269 6769 6e61 6c20  .- The original 
-000003d0: 6461 7461 7365 7473 2061 7265 205b 4865  datasets are [He
-000003e0: 7265 5d28 2920 616e 6420 7468 6520 6461  re]() and the da
-000003f0: 7461 7365 7473 2070 7265 7072 6f63 6573  tasets preproces
-00000400: 7365 6420 6279 2042 656e 6368 5465 4d50  sed by BenchTeMP
-00000410: 2061 7265 205b 4865 7265 5d28 292e 0a2d   are [Here]()..-
-00000420: 2054 6865 2047 6974 4875 6220 6f66 2042   The GitHub of B
-00000430: 656e 6368 5465 4d50 2070 726f 6a65 6374  enchTeMP project
-00000440: 2069 7320 5b48 6572 655d 2829 2e0a 2d20   is [Here]()..- 
-00000450: 5468 6520 736f 7572 6365 2063 6f64 6573  The source codes
-00000460: 2066 6f72 2065 7661 6c75 6174 696e 6720   for evaluating 
-00000470: 6578 6973 7469 6e67 2054 656d 706f 7261  existing Tempora
-00000480: 6c20 4772 6170 6820 6d6f 6465 6c73 2062  l Graph models b
-00000490: 6173 6564 206f 6e20 4265 6e63 6854 654d  ased on BenchTeM
-000004a0: 5020 6172 6520 5b48 6572 655d 2829 2e20  P are [Here](). 
-000004b0: 0a2d 2054 6865 206c 6561 6465 7262 6f61  .- The leaderboa
-000004c0: 7264 7320 7765 6273 6974 6520 6372 6561  rds website crea
-000004d0: 7465 6420 6279 206f 7572 2074 6561 6d20  ted by our team 
-000004e0: 666f 7220 5465 6d70 6f72 616c 2047 7261  for Temporal Gra
-000004f0: 7068 206d 6f64 656c 7320 6973 205b 4865  ph models is [He
-00000500: 7265 5d28 292e 0a0a 2323 2049 6e73 7461  re]()...## Insta
-00000510: 6c6c 6174 696f 6e0a 2323 2320 5265 7175  llation.### Requ
-00000520: 6972 656d 656e 7473 0a50 6c65 6173 6520  irements.Please 
-00000530: 656e 7375 7265 2074 6861 7420 796f 7520  ensure that you 
-00000540: 6861 7665 2069 6e73 7461 6c6c 6564 2074  have installed t
-00000550: 6865 2066 6f6c 6c6f 7769 6e67 2064 6570  he following dep
-00000560: 656e 6465 6e63 6965 733a 0a0a 2d20 6e75  endencies:..- nu
-00000570: 6d70 7920 3e3d 2031 2e31 382e 300a 2d20  mpy >= 1.18.0.- 
-00000580: 7061 6e64 6173 203e 3d20 312e 322e 300a  pandas >= 1.2.0.
-00000590: 2d20 736b 6c65 6172 6e20 3e3d 2030 2e32  - sklearn >= 0.2
-000005a0: 302e 300a 0a23 2323 2050 7950 4920 696e  0.0..### PyPI in
-000005b0: 7374 616c 6c0a 6060 6062 6173 680a 7069  stall.```bash.pi
-000005c0: 7033 2069 6e73 7461 6c6c 2062 656e 6368  p3 install bench
-000005d0: 7465 6d70 200a 6060 600a 0a23 2320 5061  temp .```..## Pa
-000005e0: 636b 6167 6520 5573 6167 650a 2323 2320  ckage Usage.### 
-000005f0: 4461 7461 7365 7473 0a54 6865 2064 6174  Datasets.The dat
-00000600: 6173 6574 7320 7468 6174 2068 6176 6520  asets that have 
-00000610: 6265 656e 2070 7265 7072 6f63 6573 7365  been preprocesse
-00000620: 6420 6279 2042 656e 6368 5465 4d50 2061  d by BenchTeMP a
-00000630: 7265 205b 4865 7265 5d28 292e 0a59 6f75  re [Here]()..You
-00000640: 2063 616e 2064 6972 6563 746c 7920 646f   can directly do
-00000650: 776e 6c6f 6164 2074 6865 2064 6174 6173  wnload the datas
-00000660: 6574 7320 616e 6420 7468 656e 2070 7574  ets and then put
-00000670: 2074 6865 6d20 696e 746f 2074 6865 2064   them into the d
-00000680: 6972 6563 746f 7279 2027 2e2f 6461 7461  irectory './data
-00000690: 272e 0a0a 496e 2061 6464 6974 696f 6e2c  '...In addition,
-000006a0: 2042 656e 6368 5465 4d50 2070 726f 7669   BenchTeMP provi
-000006b0: 6465 7320 6461 7461 2070 726f 6365 7373  des data process
-000006c0: 696e 6720 6675 6e63 7469 6f6e 732e 2079  ing functions. y
-000006d0: 6f75 2063 616e 2064 6f77 6e6c 6f61 6420  ou can download 
-000006e0: 7468 6520 6f72 6967 696e 616c 2064 6174  the original dat
-000006f0: 6173 6574 7320 5b48 6572 655d 2829 2061  asets [Here]() a
-00000700: 6e64 2074 6865 6e20 0a75 7365 2074 6865  nd then .use the
-00000710: 2066 756e 6374 696f 6e73 2070 726f 7669   functions provi
-00000720: 6465 6420 6279 2042 656e 6368 5465 4d50  ded by BenchTeMP
-00000730: 2066 6f72 2064 6174 6120 7072 6570 726f   for data prepro
-00000740: 6365 7373 696e 672e 0a0a 4675 6e63 7469  cessing...Functi
-00000750: 6f6e 3a0a 2a2a 6265 6e63 6874 656d 702e  on:.**benchtemp.
-00000760: 7072 6570 726f 6365 7373 696e 672e 6461  preprocessing.da
-00000770: 7461 2e64 6174 615f 7072 6570 726f 6365  ta.data_preproce
-00000780: 7373 2864 6174 615f 6e61 6d65 203a 2073  ss(data_name : s
-00000790: 7472 2c20 6269 7061 7274 6974 6520 3a20  tr, bipartite : 
-000007a0: 626f 6f6c 3d54 7275 6529 2a2a 0a0a 5061  bool=True)**..Pa
-000007b0: 7261 6d65 7465 7273 3a0a 2d20 2a2a 6461  rameters:.- **da
-000007c0: 7461 5f6e 616d 6520 3a20 7374 722a 2a20  ta_name : str** 
-000007d0: 2d20 7468 6520 6e61 6d65 206f 6620 7468  - the name of th
-000007e0: 6520 6461 7461 7365 742e 0a2d 202a 2a62  e dataset..- **b
-000007f0: 6970 6172 7469 7465 203a 2062 6f6f 6c2a  ipartite : bool*
-00000800: 2a20 2d20 5768 6574 6865 7220 7468 6520  * - Whether the 
-00000810: 5465 6d70 6f72 616c 2047 7261 7068 2069  Temporal Graph i
-00000820: 7320 6269 7061 7274 6974 6520 6772 6170  s bipartite grap
-00000830: 682e 0a0a 5265 7475 726e 733a 0a2d 202a  h...Returns:.- *
-00000840: 2a6d 6c5f 7b64 6174 615f 6e61 6d65 7d2e  *ml_{data_name}.
-00000850: 6373 762a 2a20 2d20 7468 6520 6373 7620  csv** - the csv 
-00000860: 6669 6c65 206f 6620 7468 6520 5465 6d70  file of the Temp
-00000870: 6f72 616c 2047 7261 7068 2e0a 2d20 2a2a  oral Graph..- **
-00000880: 6d6c 5f7b 6461 7461 5f6e 616d 657d 2e6e  ml_{data_name}.n
-00000890: 7079 2a2a 202d 2074 6865 2065 6467 6520  py** - the edge 
-000008a0: 6665 6174 7572 6573 206f 6620 7468 6520  features of the 
-000008b0: 5465 6d70 6f72 616c 2047 7261 7068 2e0a  Temporal Graph..
-000008c0: 2d20 2a2a 6d6c 5f7b 6461 7461 5f6e 616d  - **ml_{data_nam
-000008d0: 657d 5f6e 6f64 652e 6e70 792a 2a20 2d20  e}_node.npy** - 
-000008e0: 7468 6520 6e6f 6465 2066 6561 7475 7265  the node feature
-000008f0: 7320 6f66 2074 6865 2054 656d 706f 7261  s of the Tempora
-00000900: 6c20 4772 6170 682e 0a0a 4578 616d 706c  l Graph...Exampl
-00000910: 653a 0a60 6060 7079 7468 6f6e 0a66 726f  e:.```python.fro
-00000920: 6d20 6265 6e63 6874 656d 702e 7072 6570  m benchtemp.prep
-00000930: 726f 6365 7373 696e 672e 6461 7461 2069  rocessing.data i
-00000940: 6d70 6f72 7420 6461 7461 5f70 7265 7072  mport data_prepr
-00000950: 6f63 6573 730a 0a0a 2320 4966 2074 6865  ocess...# If the
-00000960: 2064 6174 6173 6574 2069 7320 6269 7061   dataset is bipa
-00000970: 7274 6974 6520 6772 6170 682c 2069 2e65  rtite graph, i.e
-00000980: 2e20 7468 6520 7573 6572 2028 736f 7572  . the user (sour
-00000990: 6365 206e 6f64 6573 2920 616e 6420 7468  ce nodes) and th
-000009a0: 6520 6974 656d 2028 6465 7374 696e 6174  e item (destinat
-000009b0: 696f 6e20 6e6f 6465 7329 2061 7265 206f  ion nodes) are o
-000009c0: 6620 7468 6520 7361 6d65 2074 7970 652e  f the same type.
-000009d0: 0a64 6174 615f 7072 6570 726f 6365 7373  .data_preprocess
-000009e0: 2822 6461 7461 5f6e 616d 6522 2c20 6269  ("data_name", bi
-000009f0: 7061 7274 6974 653d 5472 7565 290a 0a23  partite=True)..#
-00000a00: 206e 6f6e 2d62 6970 6172 7469 7465 2067   non-bipartite g
-00000a10: 7261 7068 2e0a 6461 7461 5f70 7265 7072  raph..data_prepr
-00000a20: 6f63 6573 7328 2264 6174 615f 6e61 6d65  ocess("data_name
-00000a30: 222c 2062 6970 6172 7469 7465 3d46 616c  ", bipartite=Fal
-00000a40: 7365 290a 6060 600a 0a4e 6f74 6573 3a0a  se).```..Notes:.
-00000a50: 0a46 6f72 2062 6970 6172 7469 7465 2067  .For bipartite g
-00000a60: 7261 7068 2c20 4265 6e63 6854 654d 5020  raph, BenchTeMP 
-00000a70: 7769 6c6c 2066 6163 746f 7269 7a65 2074  will factorize t
-00000a80: 6865 2073 6f75 7263 6520 6e6f 6465 2069  he source node i
-00000a90: 6e64 6578 2061 6e64 200a 7468 6520 6465  ndex and .the de
-00000aa0: 7374 696e 6174 696f 6e20 6e6f 6465 2069  stination node i
-00000ab0: 6e64 6578 2c20 7265 7370 6563 7469 7665  ndex, respective
-00000ac0: 6c79 2e20 0a60 6060 7079 7468 6f6e 0a69  ly. .```python.i
-00000ad0: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
-00000ae0: 7064 0a0a 6173 7365 7274 206c 656e 2873  pd..assert len(s
-00000af0: 6f75 7263 6573 2920 3d3d 206c 656e 2864  ources) == len(d
-00000b00: 6573 7469 6e61 7469 6f6e 7329 0a0a 2320  estinations)..# 
-00000b10: 6269 7061 7274 6974 6520 6772 6170 680a  bipartite graph.
-00000b20: 736f 7572 6365 732c 205f 203d 2070 642e  sources, _ = pd.
-00000b30: 6661 6374 6f72 697a 6528 736f 7572 6365  factorize(source
-00000b40: 7329 0a64 6573 7469 6e61 7469 6f6e 732c  s).destinations,
-00000b50: 205f 203d 2070 642e 6661 6374 6f72 697a   _ = pd.factoriz
-00000b60: 6528 6465 7374 696e 6174 696f 6e73 290a  e(destinations).
-00000b70: 0a75 7070 6572 5f75 203d 2073 6f75 7263  .upper_u = sourc
-00000b80: 6573 2e6d 6178 202b 2031 0a64 6573 7469  es.max + 1.desti
-00000b90: 6e61 7469 6f6e 7320 3d20 6465 7374 696e  nations = destin
-00000ba0: 6174 696f 6e73 202b 2075 7070 6572 5f75  ations + upper_u
-00000bb0: 0a60 6060 0a46 6f72 206e 6f6e 2d62 6970  .```.For non-bip
-00000bc0: 6172 7469 7465 2067 7261 7068 2c20 4265  artite graph, Be
-00000bd0: 6e63 6854 654d 5020 7769 6c6c 2066 6163  nchTeMP will fac
-00000be0: 746f 7269 7a65 2074 6865 2063 6f6e 6361  torize the conca
-00000bf0: 7465 6e61 7469 6f6e 206f 6620 736f 7572  tenation of sour
-00000c00: 6365 206e 6f64 6520 6172 7261 7920 616e  ce node array an
-00000c10: 6420 0a74 6865 2064 6573 7469 6e61 7469  d .the destinati
-00000c20: 6f6e 206e 6f64 6520 6172 7261 792e 200a  on node array. .
-00000c30: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
-00000c40: 7420 7061 6e64 6173 2061 7320 7064 0a69  t pandas as pd.i
-00000c50: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
-00000c60: 700a 0a61 7373 6572 7420 6c65 6e28 736f  p..assert len(so
-00000c70: 7572 6365 7329 203d 3d20 6c65 6e28 6465  urces) == len(de
-00000c80: 7374 696e 6174 696f 6e73 290a 696e 7465  stinations).inte
-00000c90: 7261 6374 696f 6e5f 6e75 6d20 3d20 6c65  raction_num = le
-00000ca0: 6e28 736f 7572 6365 7329 0a0a 2320 6e6f  n(sources)..# no
-00000cb0: 6e2d 6269 7061 7274 6974 6520 6772 6170  n-bipartite grap
-00000cc0: 680a 6e6f 6465 5f69 6e64 6578 2c20 5f20  h.node_index, _ 
-00000cd0: 3d20 7064 2e66 6163 746f 7269 7a65 286e  = pd.factorize(n
-00000ce0: 702e 636f 6e63 6174 656e 6174 6528 2873  p.concatenate((s
-00000cf0: 6f75 7263 6573 2c20 6465 7374 696e 6174  ources, destinat
-00000d00: 696f 6e73 292c 2061 7869 733d 3029 290a  ions), axis=0)).
-00000d10: 0a73 6f75 7263 6573 203d 206e 6f64 655f  .sources = node_
-00000d20: 696e 6465 785b 5b30 3a69 6e74 6572 6163  index[[0:interac
-00000d30: 7469 6f6e 5f6e 756d 5d5d 0a64 6573 7469  tion_num]].desti
-00000d40: 6e61 7469 6f6e 7320 3d20 6e6f 6465 5f69  nations = node_i
-00000d50: 6e64 6578 5b5b 696e 7465 7261 6374 696f  ndex[[interactio
-00000d60: 6e5f 6e75 6d3a 696e 7465 7261 6374 696f  n_num:interactio
-00000d70: 6e5f 6e75 6d20 2b20 696e 7465 7261 6374  n_num + interact
-00000d80: 696f 6e5f 6e75 6d5d 5d0a 6060 600a 0a0a  ion_num]].```...
-00000d90: 2323 2320 5465 6d70 6f72 616c 4461 7461  ### TemporalData
-00000da0: 2043 6c61 7373 0a43 6c61 7373 3a0a 0a2a   Class.Class:..*
-00000db0: 2a44 6174 6128 736f 7572 6365 7320 3a20  *Data(sources : 
-00000dc0: 6e75 6d70 792e 6e64 6172 7261 792c 0a64  numpy.ndarray,.d
-00000dd0: 6573 7469 6e61 7469 6f6e 7320 3a20 6e75  estinations : nu
-00000de0: 6d70 792e 6e64 6172 7261 792c 0a74 696d  mpy.ndarray,.tim
-00000df0: 6573 7461 6d70 7320 3a20 6e75 6d70 792e  estamps : numpy.
-00000e00: 6e64 6172 7261 792c 0a65 6467 655f 6964  ndarray,.edge_id
-00000e10: 7873 203a 206e 756d 7079 2e6e 6461 7272  xs : numpy.ndarr
-00000e20: 6179 2c0a 6c61 6265 6c73 203a 206e 756d  ay,.labels : num
-00000e30: 7079 2e6e 6461 7272 6179 292a 2a0a 0a50  py.ndarray)**..P
-00000e40: 6172 616d 6574 6572 733a 0a2d 202a 2a73  arameters:.- **s
-00000e50: 6f75 7263 6573 203a 206e 756d 7079 2e6e  ources : numpy.n
-00000e60: 6461 7272 6179 2a2a 202d 2041 7272 6179  darray** - Array
-00000e70: 206f 6620 736f 7572 6365 7320 6f66 2054   of sources of T
-00000e80: 656d 706f 7261 6c20 4772 6170 6820 6564  emporal Graph ed
-00000e90: 6765 732e 0a2d 202a 2a64 6573 7469 6e61  ges..- **destina
-00000ea0: 7469 6f6e 7320 3a20 6e75 6d70 792e 6e64  tions : numpy.nd
-00000eb0: 6172 7261 792a 2a20 2d20 4172 7261 7920  array** - Array 
-00000ec0: 6f66 2064 6573 7469 6e61 7469 6f6e 7320  of destinations 
-00000ed0: 6f66 2054 656d 706f 7261 6c20 4772 6170  of Temporal Grap
-00000ee0: 6820 6564 6765 732e 0a2d 202a 2a74 696d  h edges..- **tim
-00000ef0: 6573 7461 6d70 7320 3a20 6e75 6d70 792e  estamps : numpy.
-00000f00: 6e64 6172 7261 792a 2a20 2d20 4172 7261  ndarray** - Arra
-00000f10: 7920 6f66 2074 696d 6573 7461 6d70 7320  y of timestamps 
-00000f20: 6f66 2054 656d 706f 7261 6c20 4772 6170  of Temporal Grap
-00000f30: 6820 6564 6765 732e 0a2d 202a 2a65 6467  h edges..- **edg
-00000f40: 655f 6964 7873 203a 206e 756d 7079 2e6e  e_idxs : numpy.n
-00000f50: 6461 7272 6179 2a2a 202d 2041 7272 6179  darray** - Array
-00000f60: 206f 6620 6564 6765 2049 4473 206f 6620   of edge IDs of 
-00000f70: 5465 6d70 6f72 616c 2047 7261 7068 2065  Temporal Graph e
-00000f80: 6467 6573 2e0a 2d20 2a2a 6c61 6265 6c73  dges..- **labels
-00000f90: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
-00000fa0: 2a2a 202d 2041 7272 6179 206f 6620 6c61  ** - Array of la
-00000fb0: 6265 6c73 206f 6620 5465 6d70 6f72 616c  bels of Temporal
-00000fc0: 2047 7261 7068 6520 6467 6573 2e0a 0a52   Graphe dges...R
-00000fd0: 6574 7572 6e73 3a20 0a2d 202a 2a62 656e  eturns: .- **ben
-00000fe0: 6368 7465 6d70 2e44 6174 612a 2a2e 2041  chtemp.Data**. A
-00000ff0: 2054 656d 706f 7261 6c20 4772 6170 682e   Temporal Graph.
-00001000: 0a0a 0a0a 0a45 7861 6d70 6c65 3a0a 6060  .....Example:.``
-00001010: 6070 7974 686f 6e0a 696d 706f 7274 2070  `python.import p
-00001020: 616e 6461 7320 6173 2070 640a 696d 706f  andas as pd.impo
-00001030: 7274 206e 756d 7079 2061 7320 6e70 0a66  rt numpy as np.f
-00001040: 726f 6d20 6265 6e63 6874 656d 702e 7574  rom benchtemp.ut
-00001050: 696c 7320 696d 706f 7274 2044 6174 610a  ils import Data.
-00001060: 0a67 7261 7068 5f64 6620 3d20 7064 2e72  .graph_df = pd.r
-00001070: 6561 645f 6373 7628 2264 6174 6173 6574  ead_csv("dataset
-00001080: 5f70 6174 6822 290a 0a73 6f75 7263 6573  _path")..sources
-00001090: 203d 2067 7261 7068 5f64 662e 752e 7661   = graph_df.u.va
-000010a0: 6c75 6573 0a64 6573 7469 6e61 7469 6f6e  lues.destination
-000010b0: 7320 3d20 6772 6170 685f 6466 2e69 2e76  s = graph_df.i.v
-000010c0: 616c 7565 730a 6564 6765 5f69 6478 7320  alues.edge_idxs 
-000010d0: 3d20 6772 6170 685f 6466 2e69 6478 2e76  = graph_df.idx.v
-000010e0: 616c 7565 730a 6c61 6265 6c73 203d 2067  alues.labels = g
-000010f0: 7261 7068 5f64 662e 6c61 6265 6c2e 7661  raph_df.label.va
-00001100: 6c75 6573 0a74 696d 6573 7461 6d70 7320  lues.timestamps 
-00001110: 3d20 6772 6170 685f 6466 2e74 732e 7661  = graph_df.ts.va
-00001120: 6c75 6573 0a0a 2320 466f 7220 6578 616d  lues..# For exam
-00001130: 706c 652c 2074 6865 2066 756c 6c20 5465  ple, the full Te
-00001140: 6d70 6f72 616c 2047 7261 7068 206f 6620  mporal Graph of 
-00001150: 7468 6520 6461 7461 7365 7420 6973 2066  the dataset is f
-00001160: 756c 6c5f 6461 7461 2e0a 6675 6c6c 5f64  ull_data..full_d
-00001170: 6174 6120 3d20 4461 7461 2873 6f75 7263  ata = Data(sourc
-00001180: 6573 2c20 6465 7374 696e 6174 696f 6e73  es, destinations
-00001190: 2c20 7469 6d65 7374 616d 7073 2c20 6564  , timestamps, ed
-000011a0: 6765 5f69 6478 732c 206c 6162 656c 7329  ge_idxs, labels)
-000011b0: 0a60 6060 0a0a 0a23 2323 2044 6174 614c  .```...### DataL
-000011c0: 6f61 6465 720a 2323 2320 2831 2920 4c69  oader.### (1) Li
-000011d0: 6e6b 2050 7265 6469 6374 696f 6e20 7461  nk Prediction ta
-000011e0: 736b 0a46 756e 6374 696f 6e3a 0a0a 2a2a  sk.Function:..**
-000011f0: 6265 6e63 6874 656d 702e 6c70 2e72 6561  benchtemp.lp.rea
-00001200: 6465 7273 2e67 6574 5f64 6174 6128 6461  ders.get_data(da
-00001210: 7461 7365 745f 6e61 6d65 203a 2073 7472  taset_name : str
-00001220: 2c20 6469 6666 6572 656e 745f 6e65 775f  , different_new_
-00001230: 6e6f 6465 735f 6265 7477 6565 6e5f 7661  nodes_between_va
-00001240: 6c5f 616e 645f 7465 7374 3d46 616c 7365  l_and_test=False
-00001250: 2c20 7261 6e64 6f6d 697a 655f 6665 6174  , randomize_feat
-00001260: 7572 6573 3d46 616c 7365 292a 2a0a 200a  ures=False)**. .
-00001270: 5061 7261 6d65 7465 7273 3a0a 2d20 2a2a  Parameters:.- **
-00001280: 6461 7461 7365 745f 6e61 6d65 203a 2073  dataset_name : s
-00001290: 7472 2a2a 202d 2054 6865 206e 616d 6520  tr** - The name 
-000012a0: 6f66 2074 6865 2064 6174 6173 6574 2e20  of the dataset. 
-000012b0: 5468 6520 6461 7461 7365 7420 6669 6c65  The dataset file
-000012c0: 2028 2e63 7376 2066 696c 6520 6f66 2074   (.csv file of t
-000012d0: 6865 2054 656d 706f 7261 6c20 4772 6170  he Temporal Grap
-000012e0: 682c 202e 6e70 7920 6669 6c65 206f 6620  h, .npy file of 
-000012f0: 7468 6520 6e6f 6465 2066 6561 7475 7265  the node feature
-00001300: 7320 616e 6420 2e6e 7079 2066 696c 6520  s and .npy file 
-00001310: 6f66 2074 6865 2065 6467 6520 6665 6174  of the edge feat
-00001320: 7572 6573 2920 7368 6f75 6c64 2062 6520  ures) should be 
-00001330: 696e 2022 2e2f 6461 7461 2220 6469 7265  in "./data" dire
-00001340: 6374 6f72 792e 0a2d 202a 2a64 6966 6665  ctory..- **diffe
-00001350: 7265 6e74 5f6e 6577 5f6e 6f64 6573 5f62  rent_new_nodes_b
-00001360: 6574 7765 656e 5f76 616c 5f61 6e64 5f74  etween_val_and_t
-00001370: 6573 7420 3a20 626f 6f6c 2a2a 202d 2044  est : bool** - D
-00001380: 6966 6665 7265 6e74 206e 6577 206e 6f64  ifferent new nod
-00001390: 6573 2062 6574 7765 656e 2020 7468 6520  es between  the 
-000013a0: 7661 6c69 6461 7469 6f6e 2061 6e64 2074  validation and t
-000013b0: 6573 7420 6461 7461 7365 742e 0a2d 202a  est dataset..- *
-000013c0: 2a72 616e 646f 6d69 7a65 5f66 6561 7475  *randomize_featu
-000013d0: 7265 7320 3a20 626f 6f6c 2a2a 202d 2052  res : bool** - R
-000013e0: 616e 646f 6d20 696e 6974 6961 6c69 7a61  andom initializa
-000013f0: 7469 6f6e 206f 6620 6e6f 6465 2046 6561  tion of node Fea
-00001400: 7475 7265 732e 200a 0a52 6574 7572 6e73  tures. ..Returns
-00001410: 3a0a 2d20 2a2a 6e6f 6465 5f66 6561 7475  :.- **node_featu
-00001420: 7265 7320 3a20 6e75 6d70 792e 6e64 6172  res : numpy.ndar
-00001430: 7261 792a 2a20 2d20 4172 7261 7920 6f66  ray** - Array of
-00001440: 2074 6865 204e 6f64 6520 4665 6174 7572   the Node Featur
-00001450: 6573 206f 6620 7468 6520 5465 6d70 6f72  es of the Tempor
-00001460: 616c 2047 7261 7068 2e20 0a2d 202a 2a65  al Graph. .- **e
-00001470: 6467 655f 6665 6174 7572 6573 203a 206e  dge_features : n
-00001480: 756d 7079 2e6e 6461 7272 6179 2a2a 202d  umpy.ndarray** -
-00001490: 2041 7272 6179 206f 6620 7468 6520 4564   Array of the Ed
-000014a0: 6765 2046 6561 7475 7265 7320 6f66 2074  ge Features of t
-000014b0: 6865 2054 656d 706f 7261 6c20 4772 6170  he Temporal Grap
-000014c0: 682e 0a2d 202a 2a66 756c 6c5f 6461 7461  h..- **full_data
-000014d0: 203a 2062 656e 6368 7465 6d70 2e44 6174   : benchtemp.Dat
-000014e0: 612a 2a20 2d20 4675 6c6c 2054 656d 706f  a** - Full Tempo
-000014f0: 7261 6c20 4772 6170 6820 6461 7461 7365  ral Graph datase
-00001500: 742e 200a 2d20 2a2a 7472 6169 6e5f 6461  t. .- **train_da
-00001510: 7461 203a 2062 656e 6368 7465 6d70 2e44  ta : benchtemp.D
-00001520: 6174 612a 2a20 2d20 5468 6520 7472 6169  ata** - The trai
-00001530: 6e69 6e67 2054 656d 706f 7261 6c20 4772  ning Temporal Gr
-00001540: 6170 6820 6461 7461 7365 742e 200a 2d20  aph dataset. .- 
-00001550: 2a2a 7661 6c5f 6461 7461 203a 2062 656e  **val_data : ben
-00001560: 6368 7465 6d70 2e44 6174 612a 2a20 2d20  chtemp.Data** - 
-00001570: 5468 6520 7661 6c69 6461 7469 6f6e 2054  The validation T
-00001580: 656d 706f 7261 6c20 4772 6170 6820 6461  emporal Graph da
-00001590: 7461 7365 742e 0a2d 202a 2a74 6573 745f  taset..- **test_
-000015a0: 6461 7461 203a 2062 656e 6368 7465 6d70  data : benchtemp
-000015b0: 2e44 6174 612a 2a20 202d 2054 6865 202a  .Data**  - The *
-000015c0: 2a74 7261 6e73 6475 6374 6976 652a 2a20  *transductive** 
-000015d0: 7465 7374 2054 656d 706f 7261 6c20 4772  test Temporal Gr
-000015e0: 6170 6820 6461 7461 7365 742e 0a2d 202a  aph dataset..- *
-000015f0: 2a6e 6577 5f6e 6f64 655f 7661 6c5f 6461  *new_node_val_da
-00001600: 7461 203a 2062 656e 6368 7465 6d70 2e44  ta : benchtemp.D
-00001610: 6174 612a 2a20 2d20 5468 6520 2a2a 696e  ata** - The **in
-00001620: 6475 6374 6976 6520 5b6e 6577 2d5d 2a2a  ductive [new-]**
-00001630: 2073 6574 7469 6e67 2076 616c 6964 6174   setting validat
-00001640: 696f 6e20 5465 6d70 6f72 616c 2047 7261  ion Temporal Gra
-00001650: 7068 2064 6174 6173 6574 2e0a 2d20 2a2a  ph dataset..- **
-00001660: 6e65 775f 6e6f 6465 5f74 6573 745f 6461  new_node_test_da
-00001670: 7461 203a 2062 656e 6368 7465 6d70 2e44  ta : benchtemp.D
-00001680: 6174 612a 2a20 2d20 5468 6520 2a2a 696e  ata** - The **in
-00001690: 6475 6374 6976 6520 5b6e 6577 2d5d 2a2a  ductive [new-]**
-000016a0: 2073 6574 7469 6e67 2074 6573 7420 5465   setting test Te
-000016b0: 6d70 6f72 616c 2047 7261 7068 2064 6174  mporal Graph dat
-000016c0: 6173 6574 2e0a 2d20 2a2a 6e65 775f 6f6c  aset..- **new_ol
-000016d0: 645f 6e6f 6465 5f76 616c 5f64 6174 6120  d_node_val_data 
-000016e0: 3a20 6265 6e63 6874 656d 702e 4461 7461  : benchtemp.Data
-000016f0: 2a2a 202d 2054 6865 202a 2a69 6e64 7563  ** - The **induc
-00001700: 7469 7665 205b 6e65 772d 6f6c 645d 2a2a  tive [new-old]**
-00001710: 2073 6574 7469 6e67 2076 616c 6964 6174   setting validat
-00001720: 696f 6e20 5465 6d70 6f72 616c 2047 7261  ion Temporal Gra
-00001730: 7068 2064 6174 6173 6574 2e0a 2d20 2a2a  ph dataset..- **
-00001740: 6e65 775f 6f6c 645f 6e6f 6465 5f74 6573  new_old_node_tes
-00001750: 745f 6461 7461 203a 2062 656e 6368 7465  t_data : benchte
-00001760: 6d70 2e44 6174 612a 2a20 2d20 5468 6520  mp.Data** - The 
-00001770: 2a2a 696e 6475 6374 6976 6520 5b6e 6577  **inductive [new
-00001780: 2d6f 6c64 5d2a 2a20 7365 7474 696e 6720  -old]** setting 
-00001790: 7465 7374 2054 656d 706f 7261 6c20 4772  test Temporal Gr
-000017a0: 6170 6820 6461 7461 7365 742e 0a2d 202a  aph dataset..- *
-000017b0: 2a6e 6577 5f6e 6577 5f6e 6f64 655f 7661  *new_new_node_va
-000017c0: 6c5f 6461 7461 203a 2062 656e 6368 7465  l_data : benchte
-000017d0: 6d70 2e44 6174 612a 2a20 2d20 5468 6520  mp.Data** - The 
-000017e0: 2a2a 696e 6475 6374 6976 6520 5b6e 6577  **inductive [new
-000017f0: 2d6e 6577 5d2a 2a20 7365 7474 696e 6720  -new]** setting 
-00001800: 7661 6c69 6461 7469 6f6e 2054 656d 706f  validation Tempo
-00001810: 7261 6c20 4772 6170 6820 6461 7461 7365  ral Graph datase
-00001820: 742e 0a2d 202a 2a6e 6577 5f6e 6577 5f6e  t..- **new_new_n
-00001830: 6f64 655f 7465 7374 5f64 6174 6120 3a20  ode_test_data : 
-00001840: 6265 6e63 6874 656d 702e 4461 7461 2a2a  benchtemp.Data**
-00001850: 202d 2054 6865 202a 2a69 6e64 7563 7469   - The **inducti
-00001860: 7665 205b 6e65 772d 6e65 775d 2a2a 2073  ve [new-new]** s
-00001870: 6574 7469 6e67 2074 6573 7420 5465 6d70  etting test Temp
-00001880: 6f72 616c 2047 7261 7068 2064 6174 6173  oral Graph datas
-00001890: 6574 2e0a 2d20 2a2a 756e 7365 656e 5f6e  et..- **unseen_n
-000018a0: 6f64 6573 5f6e 756d 203a 2069 6e74 2a2a  odes_num : int**
-000018b0: 202d 2054 6865 206e 756d 6265 7220 6f66   - The number of
-000018c0: 2075 6e73 6565 6e20 6e6f 6465 7320 6f66   unseen nodes of
-000018d0: 2069 6e64 7563 7469 7665 2073 6574 7469   inductive setti
-000018e0: 6e67 2e0a 0a45 7861 6d70 6c65 3a0a 6060  ng...Example:.``
-000018f0: 6070 7974 686f 6e0a 6672 6f6d 2062 656e  `python.from ben
-00001900: 6368 7465 6d70 2e6c 702e 7265 6164 6572  chtemp.lp.reader
-00001910: 7320 696d 706f 7274 2067 6574 5f64 6174  s import get_dat
-00001920: 610a 0a6e 6f64 655f 6665 6174 7572 6573  a..node_features
-00001930: 2c20 6564 6765 5f66 6561 7475 7265 732c  , edge_features,
-00001940: 2066 756c 6c5f 6461 7461 2c20 7472 6169   full_data, trai
-00001950: 6e5f 6461 7461 2c20 7661 6c5f 6461 7461  n_data, val_data
-00001960: 2c20 7465 7374 5f64 6174 612c 206e 6577  , test_data, new
-00001970: 5f6e 6f64 655f 7661 6c5f 6461 7461 2c20  _node_val_data, 
-00001980: 6e65 775f 6e6f 6465 5f74 6573 745f 6461  new_node_test_da
-00001990: 7461 2c20 6e65 775f 6f6c 645f 6e6f 6465  ta, new_old_node
-000019a0: 5f76 616c 5f64 6174 612c 206e 6577 5f6f  _val_data, new_o
-000019b0: 6c64 5f6e 6f64 655f 7465 7374 5f64 6174  ld_node_test_dat
-000019c0: 612c 206e 6577 5f6e 6577 5f6e 6f64 655f  a, new_new_node_
-000019d0: 7661 6c5f 6461 7461 2c20 6e65 775f 6e65  val_data, new_ne
-000019e0: 775f 6e6f 6465 5f74 6573 745f 6461 7461  w_node_test_data
-000019f0: 2c20 756e 7365 656e 5f6e 6f64 6573 5f6e  , unseen_nodes_n
-00001a00: 756d 203d 2067 6574 5f64 6174 6128 6461  um = get_data(da
-00001a10: 7461 7365 745f 6e61 6d65 2c20 6469 6666  taset_name, diff
-00001a20: 6572 656e 745f 6e65 775f 6e6f 6465 735f  erent_new_nodes_
-00001a30: 6265 7477 6565 6e5f 7661 6c5f 616e 645f  between_val_and_
-00001a40: 7465 7374 3d46 616c 7365 2c20 7261 6e64  test=False, rand
-00001a50: 6f6d 697a 655f 6665 6174 7572 6573 3d46  omize_features=F
-00001a60: 616c 7365 290a 6060 600a 0a23 2323 2045  alse).```..### E
-00001a70: 6467 6553 616d 706c 6572 0a42 656e 6368  dgeSampler.Bench
-00001a80: 5465 4d50 2070 726f 7669 6465 7320 7468  TeMP provides th
-00001a90: 6520 756e 6966 6965 640a 6e65 6761 7469  e unified.negati
-00001aa0: 7665 2065 6467 6520 7361 6d70 6c65 7220  ve edge sampler 
-00001ab0: 7769 7468 202a 2a73 6565 642a 2a20 666f  with **seed** fo
-00001ac0: 7220 4c69 6e6b 2050 7265 6469 6374 696f  r Link Predictio
-00001ad0: 6e20 7461 736b 2074 6f20 2073 616d 706c  n task to  sampl
-00001ae0: 6520 616e 2065 7175 616c 2061 6d6f 756e  e an equal amoun
-00001af0: 7420 6f66 206e 6567 6174 6976 6573 2074  t of negatives t
-00001b00: 6f20 7468 6520 706f 7369 7469 7665 2069  o the positive i
-00001b10: 6e74 6572 6163 7469 6f6e 732e 0a0a 436c  nteractions...Cl
-00001b20: 6173 733a 0a0a 2a2a 5261 6e64 4564 6765  ass:..**RandEdge
-00001b30: 5361 6d70 6c65 7228 7372 635f 6c69 7374  Sampler(src_list
-00001b40: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
-00001b50: 2c20 6473 745f 6c69 7374 203a 206e 756d  , dst_list : num
-00001b60: 7079 2e6e 6461 7272 6179 2c20 7365 6564  py.ndarray, seed
-00001b70: 203a 2069 6e74 203d 4e6f 6e65 292a 2a0a   : int =None)**.
-00001b80: 0a50 6172 616d 6574 6572 733a 0a2d 202a  .Parameters:.- *
-00001b90: 2a73 7263 5f6c 6973 7420 3a20 6e75 6d70  *src_list : nump
-00001ba0: 792e 6e64 6172 7261 792a 2a20 2d20 7468  y.ndarray** - th
-00001bb0: 6520 6c69 7374 206f 6620 736f 7572 6365  e list of source
-00001bc0: 206e 6f64 6573 2e0a 2d20 2a2a 6473 745f   nodes..- **dst_
-00001bd0: 6c69 7374 203a 206e 756d 7079 2e6e 6461  list : numpy.nda
-00001be0: 7272 6179 2a2a 202d 2074 6865 206c 6973  rray** - the lis
-00001bf0: 7420 6f66 2064 6573 7469 6e61 7469 6f6e  t of destination
-00001c00: 206e 6f64 6573 2e0a 2d20 2a2a 7365 6564   nodes..- **seed
-00001c10: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
-00001c20: 2a2a 202d 2073 6565 6420 6f66 2072 616e  ** - seed of ran
-00001c30: 646f 6d2e 0a0a 5265 7475 726e 733a 200a  dom...Returns: .
-00001c40: 0a2d 202a 2a62 656e 6368 7465 6d70 2e52  .- **benchtemp.R
-00001c50: 616e 6445 6467 6553 616d 706c 6572 2a2a  andEdgeSampler**
-00001c60: 0a0a 4578 616d 706c 653a 0a60 6060 7079  ..Example:.```py
-00001c70: 7468 6f6e 0a66 726f 6d20 6265 6e63 6874  thon.from bencht
-00001c80: 656d 702e 6c70 2e73 616d 706c 6572 2069  emp.lp.sampler i
-00001c90: 6d70 6f72 7420 5261 6e64 4564 6765 5361  mport RandEdgeSa
-00001ca0: 6d70 6c65 720a 0a23 2046 6f72 2065 7861  mpler..# For exa
-00001cb0: 6d70 6c65 2c20 6966 2079 6f75 2061 7265  mple, if you are
-00001cc0: 2074 7261 696e 696e 6720 2c20 796f 7520   training , you 
-00001cd0: 7368 6f75 6c64 2063 7265 6174 6520 6120  should create a 
-00001ce0: 7472 6169 6e69 6e67 2020 5261 6e64 4564  training  RandEd
-00001cf0: 6765 5361 6d70 6c65 7220 6261 7365 6420  geSampler based 
-00001d00: 6f6e 2074 6865 2074 7261 696e 696e 6720  on the training 
-00001d10: 6461 7461 7365 742e 0a74 7261 696e 5f72  dataset..train_r
-00001d20: 616e 645f 7361 6d70 6c65 7220 3d20 5261  and_sampler = Ra
-00001d30: 6e64 4564 6765 5361 6d70 6c65 7228 7472  ndEdgeSampler(tr
-00001d40: 6169 6e5f 6461 7461 2e73 6f75 7263 6573  ain_data.sources
-00001d50: 2c20 7472 6169 6e5f 6461 7461 2e64 6573  , train_data.des
-00001d60: 7469 6e61 7469 6f6e 7329 0a0a 2e2e 2e0a  tinations)......
-00001d70: 666f 7220 6570 6f63 6820 696e 2072 616e  for epoch in ran
-00001d80: 6765 2861 7267 732e 6570 6f63 6873 293a  ge(args.epochs):
-00001d90: 0a20 2020 202e 2e2e 0a20 2020 2023 2073  .    ....    # s
-00001da0: 616d 706c 6520 616e 2065 7175 616c 2061  ample an equal a
-00001db0: 6d6f 756e 7420 6f66 206e 6567 6174 6976  mount of negativ
-00001dc0: 6573 2074 6f20 7468 6520 706f 7369 7469  es to the positi
-00001dd0: 7665 2069 6e74 6572 6163 7469 6f6e 732e  ve interactions.
-00001de0: 0a20 2020 205f 2c20 6e65 6761 7469 7665  .    _, negative
-00001df0: 735f 6261 7463 6820 3d20 7472 6169 6e5f  s_batch = train_
-00001e00: 7261 6e64 5f73 616d 706c 6572 2e73 616d  rand_sampler.sam
-00001e10: 706c 6528 7369 7a65 290a 2020 2020 2e2e  ple(size).    ..
-00001e20: 2e0a 2e2e 2e0a 6060 600a 2323 2320 2832  ......```.### (2
-00001e30: 2920 4e6f 6465 2043 6c61 7373 6966 6963  ) Node Classific
-00001e40: 6174 696f 6e20 7461 736b 0a46 756e 6374  ation task.Funct
-00001e50: 696f 6e3a 0a0a 0a0a 2a2a 6265 6e63 6874  ion:....**bencht
-00001e60: 656d 702e 6e63 2e72 6561 6465 7273 2e67  emp.nc.readers.g
-00001e70: 6574 5f64 6174 615f 6e6f 6465 5f63 6c61  et_data_node_cla
-00001e80: 7373 6966 6963 6174 696f 6e28 2864 6174  ssification((dat
-00001e90: 6173 6574 5f6e 616d 6520 3a20 7374 722c  aset_name : str,
-00001ea0: 2075 7365 5f76 616c 6964 6174 696f 6e20   use_validation 
-00001eb0: 3a20 626f 6f6c 3d46 616c 7365 2929 2a2a  : bool=False))**
-00001ec0: 200a 0a50 6172 616d 6574 6572 733a 0a2d   ..Parameters:.-
-00001ed0: 2064 6174 6173 6574 5f6e 616d 6520 3a20   dataset_name : 
-00001ee0: 7374 7220 2d20 5468 6520 6e61 6d65 206f  str - The name o
-00001ef0: 6620 7468 6520 6461 7461 7365 742e 2054  f the dataset. T
-00001f00: 6865 2064 6174 6173 6574 2066 696c 6520  he dataset file 
-00001f10: 282e 6373 7620 6669 6c65 206f 6620 7468  (.csv file of th
-00001f20: 6520 5465 6d70 6f72 616c 2047 7261 7068  e Temporal Graph
-00001f30: 2c20 2e6e 7079 2066 696c 6520 6f66 2074  , .npy file of t
-00001f40: 6865 206e 6f64 6520 6665 6174 7572 6573  he node features
-00001f50: 2061 6e64 202e 6e70 7920 6669 6c65 206f   and .npy file o
-00001f60: 6620 7468 6520 6564 6765 2066 6561 7475  f the edge featu
-00001f70: 7265 7329 2073 686f 756c 6420 6265 2069  res) should be i
-00001f80: 6e20 222e 2f64 6174 6122 2064 6972 6563  n "./data" direc
-00001f90: 746f 7279 2e0a 2d20 7573 655f 7661 6c69  tory..- use_vali
-00001fa0: 6461 7469 6f6e 203a 2062 6f6f 6c20 2d20  dation : bool - 
-00001fb0: 5768 6574 6865 7220 7573 6520 7661 6c69  Whether use vali
-00001fc0: 6461 7469 6f6e 2064 6174 6173 6574 206f  dation dataset o
-00001fd0: 7220 6e6f 742e 0a0a 5265 7475 726e 733a  r not...Returns:
-00001fe0: 0a2d 202a 2a6e 6f64 655f 6665 6174 7572  .- **node_featur
-00001ff0: 6573 203a 206e 756d 7079 2e6e 6461 7272  es : numpy.ndarr
-00002000: 6179 2a2a 202d 2041 7272 6179 206f 6620  ay** - Array of 
-00002010: 7468 6520 4e6f 6465 2046 6561 7475 7265  the Node Feature
-00002020: 7320 6f66 2074 6865 2054 656d 706f 7261  s of the Tempora
-00002030: 6c20 4772 6170 682e 200a 2d20 2a2a 6564  l Graph. .- **ed
-00002040: 6765 5f66 6561 7475 7265 7320 3a20 6e75  ge_features : nu
-00002050: 6d70 792e 6e64 6172 7261 792a 2a20 2d20  mpy.ndarray** - 
-00002060: 4172 7261 7920 6f66 2074 6865 2045 6467  Array of the Edg
-00002070: 6520 4665 6174 7572 6573 206f 6620 7468  e Features of th
-00002080: 6520 5465 6d70 6f72 616c 2047 7261 7068  e Temporal Graph
-00002090: 2e0a 2d20 2a2a 6675 6c6c 5f64 6174 6120  ..- **full_data 
-000020a0: 3a20 6265 6e63 6874 656d 702e 4461 7461  : benchtemp.Data
-000020b0: 2a2a 202d 2046 756c 6c20 5465 6d70 6f72  ** - Full Tempor
-000020c0: 616c 2047 7261 7068 2064 6174 6173 6574  al Graph dataset
-000020d0: 2066 6f72 204e 6f64 6520 436c 6173 7369   for Node Classi
-000020e0: 6669 6361 7469 6f6e 2074 6173 6b2e 200a  fication task. .
-000020f0: 2d20 2a2a 7472 6169 6e5f 6461 7461 203a  - **train_data :
-00002100: 2062 656e 6368 7465 6d70 2e44 6174 612a   benchtemp.Data*
-00002110: 2a20 2d20 5468 6520 7472 6169 6e69 6e67  * - The training
-00002120: 2054 656d 706f 7261 6c20 4772 6170 6820   Temporal Graph 
-00002130: 6461 7461 7365 7420 666f 7220 4e6f 6465  dataset for Node
-00002140: 2043 6c61 7373 6966 6963 6174 696f 6e20   Classification 
-00002150: 7461 736b 2e20 0a2d 202a 2a76 616c 5f64  task. .- **val_d
-00002160: 6174 6120 3a20 6265 6e63 6874 656d 702e  ata : benchtemp.
-00002170: 4461 7461 2a2a 202d 2054 6865 2076 616c  Data** - The val
-00002180: 6964 6174 696f 6e20 5465 6d70 6f72 616c  idation Temporal
-00002190: 2047 7261 7068 2064 6174 6173 6574 2066   Graph dataset f
-000021a0: 6f72 204e 6f64 6520 436c 6173 7369 6669  or Node Classifi
-000021b0: 6361 7469 6f6e 2074 6173 6b2e 0a2d 202a  cation task..- *
-000021c0: 2a74 6573 745f 6461 7461 203a 2062 656e  *test_data : ben
-000021d0: 6368 7465 6d70 2e44 6174 612a 2a20 202d  chtemp.Data**  -
-000021e0: 2054 6865 2074 6573 7420 5465 6d70 6f72   The test Tempor
-000021f0: 616c 2047 7261 7068 2064 6174 6173 6574  al Graph dataset
-00002200: 2066 6f72 204e 6f64 6520 436c 6173 7369   for Node Classi
-00002210: 6669 6361 7469 6f6e 2074 6173 6b2e 0a0a  fication task...
-00002220: 0a0a 2323 2320 4561 726c 7953 746f 704d  ..### EarlyStopM
-00002230: 6f6e 6974 6f72 0a43 6c61 7373 3a0a 0a2a  onitor.Class:..*
-00002240: 2a45 6172 6c79 5374 6f70 4d6f 6e69 746f  *EarlyStopMonito
-00002250: 7228 6d61 785f 726f 756e 643d 332c 2068  r(max_round=3, h
-00002260: 6967 6865 725f 6265 7474 6572 3d54 7275  igher_better=Tru
-00002270: 652c 2074 6f6c 6572 616e 6365 3d31 652d  e, tolerance=1e-
-00002280: 3130 292a 2a0a 0a50 6172 616d 6574 6572  10)**..Parameter
-00002290: 733a 0a2d 202a 2a6d 6178 5f72 6f75 6e64  s:.- **max_round
-000022a0: 203a 2069 6e74 2a2a 202d 2074 6865 206d   : int** - the m
-000022b0: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
-000022c0: 2072 6f75 6e64 7320 6f66 2045 6172 6c79   rounds of Early
-000022d0: 5374 6f70 4d6f 6e69 746f 722e 0a2d 202a  StopMonitor..- *
-000022e0: 2a68 6967 6865 725f 6265 7474 6572 203a  *higher_better :
-000022f0: 2062 6f6f 6c2a 2a20 2d20 6265 7474 6572   bool** - better
-00002300: 2074 6865 2070 6572 666f 726d 616e 6365   the performance
-00002310: 2e0a 2d20 2a2a 746f 6c65 7261 6e63 6520  ..- **tolerance 
-00002320: 3a20 666c 6f61 742a 2a20 2d20 7468 6520  : float** - the 
-00002330: 746f 6c65 7261 6e63 6520 6f66 2074 6865  tolerance of the
-00002340: 2045 6172 6c79 5374 6f70 4d6f 6e69 746f   EarlyStopMonito
-00002350: 722e 0a0a 5265 7475 726e 733a 0a2d 202a  r...Returns:.- *
-00002360: 2a62 656e 6368 7465 6d70 2e45 6172 6c79  *benchtemp.Early
-00002370: 5374 6f70 4d6f 6e69 746f 722a 2a0a 0a45  StopMonitor**..E
-00002380: 7861 6d70 6c65 3a0a 6060 6070 7974 686f  xample:.```pytho
-00002390: 6e0a 6672 6f6d 2062 656e 6368 7465 6d70  n.from benchtemp
-000023a0: 2e75 7469 6c73 2069 6d70 6f72 7420 4561  .utils import Ea
-000023b0: 726c 7953 746f 704d 6f6e 6974 6f72 0a0a  rlyStopMonitor..
-000023c0: 2e2e 2e0a 6561 726c 795f 7374 6f70 7065  ....early_stoppe
-000023d0: 7220 3d20 4561 726c 7953 746f 704d 6f6e  r = EarlyStopMon
-000023e0: 6974 6f72 286d 6178 5f72 6f75 6e64 3d61  itor(max_round=a
-000023f0: 7267 732e 7061 7469 656e 6365 290a 666f  rgs.patience).fo
-00002400: 7220 6570 6f63 6820 696e 2072 616e 6765  r epoch in range
-00002410: 2861 7267 732e 6570 6f63 6873 293a 0a20  (args.epochs):. 
-00002420: 2020 202e 2e2e 0a20 2020 2076 616c 5f61     ....    val_a
-00002430: 7020 3d20 6d6f 6465 6c28 7661 6c5f 6461  p = model(val_da
-00002440: 7461 7365 7473 290a 2020 2020 6966 2065  tasets).    if e
-00002450: 6172 6c79 5f73 746f 7070 6572 2e65 6172  arly_stopper.ear
-00002460: 6c79 5f73 746f 705f 6368 6563 6b28 7661  ly_stop_check(va
-00002470: 6c5f 6170 293a 0a20 2020 2020 2020 2062  l_ap):.        b
-00002480: 7265 616b 0a20 2020 202e 2e2e 0a2e 2e2e  reak.    .......
-00002490: 0a60 6060 0a0a 2323 2320 4576 616c 7561  .```..### Evalua
-000024a0: 746f 720a 0a2a 2a4c 696e 6b20 5072 6564  tor..**Link Pred
-000024b0: 6963 7469 6f6e 2a2a 2045 7661 6c75 6174  iction** Evaluat
-000024c0: 696f 6e20 4d65 7472 6963 7320 2061 7265  ion Metrics  are
-000024d0: 202a 2a41 7265 6120 556e 6465 7220 7468   **Area Under th
-000024e0: 6520 5265 6365 6976 6572 204f 7065 7261  e Receiver Opera
-000024f0: 7469 6e67 2043 6861 7261 6374 6572 6973  ting Characteris
-00002500: 7469 6320 4375 7276 6520 2852 4f43 2041  tic Curve (ROC A
-00002510: 5543 292a 2a20 616e 6420 2a2a 6176 6572  UC)** and **aver
-00002520: 6167 6520 7072 6563 6973 696f 6e20 2841  age precision (A
-00002530: 5029 2a2a 0a0a 2a2a 4e6f 6465 2043 6c61  P)**..**Node Cla
-00002540: 7373 6966 6963 6174 696f 6e2a 2a20 4576  ssification** Ev
-00002550: 616c 7561 7469 6f6e 204d 6574 7269 6320  aluation Metric 
-00002560: 6973 202a 2a41 7265 6120 556e 6465 7220  is **Area Under 
-00002570: 7468 6520 5265 6365 6976 6572 204f 7065  the Receiver Ope
-00002580: 7261 7469 6e67 2043 6861 7261 6374 6572  rating Character
-00002590: 6973 7469 6320 4375 7276 6520 2852 4f43  istic Curve (ROC
-000025a0: 2041 5543 292a 2a0a 0a43 6c61 7373 3a20   AUC)**..Class: 
-000025b0: 0a0a 2a2a 4576 616c 7561 746f 7228 7461  ..**Evaluator(ta
-000025c0: 736b 5f6e 616d 653a 2073 7472 203d 2022  sk_name: str = "
-000025d0: 4c50 2229 2a2a 0a0a 5061 7261 6d65 7465  LP")**..Paramete
-000025e0: 7273 3a0a 2d20 7461 736b 5f6e 616d 6520  rs:.- task_name 
-000025f0: 3a20 7374 7220 202d 2074 6865 206e 616d  : str  - the nam
-00002600: 6520 6f66 2074 6865 2074 6173 6b2c 2063  e of the task, c
-00002610: 686f 6963 6520 696e 202a 2a5b 224c 5022  hoice in **["LP"
-00002620: 2c20 224e 4322 5d2a 2a2e 0a0a 5265 7475  , "NC"]**...Retu
-00002630: 726e 733a 0a2d 202a 2a62 656e 6368 7465  rns:.- **benchte
-00002640: 6d70 2e45 7661 6c75 6174 6f72 2a2a 0a0a  mp.Evaluator**..
-00002650: 4578 616d 706c 653a 0a0a 6060 6070 7974  Example:..```pyt
-00002660: 686f 6e0a 6672 6f6d 2062 656e 6368 7465  hon.from benchte
-00002670: 6d70 2e75 7469 6c73 2069 6d70 6f72 7420  mp.utils import 
-00002680: 4576 616c 7561 746f 720a 0a23 2046 6f72  Evaluator..# For
-00002690: 2065 7861 6d70 6c65 2c20 4c69 6e6b 2070   example, Link p
-000026a0: 7265 6469 6374 696f 6e20 7461 736b 2e20  rediction task. 
-000026b0: 4576 616c 7561 7469 6f6e 204d 6574 7269  Evaluation Metri
-000026c0: 6373 3a20 4155 432c 2041 502e 0a65 7661  cs: AUC, AP..eva
-000026d0: 6c75 6174 6f72 203d 2045 7661 6c75 6174  luator = Evaluat
-000026e0: 6f72 2822 4c50 2229 0a0a 2e2e 2e0a 2320  or("LP")......# 
-000026f0: 7465 7374 2064 6174 610a 7072 6564 5f73  test data.pred_s
-00002700: 636f 7265 203d 206d 6f64 656c 2874 6573  core = model(tes
-00002710: 745f 6461 7461 290a 7465 7374 5f61 7563  t_data).test_auc
-00002720: 2c20 7465 7374 5f61 7020 3d20 4576 616c  , test_ap = Eval
-00002730: 7561 746f 722e 6576 616c 2870 7265 645f  uator.eval(pred_
-00002740: 7363 6f72 652c 2074 7275 655f 6c61 6265  score, true_labe
-00002750: 6c29 0a2e 2e2e 0a60 6060 0a0a 6060 6070  l).....```..```p
-00002760: 7974 686f 6e0a 6672 6f6d 2062 656e 6368  ython.from bench
-00002770: 7465 6d70 2e75 7469 6c73 2069 6d70 6f72  temp.utils impor
-00002780: 7420 4576 616c 7561 746f 720a 0a23 2046  t Evaluator..# F
-00002790: 6f72 2065 7861 6d70 6c65 2c20 4e6f 6465  or example, Node
-000027a0: 2043 6c61 7373 6966 6963 6174 696f 6e20   Classification 
-000027b0: 7461 736b 2e20 4576 616c 7561 7469 6f6e  task. Evaluation
-000027c0: 204d 6574 7269 6373 3a20 4155 432e 0a65   Metrics: AUC..e
-000027d0: 7661 6c75 6174 6f72 203d 2045 7661 6c75  valuator = Evalu
-000027e0: 6174 6f72 2822 4e43 2229 0a0a 2e2e 2e0a  ator("NC")......
-000027f0: 2320 7465 7374 2064 6174 610a 7072 6564  # test data.pred
-00002800: 5f73 636f 7265 203d 206d 6f64 656c 2874  _score = model(t
-00002810: 6573 745f 6461 7461 290a 7465 7374 5f61  est_data).test_a
-00002820: 7563 203d 2045 7661 6c75 6174 6f72 2e65  uc = Evaluator.e
-00002830: 7661 6c28 7072 6564 5f73 636f 7265 2c20  val(pred_score, 
-00002840: 7472 7565 5f6c 6162 656c 290a 2e2e 2e0a  true_label).....
-00002850: 6060 600a 0a23 2320 4361 6c6c 2066 6f72  ```..## Call for
-00002860: 2043 6f6e 7472 6962 7574 696f 6e73 0a0a   Contributions..
-00002870: 2a2a 4265 6e63 6854 654d 502a 2a20 7072  **BenchTeMP** pr
-00002880: 6f6a 6563 7420 6973 206c 6f6f 6b69 6e67  oject is looking
-00002890: 2066 6f72 2063 6f6e 7472 6962 7574 6f72   for contributor
-000028a0: 7320 7769 7468 200a 6578 7065 7274 6973  s with .expertis
-000028b0: 6520 616e 6420 656e 7468 7573 6961 736d  e and enthusiasm
-000028c0: 2120 4966 2079 6f75 2068 6176 6520 6120  ! If you have a 
-000028d0: 6465 7369 7265 2074 6f20 636f 6e74 7269  desire to contri
-000028e0: 6275 7465 2074 6f20 2a2a 4265 6e63 6854  bute to **BenchT
-000028f0: 654d 502a 2a2c 200a 706c 6561 7365 2063  eMP**, .please c
-00002900: 6f6e 7461 6374 205b 4265 6e63 6854 654d  ontact [BenchTeM
-00002910: 5020 7465 616d 5d28 6d61 696c 746f 3a6a  P team](mailto:j
-00002920: 6f6e 6e79 6875 616e 6768 6e75 4067 6d61  onnyhuanghnu@gma
-00002930: 696c 2e63 6f6d 292e 0a0a 5c69 7465 6d20  il.com)...\item 
-00002940: 5765 2072 656c 6561 7365 205c 7379 732c  We release \sys,
-00002950: 2061 2067 656e 6572 616c 2062 656e 6368   a general bench
-00002960: 6d61 726b 206c 6962 7261 7279 2066 6f72  mark library for
-00002970: 2065 7661 6c75 6174 696e 6720 7465 6d70   evaluating temp
-00002980: 6f72 616c 2067 7261 7068 206d 6f64 656c  oral graph model
-00002990: 733b 0a0a 5c69 7465 6d20 5765 2070 726f  s;..\item We pro
-000029a0: 7669 6465 7320 756e 6966 6965 6420 6265  vides unified be
-000029b0: 6e63 6b6d 6172 6b20 7465 6d70 6f72 616c  nckmark temporal
-000029c0: 2067 7261 7068 2064 6174 6173 6574 7320   graph datasets 
-000029d0: 7072 6f63 6573 7365 6420 6279 205c 7379  processed by \sy
-000029e0: 733b 0a0a 5c69 7465 6d20 5765 2062 656e  s;..\item We ben
-000029f0: 6368 6d61 726b 2065 7869 7374 696e 6720  chmark existing 
-00002a00: 7465 6d70 6f72 616c 2067 7261 7068 206d  temporal graph m
-00002a10: 6f64 656c 7320 6261 7365 6420 6f6e 205c  odels based on \
-00002a20: 7379 7320 2066 6f72 2072 6f62 7573 7420  sys  for robust 
-00002a30: 6465 7665 6c6f 706d 656e 7473 2061 6e64  developments and
-00002a40: 2061 6e61 6c79 7369 7320 7468 6520 7065   analysis the pe
-00002a50: 7266 6f72 6d61 6e63 6520 6f66 206d 6f64  rformance of mod
-00002a60: 656c 7320 696e 2064 6574 6169 6c3b 0a0a  els in detail;..
-00002a70: 5c69 7465 6d20 5765 2072 656c 7365 6420  \item We relsed 
-00002a80: 7468 6520 6c65 6164 6572 626f 6172 6473  the leaderboards
-00002a90: 2066 6f72 2074 656d 706f 7261 6c20 6772   for temporal gr
-00002aa0: 6170 6820 6d6f 6465 6c73 2e0a 0a         aph models...
+00000030: 2e31 2e30 0a53 756d 6d61 7279 3a20 4265  .1.0.Summary: Be
+00000040: 6e63 6854 656d 703a 2041 2047 656e 6572  nchTemp: A Gener
+00000050: 616c 2042 656e 6368 6d61 726b 2066 6f72  al Benchmark for
+00000060: 2045 7661 6c75 6174 696e 6720 5465 6d70   Evaluating Temp
+00000070: 6f72 616c 2047 7261 7068 204e 6575 7261  oral Graph Neura
+00000080: 6c20 4e65 7477 6f72 6b73 0a50 726f 6a65  l Networks.Proje
+00000090: 6374 2d55 524c 3a20 4275 6720 5472 6163  ct-URL: Bug Trac
+000000a0: 6b65 722c 2068 7474 7073 3a2f 2f67 6974  ker, https://git
+000000b0: 6875 622e 636f 6d2f 7169 616e 6768 7561  hub.com/qianghua
+000000c0: 6e67 7768 752f 6265 6e63 6874 656d 702f  ngwhu/benchtemp/
+000000d0: 6973 7375 6573 0a50 726f 6a65 6374 2d55  issues.Project-U
+000000e0: 524c 3a20 486f 6d65 7061 6765 2c20 6874  RL: Homepage, ht
+000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000100: 2f71 6961 6e67 6875 616e 6777 6875 2f62  /qianghuangwhu/b
+00000110: 656e 6368 7465 6d70 0a41 7574 686f 722d  enchtemp.Author-
+00000120: 656d 6169 6c3a 2051 6961 6e67 2048 7561  email: Qiang Hua
+00000130: 6e67 203c 6a6f 6e6e 7968 7561 6e67 686e  ng <jonnyhuanghn
+00000140: 7540 676d 6169 6c2e 636f 6d3e 0a43 6c61  u@gmail.com>.Cla
+00000150: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
+00000160: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000170: 203a 3a20 4d49 5420 4c69 6365 6e73 650a   :: MIT License.
+00000180: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
+00000190: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+000001a0: 4f53 2049 6e64 6570 656e 6465 6e74 0a43  OS Independent.C
+000001b0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000001c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0a52  :: Python :: 3.R
+000001e0: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
+000001f0: 3e3d 332e 360a 4465 7363 7269 7074 696f  >=3.6.Descriptio
+00000200: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+00000210: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a23  text/markdown..#
+00000220: 2042 656e 6368 5465 6d70 3a20 4120 4765   BenchTemp: A Ge
+00000230: 6e65 7261 6c20 4265 6e63 686d 6172 6b20  neral Benchmark 
+00000240: 666f 7220 4576 616c 7561 7469 6e67 2054  for Evaluating T
+00000250: 656d 706f 7261 6c20 4772 6170 6820 4e65  emporal Graph Ne
+00000260: 7572 616c 204e 6574 776f 726b 730a 0a23  ural Networks..#
+00000270: 2320 4265 6e63 6854 656d 7020 4672 616d  # BenchTemp Fram
+00000280: 6577 6f72 6b0a 3c69 6d67 2073 7263 3d22  ework.<img src="
+00000290: 696d 672f 6672 616d 6577 6f72 6b2e 706e  img/framework.pn
+000002a0: 6722 2061 6c74 3d22 4f76 6572 7669 6577  g" alt="Overview
+000002b0: 206f 6620 4265 6e63 6854 656d 7022 2073   of BenchTemp" s
+000002c0: 7479 6c65 3d22 7769 6474 683a 3130 3025  tyle="width:100%
+000002d0: 3b22 202f 3e0a 0a23 2320 4265 6e63 6854  ;" />..## BenchT
+000002e0: 656d 7020 5069 7065 6c69 6e65 0a3c 696d  emp Pipeline.<im
+000002f0: 6720 7372 633d 2269 6d67 2f70 6970 656c  g src="img/pipel
+00000300: 696e 652e 706e 6722 2061 6c74 3d22 4265  ine.png" alt="Be
+00000310: 6e63 6854 656d 7020 5069 7065 6c69 6e65  nchTemp Pipeline
+00000320: 2220 7374 796c 653d 2277 6964 7468 3a31  " style="width:1
+00000330: 3030 253b 2220 2f3e 0a0a 2323 204f 7665  00%;" />..## Ove
+00000340: 7276 6965 770a 2a2a 4265 6e63 6854 656d  rview.**BenchTem
+00000350: 702a 2a20 6973 2061 2067 656e 6572 616c  p** is a general
+00000360: 2042 656e 6368 6d61 726b 2050 7974 686f   Benchmark Pytho
+00000370: 6e20 4c69 6272 6172 7920 666f 7220 7573  n Library for us
+00000380: 6572 7320 746f 2065 7661 6c75 6174 6520  ers to evaluate 
+00000390: 5465 6d70 6f72 616c 2047 7261 7068 204e  Temporal Graph N
+000003a0: 6575 7261 6c20 4e65 7477 6f72 6b73 2028  eural Networks (
+000003b0: 5447 4e4e 7329 2071 7569 636b 6c79 2061  TGNNs) quickly a
+000003c0: 6e64 2065 6666 6963 6965 6e74 6c79 206f  nd efficiently o
+000003d0: 6e20 7661 7269 6f75 7320 776f 726b 6c6f  n various worklo
+000003e0: 6164 732e 200a 2a2a 4265 6e63 6854 656d  ads. .**BenchTem
+000003f0: 702a 2a20 7072 6f76 6964 6573 202a 2a42  p** provides **B
+00000400: 656e 6368 6d61 726b 2044 6174 6173 6574  enchmark Dataset
+00000410: 732a 2a2c 2061 6e64 2075 6e69 6669 6564  s**, and unified
+00000420: 2070 6970 656c 696e 6573 2028 2a2a 4461   pipelines (**Da
+00000430: 7461 5072 6570 726f 6365 7373 6f72 2c20  taPreprocessor, 
+00000440: 4461 7461 4c6f 6164 6572 2045 6467 6553  DataLoader EdgeS
+00000450: 616d 706c 6572 2c20 4576 616c 7561 746f  ampler, Evaluato
+00000460: 722c 2045 6172 6c79 5374 6f70 4d6f 6e69  r, EarlyStopMoni
+00000470: 746f 722c 2042 4345 4c6f 7373 2c20 4f70  tor, BCELoss, Op
+00000480: 7469 6d69 7a65 722c 616e 6420 4c65 6164  timizer,and Lead
+00000490: 6572 626f 6172 642a 2a20 2920 666f 7220  erboard** ) for 
+000004a0: 6576 616c 7561 7469 6e67 2054 656d 706f  evaluating Tempo
+000004b0: 7261 6c20 4772 6170 6820 4e65 7572 616c  ral Graph Neural
+000004c0: 204e 6574 776f 726b 7320 6f6e 2062 6f74   Networks on bot
+000004d0: 6820 6c69 6e6b 2070 7265 6469 6374 696f  h link predictio
+000004e0: 6e20 616e 6420 6e6f 6465 2063 6c61 7373  n and node class
+000004f0: 6966 6963 6174 696f 6e20 7461 736b 732e  ification tasks.
+00000500: 0a0a 2d20 5468 6520 4265 6e63 6854 656d  ..- The BenchTem
+00000510: 7020 5079 5049 2057 6562 7369 7465 2069  p PyPI Website i
+00000520: 7320 3c61 2068 7265 663d 2268 7474 7073  s <a href="https
+00000530: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000540: 6563 742f 6265 6e63 6874 656d 702f 2220  ect/benchtemp/" 
+00000550: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00000560: 4865 7265 3c2f 613e 2e0a 0a2d 2054 6865  Here</a>...- The
+00000570: 2047 6974 4875 6220 6f66 2042 656e 6368   GitHub of Bench
+00000580: 5465 6d70 2070 726f 6a65 6374 2069 7320  Temp project is 
+00000590: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000005a0: 2f67 6974 6875 622e 636f 6d2f 7169 616e  /github.com/qian
+000005b0: 6768 7561 6e67 7768 752f 6265 6e63 6874  ghuangwhu/bencht
+000005c0: 656d 7022 2074 6172 6765 743d 225f 626c  emp" target="_bl
+000005d0: 616e 6b22 3e48 6572 653c 2f61 3e2e 200a  ank">Here</a>. .
+000005e0: 0a2d 2054 6865 2064 6174 6173 6574 7320  .- The datasets 
+000005f0: 6172 6520 3c61 2068 7265 663d 2268 7474  are <a href="htt
+00000600: 7073 3a2f 2f64 7269 7665 2e67 6f6f 676c  ps://drive.googl
+00000610: 652e 636f 6d2f 6472 6976 652f 666f 6c64  e.com/drive/fold
+00000620: 6572 732f 3148 4b53 4647 4566 7848 446c  ers/1HKSFGEfxHDl
+00000630: 4875 515a 366e 4b34 534c 4345 4d46 5149  HuQZ6nK4SLCEMFQI
+00000640: 4f74 7a70 7a3f 7573 703d 7368 6172 696e  Otzpz?usp=sharin
+00000650: 6722 2074 6172 6765 743d 225f 626c 616e  g" target="_blan
+00000660: 6b22 3e48 6572 653c 2f61 3e2e 200a 0a2d  k">Here</a>. ..-
+00000670: 2054 6865 206c 6561 6465 7262 6f61 7264   The leaderboard
+00000680: 7320 7765 6273 6974 6520 666f 7220 5465  s website for Te
+00000690: 6d70 6f72 616c 2047 7261 7068 204e 6575  mporal Graph Neu
+000006a0: 7261 6c20 4e65 7477 6f72 6b73 206f 6e20  ral Networks on 
+000006b0: 626f 7468 204c 696e 6b20 5072 6564 6963  both Link Predic
+000006c0: 7469 6f6e 2061 6e64 204e 6f64 6520 436c  tion and Node Cl
+000006d0: 6173 7369 6669 6361 7469 6f6e 2074 6173  assification tas
+000006e0: 6b73 2069 7320 3c61 2068 7265 663d 2268  ks is <a href="h
+000006f0: 7474 7073 3a2f 2f6d 792d 7765 6273 6974  ttps://my-websit
+00000700: 652d 3667 6e70 6961 796d 3038 3931 3730  e-6gnpiaym089170
+00000710: 3262 2d31 3235 3732 3539 3235 342e 7463  2b-1257259254.tc
+00000720: 6c6f 7564 6261 7365 6170 702e 636f 6d2f  loudbaseapp.com/
+00000730: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000740: 223e 4865 7265 3c2f 613e 2e0a 2d20 5468  ">Here</a>..- Th
+00000750: 6520 736f 7572 6365 2063 6f64 6573 2066  e source codes f
+00000760: 6f72 2065 7661 6c75 6174 696e 6720 6578  or evaluating ex
+00000770: 6973 7469 6e67 2054 656d 706f 7261 6c20  isting Temporal 
+00000780: 4772 6170 6820 4e65 7572 616c 204e 6574  Graph Neural Net
+00000790: 776f 726b 7320 6261 7365 6420 6f6e 2042  works based on B
+000007a0: 656e 6368 5465 6d70 2061 7265 203c 6120  enchTemp are <a 
+000007b0: 6872 6566 3d22 6874 7470 733a 2f2f 6d79  href="https://my
+000007c0: 2d77 6562 7369 7465 2d36 676e 7069 6179  -website-6gnpiay
+000007d0: 6d30 3839 3137 3032 622d 3132 3537 3235  m0891702b-125725
+000007e0: 3932 3534 2e74 636c 6f75 6462 6173 6561  9254.tcloudbasea
+000007f0: 7070 2e63 6f6d 2f22 2074 6172 6765 743d  pp.com/" target=
+00000800: 225f 626c 616e 6b22 3e63 6f6d 696e 6720  "_blank">coming 
+00000810: 736f 6f6e 3c2f 613e 2e0a 0a0a 2323 2049  soon</a>....## I
+00000820: 6e73 7461 6c6c 6174 696f 6e0a 2323 2320  nstallation.### 
+00000830: 5265 7175 6972 656d 656e 7473 0a50 6c65  Requirements.Ple
+00000840: 6173 6520 656e 7375 7265 2074 6861 7420  ase ensure that 
+00000850: 796f 7520 6861 7665 2069 6e73 7461 6c6c  you have install
+00000860: 6564 2074 6865 2066 6f6c 6c6f 7769 6e67  ed the following
+00000870: 2064 6570 656e 6465 6e63 6965 733a 0a0a   dependencies:..
+00000880: 2d20 6e75 6d70 7920 3e3d 2031 2e31 382e  - numpy >= 1.18.
+00000890: 300a 2d20 7061 6e64 6173 203e 3d20 312e  0.- pandas >= 1.
+000008a0: 322e 300a 2d20 736b 6c65 6172 6e20 3e3d  2.0.- sklearn >=
+000008b0: 2030 2e32 302e 300a 0a23 2323 2042 656e   0.20.0..### Ben
+000008c0: 6368 5465 6d70 2050 7950 4920 696e 7374  chTemp PyPI inst
+000008d0: 616c 6c0a 0a60 6060 6261 7368 0a70 6970  all..```bash.pip
+000008e0: 3320 696e 7374 616c 6c20 6265 6e63 6874  3 install bencht
+000008f0: 656d 7020 0a60 6060 0a0a 0a23 2320 5061  emp .```...## Pa
+00000900: 636b 6167 6520 5573 6167 650a 0a0a 2323  ckage Usage...##
+00000910: 2320 4461 7461 7365 7473 0a54 6865 2064  # Datasets.The d
+00000920: 6174 6173 6574 7320 7468 6174 2068 6176  atasets that hav
+00000930: 6520 6265 656e 2070 7265 7072 6f63 6573  e been preproces
+00000940: 7365 6420 6279 2042 656e 6368 5465 6d70  sed by BenchTemp
+00000950: 2061 7265 205b 4865 7265 5d28 6874 7470   are [Here](http
+00000960: 733a 2f2f 6472 6976 652e 676f 6f67 6c65  s://drive.google
+00000970: 2e63 6f6d 2f64 7269 7665 2f66 6f6c 6465  .com/drive/folde
+00000980: 7273 2f31 484b 5346 4745 6678 4844 6c48  rs/1HKSFGEfxHDlH
+00000990: 7551 5a36 6e4b 3453 4c43 454d 4651 494f  uQZ6nK4SLCEMFQIO
+000009a0: 747a 707a 3f75 7370 3d73 6861 7269 6e67  tzpz?usp=sharing
+000009b0: 292e 0a59 6f75 2063 616e 2064 6972 6563  )..You can direc
+000009c0: 746c 7920 646f 776e 6c6f 6164 2074 6865  tly download the
+000009d0: 2064 6174 6173 6574 7320 616e 6420 7468   datasets and th
+000009e0: 656e 2070 7574 2074 6865 6d20 696e 746f  en put them into
+000009f0: 2074 6865 2064 6972 6563 746f 7279 2027   the directory '
+00000a00: 2e2f 6461 7461 272e 0a0a 496e 2061 6464  ./data'...In add
+00000a10: 6974 696f 6e2c 2042 656e 6368 5465 6d70  ition, BenchTemp
+00000a20: 2070 726f 7669 6465 7320 6461 7461 2070   provides data p
+00000a30: 726f 6365 7373 696e 6720 6675 6e63 7469  rocessing functi
+00000a40: 6f6e 7320 666f 7220 796f 7520 746f 2070  ons for you to p
+00000a50: 7265 7072 6f63 6573 7320 796f 7572 7320  reprocess yours 
+00000a60: 5447 4e4e 7320 6461 7461 7365 7473 2e20  TGNNs datasets. 
+00000a70: 0a3c 212d 2d20 796f 7520 6361 6e20 646f  .<!-- you can do
+00000a80: 776e 6c6f 6164 2074 6865 206f 7269 6769  wnload the origi
+00000a90: 6e61 6c20 6461 7461 7365 7473 205b 4865  nal datasets [He
+00000aa0: 7265 5d28 2920 616e 6420 7468 656e 2020  re]() and then  
+00000ab0: 2d2d 3e0a 3c21 2d2d 2075 7365 2074 6865  -->.<!-- use the
+00000ac0: 2066 756e 6374 696f 6e73 2070 726f 7669   functions provi
+00000ad0: 6465 6420 6279 2042 656e 6368 5465 6d70  ded by BenchTemp
+00000ae0: 2066 6f72 2064 6174 6120 6461 7461 2e20   for data data. 
+00000af0: 2d2d 3e0a 0a46 756e 6374 696f 6e3a 0a2a  -->..Function:.*
+00000b00: 2a62 656e 6368 7465 6d70 2e70 7265 7072  *benchtemp.prepr
+00000b10: 6f63 6573 7369 6e67 2e64 6174 612e 6461  ocessing.data.da
+00000b20: 7461 5f70 7265 7072 6f63 6573 7328 6461  ta_preprocess(da
+00000b30: 7461 5f6e 616d 6520 3a20 7374 722c 2062  ta_name : str, b
+00000b40: 6970 6172 7469 7465 203a 2062 6f6f 6c3d  ipartite : bool=
+00000b50: 5472 7565 292a 2a0a 0a50 6172 616d 6574  True)**..Paramet
+00000b60: 6572 733a 0a2d 202a 2a64 6174 615f 6e61  ers:.- **data_na
+00000b70: 6d65 203a 2073 7472 2a2a 202d 2074 6865  me : str** - the
+00000b80: 206e 616d 6520 6f66 2074 6865 2064 6174   name of the dat
+00000b90: 6173 6574 2e0a 2d20 2a2a 6269 7061 7274  aset..- **bipart
+00000ba0: 6974 6520 3a20 626f 6f6c 2a2a 202d 2057  ite : bool** - W
+00000bb0: 6865 7468 6572 2074 6865 2054 656d 706f  hether the Tempo
+00000bc0: 7261 6c20 4772 6170 6820 6973 2062 6970  ral Graph is bip
+00000bd0: 6172 7469 7465 2067 7261 7068 2e0a 0a52  artite graph...R
+00000be0: 6574 7572 6e73 3a0a 2d20 2a2a 6d6c 5f7b  eturns:.- **ml_{
+00000bf0: 6461 7461 5f6e 616d 657d 2e63 7376 2a2a  data_name}.csv**
+00000c00: 202d 2074 6865 2063 7376 2066 696c 6520   - the csv file 
+00000c10: 6f66 2074 6865 2054 656d 706f 7261 6c20  of the Temporal 
+00000c20: 4772 6170 682e 0a2d 202a 2a6d 6c5f 7b64  Graph..- **ml_{d
+00000c30: 6174 615f 6e61 6d65 7d2e 6e70 792a 2a20  ata_name}.npy** 
+00000c40: 2d20 7468 6520 6564 6765 2066 6561 7475  - the edge featu
+00000c50: 7265 7320 6f66 2074 6865 2054 656d 706f  res of the Tempo
+00000c60: 7261 6c20 4772 6170 682e 0a2d 202a 2a6d  ral Graph..- **m
+00000c70: 6c5f 7b64 6174 615f 6e61 6d65 7d5f 6e6f  l_{data_name}_no
+00000c80: 6465 2e6e 7079 2a2a 202d 2074 6865 206e  de.npy** - the n
+00000c90: 6f64 6520 6665 6174 7572 6573 206f 6620  ode features of 
+00000ca0: 7468 6520 5465 6d70 6f72 616c 2047 7261  the Temporal Gra
+00000cb0: 7068 2e0a 0a45 7861 6d70 6c65 3a0a 0a60  ph...Example:..`
+00000cc0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+00000cd0: 6265 6e63 6874 656d 7020 6173 2062 740a  benchtemp as bt.
+00000ce0: 0a70 726f 6365 7373 6f72 203d 2062 742e  .processor = bt.
+00000cf0: 4461 7461 5072 6570 726f 6365 7373 6f72  DataPreprocessor
+00000d00: 2864 6174 615f 7061 7468 3d22 2e2f 6461  (data_path="./da
+00000d10: 7461 2f22 2c20 6461 7461 5f6e 616d 653d  ta/", data_name=
+00000d20: 226d 6f6f 6322 290a 2320 4966 2074 6865  "mooc").# If the
+00000d30: 2064 6174 6173 6574 2069 7320 6269 7061   dataset is bipa
+00000d40: 7274 6974 6520 6772 6170 682c 2069 2e65  rtite graph, i.e
+00000d50: 2e20 7468 6520 7573 6572 2028 736f 7572  . the user (sour
+00000d60: 6365 206e 6f64 6573 2920 616e 6420 7468  ce nodes) and th
+00000d70: 6520 6974 656d 2028 6465 7374 696e 6174  e item (destinat
+00000d80: 696f 6e20 6e6f 6465 7329 2061 7265 206f  ion nodes) are o
+00000d90: 6620 7468 6520 7361 6d65 2074 7970 652e  f the same type.
+00000da0: 0a70 726f 6365 7373 6f72 2e64 6174 615f  .processor.data_
+00000db0: 7072 6570 726f 6365 7373 2862 6970 6172  preprocess(bipar
+00000dc0: 7469 7465 3d54 7275 6529 0a0a 2320 6e6f  tite=True)..# no
+00000dd0: 6e2d 6269 7061 7274 6974 6520 6772 6170  n-bipartite grap
+00000de0: 682e 0a70 726f 6365 7373 6f72 2e64 6174  h..processor.dat
+00000df0: 615f 7072 6570 726f 6365 7373 2862 6970  a_preprocess(bip
+00000e00: 6172 7469 7465 3d46 616c 7365 290a 6060  artite=False).``
+00000e10: 600a 0a4e 6f74 6573 3a0a 0a46 6f72 2062  `..Notes:..For b
+00000e20: 6970 6172 7469 7465 2067 7261 7068 2c20  ipartite graph, 
+00000e30: 4265 6e63 6854 656d 7020 7769 6c6c 2066  BenchTemp will f
+00000e40: 6163 746f 7269 7a65 2074 6865 2073 6f75  actorize the sou
+00000e50: 7263 6520 6e6f 6465 2069 6e64 6578 2061  rce node index a
+00000e60: 6e64 200a 7468 6520 6465 7374 696e 6174  nd .the destinat
+00000e70: 696f 6e20 6e6f 6465 2069 6e64 6578 2c20  ion node index, 
+00000e80: 7265 7370 6563 7469 7665 6c79 2e20 0a60  respectively. .`
+00000e90: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+00000ea0: 7061 6e64 6173 2061 7320 7064 0a0a 6173  pandas as pd..as
+00000eb0: 7365 7274 206c 656e 2873 6f75 7263 6573  sert len(sources
+00000ec0: 2920 3d3d 206c 656e 2864 6573 7469 6e61  ) == len(destina
+00000ed0: 7469 6f6e 7329 0a0a 2320 6269 7061 7274  tions)..# bipart
+00000ee0: 6974 6520 6772 6170 680a 736f 7572 6365  ite graph.source
+00000ef0: 732c 205f 203d 2070 642e 6661 6374 6f72  s, _ = pd.factor
+00000f00: 697a 6528 736f 7572 6365 7329 0a64 6573  ize(sources).des
+00000f10: 7469 6e61 7469 6f6e 732c 205f 203d 2070  tinations, _ = p
+00000f20: 642e 6661 6374 6f72 697a 6528 6465 7374  d.factorize(dest
+00000f30: 696e 6174 696f 6e73 290a 0a75 7070 6572  inations)..upper
+00000f40: 5f75 203d 2073 6f75 7263 6573 2e6d 6178  _u = sources.max
+00000f50: 202b 2031 0a64 6573 7469 6e61 7469 6f6e   + 1.destination
+00000f60: 7320 3d20 6465 7374 696e 6174 696f 6e73  s = destinations
+00000f70: 202b 2075 7070 6572 5f75 0a60 6060 0a46   + upper_u.```.F
+00000f80: 6f72 206e 6f6e 2d62 6970 6172 7469 7465  or non-bipartite
+00000f90: 2067 7261 7068 2c20 4265 6e63 6854 656d   graph, BenchTem
+00000fa0: 7020 7769 6c6c 2066 6163 746f 7269 7a65  p will factorize
+00000fb0: 2074 6865 2063 6f6e 6361 7465 6e61 7469   the concatenati
+00000fc0: 6f6e 206f 6620 736f 7572 6365 206e 6f64  on of source nod
+00000fd0: 6520 6172 7261 7920 616e 6420 0a74 6865  e array and .the
+00000fe0: 2064 6573 7469 6e61 7469 6f6e 206e 6f64   destination nod
+00000ff0: 6520 6172 7261 792e 200a 0a60 6060 7079  e array. ..```py
+00001000: 7468 6f6e 0a69 6d70 6f72 7420 7061 6e64  thon.import pand
+00001010: 6173 2061 7320 7064 0a69 6d70 6f72 7420  as as pd.import 
+00001020: 6e75 6d70 7920 6173 206e 700a 0a61 7373  numpy as np..ass
+00001030: 6572 7420 6c65 6e28 736f 7572 6365 7329  ert len(sources)
+00001040: 203d 3d20 6c65 6e28 6465 7374 696e 6174   == len(destinat
+00001050: 696f 6e73 290a 696e 7465 7261 6374 696f  ions).interactio
+00001060: 6e5f 6e75 6d20 3d20 6c65 6e28 736f 7572  n_num = len(sour
+00001070: 6365 7329 0a0a 2320 6e6f 6e2d 6269 7061  ces)..# non-bipa
+00001080: 7274 6974 6520 6772 6170 680a 6e6f 6465  rtite graph.node
+00001090: 5f69 6e64 6578 2c20 5f20 3d20 7064 2e66  _index, _ = pd.f
+000010a0: 6163 746f 7269 7a65 286e 702e 636f 6e63  actorize(np.conc
+000010b0: 6174 656e 6174 6528 2873 6f75 7263 6573  atenate((sources
+000010c0: 2c20 6465 7374 696e 6174 696f 6e73 292c  , destinations),
+000010d0: 2061 7869 733d 3029 290a 0a73 6f75 7263   axis=0))..sourc
+000010e0: 6573 203d 206e 6f64 655f 696e 6465 785b  es = node_index[
+000010f0: 5b30 3a69 6e74 6572 6163 7469 6f6e 5f6e  [0:interaction_n
+00001100: 756d 5d5d 0a64 6573 7469 6e61 7469 6f6e  um]].destination
+00001110: 7320 3d20 6e6f 6465 5f69 6e64 6578 5b5b  s = node_index[[
+00001120: 696e 7465 7261 6374 696f 6e5f 6e75 6d3a  interaction_num:
+00001130: 696e 7465 7261 6374 696f 6e5f 6e75 6d20  interaction_num 
+00001140: 2b20 696e 7465 7261 6374 696f 6e5f 6e75  + interaction_nu
+00001150: 6d5d 5d0a 6060 600a 0a0a 2323 2320 5465  m]].```...### Te
+00001160: 6d70 6f72 616c 4461 7461 2043 6c61 7373  mporalData Class
+00001170: 0a43 6c61 7373 3a0a 0a2a 2a44 6174 6128  .Class:..**Data(
+00001180: 736f 7572 6365 7320 3a20 6e75 6d70 792e  sources : numpy.
+00001190: 6e64 6172 7261 792c 0a64 6573 7469 6e61  ndarray,.destina
+000011a0: 7469 6f6e 7320 3a20 6e75 6d70 792e 6e64  tions : numpy.nd
+000011b0: 6172 7261 792c 0a74 696d 6573 7461 6d70  array,.timestamp
+000011c0: 7320 3a20 6e75 6d70 792e 6e64 6172 7261  s : numpy.ndarra
+000011d0: 792c 0a65 6467 655f 6964 7873 203a 206e  y,.edge_idxs : n
+000011e0: 756d 7079 2e6e 6461 7272 6179 2c0a 6c61  umpy.ndarray,.la
+000011f0: 6265 6c73 203a 206e 756d 7079 2e6e 6461  bels : numpy.nda
+00001200: 7272 6179 292a 2a0a 0a50 6172 616d 6574  rray)**..Paramet
+00001210: 6572 733a 0a2d 202a 2a73 6f75 7263 6573  ers:.- **sources
+00001220: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
+00001230: 2a2a 202d 2041 7272 6179 206f 6620 736f  ** - Array of so
+00001240: 7572 6365 7320 6f66 2054 656d 706f 7261  urces of Tempora
+00001250: 6c20 4772 6170 6820 6564 6765 732e 0a2d  l Graph edges..-
+00001260: 202a 2a64 6573 7469 6e61 7469 6f6e 7320   **destinations 
+00001270: 3a20 6e75 6d70 792e 6e64 6172 7261 792a  : numpy.ndarray*
+00001280: 2a20 2d20 4172 7261 7920 6f66 2064 6573  * - Array of des
+00001290: 7469 6e61 7469 6f6e 7320 6f66 2054 656d  tinations of Tem
+000012a0: 706f 7261 6c20 4772 6170 6820 6564 6765  poral Graph edge
+000012b0: 732e 0a2d 202a 2a74 696d 6573 7461 6d70  s..- **timestamp
+000012c0: 7320 3a20 6e75 6d70 792e 6e64 6172 7261  s : numpy.ndarra
+000012d0: 792a 2a20 2d20 4172 7261 7920 6f66 2074  y** - Array of t
+000012e0: 696d 6573 7461 6d70 7320 6f66 2054 656d  imestamps of Tem
+000012f0: 706f 7261 6c20 4772 6170 6820 6564 6765  poral Graph edge
+00001300: 732e 0a2d 202a 2a65 6467 655f 6964 7873  s..- **edge_idxs
+00001310: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
+00001320: 2a2a 202d 2041 7272 6179 206f 6620 6564  ** - Array of ed
+00001330: 6765 2049 4473 206f 6620 5465 6d70 6f72  ge IDs of Tempor
+00001340: 616c 2047 7261 7068 2065 6467 6573 2e0a  al Graph edges..
+00001350: 2d20 2a2a 6c61 6265 6c73 203a 206e 756d  - **labels : num
+00001360: 7079 2e6e 6461 7272 6179 2a2a 202d 2041  py.ndarray** - A
+00001370: 7272 6179 206f 6620 6c61 6265 6c73 206f  rray of labels o
+00001380: 6620 5465 6d70 6f72 616c 2047 7261 7068  f Temporal Graph
+00001390: 6520 6467 6573 2e0a 0a52 6574 7572 6e73  e dges...Returns
+000013a0: 3a20 0a2d 202a 2a62 656e 6368 7465 6d70  : .- **benchtemp
+000013b0: 2e44 6174 612a 2a2e 2041 2054 656d 706f  .Data**. A Tempo
+000013c0: 7261 6c20 4772 6170 682e 0a0a 0a0a 0a45  ral Graph......E
+000013d0: 7861 6d70 6c65 3a0a 6060 6070 7974 686f  xample:.```pytho
+000013e0: 6e0a 696d 706f 7274 2070 616e 6461 7320  n.import pandas 
+000013f0: 6173 2070 640a 696d 706f 7274 206e 756d  as pd.import num
+00001400: 7079 2061 7320 6e70 0a69 6d70 6f72 7420  py as np.import 
+00001410: 6265 6e63 6874 656d 7020 6173 2062 740a  benchtemp as bt.
+00001420: 0a0a 6772 6170 685f 6466 203d 2070 642e  ..graph_df = pd.
+00001430: 7265 6164 5f63 7376 2822 6461 7461 7365  read_csv("datase
+00001440: 745f 7061 7468 2229 0a0a 736f 7572 6365  t_path")..source
+00001450: 7320 3d20 6772 6170 685f 6466 2e75 2e76  s = graph_df.u.v
+00001460: 616c 7565 730a 6465 7374 696e 6174 696f  alues.destinatio
+00001470: 6e73 203d 2067 7261 7068 5f64 662e 692e  ns = graph_df.i.
+00001480: 7661 6c75 6573 0a65 6467 655f 6964 7873  values.edge_idxs
+00001490: 203d 2067 7261 7068 5f64 662e 6964 782e   = graph_df.idx.
+000014a0: 7661 6c75 6573 0a6c 6162 656c 7320 3d20  values.labels = 
+000014b0: 6772 6170 685f 6466 2e6c 6162 656c 2e76  graph_df.label.v
+000014c0: 616c 7565 730a 7469 6d65 7374 616d 7073  alues.timestamps
+000014d0: 203d 2067 7261 7068 5f64 662e 7473 2e76   = graph_df.ts.v
+000014e0: 616c 7565 730a 0a23 2046 6f72 2065 7861  alues..# For exa
+000014f0: 6d70 6c65 2c20 7468 6520 6675 6c6c 2054  mple, the full T
+00001500: 656d 706f 7261 6c20 4772 6170 6820 6f66  emporal Graph of
+00001510: 2074 6865 2064 6174 6173 6574 2069 7320   the dataset is 
+00001520: 6675 6c6c 5f64 6174 612e 0a66 756c 6c5f  full_data..full_
+00001530: 6461 7461 203d 2062 742e 4461 7461 2873  data = bt.Data(s
+00001540: 6f75 7263 6573 2c20 6465 7374 696e 6174  ources, destinat
+00001550: 696f 6e73 2c20 7469 6d65 7374 616d 7073  ions, timestamps
+00001560: 2c20 6564 6765 5f69 6478 732c 206c 6162  , edge_idxs, lab
+00001570: 656c 7329 0a60 6060 0a0a 0a23 2323 2044  els).```...### D
+00001580: 6174 614c 6f61 6465 720a 2323 2320 2831  ataLoader.### (1
+00001590: 2920 4c69 6e6b 2050 7265 6469 6374 696f  ) Link Predictio
+000015a0: 6e20 7461 736b 0a46 756e 6374 696f 6e3a  n task.Function:
+000015b0: 0a0a 2a2a 6265 6e63 6874 656d 702e 6c70  ..**benchtemp.lp
+000015c0: 2e72 6561 6465 7273 2e67 6574 5f64 6174  .readers.get_dat
+000015d0: 6128 6461 7461 7365 745f 6e61 6d65 203a  a(dataset_name :
+000015e0: 2073 7472 2c20 6469 6666 6572 656e 745f   str, different_
+000015f0: 6e65 775f 6e6f 6465 735f 6265 7477 6565  new_nodes_betwee
+00001600: 6e5f 7661 6c5f 616e 645f 7465 7374 3d46  n_val_and_test=F
+00001610: 616c 7365 2c20 7261 6e64 6f6d 697a 655f  alse, randomize_
+00001620: 6665 6174 7572 6573 3d46 616c 7365 292a  features=False)*
+00001630: 2a0a 200a 5061 7261 6d65 7465 7273 3a0a  *. .Parameters:.
+00001640: 2d20 2a2a 6461 7461 7365 745f 6e61 6d65  - **dataset_name
+00001650: 203a 2073 7472 2a2a 202d 2054 6865 206e   : str** - The n
+00001660: 616d 6520 6f66 2074 6865 2064 6174 6173  ame of the datas
+00001670: 6574 2e20 5468 6520 6461 7461 7365 7420  et. The dataset 
+00001680: 6669 6c65 2028 2e63 7376 2066 696c 6520  file (.csv file 
+00001690: 6f66 2074 6865 2054 656d 706f 7261 6c20  of the Temporal 
+000016a0: 4772 6170 682c 202e 6e70 7920 6669 6c65  Graph, .npy file
+000016b0: 206f 6620 7468 6520 6e6f 6465 2066 6561   of the node fea
+000016c0: 7475 7265 7320 616e 6420 2e6e 7079 2066  tures and .npy f
+000016d0: 696c 6520 6f66 2074 6865 2065 6467 6520  ile of the edge 
+000016e0: 6665 6174 7572 6573 2920 7368 6f75 6c64  features) should
+000016f0: 2062 6520 696e 2022 2e2f 6461 7461 2220   be in "./data" 
+00001700: 6469 7265 6374 6f72 792e 0a2d 202a 2a64  directory..- **d
+00001710: 6966 6665 7265 6e74 5f6e 6577 5f6e 6f64  ifferent_new_nod
+00001720: 6573 5f62 6574 7765 656e 5f76 616c 5f61  es_between_val_a
+00001730: 6e64 5f74 6573 7420 3a20 626f 6f6c 2a2a  nd_test : bool**
+00001740: 202d 2044 6966 6665 7265 6e74 206e 6577   - Different new
+00001750: 206e 6f64 6573 2062 6574 7765 656e 2020   nodes between  
+00001760: 7468 6520 7661 6c69 6461 7469 6f6e 2061  the validation a
+00001770: 6e64 2074 6573 7420 6461 7461 7365 742e  nd test dataset.
+00001780: 0a2d 202a 2a72 616e 646f 6d69 7a65 5f66  .- **randomize_f
+00001790: 6561 7475 7265 7320 3a20 626f 6f6c 2a2a  eatures : bool**
+000017a0: 202d 2052 616e 646f 6d20 696e 6974 6961   - Random initia
+000017b0: 6c69 7a61 7469 6f6e 206f 6620 6e6f 6465  lization of node
+000017c0: 2046 6561 7475 7265 732e 200a 0a52 6574   Features. ..Ret
+000017d0: 7572 6e73 3a0a 2d20 2a2a 6e6f 6465 5f66  urns:.- **node_f
+000017e0: 6561 7475 7265 7320 3a20 6e75 6d70 792e  eatures : numpy.
+000017f0: 6e64 6172 7261 792a 2a20 2d20 4172 7261  ndarray** - Arra
+00001800: 7920 6f66 2074 6865 204e 6f64 6520 4665  y of the Node Fe
+00001810: 6174 7572 6573 206f 6620 7468 6520 5465  atures of the Te
+00001820: 6d70 6f72 616c 2047 7261 7068 2e20 0a2d  mporal Graph. .-
+00001830: 202a 2a65 6467 655f 6665 6174 7572 6573   **edge_features
+00001840: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
+00001850: 2a2a 202d 2041 7272 6179 206f 6620 7468  ** - Array of th
+00001860: 6520 4564 6765 2046 6561 7475 7265 7320  e Edge Features 
+00001870: 6f66 2074 6865 2054 656d 706f 7261 6c20  of the Temporal 
+00001880: 4772 6170 682e 0a2d 202a 2a66 756c 6c5f  Graph..- **full_
+00001890: 6461 7461 203a 2062 656e 6368 7465 6d70  data : benchtemp
+000018a0: 2e44 6174 612a 2a20 2d20 4675 6c6c 2054  .Data** - Full T
+000018b0: 656d 706f 7261 6c20 4772 6170 6820 6461  emporal Graph da
+000018c0: 7461 7365 742e 200a 2d20 2a2a 7472 6169  taset. .- **trai
+000018d0: 6e5f 6461 7461 203a 2062 656e 6368 7465  n_data : benchte
+000018e0: 6d70 2e44 6174 612a 2a20 2d20 5468 6520  mp.Data** - The 
+000018f0: 7472 6169 6e69 6e67 2054 656d 706f 7261  training Tempora
+00001900: 6c20 4772 6170 6820 6461 7461 7365 742e  l Graph dataset.
+00001910: 200a 2d20 2a2a 7661 6c5f 6461 7461 203a   .- **val_data :
+00001920: 2062 656e 6368 7465 6d70 2e44 6174 612a   benchtemp.Data*
+00001930: 2a20 2d20 5468 6520 7661 6c69 6461 7469  * - The validati
+00001940: 6f6e 2054 656d 706f 7261 6c20 4772 6170  on Temporal Grap
+00001950: 6820 6461 7461 7365 742e 0a2d 202a 2a74  h dataset..- **t
+00001960: 6573 745f 6461 7461 203a 2062 656e 6368  est_data : bench
+00001970: 7465 6d70 2e44 6174 612a 2a20 202d 2054  temp.Data**  - T
+00001980: 6865 202a 2a74 7261 6e73 6475 6374 6976  he **transductiv
+00001990: 652a 2a20 7465 7374 2054 656d 706f 7261  e** test Tempora
+000019a0: 6c20 4772 6170 6820 6461 7461 7365 742e  l Graph dataset.
+000019b0: 0a2d 202a 2a6e 6577 5f6e 6f64 655f 7661  .- **new_node_va
+000019c0: 6c5f 6461 7461 203a 2062 656e 6368 7465  l_data : benchte
+000019d0: 6d70 2e44 6174 612a 2a20 2d20 5468 6520  mp.Data** - The 
+000019e0: 2a2a 696e 6475 6374 6976 6520 5b6e 6577  **inductive [new
+000019f0: 2d5d 2a2a 2073 6574 7469 6e67 2076 616c  -]** setting val
+00001a00: 6964 6174 696f 6e20 5465 6d70 6f72 616c  idation Temporal
+00001a10: 2047 7261 7068 2064 6174 6173 6574 2e0a   Graph dataset..
+00001a20: 2d20 2a2a 6e65 775f 6e6f 6465 5f74 6573  - **new_node_tes
+00001a30: 745f 6461 7461 203a 2062 656e 6368 7465  t_data : benchte
+00001a40: 6d70 2e44 6174 612a 2a20 2d20 5468 6520  mp.Data** - The 
+00001a50: 2a2a 696e 6475 6374 6976 6520 5b6e 6577  **inductive [new
+00001a60: 2d5d 2a2a 2073 6574 7469 6e67 2074 6573  -]** setting tes
+00001a70: 7420 5465 6d70 6f72 616c 2047 7261 7068  t Temporal Graph
+00001a80: 2064 6174 6173 6574 2e0a 2d20 2a2a 6e65   dataset..- **ne
+00001a90: 775f 6f6c 645f 6e6f 6465 5f76 616c 5f64  w_old_node_val_d
+00001aa0: 6174 6120 3a20 6265 6e63 6874 656d 702e  ata : benchtemp.
+00001ab0: 4461 7461 2a2a 202d 2054 6865 202a 2a69  Data** - The **i
+00001ac0: 6e64 7563 7469 7665 205b 6e65 772d 6f6c  nductive [new-ol
+00001ad0: 645d 2a2a 2073 6574 7469 6e67 2076 616c  d]** setting val
+00001ae0: 6964 6174 696f 6e20 5465 6d70 6f72 616c  idation Temporal
+00001af0: 2047 7261 7068 2064 6174 6173 6574 2e0a   Graph dataset..
+00001b00: 2d20 2a2a 6e65 775f 6f6c 645f 6e6f 6465  - **new_old_node
+00001b10: 5f74 6573 745f 6461 7461 203a 2062 656e  _test_data : ben
+00001b20: 6368 7465 6d70 2e44 6174 612a 2a20 2d20  chtemp.Data** - 
+00001b30: 5468 6520 2a2a 696e 6475 6374 6976 6520  The **inductive 
+00001b40: 5b6e 6577 2d6f 6c64 5d2a 2a20 7365 7474  [new-old]** sett
+00001b50: 696e 6720 7465 7374 2054 656d 706f 7261  ing test Tempora
+00001b60: 6c20 4772 6170 6820 6461 7461 7365 742e  l Graph dataset.
+00001b70: 0a2d 202a 2a6e 6577 5f6e 6577 5f6e 6f64  .- **new_new_nod
+00001b80: 655f 7661 6c5f 6461 7461 203a 2062 656e  e_val_data : ben
+00001b90: 6368 7465 6d70 2e44 6174 612a 2a20 2d20  chtemp.Data** - 
+00001ba0: 5468 6520 2a2a 696e 6475 6374 6976 6520  The **inductive 
+00001bb0: 5b6e 6577 2d6e 6577 5d2a 2a20 7365 7474  [new-new]** sett
+00001bc0: 696e 6720 7661 6c69 6461 7469 6f6e 2054  ing validation T
+00001bd0: 656d 706f 7261 6c20 4772 6170 6820 6461  emporal Graph da
+00001be0: 7461 7365 742e 0a2d 202a 2a6e 6577 5f6e  taset..- **new_n
+00001bf0: 6577 5f6e 6f64 655f 7465 7374 5f64 6174  ew_node_test_dat
+00001c00: 6120 3a20 6265 6e63 6874 656d 702e 4461  a : benchtemp.Da
+00001c10: 7461 2a2a 202d 2054 6865 202a 2a69 6e64  ta** - The **ind
+00001c20: 7563 7469 7665 205b 6e65 772d 6e65 775d  uctive [new-new]
+00001c30: 2a2a 2073 6574 7469 6e67 2074 6573 7420  ** setting test 
+00001c40: 5465 6d70 6f72 616c 2047 7261 7068 2064  Temporal Graph d
+00001c50: 6174 6173 6574 2e0a 2d20 2a2a 756e 7365  ataset..- **unse
+00001c60: 656e 5f6e 6f64 6573 5f6e 756d 203a 2069  en_nodes_num : i
+00001c70: 6e74 2a2a 202d 2054 6865 206e 756d 6265  nt** - The numbe
+00001c80: 7220 6f66 2075 6e73 6565 6e20 6e6f 6465  r of unseen node
+00001c90: 7320 6f66 2069 6e64 7563 7469 7665 2073  s of inductive s
+00001ca0: 6574 7469 6e67 2e0a 0a45 7861 6d70 6c65  etting...Example
+00001cb0: 3a0a 0a60 6060 7079 7468 6f6e 0a69 6d70  :..```python.imp
+00001cc0: 6f72 7420 6265 6e63 6874 656d 7020 6173  ort benchtemp as
+00001cd0: 2062 740a 0a64 6174 6120 3d20 6274 2e6c   bt..data = bt.l
+00001ce0: 702e 4461 7461 4c6f 6164 6572 2864 6174  p.DataLoader(dat
+00001cf0: 6173 6574 5f70 6174 683d 222e 2f64 6174  aset_path="./dat
+00001d00: 612f 222c 2064 6174 6173 6574 5f6e 616d  a/", dataset_nam
+00001d10: 653d 276d 6f6f 6327 290a 0a6e 6f64 655f  e='mooc')..node_
+00001d20: 6665 6174 7572 6573 2c20 6564 6765 5f66  features, edge_f
+00001d30: 6561 7475 7265 732c 2066 756c 6c5f 6461  eatures, full_da
+00001d40: 7461 2c20 7472 6169 6e5f 6461 7461 2c20  ta, train_data, 
+00001d50: 7661 6c5f 6461 7461 2c20 7465 7374 5f64  val_data, test_d
+00001d60: 6174 612c 206e 6577 5f6e 6f64 655f 7661  ata, new_node_va
+00001d70: 6c5f 6461 7461 2c20 6e65 775f 6e6f 6465  l_data, new_node
+00001d80: 5f74 6573 745f 6461 7461 2c20 6e65 775f  _test_data, new_
+00001d90: 6f6c 645f 6e6f 6465 5f76 616c 5f64 6174  old_node_val_dat
+00001da0: 612c 206e 6577 5f6f 6c64 5f6e 6f64 655f  a, new_old_node_
+00001db0: 7465 7374 5f64 6174 612c 206e 6577 5f6e  test_data, new_n
+00001dc0: 6577 5f6e 6f64 655f 7661 6c5f 6461 7461  ew_node_val_data
+00001dd0: 2c20 6e65 775f 6e65 775f 6e6f 6465 5f74  , new_new_node_t
+00001de0: 6573 745f 6461 7461 2c20 756e 7365 656e  est_data, unseen
+00001df0: 5f6e 6f64 6573 5f6e 756d 203d 2064 6174  _nodes_num = dat
+00001e00: 612e 6c6f 6164 2829 0a60 6060 0a0a 2323  a.load().```..##
+00001e10: 2320 4564 6765 5361 6d70 6c65 720a 4265  # EdgeSampler.Be
+00001e20: 6e63 6854 656d 7020 7072 6f76 6964 6573  nchTemp provides
+00001e30: 2074 6865 2075 6e69 6669 6564 0a6e 6567   the unified.neg
+00001e40: 6174 6976 6520 6564 6765 2073 616d 706c  ative edge sampl
+00001e50: 6572 2077 6974 6820 2a2a 7365 6564 2a2a  er with **seed**
+00001e60: 2066 6f72 204c 696e 6b20 5072 6564 6963   for Link Predic
+00001e70: 7469 6f6e 2074 6173 6b20 746f 2020 7361  tion task to  sa
+00001e80: 6d70 6c65 2061 6e20 6571 7561 6c20 616d  mple an equal am
+00001e90: 6f75 6e74 206f 6620 6e65 6761 7469 7665  ount of negative
+00001ea0: 7320 746f 2074 6865 2070 6f73 6974 6976  s to the positiv
+00001eb0: 6520 696e 7465 7261 6374 696f 6e73 2e0a  e interactions..
+00001ec0: 0a43 6c61 7373 3a0a 0a2a 2a52 616e 6445  .Class:..**RandE
+00001ed0: 6467 6553 616d 706c 6572 2873 7263 5f6c  dgeSampler(src_l
+00001ee0: 6973 7420 3a20 6e75 6d70 792e 6e64 6172  ist : numpy.ndar
+00001ef0: 7261 792c 2064 7374 5f6c 6973 7420 3a20  ray, dst_list : 
+00001f00: 6e75 6d70 792e 6e64 6172 7261 792c 2073  numpy.ndarray, s
+00001f10: 6565 6420 3a20 696e 7420 3d4e 6f6e 6529  eed : int =None)
+00001f20: 2a2a 0a0a 5061 7261 6d65 7465 7273 3a0a  **..Parameters:.
+00001f30: 2d20 2a2a 7372 635f 6c69 7374 203a 206e  - **src_list : n
+00001f40: 756d 7079 2e6e 6461 7272 6179 2a2a 202d  umpy.ndarray** -
+00001f50: 2074 6865 206c 6973 7420 6f66 2073 6f75   the list of sou
+00001f60: 7263 6520 6e6f 6465 732e 0a2d 202a 2a64  rce nodes..- **d
+00001f70: 7374 5f6c 6973 7420 3a20 6e75 6d70 792e  st_list : numpy.
+00001f80: 6e64 6172 7261 792a 2a20 2d20 7468 6520  ndarray** - the 
+00001f90: 6c69 7374 206f 6620 6465 7374 696e 6174  list of destinat
+00001fa0: 696f 6e20 6e6f 6465 732e 0a2d 202a 2a73  ion nodes..- **s
+00001fb0: 6565 6420 3a20 6e75 6d70 792e 6e64 6172  eed : numpy.ndar
+00001fc0: 7261 792a 2a20 2d20 7365 6564 206f 6620  ray** - seed of 
+00001fd0: 7261 6e64 6f6d 2e0a 0a52 6574 7572 6e73  random...Returns
+00001fe0: 3a20 0a0a 2d20 2a2a 6265 6e63 6874 656d  : ..- **benchtem
+00001ff0: 702e 5261 6e64 4564 6765 5361 6d70 6c65  p.RandEdgeSample
+00002000: 722a 2a0a 0a45 7861 6d70 6c65 3a0a 0a60  r**..Example:..`
+00002010: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+00002020: 6265 6e63 6874 656d 7020 6173 2062 740a  benchtemp as bt.
+00002030: 0a23 2046 6f72 2065 7861 6d70 6c65 2c20  .# For example, 
+00002040: 6966 2079 6f75 2061 7265 2074 7261 696e  if you are train
+00002050: 696e 6720 2c20 796f 7520 7368 6f75 6c64  ing , you should
+00002060: 2063 7265 6174 6520 6120 7472 6169 6e69   create a traini
+00002070: 6e67 2020 5261 6e64 4564 6765 5361 6d70  ng  RandEdgeSamp
+00002080: 6c65 7220 6261 7365 6420 6f6e 2074 6865  ler based on the
+00002090: 2074 7261 696e 696e 6720 6461 7461 7365   training datase
+000020a0: 742e 0a74 7261 696e 5f72 616e 645f 7361  t..train_rand_sa
+000020b0: 6d70 6c65 7220 3d20 6274 2e6c 702e 5261  mpler = bt.lp.Ra
+000020c0: 6e64 4564 6765 5361 6d70 6c65 7228 7472  ndEdgeSampler(tr
+000020d0: 6169 6e5f 6461 7461 2e73 6f75 7263 6573  ain_data.sources
+000020e0: 2c20 7472 6169 6e5f 6461 7461 2e64 6573  , train_data.des
+000020f0: 7469 6e61 7469 6f6e 7329 0a0a 2e2e 2e0a  tinations)......
+00002100: 666f 7220 6570 6f63 6820 696e 2072 616e  for epoch in ran
+00002110: 6765 2861 7267 732e 6570 6f63 6873 293a  ge(args.epochs):
+00002120: 0a20 2020 202e 2e2e 0a20 2020 2023 2073  .    ....    # s
+00002130: 616d 706c 6520 616e 2065 7175 616c 2061  ample an equal a
+00002140: 6d6f 756e 7420 6f66 206e 6567 6174 6976  mount of negativ
+00002150: 6573 2074 6f20 7468 6520 706f 7369 7469  es to the positi
+00002160: 7665 2069 6e74 6572 6163 7469 6f6e 732e  ve interactions.
+00002170: 0a20 2020 205f 2c20 6e65 6761 7469 7665  .    _, negative
+00002180: 735f 6261 7463 6820 3d20 7472 6169 6e5f  s_batch = train_
+00002190: 7261 6e64 5f73 616d 706c 6572 2e73 616d  rand_sampler.sam
+000021a0: 706c 6528 7369 7a65 290a 2020 2020 2e2e  ple(size).    ..
+000021b0: 2e0a 2e2e 2e0a 6060 600a 2323 2320 2832  ......```.### (2
+000021c0: 2920 4e6f 6465 2043 6c61 7373 6966 6963  ) Node Classific
+000021d0: 6174 696f 6e20 7461 736b 0a46 756e 6374  ation task.Funct
+000021e0: 696f 6e3a 0a0a 0a0a 2a2a 6265 6e63 6874  ion:....**bencht
+000021f0: 656d 702e 6e63 2e72 6561 6465 7273 2e67  emp.nc.readers.g
+00002200: 6574 5f64 6174 615f 6e6f 6465 5f63 6c61  et_data_node_cla
+00002210: 7373 6966 6963 6174 696f 6e28 2864 6174  ssification((dat
+00002220: 6173 6574 5f6e 616d 6520 3a20 7374 722c  aset_name : str,
+00002230: 2075 7365 5f76 616c 6964 6174 696f 6e20   use_validation 
+00002240: 3a20 626f 6f6c 3d46 616c 7365 2929 2a2a  : bool=False))**
+00002250: 200a 0a50 6172 616d 6574 6572 733a 0a2d   ..Parameters:.-
+00002260: 2064 6174 6173 6574 5f6e 616d 6520 3a20   dataset_name : 
+00002270: 7374 7220 2d20 5468 6520 6e61 6d65 206f  str - The name o
+00002280: 6620 7468 6520 6461 7461 7365 742e 2054  f the dataset. T
+00002290: 6865 2064 6174 6173 6574 2066 696c 6520  he dataset file 
+000022a0: 282e 6373 7620 6669 6c65 206f 6620 7468  (.csv file of th
+000022b0: 6520 5465 6d70 6f72 616c 2047 7261 7068  e Temporal Graph
+000022c0: 2c20 2e6e 7079 2066 696c 6520 6f66 2074  , .npy file of t
+000022d0: 6865 206e 6f64 6520 6665 6174 7572 6573  he node features
+000022e0: 2061 6e64 202e 6e70 7920 6669 6c65 206f   and .npy file o
+000022f0: 6620 7468 6520 6564 6765 2066 6561 7475  f the edge featu
+00002300: 7265 7329 2073 686f 756c 6420 6265 2069  res) should be i
+00002310: 6e20 222e 2f64 6174 6122 2064 6972 6563  n "./data" direc
+00002320: 746f 7279 2e0a 2d20 7573 655f 7661 6c69  tory..- use_vali
+00002330: 6461 7469 6f6e 203a 2062 6f6f 6c20 2d20  dation : bool - 
+00002340: 5768 6574 6865 7220 7573 6520 7661 6c69  Whether use vali
+00002350: 6461 7469 6f6e 2064 6174 6173 6574 206f  dation dataset o
+00002360: 7220 6e6f 742e 0a0a 5265 7475 726e 733a  r not...Returns:
+00002370: 0a2d 202a 2a6e 6f64 655f 6665 6174 7572  .- **node_featur
+00002380: 6573 203a 206e 756d 7079 2e6e 6461 7272  es : numpy.ndarr
+00002390: 6179 2a2a 202d 2041 7272 6179 206f 6620  ay** - Array of 
+000023a0: 7468 6520 4e6f 6465 2046 6561 7475 7265  the Node Feature
+000023b0: 7320 6f66 2074 6865 2054 656d 706f 7261  s of the Tempora
+000023c0: 6c20 4772 6170 682e 200a 2d20 2a2a 6564  l Graph. .- **ed
+000023d0: 6765 5f66 6561 7475 7265 7320 3a20 6e75  ge_features : nu
+000023e0: 6d70 792e 6e64 6172 7261 792a 2a20 2d20  mpy.ndarray** - 
+000023f0: 4172 7261 7920 6f66 2074 6865 2045 6467  Array of the Edg
+00002400: 6520 4665 6174 7572 6573 206f 6620 7468  e Features of th
+00002410: 6520 5465 6d70 6f72 616c 2047 7261 7068  e Temporal Graph
+00002420: 2e0a 2d20 2a2a 6675 6c6c 5f64 6174 6120  ..- **full_data 
+00002430: 3a20 6265 6e63 6874 656d 702e 4461 7461  : benchtemp.Data
+00002440: 2a2a 202d 2046 756c 6c20 5465 6d70 6f72  ** - Full Tempor
+00002450: 616c 2047 7261 7068 2064 6174 6173 6574  al Graph dataset
+00002460: 2066 6f72 204e 6f64 6520 436c 6173 7369   for Node Classi
+00002470: 6669 6361 7469 6f6e 2074 6173 6b2e 200a  fication task. .
+00002480: 2d20 2a2a 7472 6169 6e5f 6461 7461 203a  - **train_data :
+00002490: 2062 656e 6368 7465 6d70 2e44 6174 612a   benchtemp.Data*
+000024a0: 2a20 2d20 5468 6520 7472 6169 6e69 6e67  * - The training
+000024b0: 2054 656d 706f 7261 6c20 4772 6170 6820   Temporal Graph 
+000024c0: 6461 7461 7365 7420 666f 7220 4e6f 6465  dataset for Node
+000024d0: 2043 6c61 7373 6966 6963 6174 696f 6e20   Classification 
+000024e0: 7461 736b 2e20 0a2d 202a 2a76 616c 5f64  task. .- **val_d
+000024f0: 6174 6120 3a20 6265 6e63 6874 656d 702e  ata : benchtemp.
+00002500: 4461 7461 2a2a 202d 2054 6865 2076 616c  Data** - The val
+00002510: 6964 6174 696f 6e20 5465 6d70 6f72 616c  idation Temporal
+00002520: 2047 7261 7068 2064 6174 6173 6574 2066   Graph dataset f
+00002530: 6f72 204e 6f64 6520 436c 6173 7369 6669  or Node Classifi
+00002540: 6361 7469 6f6e 2074 6173 6b2e 0a2d 202a  cation task..- *
+00002550: 2a74 6573 745f 6461 7461 203a 2062 656e  *test_data : ben
+00002560: 6368 7465 6d70 2e44 6174 612a 2a20 202d  chtemp.Data**  -
+00002570: 2054 6865 2074 6573 7420 5465 6d70 6f72   The test Tempor
+00002580: 616c 2047 7261 7068 2064 6174 6173 6574  al Graph dataset
+00002590: 2066 6f72 204e 6f64 6520 436c 6173 7369   for Node Classi
+000025a0: 6669 6361 7469 6f6e 2074 6173 6b2e 0a0a  fication task...
+000025b0: 0a0a 2323 2320 4561 726c 7953 746f 704d  ..### EarlyStopM
+000025c0: 6f6e 6974 6f72 0a43 6c61 7373 3a0a 0a2a  onitor.Class:..*
+000025d0: 2a45 6172 6c79 5374 6f70 4d6f 6e69 746f  *EarlyStopMonito
+000025e0: 7228 6d61 785f 726f 756e 643d 332c 2068  r(max_round=3, h
+000025f0: 6967 6865 725f 6265 7474 6572 3d54 7275  igher_better=Tru
+00002600: 652c 2074 6f6c 6572 616e 6365 3d31 652d  e, tolerance=1e-
+00002610: 3130 292a 2a0a 0a50 6172 616d 6574 6572  10)**..Parameter
+00002620: 733a 0a2d 202a 2a6d 6178 5f72 6f75 6e64  s:.- **max_round
+00002630: 203a 2069 6e74 2a2a 202d 2074 6865 206d   : int** - the m
+00002640: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+00002650: 2072 6f75 6e64 7320 6f66 2045 6172 6c79   rounds of Early
+00002660: 5374 6f70 4d6f 6e69 746f 722e 0a2d 202a  StopMonitor..- *
+00002670: 2a68 6967 6865 725f 6265 7474 6572 203a  *higher_better :
+00002680: 2062 6f6f 6c2a 2a20 2d20 6265 7474 6572   bool** - better
+00002690: 2074 6865 2070 6572 666f 726d 616e 6365   the performance
+000026a0: 2e0a 2d20 2a2a 746f 6c65 7261 6e63 6520  ..- **tolerance 
+000026b0: 3a20 666c 6f61 742a 2a20 2d20 7468 6520  : float** - the 
+000026c0: 746f 6c65 7261 6e63 6520 6f66 2074 6865  tolerance of the
+000026d0: 2045 6172 6c79 5374 6f70 4d6f 6e69 746f   EarlyStopMonito
+000026e0: 722e 0a0a 5265 7475 726e 733a 0a2d 202a  r...Returns:.- *
+000026f0: 2a62 656e 6368 7465 6d70 2e45 6172 6c79  *benchtemp.Early
+00002700: 5374 6f70 4d6f 6e69 746f 722a 2a0a 0a45  StopMonitor**..E
+00002710: 7861 6d70 6c65 3a0a 6060 6070 7974 686f  xample:.```pytho
+00002720: 6e0a 696d 706f 7274 2062 656e 6368 7465  n.import benchte
+00002730: 6d70 2061 7320 6274 0a0a 2e2e 2e0a 6561  mp as bt......ea
+00002740: 726c 795f 7374 6f70 7065 7220 3d20 6274  rly_stopper = bt
+00002750: 2e45 6172 6c79 5374 6f70 4d6f 6e69 746f  .EarlyStopMonito
+00002760: 7228 6d61 785f 726f 756e 643d 6172 6773  r(max_round=args
+00002770: 2e70 6174 6965 6e63 6529 0a66 6f72 2065  .patience).for e
+00002780: 706f 6368 2069 6e20 7261 6e67 6528 6172  poch in range(ar
+00002790: 6773 2e65 706f 6368 7329 3a0a 2020 2020  gs.epochs):.    
+000027a0: 2e2e 2e0a 2020 2020 7661 6c5f 6170 203d  ....    val_ap =
+000027b0: 206d 6f64 656c 2876 616c 5f64 6174 6173   model(val_datas
+000027c0: 6574 7329 0a20 2020 2069 6620 6561 726c  ets).    if earl
+000027d0: 795f 7374 6f70 7065 722e 6561 726c 795f  y_stopper.early_
+000027e0: 7374 6f70 5f63 6865 636b 2876 616c 5f61  stop_check(val_a
+000027f0: 7029 3a0a 2020 2020 2020 2020 6272 6561  p):.        brea
+00002800: 6b0a 2020 2020 2e2e 2e0a 2e2e 2e0a 6060  k.    ........``
+00002810: 600a 0a23 2323 2045 7661 6c75 6174 6f72  `..### Evaluator
+00002820: 0a0a 2a2a 4c69 6e6b 2050 7265 6469 6374  ..**Link Predict
+00002830: 696f 6e2a 2a20 4576 616c 7561 7469 6f6e  ion** Evaluation
+00002840: 204d 6574 7269 6373 2020 6172 6520 2a2a   Metrics  are **
+00002850: 4172 6561 2055 6e64 6572 2074 6865 2052  Area Under the R
+00002860: 6563 6569 7665 7220 4f70 6572 6174 696e  eceiver Operatin
+00002870: 6720 4368 6172 6163 7465 7269 7374 6963  g Characteristic
+00002880: 2043 7572 7665 2028 524f 4320 4155 4329   Curve (ROC AUC)
+00002890: 2a2a 2061 6e64 202a 2a61 7665 7261 6765  ** and **average
+000028a0: 2070 7265 6369 7369 6f6e 2028 4150 292a   precision (AP)*
+000028b0: 2a0a 0a2a 2a4e 6f64 6520 436c 6173 7369  *..**Node Classi
+000028c0: 6669 6361 7469 6f6e 2a2a 2045 7661 6c75  fication** Evalu
+000028d0: 6174 696f 6e20 4d65 7472 6963 2069 7320  ation Metric is 
+000028e0: 2a2a 4172 6561 2055 6e64 6572 2074 6865  **Area Under the
+000028f0: 2052 6563 6569 7665 7220 4f70 6572 6174   Receiver Operat
+00002900: 696e 6720 4368 6172 6163 7465 7269 7374  ing Characterist
+00002910: 6963 2043 7572 7665 2028 524f 4320 4155  ic Curve (ROC AU
+00002920: 4329 2a2a 0a0a 436c 6173 733a 200a 0a2a  C)**..Class: ..*
+00002930: 2a45 7661 6c75 6174 6f72 2874 6173 6b5f  *Evaluator(task_
+00002940: 6e61 6d65 3a20 7374 7220 3d20 224c 5022  name: str = "LP"
+00002950: 292a 2a0a 0a50 6172 616d 6574 6572 733a  )**..Parameters:
+00002960: 0a2d 2074 6173 6b5f 6e61 6d65 203a 2073  .- task_name : s
+00002970: 7472 2020 2d20 7468 6520 6e61 6d65 206f  tr  - the name o
+00002980: 6620 7468 6520 7461 736b 2c20 6368 6f69  f the task, choi
+00002990: 6365 2069 6e20 2a2a 5b22 4c50 222c 2022  ce in **["LP", "
+000029a0: 4e43 225d 2a2a 2e0a 0a52 6574 7572 6e73  NC"]**...Returns
+000029b0: 3a0a 2d20 2a2a 6265 6e63 6874 656d 702e  :.- **benchtemp.
+000029c0: 4576 616c 7561 746f 722a 2a0a 0a45 7861  Evaluator**..Exa
+000029d0: 6d70 6c65 3a0a 0a60 6060 7079 7468 6f6e  mple:..```python
+000029e0: 0a69 6d70 6f72 7420 6265 6e63 6874 656d  .import benchtem
+000029f0: 7020 6173 2062 740a 0a23 2046 6f72 2065  p as bt..# For e
+00002a00: 7861 6d70 6c65 2c20 4c69 6e6b 2070 7265  xample, Link pre
+00002a10: 6469 6374 696f 6e20 7461 736b 2e20 4576  diction task. Ev
+00002a20: 616c 7561 7469 6f6e 204d 6574 7269 6373  aluation Metrics
+00002a30: 3a20 4155 432c 2041 502e 0a65 7661 6c75  : AUC, AP..evalu
+00002a40: 6174 6f72 203d 2062 742e 4576 616c 7561  ator = bt.Evalua
+00002a50: 746f 7228 224c 5022 290a 0a2e 2e2e 0a23  tor("LP")......#
+00002a60: 2074 6573 7420 6461 7461 0a70 7265 645f   test data.pred_
+00002a70: 7363 6f72 6520 3d20 6d6f 6465 6c28 7465  score = model(te
+00002a80: 7374 5f64 6174 6129 0a74 6573 745f 6175  st_data).test_au
+00002a90: 632c 2074 6573 745f 6170 203d 2065 7661  c, test_ap = eva
+00002aa0: 6c75 6174 6f72 2e65 7661 6c28 7072 6564  luator.eval(pred
+00002ab0: 5f73 636f 7265 2c20 7472 7565 5f6c 6162  _score, true_lab
+00002ac0: 656c 290a 2e2e 2e0a 6060 600a 0a60 6060  el).....```..```
+00002ad0: 7079 7468 6f6e 0a69 6d70 6f72 7420 6265  python.import be
+00002ae0: 6e63 6874 656d 7020 6173 2062 740a 0a23  nchtemp as bt..#
+00002af0: 2046 6f72 2065 7861 6d70 6c65 2c20 4e6f   For example, No
+00002b00: 6465 2043 6c61 7373 6966 6963 6174 696f  de Classificatio
+00002b10: 6e20 7461 736b 2e20 4576 616c 7561 7469  n task. Evaluati
+00002b20: 6f6e 204d 6574 7269 6373 3a20 4155 432e  on Metrics: AUC.
+00002b30: 0a65 7661 6c75 6174 6f72 203d 2062 742e  .evaluator = bt.
+00002b40: 4576 616c 7561 746f 7228 224e 4322 290a  Evaluator("NC").
+00002b50: 0a2e 2e2e 0a23 2074 6573 7420 6461 7461  .....# test data
+00002b60: 0a70 7265 645f 7363 6f72 6520 3d20 6d6f  .pred_score = mo
+00002b70: 6465 6c28 7465 7374 5f64 6174 6129 0a74  del(test_data).t
+00002b80: 6573 745f 6175 6320 3d20 6576 616c 7561  est_auc = evalua
+00002b90: 746f 722e 6576 616c 2870 7265 645f 7363  tor.eval(pred_sc
+00002ba0: 6f72 652c 2074 7275 655f 6c61 6265 6c29  ore, true_label)
+00002bb0: 0a2e 2e2e 0a60 6060 0a0a 2323 2043 616c  .....```..## Cal
+00002bc0: 6c20 666f 7220 436f 6e74 7269 6275 7469  l for Contributi
+00002bd0: 6f6e 730a 0a2a 2a42 656e 6368 5465 6d70  ons..**BenchTemp
+00002be0: 2a2a 2070 726f 6a65 6374 2069 7320 6c6f  ** project is lo
+00002bf0: 6f6b 696e 6720 666f 7220 636f 6e74 7269  oking for contri
+00002c00: 6275 746f 7273 2077 6974 6820 0a65 7870  butors with .exp
+00002c10: 6572 7469 7365 2061 6e64 2065 6e74 6875  ertise and enthu
+00002c20: 7369 6173 6d21 2049 6620 796f 7520 6861  siasm! If you ha
+00002c30: 7665 2061 2064 6573 6972 6520 746f 2063  ve a desire to c
+00002c40: 6f6e 7472 6962 7574 6520 746f 202a 2a42  ontribute to **B
+00002c50: 656e 6368 5465 6d70 2a2a 2c20 0a70 6c65  enchTemp**, .ple
+00002c60: 6173 6520 636f 6e74 6163 7420 5b42 656e  ase contact [Ben
+00002c70: 6368 5465 6d70 2074 6561 6d5d 286d 6169  chTemp team](mai
+00002c80: 6c74 6f3a 6a6f 6e6e 7968 7561 6e67 686e  lto:jonnyhuanghn
+00002c90: 7540 676d 6169 6c2e 636f 6d29 2e0a 0a5c  u@gmail.com)...\
+00002ca0: 6974 656d 2057 6520 7265 6c65 6173 6520  item We release 
+00002cb0: 5c73 7973 2c20 6120 6765 6e65 7261 6c20  \sys, a general 
+00002cc0: 6265 6e63 686d 6172 6b20 6c69 6272 6172  benchmark librar
+00002cd0: 7920 666f 7220 6576 616c 7561 7469 6e67  y for evaluating
+00002ce0: 2074 656d 706f 7261 6c20 6772 6170 6820   temporal graph 
+00002cf0: 6d6f 6465 6c73 3b0a 0a5c 6974 656d 2057  models;..\item W
+00002d00: 6520 7072 6f76 6964 6573 2075 6e69 6669  e provides unifi
+00002d10: 6564 2062 656e 636b 6d61 726b 2074 656d  ed benckmark tem
+00002d20: 706f 7261 6c20 6772 6170 6820 6461 7461  poral graph data
+00002d30: 7365 7473 2070 726f 6365 7373 6564 2062  sets processed b
+00002d40: 7920 5c73 7973 3b0a 0a5c 6974 656d 2057  y \sys;..\item W
+00002d50: 6520 6265 6e63 686d 6172 6b20 6578 6973  e benchmark exis
+00002d60: 7469 6e67 2074 656d 706f 7261 6c20 6772  ting temporal gr
+00002d70: 6170 6820 6d6f 6465 6c73 2062 6173 6564  aph models based
+00002d80: 206f 6e20 5c73 7973 2020 666f 7220 726f   on \sys  for ro
+00002d90: 6275 7374 2064 6576 656c 6f70 6d65 6e74  bust development
+00002da0: 7320 616e 6420 616e 616c 7973 6973 2074  s and analysis t
+00002db0: 6865 2070 6572 666f 726d 616e 6365 206f  he performance o
+00002dc0: 6620 6d6f 6465 6c73 2069 6e20 6465 7461  f models in deta
+00002dd0: 696c 3b0a 0a5c 6974 656d 2057 6520 7265  il;..\item We re
+00002de0: 6c73 6564 2074 6865 206c 6561 6465 7262  lsed the leaderb
+00002df0: 6f61 7264 7320 666f 7220 7465 6d70 6f72  oards for tempor
+00002e00: 616c 2067 7261 7068 206d 6f64 656c 732e  al graph models.
+00002e10: 0a0a                                     ..
```

