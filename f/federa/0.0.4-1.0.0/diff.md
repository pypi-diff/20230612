# Comparing `tmp/federa-0.0.4.tar.gz` & `tmp/federa-1.0.0.tar.gz`

## Comparing `federa-0.0.4.tar` & `federa-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 federa-0.0.4/federa/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.4/federa/client/__init__.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 federa-0.0.4/federa/client/start_client.py
--rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 federa-0.0.4/federa/client/src/ClientConnection_pb2.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 federa-0.0.4/federa/client/src/ClientConnection_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.4/federa/client/src/__init__.py
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 federa-0.0.4/federa/client/src/client.py
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 federa-0.0.4/federa/client/src/client_lib.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 federa-0.0.4/federa/client/src/data_utils.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 federa-0.0.4/federa/client/src/distribution.py
--rw-r--r--   0        0        0     5096 2020-02-02 00:00:00.000000 federa-0.0.4/federa/client/src/get_data.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 federa-0.0.4/federa/client/src/net.py
--rw-r--r--   0        0        0    15264 2020-02-02 00:00:00.000000 federa-0.0.4/federa/client/src/net_lib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/__init__.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/start_server.py
--rw-r--r--   0        0        0    16361 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/ClientConnection_pb2.py
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/ClientConnection_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/__init__.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/client_connection_servicer.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/client_manager.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/client_wrapper.py
--rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/server.py
--rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/server_lib.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/verification.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/algorithms/fedadagrad.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/algorithms/fedadam.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/algorithms/fedavg.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/algorithms/fedavgm.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/algorithms/feddyn.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/algorithms/fedyogi.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/algorithms/mime.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/algorithms/mimelite.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/algorithms/scaffold.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/server_evaluate/__init__.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 federa-0.0.4/federa/server/src/server_evaluate/eval_lib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 federa-0.0.4/LICENSE
--rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 federa-0.0.4/README.md
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 federa-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 federa-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 federa-1.0.0/federa/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-1.0.0/federa/client/__init__.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 federa-1.0.0/federa/client/start_client.py
+-rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 federa-1.0.0/federa/client/src/ClientConnection_pb2.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 federa-1.0.0/federa/client/src/ClientConnection_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-1.0.0/federa/client/src/__init__.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 federa-1.0.0/federa/client/src/client.py
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 federa-1.0.0/federa/client/src/client_lib.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 federa-1.0.0/federa/client/src/data_utils.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 federa-1.0.0/federa/client/src/distribution.py
+-rw-r--r--   0        0        0     5096 2020-02-02 00:00:00.000000 federa-1.0.0/federa/client/src/get_data.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 federa-1.0.0/federa/client/src/net.py
+-rw-r--r--   0        0        0    15264 2020-02-02 00:00:00.000000 federa-1.0.0/federa/client/src/net_lib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/__init__.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/start_server.py
+-rw-r--r--   0        0        0    16361 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/ClientConnection_pb2.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/ClientConnection_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/__init__.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/client_connection_servicer.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/client_manager.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/client_wrapper.py
+-rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/server.py
+-rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/server_lib.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/verification.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/algorithms/fedadagrad.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/algorithms/fedadam.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/algorithms/fedavg.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/algorithms/fedavgm.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/algorithms/feddyn.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/algorithms/fedyogi.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/algorithms/mime.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/algorithms/mimelite.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/algorithms/scaffold.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/server_evaluate/__init__.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 federa-1.0.0/federa/server/src/server_evaluate/eval_lib.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 federa-1.0.0/federa/tests/minitest.json
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 federa-1.0.0/federa/tests/minitest.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 federa-1.0.0/federa/tests/misc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 federa-1.0.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 federa-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 federa-1.0.0/README.md
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 federa-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 federa-1.0.0/PKG-INFO
```

### Comparing `federa-0.0.4/federa/client/start_client.py` & `federa-1.0.0/federa/client/start_client.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/client/src/ClientConnection_pb2.py` & `federa-1.0.0/federa/client/src/ClientConnection_pb2.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/client/src/ClientConnection_pb2_grpc.py` & `federa-1.0.0/federa/client/src/ClientConnection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/client/src/client.py` & `federa-1.0.0/federa/client/src/client.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/client/src/client_lib.py` & `federa-1.0.0/federa/client/src/client_lib.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/client/src/data_utils.py` & `federa-1.0.0/federa/client/src/data_utils.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/client/src/distribution.py` & `federa-1.0.0/federa/client/src/distribution.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/client/src/get_data.py` & `federa-1.0.0/federa/client/src/get_data.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/client/src/net.py` & `federa-1.0.0/federa/client/src/net.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,35 +35,27 @@
         if config['dataset'] in ['MNIST', 'FashionMNIST', 'CUSTOM']:
             net = LeNet(in_channels=1, num_classes=10)
         elif config['dataset'] == 'CIFAR10':
             net = LeNet(in_channels=3, num_classes=10)
         else:
             net = LeNet(in_channels=3, num_classes=100)
     if config["net"] == 'resnet18':
