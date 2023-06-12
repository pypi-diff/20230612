# Comparing `tmp/horovod-0.9.8.tar.gz` & `tmp/horovod-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/horovod-0.9.8.tar", last modified: Wed Oct 11 19:34:36 2017, max compression
+gzip compressed data, was "dist/horovod-0.9.9.tar", last modified: Thu Oct 12 00:35:16 2017, max compression
```

## Comparing `horovod-0.9.8.tar` & `horovod-0.9.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-11 19:34:36.000000 horovod-0.9.8/
-drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-11 19:34:36.000000 horovod-0.9.8/docs/
--rw-r--r--   0 asergeev   (501) staff       (20)     1680 2017-09-26 17:57:01.000000 horovod-0.9.8/docs/concepts.md
--rw-r--r--   0 asergeev   (501) staff       (20)     4835 2017-09-26 17:57:01.000000 horovod-0.9.8/docs/gpus.md
--rw-r--r--   0 asergeev   (501) staff       (20)     1013 2017-09-26 17:57:01.000000 horovod-0.9.8/docs/inference.md
--rw-r--r--   0 asergeev   (501) staff       (20)     1381 2017-09-26 17:57:01.000000 horovod-0.9.8/docs/tensor-fusion.md
--rw-r--r--   0 asergeev   (501) staff       (20)     2397 2017-09-26 17:57:01.000000 horovod-0.9.8/docs/timeline.md
--rw-r--r--   0 asergeev   (501) staff       (20)     8340 2017-09-26 17:57:01.000000 horovod-0.9.8/docs/troubleshooting.md
-drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-11 19:34:36.000000 horovod-0.9.8/horovod/
--rw-r--r--   0 asergeev   (501) staff       (20)        0 2017-08-10 01:37:50.000000 horovod-0.9.8/horovod/__init__.py
-drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-11 19:34:36.000000 horovod-0.9.8/horovod/tensorflow/
--rw-r--r--   0 asergeev   (501) staff       (20)     9432 2017-08-10 02:02:12.000000 horovod-0.9.8/horovod/tensorflow/__init__.py
--rw-r--r--   0 asergeev   (501) staff       (20)     1232 2017-08-10 01:37:50.000000 horovod-0.9.8/horovod/tensorflow/hash_vector.h
--rw-r--r--   0 asergeev   (501) staff       (20)     8537 2017-08-27 02:31:26.000000 horovod-0.9.8/horovod/tensorflow/mpi_message.cc
--rw-r--r--   0 asergeev   (501) staff       (20)     4730 2017-08-27 02:31:26.000000 horovod-0.9.8/horovod/tensorflow/mpi_message.h
--rw-r--r--   0 asergeev   (501) staff       (20)    71518 2017-10-05 00:23:20.000000 horovod-0.9.8/horovod/tensorflow/mpi_ops.cc
--rw-r--r--   0 asergeev   (501) staff       (20)     6435 2017-08-10 01:37:50.000000 horovod-0.9.8/horovod/tensorflow/mpi_ops.py
--rw-r--r--   0 asergeev   (501) staff       (20)    22250 2017-09-04 06:51:03.000000 horovod-0.9.8/horovod/tensorflow/mpi_ops_test.py
--rw-r--r--   0 asergeev   (501) staff       (20)     6901 2017-08-26 03:48:12.000000 horovod-0.9.8/horovod/tensorflow/timeline.cc
--rw-r--r--   0 asergeev   (501) staff       (20)     2990 2017-08-26 03:48:12.000000 horovod-0.9.8/horovod/tensorflow/timeline.h
-drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-11 19:34:36.000000 horovod-0.9.8/horovod/tensorflow/wire/
-drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-11 19:34:36.000000 horovod-0.9.8/horovod/tensorflow/wire/flatbuffers/
--rw-r--r--   0 asergeev   (501) staff       (20)    67819 2017-08-10 01:37:50.000000 horovod-0.9.8/horovod/tensorflow/wire/flatbuffers/flatbuffers.h
--rw-r--r--   0 asergeev   (501) staff       (20)    12222 2017-08-27 02:31:26.000000 horovod-0.9.8/horovod/tensorflow/wire/mpi_message_generated.h
-drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-11 19:34:36.000000 horovod-0.9.8/horovod.egg-info/
--rw-r--r--   0 asergeev   (501) staff       (20)        1 2017-10-11 19:34:36.000000 horovod-0.9.8/horovod.egg-info/dependency_links.txt
--rw-r--r--   0 asergeev   (501) staff       (20)        1 2017-08-10 05:27:45.000000 horovod-0.9.8/horovod.egg-info/not-zip-safe
--rw-r--r--   0 asergeev   (501) staff       (20)      471 2017-10-11 19:34:36.000000 horovod-0.9.8/horovod.egg-info/PKG-INFO
--rw-r--r--   0 asergeev   (501) staff       (20)      708 2017-10-11 19:34:36.000000 horovod-0.9.8/horovod.egg-info/SOURCES.txt
--rw-r--r--   0 asergeev   (501) staff       (20)        8 2017-10-11 19:34:36.000000 horovod-0.9.8/horovod.egg-info/top_level.txt
--rw-r--r--   0 asergeev   (501) staff       (20)    13232 2017-08-10 01:37:50.000000 horovod-0.9.8/LICENSE
--rw-r--r--   0 asergeev   (501) staff       (20)       50 2017-09-26 17:57:01.000000 horovod-0.9.8/MANIFEST.in
--rw-r--r--   0 asergeev   (501) staff       (20)      471 2017-10-11 19:34:36.000000 horovod-0.9.8/PKG-INFO
--rw-r--r--   0 asergeev   (501) staff       (20)     8915 2017-10-07 05:32:18.000000 horovod-0.9.8/README.md
--rw-r--r--   0 asergeev   (501) staff       (20)       38 2017-10-11 19:34:36.000000 horovod-0.9.8/setup.cfg
--rw-r--r--   0 asergeev   (501) staff       (20)    12971 2017-10-11 19:33:31.000000 horovod-0.9.8/setup.py
+drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-12 00:35:16.000000 horovod-0.9.9/
+drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-12 00:35:16.000000 horovod-0.9.9/docs/
+-rw-r--r--   0 asergeev   (501) staff       (20)     1680 2017-09-26 17:57:01.000000 horovod-0.9.9/docs/concepts.md
+-rw-r--r--   0 asergeev   (501) staff       (20)     4835 2017-09-26 17:57:01.000000 horovod-0.9.9/docs/gpus.md
+-rw-r--r--   0 asergeev   (501) staff       (20)     1013 2017-09-26 17:57:01.000000 horovod-0.9.9/docs/inference.md
+-rw-r--r--   0 asergeev   (501) staff       (20)     1381 2017-09-26 17:57:01.000000 horovod-0.9.9/docs/tensor-fusion.md
+-rw-r--r--   0 asergeev   (501) staff       (20)     2397 2017-09-26 17:57:01.000000 horovod-0.9.9/docs/timeline.md
+-rw-r--r--   0 asergeev   (501) staff       (20)     9607 2017-10-12 00:22:31.000000 horovod-0.9.9/docs/troubleshooting.md
+drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-12 00:35:16.000000 horovod-0.9.9/horovod/
+-rw-r--r--   0 asergeev   (501) staff       (20)        0 2017-08-10 01:37:50.000000 horovod-0.9.9/horovod/__init__.py
+drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-12 00:35:16.000000 horovod-0.9.9/horovod/tensorflow/
+-rw-r--r--   0 asergeev   (501) staff       (20)     9432 2017-10-11 23:34:47.000000 horovod-0.9.9/horovod/tensorflow/__init__.py
+-rw-r--r--   0 asergeev   (501) staff       (20)     1232 2017-08-10 01:37:50.000000 horovod-0.9.9/horovod/tensorflow/hash_vector.h
+-rw-r--r--   0 asergeev   (501) staff       (20)     8537 2017-08-27 02:31:26.000000 horovod-0.9.9/horovod/tensorflow/mpi_message.cc
+-rw-r--r--   0 asergeev   (501) staff       (20)     4730 2017-08-27 02:31:26.000000 horovod-0.9.9/horovod/tensorflow/mpi_message.h
+-rw-r--r--   0 asergeev   (501) staff       (20)    71665 2017-10-12 00:34:11.000000 horovod-0.9.9/horovod/tensorflow/mpi_ops.cc
+-rw-r--r--   0 asergeev   (501) staff       (20)     6435 2017-08-10 01:37:50.000000 horovod-0.9.9/horovod/tensorflow/mpi_ops.py
+-rw-r--r--   0 asergeev   (501) staff       (20)    22250 2017-09-04 06:51:03.000000 horovod-0.9.9/horovod/tensorflow/mpi_ops_test.py
+-rw-r--r--   0 asergeev   (501) staff       (20)     6901 2017-08-26 03:48:12.000000 horovod-0.9.9/horovod/tensorflow/timeline.cc
+-rw-r--r--   0 asergeev   (501) staff       (20)     2990 2017-08-26 03:48:12.000000 horovod-0.9.9/horovod/tensorflow/timeline.h
+drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-12 00:35:16.000000 horovod-0.9.9/horovod/tensorflow/wire/
+drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-12 00:35:16.000000 horovod-0.9.9/horovod/tensorflow/wire/flatbuffers/
+-rw-r--r--   0 asergeev   (501) staff       (20)    67819 2017-08-10 01:37:50.000000 horovod-0.9.9/horovod/tensorflow/wire/flatbuffers/flatbuffers.h
+-rw-r--r--   0 asergeev   (501) staff       (20)    12222 2017-08-27 02:31:26.000000 horovod-0.9.9/horovod/tensorflow/wire/mpi_message_generated.h
+drwxr-xr-x   0 asergeev   (501) staff       (20)        0 2017-10-12 00:35:16.000000 horovod-0.9.9/horovod.egg-info/
+-rw-r--r--   0 asergeev   (501) staff       (20)        1 2017-10-12 00:35:16.000000 horovod-0.9.9/horovod.egg-info/dependency_links.txt
+-rw-r--r--   0 asergeev   (501) staff       (20)        1 2017-08-10 05:27:45.000000 horovod-0.9.9/horovod.egg-info/not-zip-safe
+-rw-r--r--   0 asergeev   (501) staff       (20)      471 2017-10-12 00:35:16.000000 horovod-0.9.9/horovod.egg-info/PKG-INFO
+-rw-r--r--   0 asergeev   (501) staff       (20)      708 2017-10-12 00:35:16.000000 horovod-0.9.9/horovod.egg-info/SOURCES.txt
+-rw-r--r--   0 asergeev   (501) staff       (20)        8 2017-10-12 00:35:16.000000 horovod-0.9.9/horovod.egg-info/top_level.txt
+-rw-r--r--   0 asergeev   (501) staff       (20)    13232 2017-08-10 01:37:50.000000 horovod-0.9.9/LICENSE
+-rw-r--r--   0 asergeev   (501) staff       (20)       50 2017-09-26 17:57:01.000000 horovod-0.9.9/MANIFEST.in
+-rw-r--r--   0 asergeev   (501) staff       (20)      471 2017-10-12 00:35:16.000000 horovod-0.9.9/PKG-INFO
+-rw-r--r--   0 asergeev   (501) staff       (20)     8915 2017-10-11 23:34:52.000000 horovod-0.9.9/README.md
+-rw-r--r--   0 asergeev   (501) staff       (20)       38 2017-10-12 00:35:16.000000 horovod-0.9.9/setup.cfg
+-rw-r--r--   0 asergeev   (501) staff       (20)    12971 2017-10-12 00:34:11.000000 horovod-0.9.9/setup.py
```

### Comparing `horovod-0.9.8/docs/concepts.md` & `horovod-0.9.9/docs/concepts.md`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/docs/gpus.md` & `horovod-0.9.9/docs/gpus.md`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/docs/inference.md` & `horovod-0.9.9/docs/inference.md`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/docs/tensor-fusion.md` & `horovod-0.9.9/docs/tensor-fusion.md`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/docs/timeline.md` & `horovod-0.9.9/docs/timeline.md`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/docs/troubleshooting.md` & `horovod-0.9.9/docs/troubleshooting.md`

 * *Files 6% similar despite different names*

