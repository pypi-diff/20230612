# Comparing `tmp/tensorflow-gnn-0.5.0rc0.tar.gz` & `tmp/tensorflow-gnn-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow-gnn-0.5.0rc0.tar", last modified: Fri Jan 27 18:15:20 2023, max compression
+gzip compressed data, was "tensorflow-gnn-0.5.1.tar", last modified: Mon Jun 12 14:40:09 2023, max compression
```

## Comparing `tensorflow-gnn-0.5.0rc0.tar` & `tensorflow-gnn-0.5.1.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      304 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/AUTHORS
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1481 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11357 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/LICENSE
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      177 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/MANIFEST.in
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)     5506 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/PKG-INFO
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4203 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/README.md
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      999 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/WORKSPACE
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.419440 tensorflow-gnn-0.5.0rc0/package/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      412 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/package/BUILD
--rwxr-xr-x   0 mparadkar (603057) primarygroup (89939)     1577 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/package/move_generated_files.sh
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      495 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/package/tfdep.bzl
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)       38 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/setup.cfg
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7184 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/setup.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.419440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1659 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8288 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/__init__.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.419440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/converters/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/converters/__init__.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.419440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/converters/ogb/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/converters/ogb/__init__.py
--rwxr-xr-x   0 mparadkar (603057) primarygroup (89939)    17657 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3645 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/converters/ogb/ogb_lib.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3291 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/converters/triples.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1567 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/converters/triples_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.419440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/data/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      986 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/data/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/data/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    41551 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/data/unigraph.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31879 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/data/unigraph_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.419440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1354 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/__init__.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.419440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31688 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/datasets.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    35246 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12073 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13830 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/models.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3138 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/reader_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11388 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/unigraph_data.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11598 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/unigraph_data_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.423440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11249 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20856 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/adjacency.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13080 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/adjacency_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    39354 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/batching_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32323 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/batching_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1289 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/dict_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1348 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/dict_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3857 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_constants.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    40947 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_piece.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28985 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_piece_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    60355 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6176 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_encode.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5885 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_encode_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20524 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_io.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27804 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_io_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    56326 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    73049 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2735 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_pprint.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1587 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_pprint_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12963 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_random.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6123 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_random_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    53315 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2635 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_test_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5414 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/normalization_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9065 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/normalization_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26955 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/padding_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26711 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/padding_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7818 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/preprocessing_common.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9088 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/preprocessing_common_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12726 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/schema_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10402 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/schema_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16641 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/schema_validation.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15373 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/schema_validation_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1134 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/tag_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1361 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/tag_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19393 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/tensor_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12925 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/tensor_utils_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.423440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2286 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1220 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6146 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/builders.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9557 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/builders_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14463 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/keras_e2e_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5581 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/keras_tensors.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13354 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/keras_tensors_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.423440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6229 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1679 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19603 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/convolution_base.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15800 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/convolution_base_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6516 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/convolutions.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5791 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/convolutions_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27129 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/graph_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    25880 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/graph_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    25485 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/graph_update.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10300 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/graph_update_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2904 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/item_dropout.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3874 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/item_dropout_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16646 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/map_features.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    23849 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/map_features_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10818 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/next_state.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4589 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/next_state_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2478 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/padding_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3698 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/padding_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2149 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/parse_example.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6313 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/parse_example_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.419440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.423440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      735 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1406 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/__init__.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.423440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1871 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5488 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/distribute_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2513 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2407 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/layers_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3720 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/tasks.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4320 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/tasks_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1648 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/layers.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.423440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gat_v2/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1022 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gat_v2/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1252 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gat_v2/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27602 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gat_v2/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26525 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gat_v2/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.423440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gcn/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      886 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gcn/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1030 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gcn/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11839 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gcn/gcn_conv.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19154 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gcn/gcn_conv_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.423440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gpt_gnn/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      759 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gpt_gnn/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      998 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gpt_gnn/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16777 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gpt_gnn/tensor_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16678 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gpt_gnn/tensor_utils_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.423440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/graph_sage/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      999 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/graph_sage/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1285 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/graph_sage/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    34468 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/graph_sage/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    23956 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/graph_sage/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.423440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/hgt/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      855 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/hgt/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1048 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/hgt/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2984 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/hgt/softmax.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5181 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/hgt/softmax_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.423440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2395 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1566 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2399 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/config_dict.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3059 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/config_dict_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2906 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1599 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    36816 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    46770 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2399 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1446 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2225 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2915 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2157 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1296 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4911 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4242 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/proto/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1013 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/proto/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/proto/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1023 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/proto/examples.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11444 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/proto/graph_schema.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2895 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/proto/graph_schema.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2887 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4590 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8308 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/distribute_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.419440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/examples/
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.419440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/examples/ogbn/
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      841 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12378 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/train.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/input/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      675 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/input/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19957 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/input/datasets.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9151 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/input/datasets_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6910 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/interfaces.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13882 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/orchestration.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5171 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/orchestration_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/tasks/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1381 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/tasks/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10249 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/tasks/classification.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8177 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/tasks/classification_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7818 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/tasks/regression.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5650 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/tasks/regression_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/trainers/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      373 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/trainers/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11673 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/trainers/keras_fit.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3268 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12942 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/attribution.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9399 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/attribution_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2243 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/model.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1324 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/model_dir.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6786 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/model_export.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9185 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/model_export_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2696 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/model_templates.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4916 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/model_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4245 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/padding.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2576 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/parsing.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4907 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/parsing_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1873 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/strategies.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1885 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19137 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/graph_sampler.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22306 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/graph_sampler_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22774 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_lib.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32206 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_lib_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6762 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_spec.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15163 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_spec_builder.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6212 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_spec_builder_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4931 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5281 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2123 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/subgraph.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13461 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/subgraph.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16517 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/subgraph_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2629 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tensorflow_gnn.bzl
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      455 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3368 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/generate_training_data.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1375 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/generate_training_data_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3926 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/print_training_data.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2080 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/print_training_data_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2700 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/sampled_stats.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8109 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/sampled_stats.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1975 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/sampled_stats_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1742 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/validate_graph_schema.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/utils/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      272 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/utils/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        1 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/utils/__init__.py
--rwxr-xr-x   0 mparadkar (603057) primarygroup (89939)     2116 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/utils/test_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2131 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn/version.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.419440 tensorflow-gnn-0.5.0rc0/tensorflow_gnn.egg-info/
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)     5506 2023-01-27 18:15:20.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn.egg-info/PKG-INFO
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)     9057 2023-01-27 18:15:20.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn.egg-info/SOURCES.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-01-27 18:15:20.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn.egg-info/dependency_links.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)      459 2023-01-27 18:15:20.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn.egg-info/entry_points.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-01-27 18:15:20.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn.egg-info/namespace_packages.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-01-27 18:15:20.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn.egg-info/not-zip-safe
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)      235 2023-01-27 18:15:20.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn.egg-info/requires.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)       22 2023-01-27 18:15:20.000000 tensorflow-gnn-0.5.0rc0/tensorflow_gnn.egg-info/top_level.txt
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/testdata/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      167 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/testdata/BUILD
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/testdata/heterogeneous/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      420 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/testdata/heterogeneous/BUILD
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/testdata/homogeneous/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      294 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/testdata/homogeneous/BUILD
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-01-27 18:15:20.427440 tensorflow-gnn-0.5.0rc0/testdata/node_vs_edge/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      295 2023-01-27 18:08:30.000000 tensorflow-gnn-0.5.0rc0/testdata/node_vs_edge/BUILD
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      304 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/AUTHORS
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1481 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11357 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/LICENSE
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      177 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/MANIFEST.in
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)     5503 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/PKG-INFO
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4203 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/README.md
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      999 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/WORKSPACE
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/package/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      412 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/package/BUILD
+-rwxrwxr-x   0 mparadkar (603057) primarygroup (89939)     1577 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/package/move_generated_files.sh
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      495 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/package/tfdep.bzl
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)       38 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/setup.cfg
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7191 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/setup.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1659 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8288 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/__init__.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/__init__.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/ogb/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/ogb/__init__.py
+-rwxrwxr-x   0 mparadkar (603057) primarygroup (89939)    17657 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3645 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/ogb/ogb_lib.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3291 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/triples.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1567 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/triples_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/data/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      986 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/data/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/data/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    41551 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/data/unigraph.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31879 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/data/unigraph_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1354 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/__init__.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31688 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/datasets.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    35246 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12073 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13830 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/models.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3138 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/reader_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11388 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/unigraph_data.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11598 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/unigraph_data_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.434229 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11249 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20856 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/adjacency.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13080 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/adjacency_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    39354 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/batching_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32323 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/batching_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1289 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/dict_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1348 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/dict_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3857 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_constants.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    40947 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_piece.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28985 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_piece_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    60355 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6176 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_encode.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5885 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_encode_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20524 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_io.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27804 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_io_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    56326 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    73049 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2735 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_pprint.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1587 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_pprint_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12963 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_random.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6123 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_random_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    53315 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2635 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_test_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5414 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/normalization_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9065 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/normalization_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26955 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/padding_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26711 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/padding_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7818 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/preprocessing_common.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9088 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/preprocessing_common_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12726 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10402 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16641 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_validation.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15373 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_validation_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1134 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tag_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1361 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tag_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19393 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tensor_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12925 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tensor_utils_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.434229 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2286 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1220 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6146 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/builders.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9557 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/builders_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14463 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/keras_e2e_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5581 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/keras_tensors.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13354 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/keras_tensors_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.434229 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6229 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1679 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19603 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolution_base.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15800 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolution_base_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6516 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolutions.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5791 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolutions_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27129 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    25880 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    25485 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_update.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10300 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_update_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2904 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/item_dropout.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3874 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/item_dropout_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16646 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/map_features.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    23849 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/map_features_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10818 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/next_state.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4589 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/next_state_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2478 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/padding_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3698 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/padding_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2149 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/parse_example.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6313 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/parse_example_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.434229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      735 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1406 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/__init__.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1871 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5488 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/distribute_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2513 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2407 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/layers_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3720 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/tasks.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4320 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/tasks_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1648 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/layers.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1022 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1252 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27602 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26525 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      886 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1030 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11839 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/gcn_conv.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19154 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/gcn_conv_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      759 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      998 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16777 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/tensor_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16678 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/tensor_utils_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      999 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1285 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    34468 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    23956 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      855 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1048 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2984 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/softmax.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5181 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/softmax_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2395 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1566 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2399 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/config_dict.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3059 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/config_dict_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2906 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1599 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    36816 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    46770 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2399 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1446 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2225 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/config_dict.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2915 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2157 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1296 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4911 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4242 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/proto/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1013 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/proto/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/proto/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1023 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/proto/examples.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11444 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/proto/graph_schema.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2895 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/proto/graph_schema.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2887 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4590 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8308 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/distribute_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/examples/
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/examples/ogbn/
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/examples/ogbn/mag/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      841 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/examples/ogbn/mag/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12378 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/examples/ogbn/mag/train.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/input/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      675 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/input/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19957 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/input/datasets.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9151 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/input/datasets_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6910 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/interfaces.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13882 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/orchestration.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5171 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/orchestration_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1381 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10249 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/classification.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8177 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/classification_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7818 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/regression.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5650 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/regression_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/trainers/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      373 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/trainers/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11673 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/trainers/keras_fit.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3268 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12942 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/attribution.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9399 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/attribution_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2243 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1324 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_dir.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6786 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_export.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9185 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_export_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2696 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_templates.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4916 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4245 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/padding.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2576 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/parsing.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4907 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/parsing_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1873 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/strategies.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1885 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19137 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/graph_sampler.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22306 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/graph_sampler_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22774 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_lib.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32206 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_lib_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6762 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_spec.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15163 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_spec_builder.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6212 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_spec_builder_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4931 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5281 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2123 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/subgraph.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13461 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/subgraph.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16517 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/subgraph_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2629 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tensorflow_gnn.bzl
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      455 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3368 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/generate_training_data.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1375 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/generate_training_data_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3926 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/print_training_data.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2080 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/print_training_data_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2700 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/sampled_stats.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8109 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/sampled_stats.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1975 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/sampled_stats_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1742 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/validate_graph_schema.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/tensorflow_gnn/utils/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      272 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/utils/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        1 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/utils/__init__.py
+-rwxrwxr-x   0 mparadkar (603057) primarygroup (89939)     2116 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/utils/test_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2128 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/version.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)     5503 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/PKG-INFO
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)     9057 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/SOURCES.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/dependency_links.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)      459 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/entry_points.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/namespace_packages.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-06-12 14:39:07.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/not-zip-safe
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)      242 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/requires.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)       27 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/top_level.txt
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/testdata/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      167 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/testdata/BUILD
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/testdata/heterogeneous/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      420 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/testdata/heterogeneous/BUILD
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/testdata/homogeneous/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      294 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/testdata/homogeneous/BUILD
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/testdata/node_vs_edge/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      295 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/testdata/node_vs_edge/BUILD
```

### Comparing `tensorflow-gnn-0.5.0rc0/BUILD` & `tensorflow-gnn-0.5.1/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/LICENSE` & `tensorflow-gnn-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/PKG-INFO` & `tensorflow-gnn-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-gnn
-Version: 0.5.0rc0
+Version: 0.5.1
 Summary: A library for building scalable graph neural networks in TensorFlow.
 Home-page: https://github.com/tensorflow/gnn
 Download-URL: https://github.com/tensorflow/gnn.git
 Author: Google LLC
 Author-email: tensorflow-gnn@googlegroups.com
 License: Apache 2.0
 Keywords: tensorflow gnn graph