-        if config['dataset'] in ['MNIST', 'FashionMNIST']:
-            net = models.resnet18(num_classes=10)
-        elif config['dataset'] == 'CIFAR10':
+        if config['dataset'] == 'CIFAR10':
             net = models.resnet18(num_classes=10)
         else:
             net = models.resnet18(num_classes=100)
     if config["net"] == 'resnet50':
-        if config['dataset'] in ['MNIST', 'FashionMNIST']:
-            net = models.resnet50(num_classes=10)
-        elif config['dataset'] == 'CIFAR10':
+        if config['dataset'] == 'CIFAR10':
             net = models.resnet50(num_classes=10)
         else:
             net = models.resnet50(num_classes=100)
     if config["net"] == 'vgg16':
-        if config['dataset'] in ['MNIST', 'FashionMNIST']:
-            net = models.vgg16(num_classes=10)
-        elif config['dataset'] == 'CIFAR10':
+        if config['dataset'] == 'CIFAR10':
             net = models.vgg16(num_classes=10)
         else:
             net = models.vgg16(num_classes=100)
     if config['net'] == 'AlexNet':
-        if config['dataset'] in ['MNIST', 'FashionMNIST']:
-            net = models.alexnet(num_classes=10)
-        elif config['dataset'] == 'CIFAR10':
+        if config['dataset'] == 'CIFAR10':
             net = models.alexnet(num_classes=10)
         else:
             net = models.alexnet(num_classes=100)
     return net
```

### Comparing `federa-0.0.4/federa/client/src/net_lib.py` & `federa-1.0.0/federa/client/src/net_lib.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/start_server.py` & `federa-1.0.0/federa/server/start_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                      help = '''Minimum score clients must have in a verification round,
                      .[0,1]''')
 parser.add_argument('--timeout', type = int, default=None,
                      help= 'Time limit for training. Specified in seconds')
 parser.add_argument('--resize_size', type = int, default = 32, help= 'resize dimension')
 parser.add_argument('--batch_size', type = int, default = 32, help= 'batch size')
 parser.add_argument('--net', type = str, default = 'LeNet', help= 'client network')