```diff
@@ -166,14 +166,32 @@
 
 For example:
 
 ```bash
 $ pip install horovod
 ```
 
+### ncclCommInitRank failed: unhandled cuda error
+
+If you see the error message below during the training, it means that NCCL is not able to initialize correctly. You can
+set the `NCCL_DEBUG` environment variable to `INFO` to have NCCL print debugging information which may reveal the reason.
+
+```
+UnknownError (see above for traceback): ncclCommInitRank failed: unhandled cuda error
+         [[Node: training/TFOptimizer/DistributedAdadeltaOptimizer_Allreduce/HorovodAllreduce_training_TFOptimizer_gradients_dense_2_BiasAdd_grad_tuple_control_dependency_1_0 = HorovodAllreduce[T=DT_FLOAT, _device="/job:localhost/replica:0/task:0/gpu:0"](training/TFOptimizer/gradients/dense_2/BiasAdd_grad/tuple/control_dependency_1)]]
+         [[Node: training/TFOptimizer/DistributedAdadeltaOptimizer/update/_94 = _Recv[client_terminated=false, recv_device="/job:localhost/replica:0/task:0/cpu:0", send_device="/job:localhost/replica:0/task:0/gpu:0", send_device_incarnation=1, tensor_name="edge_583_training/TFOptimizer/DistributedAdadeltaOptimizer/update", tensor_type=DT_FLOAT, _device="/job:localhost/replica:0/task:0/cpu:0"]()]]
+```
+
+For example:
+
+```bash
+$ export NCCL_DEBUG=INFO
+$ mpirun -np 16 -x NCCL_DEBUG -H server1:4,server2:4,server3:4,server4:4 python train.py
+```
+
 ### Running out of memory
 
 If you notice that your program is running out of GPU memory and multiple processes
 are being placed on the same GPU, it's likely that your program (or its dependencies)
 create a `tf.Session` that does not use the `config` that pins specific GPU.
 
 If possible, track down the part of program that uses these additional `tf.Session`s and pass
```