```

### Comparing `tensorflow-gnn-0.5.0rc0/README.md` & `tensorflow-gnn-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/WORKSPACE` & `tensorflow-gnn-0.5.1/WORKSPACE`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/package/move_generated_files.sh` & `tensorflow-gnn-0.5.1/package/move_generated_files.sh`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/setup.py` & `tensorflow-gnn-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     namespace_packages=[],
     install_requires=[
-        'apache-beam',
+        'apache-beam<2.47.0',
         'google-vizier>=0.0.13',
         'ml-collections',
         'networkx',
         'pyarrow',
         # pylint:disable=g-line-too-long
         'tensorflow>=2.9.0; platform_machine != "arm64" or platform_system != "Darwin"',
         'tensorflow-macos>=2.9.0; platform_machine == "arm64" and platform_system == "Darwin"',
```

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/__init__.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/converters/ogb/ogb_lib.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/converters/ogb/ogb_lib.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/converters/triples.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/converters/triples.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/converters/triples_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/converters/triples_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/data/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/data/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/data/unigraph.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/data/unigraph.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/data/unigraph_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/data/unigraph_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/__init__.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/datasets.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/datasets.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/models.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/models.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/reader_utils.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/reader_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/unigraph_data.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/unigraph_data.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/experimental/in_memory/unigraph_data_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/unigraph_data_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/adjacency.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/adjacency.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/adjacency_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/adjacency_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/batching_utils.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/batching_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/batching_utils_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/batching_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/dict_utils.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/dict_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/dict_utils_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/dict_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_constants.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_constants.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_piece.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_piece.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_piece_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_piece_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_encode.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_encode.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_encode_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_encode_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_io.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_io.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_io_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_io_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_ops.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_ops_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_pprint.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_pprint.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_pprint_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_pprint_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_random.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_random.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_random_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_random_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/graph_tensor_test_utils.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_test_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/normalization_ops.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/normalization_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/normalization_ops_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/normalization_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/padding_ops.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/padding_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/padding_ops_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/padding_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/preprocessing_common.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/preprocessing_common.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/preprocessing_common_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/preprocessing_common_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/schema_utils.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/schema_utils_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/schema_validation.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_validation.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/schema_validation_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_validation_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/tag_utils.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tag_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/tag_utils_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tag_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/tensor_utils.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/graph/tensor_utils_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tensor_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/__init__.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/builders.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/builders.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/builders_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/builders_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/keras_e2e_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/keras_e2e_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/keras_tensors.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/keras_tensors.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/keras_tensors_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/keras_tensors_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/__init__.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/convolution_base.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolution_base.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/convolution_base_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolution_base_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/convolutions.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolutions.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/convolutions_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolutions_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/graph_ops.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/graph_ops_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/graph_update.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_update.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/graph_update_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_update_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/item_dropout.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/item_dropout.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/item_dropout_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/item_dropout_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/map_features.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/map_features.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/map_features_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/map_features_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/next_state.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/next_state.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/next_state_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/next_state_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/padding_ops.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/padding_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/padding_ops_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/padding_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/parse_example.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/parse_example.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/keras/layers/parse_example_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/parse_example_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/__init__.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/distribute_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/distribute_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/layers.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/layers_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/tasks.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/tasks.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/tasks_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/tasks_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/contrastive_losses/layers.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gat_v2/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gat_v2/__init__.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gat_v2/layers.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gat_v2/layers_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gcn/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gcn/__init__.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gcn/gcn_conv.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gcn/gcn_conv_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/gcn_conv_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gpt_gnn/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gpt_gnn/__init__.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gpt_gnn/tensor_utils.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/gpt_gnn/tensor_utils_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/tensor_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/graph_sage/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/graph_sage/__init__.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/graph_sage/layers.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/graph_sage/layers_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/hgt/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/hgt/__init__.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/hgt/softmax.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/softmax.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/hgt/softmax_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/softmax_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/__init__.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/config_dict.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/config_dict.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/config_dict_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/config_dict_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/layers.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/multi_head_attention/layers_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/__init__.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/config_dict.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/layers.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/models/vanilla_mpnn/layers_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/proto/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/proto/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/proto/examples.proto` & `tensorflow-gnn-0.5.1/tensorflow_gnn/proto/examples.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/proto/graph_schema.proto` & `tensorflow-gnn-0.5.1/tensorflow_gnn/proto/graph_schema.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/proto/graph_schema.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/proto/graph_schema.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/__init__.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/distribute_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/distribute_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/examples/ogbn/mag/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/train.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/examples/ogbn/mag/train.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/input/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/input/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/input/datasets.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/input/datasets.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/input/datasets_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/input/datasets_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/interfaces.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/orchestration.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/orchestration.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/orchestration_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/orchestration_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/tasks/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/tasks/classification.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/tasks/classification_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/classification_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/tasks/regression.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/regression.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/tasks/regression_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/regression_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/trainers/keras_fit.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/trainers/keras_fit.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/attribution.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/attribution.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/attribution_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/attribution_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/model.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/model_dir.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_dir.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/model_export.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_export.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/model_export_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_export_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/model_templates.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_templates.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/model_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/padding.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/padding.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/parsing.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/parsing_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/parsing_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/runner/utils/strategies.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/strategies.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/BUILD` & `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/graph_sampler.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/graph_sampler.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/graph_sampler_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/graph_sampler_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_lib.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_lib.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_lib_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_lib_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_spec.proto` & `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_spec.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_spec_builder.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_spec_builder.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_spec_builder_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_spec_builder_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_utils.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/sampling_utils_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/subgraph.proto` & `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/subgraph.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/subgraph.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/subgraph.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/sampler/subgraph_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/subgraph_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tensorflow_gnn.bzl` & `tensorflow-gnn-0.5.1/tensorflow_gnn/tensorflow_gnn.bzl`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/generate_training_data.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/generate_training_data.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/generate_training_data_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/generate_training_data_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/print_training_data.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/print_training_data.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/print_training_data_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/print_training_data_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/sampled_stats.proto` & `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/sampled_stats.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/sampled_stats.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/sampled_stats.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/sampled_stats_test.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/sampled_stats_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/tools/validate_graph_schema.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/validate_graph_schema.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/utils/test_utils.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn/version.py` & `tensorflow-gnn-0.5.1/tensorflow_gnn/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 #
 # Patch releases X.Y.Z, Z > 0, incl. their release candidates, can be done for
 # patches on branch rX.Y as needed.
 #
 # IMPORANT: Right after branching rX.Y, bump the main branch to X.(Y+1).0.dev1.
 # (Submit a change to the Source of Truth, get it out on the main branch asap.)
 
-__version__ = "0.5.0rc0"
+__version__ = "0.5.1"
```

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn.egg-info/PKG-INFO` & `tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-gnn
-Version: 0.5.0rc0
+Version: 0.5.1
 Summary: A library for building scalable graph neural networks in TensorFlow.
 Home-page: https://github.com/tensorflow/gnn
 Download-URL: https://github.com/tensorflow/gnn.git
 Author: Google LLC
 Author-email: tensorflow-gnn@googlegroups.com
 License: Apache 2.0
 Keywords: tensorflow gnn graph
```

### Comparing `tensorflow-gnn-0.5.0rc0/tensorflow_gnn.egg-info/SOURCES.txt` & `tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