-parser.add_argument('--dataset', type = str, default= 'FashionMNIST',
+parser.add_argument('--dataset', type = str, default= 'MNIST',
                      help= 'datsset.Use CUSTOME for local dataset')
 parser.add_argument('--niid', type = int, default= 1, help= 'value should be [1, 5]')
 parser.add_argument('--carbon', type = int, default= 0,
                      help= '1 enable carbon emission at client')
 parser.add_argument('--encryption', type = int, default= 0, help= '1 enables ssl encryption')
 parser.add_argument('--server_key', type = str, default= 'server-key.pem', help= 'path to server key')
 parser.add_argument('--server_cert', type = str, default= 'server.pem', help= 'path to server certificate')
```

### Comparing `federa-0.0.4/federa/server/src/ClientConnection_pb2.py` & `federa-1.0.0/federa/server/src/ClientConnection_pb2.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/ClientConnection_pb2_grpc.py` & `federa-1.0.0/federa/server/src/ClientConnection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/client_connection_servicer.py` & `federa-1.0.0/federa/server/src/client_connection_servicer.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/client_manager.py` & `federa-1.0.0/federa/server/src/client_manager.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/client_wrapper.py` & `federa-1.0.0/federa/server/src/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/server.py` & `federa-1.0.0/federa/server/src/server.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/server_lib.py` & `federa-1.0.0/federa/server/src/server_lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,38 +124,30 @@
         if config['dataset'] in ['MNIST', 'FashionMNIST', 'CUSTOM']:
             net = LeNet(in_channels=1, num_classes=10)
         elif config['dataset'] == 'CIFAR10':
             net = LeNet(in_channels=3, num_classes=10)
         else:
             net = LeNet(in_channels=3, num_classes=100)
     if config["net"] == 'resnet18':
-        if config['dataset'] in ['MNIST', 'FashionMNIST']:
-            net = models.resnet18(num_classes=10)
-        elif config['dataset'] == 'CIFAR10':
+        if config['dataset'] == 'CIFAR10':
             net = models.resnet18(num_classes=10)
         else:
             net = models.resnet18(num_classes=100)
     if config["net"] == 'resnet50':
-        if config['dataset'] in ['MNIST', 'FashionMNIST']:
-            net = models.resnet50(num_classes=10)
-        elif config['dataset'] == 'CIFAR10':
+        if config['dataset'] == 'CIFAR10':
             net = models.resnet50(num_classes=10)
         else:
             net = models.resnet50(num_classes=100)
     if config["net"] == 'vgg16':
-        if config['dataset'] in ['MNIST', 'FashionMNIST']:
-            net = models.vgg16(num_classes=10)
-        elif config['dataset'] == 'CIFAR10':
+        if config['dataset'] == 'CIFAR10':
             net = models.vgg16(num_classes=10)
         else:
             net = models.vgg16(num_classes=100)
     if config['net'] == 'AlexNet':
-        if config['dataset'] in ['MNIST', 'FashionMNIST']:
-            net = models.alexnet(num_classes=10)
-        elif config['dataset'] == 'CIFAR10':
+        if config['dataset'] == 'CIFAR10':
             net = models.alexnet(num_classes=10)
         else:
             net = models.alexnet(num_classes=100)
     return net
 
 def train_model(net, trainloader):
     criterion = torch.nn.CrossEntropyLoss()
```

### Comparing `federa-0.0.4/federa/server/src/verification.py` & `federa-1.0.0/federa/server/src/verification.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/algorithms/fedadagrad.py` & `federa-1.0.0/federa/server/src/algorithms/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/algorithms/fedadam.py` & `federa-1.0.0/federa/server/src/algorithms/fedadam.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/algorithms/fedavg.py` & `federa-1.0.0/federa/server/src/algorithms/fedavg.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/algorithms/fedavgm.py` & `federa-1.0.0/federa/server/src/algorithms/fedavgm.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/algorithms/feddyn.py` & `federa-1.0.0/federa/server/src/algorithms/feddyn.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/algorithms/fedyogi.py` & `federa-1.0.0/federa/server/src/algorithms/fedyogi.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/algorithms/mime.py` & `federa-1.0.0/federa/server/src/algorithms/mime.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/algorithms/mimelite.py` & `federa-1.0.0/federa/server/src/algorithms/mimelite.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/federa/server/src/algorithms/scaffold.py` & `federa-1.0.0/federa/server/src/algorithms/scaffold.py`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/LICENSE` & `federa-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `federa-0.0.4/README.md` & `federa-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -67,24 +67,25 @@
 | MNIST                  | 60,000                   | 10,000             | 10                 |
 | FashionMnist           | 60,000                   | 10,000             | 10                 |
 | CIFAR-10               | 50,000                   | 10,000             | 10                 |
 | CIFAR-100              | 50,000                   | 10,000             | 100                |
 
 ### Custom Dataset Support
 
-We also provide a simple way to add your own dataset to the framework. Look into [docs](https://federa.readthedocs.io/en/latest/tutorials/dataset.html#adding-support-for-new-datasets) for more details.
+We also provide a simple way to add your own dataset to the framework. The models employed in this framework were trained using a limited subset of the publicly accessible benchmark dataset MedMNIST v2 [(link)](https://medmnist.com/). We specifically selected four different medical image classes from this dataset, which include breast ultrasound (US), chest X-ray, retinal optical coherence tomography (OCT), and tissue microscopy. Each image within the dataset possesses dimensions of 28x28 pixels.
+For the framework's implementation, we utilized this custom dataset for both the side server and the client.   Look into [docs](https://federa.readthedocs.io/en/latest/tutorials/dataset.html#adding-support-for-new-datasets) for more details.
 
 ## Models Supported
 
 `FedERA` has support for the following Deep Learning models, which are loaded from `torchvision.models`:
 
-* LeNet
-* ResNet18
-* ResNet50
-* VGG16
+* LeNet-5
+* ResNet-18
+* ResNet-50
+* VGG-16
 * AlexNet
 
 ### Custom Model Support
 
 We also provide a simple way to add your own models to the framework. Look into [docs](https://federa.readthedocs.io/en/latest/tutorials/dataset.html#adding-support-for-new-datasets) for more details.
 
 
@@ -99,11 +100,11 @@
 
 <!-- Project Investigator: [Prof. ](https://scholar.google.com/citations?user=gF0H9nEAAAAJ&hl=ennjujbj) (abc@edu).
 
 For technical issues related to __**FedERA**__ development, please contact our development team through Github issues or email:
 
 - [Name Sirname](https://scholar.google.com/citations___): _____@gmail.com -->
 
-For technical issues related to __**FedERA**__ development, please contact our development team through Github issues or email.
+For technical issues related to __**FedERA**__ development, please contact our development team through Github issues or email (federa.team@gmail.com).
```

### Comparing `federa-0.0.4/pyproject.toml` & `federa-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "federa"
-version = "0.0.4"
+version = "1.0.0"
 authors = [
   { name="Anupam Borthakur", email="anupamborthakur@kgpian.iitkgp.ac.in" },
 ]
 description = "FedERA is a highly dynamic and customizable framework that can accommodate many use cases with flexibility by implementing several functionalities over different federated learning algorithms, and essentially creating a plug-and-play architecture to accommodate different use cases."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `federa-0.0.4/PKG-INFO` & `federa-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federa
-Version: 0.0.4
+Version: 1.0.0
 Summary: FedERA is a highly dynamic and customizable framework that can accommodate many use cases with flexibility by implementing several functionalities over different federated learning algorithms, and essentially creating a plug-and-play architecture to accommodate different use cases.
 Project-URL: Homepage, https://github.com/anupamkliv/FedERA
 Project-URL: Bug Tracker, https://github.com/anupamkliv/FedERA/issues
 Author-email: Anupam Borthakur <anupamborthakur@kgpian.iitkgp.ac.in>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -91,24 +91,25 @@
 | MNIST                  | 60,000                   | 10,000             | 10                 |
 | FashionMnist           | 60,000                   | 10,000             | 10                 |
 | CIFAR-10               | 50,000                   | 10,000             | 10                 |
 | CIFAR-100              | 50,000                   | 10,000             | 100                |
 
 ### Custom Dataset Support
 
-We also provide a simple way to add your own dataset to the framework. Look into [docs](https://federa.readthedocs.io/en/latest/tutorials/dataset.html#adding-support-for-new-datasets) for more details.
+We also provide a simple way to add your own dataset to the framework. The models employed in this framework were trained using a limited subset of the publicly accessible benchmark dataset MedMNIST v2 [(link)](https://medmnist.com/). We specifically selected four different medical image classes from this dataset, which include breast ultrasound (US), chest X-ray, retinal optical coherence tomography (OCT), and tissue microscopy. Each image within the dataset possesses dimensions of 28x28 pixels.
+For the framework's implementation, we utilized this custom dataset for both the side server and the client.   Look into [docs](https://federa.readthedocs.io/en/latest/tutorials/dataset.html#adding-support-for-new-datasets) for more details.
 
 ## Models Supported
 
 `FedERA` has support for the following Deep Learning models, which are loaded from `torchvision.models`:
 
-* LeNet
-* ResNet18
-* ResNet50
-* VGG16
+* LeNet-5
+* ResNet-18
+* ResNet-50
+* VGG-16
 * AlexNet
 
 ### Custom Model Support
 
 We also provide a simple way to add your own models to the framework. Look into [docs](https://federa.readthedocs.io/en/latest/tutorials/dataset.html#adding-support-for-new-datasets) for more details.
 
 
@@ -123,11 +124,11 @@
 
 <!-- Project Investigator: [Prof. ](https://scholar.google.com/citations?user=gF0H9nEAAAAJ&hl=ennjujbj) (abc@edu).
 
 For technical issues related to __**FedERA**__ development, please contact our development team through Github issues or email:
 
 - [Name Sirname](https://scholar.google.com/citations___): _____@gmail.com -->
 
-For technical issues related to __**FedERA**__ development, please contact our development team through Github issues or email.
+For technical issues related to __**FedERA**__ development, please contact our development team through Github issues or email (federa.team@gmail.com).
```