### Comparing `horovod-0.9.8/horovod/tensorflow/__init__.py` & `horovod-0.9.9/horovod/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/horovod/tensorflow/hash_vector.h` & `horovod-0.9.9/horovod/tensorflow/hash_vector.h`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/horovod/tensorflow/mpi_message.cc` & `horovod-0.9.9/horovod/tensorflow/mpi_message.cc`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/horovod/tensorflow/mpi_message.h` & `horovod-0.9.9/horovod/tensorflow/mpi_message.h`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/horovod/tensorflow/mpi_ops.cc` & `horovod-0.9.9/horovod/tensorflow/mpi_ops.cc`

 * *Files 2% similar despite different names*

```diff
@@ -837,20 +837,23 @@
           NCCL_CHECK(entries, "ncclGetUniqueId", ncclGetUniqueId(&nccl_id))
         }
 
         MPI_CHECK(entries, "MPI_Bcast",
                   MPI_Bcast((void*)&nccl_id, sizeof(nccl_id), MPI_BYTE, 0,
                             MPI_COMM_WORLD));
 
+        ncclComm_t new_nccl_comm;
         NCCL_CHECK(entries, "ncclCommInitRank",
-                   ncclCommInitRank(&nccl_comm, horovod_global.size, nccl_id,
+                   ncclCommInitRank(&new_nccl_comm, horovod_global.size, nccl_id,
                                     horovod_global.rank))
+        nccl_comm = new_nccl_comm;
 
-        // TODO: Rohit (NVIDIA): figure out why we need this sleep
-        std::this_thread::sleep_for(std::chrono::seconds(1));
+        // Barrier helps NCCL to synchronize after initialization and avoid
+        // deadlock that we've been seeing without it.
+        MPI_CHECK(entries, "MPI_Barrier", MPI_Barrier(MPI_COMM_WORLD));
 
         ACTIVITY_END_ALL(entries, timeline)
       }
 
       ncclDataType_t dtype;
       status = GetNCCLDataType(first_entry.tensor, &dtype);
       if (!status.ok()) {
```

### Comparing `horovod-0.9.8/horovod/tensorflow/mpi_ops.py` & `horovod-0.9.9/horovod/tensorflow/mpi_ops.py`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/horovod/tensorflow/mpi_ops_test.py` & `horovod-0.9.9/horovod/tensorflow/mpi_ops_test.py`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/horovod/tensorflow/timeline.cc` & `horovod-0.9.9/horovod/tensorflow/timeline.cc`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/horovod/tensorflow/timeline.h` & `horovod-0.9.9/horovod/tensorflow/timeline.h`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/horovod/tensorflow/wire/flatbuffers/flatbuffers.h` & `horovod-0.9.9/horovod/tensorflow/wire/flatbuffers/flatbuffers.h`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/horovod/tensorflow/wire/mpi_message_generated.h` & `horovod-0.9.9/horovod/tensorflow/wire/mpi_message_generated.h`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/horovod.egg-info/SOURCES.txt` & `horovod-0.9.9/horovod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/LICENSE` & `horovod-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/README.md` & `horovod-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `horovod-0.9.8/setup.py` & `horovod-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
 class custom_build_ext(build_ext):
     def build_extensions(self):
         fully_define_extension(self)
         build_ext.build_extensions(self)
 
 
 setup(name='horovod',
-      version='0.9.8',
+      version='0.9.9',
       packages=find_packages(),
       description='Distributed training framework for TensorFlow.',
       author='Uber Technologies, Inc.',
       long_description=textwrap.dedent('''\
           Horovod is a distributed training framework for TensorFlow. 
           The goal of Horovod is to make distributed Deep Learning
           fast and easy to use.'''),
```

