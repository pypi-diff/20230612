# Comparing `tmp/sparseml-1.5.0-py3-none-any.whl.zip` & `tmp/sparseml-1.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,370 +1,370 @@
-Zip file size: 945565 bytes, number of entries: 368
--rw-rw-r--  2.0 unx     1413 b- defN 23-Jun-02 02:44 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-Jun-02 02:44 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-Jun-02 02:44 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-Jun-02 02:44 sparseml/log.py
--rw-rw-r--  2.0 unx     1510 b- defN 23-Jun-02 02:44 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-Jun-02 02:44 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17631 b- defN 23-Jun-02 02:44 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-02 02:44 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jun-02 02:44 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-02 02:44 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jun-02 02:44 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-Jun-02 02:44 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jun-02 02:44 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-Jun-02 02:44 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-02 02:44 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-Jun-02 02:44 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     4751 b- defN 23-Jun-02 02:44 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2252 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     3866 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     4470 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4571 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      730 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx     8704 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-Jun-02 02:44 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jun-02 02:44 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-Jun-02 02:44 sparseml/framework/info.py
--rw-rw-r--  2.0 unx      970 b- defN 23-Jun-02 02:44 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-Jun-02 02:44 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-02 02:44 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-Jun-02 02:44 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-Jun-02 02:44 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-Jun-02 02:44 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-Jun-02 02:44 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Jun-02 02:44 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-Jun-02 02:44 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-Jun-02 02:44 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-02 02:44 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-02 02:44 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-Jun-02 02:44 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-Jun-02 02:44 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-Jun-02 02:44 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-Jun-02 02:44 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-Jun-02 02:44 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-Jun-02 02:44 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-Jun-02 02:44 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-Jun-02 02:44 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-02 02:44 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-Jun-02 02:44 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-Jun-02 02:44 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-Jun-02 02:44 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-Jun-02 02:44 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-Jun-02 02:44 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-Jun-02 02:44 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-Jun-02 02:44 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-Jun-02 02:44 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1036 b- defN 23-Jun-02 02:44 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-Jun-02 02:44 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-Jun-02 02:44 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-Jun-02 02:44 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-Jun-02 02:44 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-02 02:44 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13274 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19634 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14520 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4514 b- defN 23-Jun-02 02:44 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-Jun-02 02:44 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-Jun-02 02:44 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-02 02:44 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-Jun-02 02:44 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13002 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    16407 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    41311 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31586 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-Jun-02 02:44 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      931 b- defN 23-Jun-02 02:44 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3694 b- defN 23-Jun-02 02:44 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-Jun-02 02:44 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-Jun-02 02:44 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-Jun-02 02:44 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-Jun-02 02:44 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-Jun-02 02:44 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-Jun-02 02:44 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-Jun-02 02:44 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-Jun-02 02:44 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     1848 b- defN 23-Jun-02 02:44 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6173 b- defN 23-Jun-02 02:44 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Jun-02 02:44 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    10826 b- defN 23-Jun-02 02:44 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-Jun-02 02:44 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Jun-02 02:44 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-Jun-02 02:44 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      753 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    20912 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-Jun-02 02:44 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40800 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-Jun-02 02:44 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-02 02:44 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-Jun-02 02:44 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-Jun-02 02:44 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-Jun-02 02:44 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-02 02:44 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26838 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-Jun-02 02:44 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-Jun-02 02:44 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-Jun-02 02:44 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-02 02:44 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-Jun-02 02:44 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24121 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26253 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17591 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    69783 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-02 02:44 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    40790 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-Jun-02 02:44 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31056 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    39284 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8809 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-02 02:44 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-Jun-02 02:44 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-02 02:44 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-Jun-02 02:44 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-Jun-02 02:44 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-02 02:44 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-Jun-02 02:44 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-Jun-02 02:44 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-Jun-02 02:44 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-Jun-02 02:44 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-Jun-02 02:44 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-Jun-02 02:44 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-Jun-02 02:44 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-Jun-02 02:44 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-Jun-02 02:44 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx      987 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-Jun-02 02:44 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-02 02:44 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    19721 b- defN 23-Jun-02 02:44 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30756 b- defN 23-Jun-02 02:44 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36557 b- defN 23-Jun-02 02:44 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40177 b- defN 23-Jun-02 02:44 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34284 b- defN 23-Jun-02 02:44 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jun-02 02:44 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-Jun-02 02:44 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    43756 b- defN 23-Jun-02 02:44 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-Jun-02 02:44 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-Jun-02 02:44 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-Jun-02 02:44 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-02 02:44 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    15797 b- defN 23-Jun-02 02:44 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-Jun-02 02:44 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-Jun-02 02:44 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26321 b- defN 23-Jun-02 02:44 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-Jun-02 02:44 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-02 02:44 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-02 02:44 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-Jun-02 02:44 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-Jun-02 02:44 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-02 02:44 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-02 02:44 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4020 b- defN 23-Jun-02 02:44 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-02 02:44 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-02 02:44 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-02 02:44 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Jun-02 02:44 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-Jun-02 02:44 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-02 02:44 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     5763 b- defN 23-Jun-02 02:44 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2502 b- defN 23-Jun-02 02:44 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-02 02:44 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     7194 b- defN 23-Jun-02 02:44 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    34525 b- defN 23-Jun-02 02:44 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2748 b- defN 23-Jun-02 02:44 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     8196 b- defN 23-Jun-02 02:44 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-Jun-02 02:44 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6298 b- defN 23-Jun-02 02:44 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     4041 b- defN 23-Jun-02 02:44 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx    21503 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2377 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    36457 b- defN 23-Jun-02 02:45 sparseml-1.5.0.dist-info/RECORD
-368 files, 3422842 bytes uncompressed, 886595 bytes compressed:  74.1%
+Zip file size: 945570 bytes, number of entries: 368
+-rw-rw-r--  2.0 unx     1413 b- defN 23-Jun-09 22:16 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-Jun-09 22:16 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Jun-09 22:16 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-Jun-09 22:16 sparseml/log.py
+-rw-rw-r--  2.0 unx     1510 b- defN 23-Jun-09 22:17 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-Jun-09 22:16 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17631 b- defN 23-Jun-09 22:16 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-09 22:16 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Jun-09 22:16 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-09 22:16 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-09 22:16 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-Jun-09 22:16 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-09 22:16 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Jun-09 22:16 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-09 22:16 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Jun-09 22:16 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     4751 b- defN 23-Jun-09 22:16 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2252 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     3866 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     4470 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4571 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx     8704 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-Jun-09 22:16 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-09 22:16 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-Jun-09 22:16 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx      970 b- defN 23-Jun-09 22:16 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-Jun-09 22:16 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-09 22:16 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-Jun-09 22:16 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-Jun-09 22:16 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-Jun-09 22:16 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Jun-09 22:16 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Jun-09 22:16 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-Jun-09 22:16 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-09 22:16 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-Jun-09 22:16 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-Jun-09 22:16 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jun-09 22:16 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-Jun-09 22:16 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jun-09 22:16 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-Jun-09 22:16 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-Jun-09 22:16 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-09 22:16 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-09 22:16 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-Jun-09 22:16 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-Jun-09 22:16 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-Jun-09 22:16 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-Jun-09 22:16 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Jun-09 22:16 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-Jun-09 22:16 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-Jun-09 22:16 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-Jun-09 22:16 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-09 22:16 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-Jun-09 22:16 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Jun-09 22:16 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-Jun-09 22:16 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-Jun-09 22:16 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Jun-09 22:16 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-Jun-09 22:16 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-Jun-09 22:16 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-Jun-09 22:16 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Jun-09 22:16 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-Jun-09 22:16 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-Jun-09 22:16 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-Jun-09 22:16 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Jun-09 22:16 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-09 22:16 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jun-09 22:16 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13274 b- defN 23-Jun-09 22:16 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19634 b- defN 23-Jun-09 22:16 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-09 22:16 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-Jun-09 22:16 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14520 b- defN 23-Jun-09 22:16 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-Jun-09 22:16 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4514 b- defN 23-Jun-09 22:16 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Jun-09 22:16 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-Jun-09 22:16 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-09 22:16 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Jun-09 22:16 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-Jun-09 22:16 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13002 b- defN 23-Jun-09 22:16 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    16407 b- defN 23-Jun-09 22:16 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-Jun-09 22:16 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    41311 b- defN 23-Jun-09 22:16 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-09 22:16 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31586 b- defN 23-Jun-09 22:16 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-Jun-09 22:16 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-Jun-09 22:16 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3694 b- defN 23-Jun-09 22:16 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-Jun-09 22:16 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-Jun-09 22:16 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-Jun-09 22:16 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-Jun-09 22:16 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-Jun-09 22:16 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-Jun-09 22:16 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-Jun-09 22:16 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-Jun-09 22:16 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     1848 b- defN 23-Jun-09 22:16 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6173 b- defN 23-Jun-09 22:16 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jun-09 22:16 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    10826 b- defN 23-Jun-09 22:16 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-Jun-09 22:16 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-Jun-09 22:16 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-Jun-09 22:16 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-Jun-09 22:16 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-Jun-09 22:16 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-Jun-09 22:16 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-Jun-09 22:16 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-Jun-09 22:16 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-Jun-09 22:16 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-Jun-09 22:16 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-09 22:16 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    20912 b- defN 23-Jun-09 22:16 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-Jun-09 22:16 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Jun-09 22:16 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-09 22:16 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-Jun-09 22:16 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-Jun-09 22:16 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-Jun-09 22:16 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-09 22:16 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-09 22:16 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-Jun-09 22:16 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-Jun-09 22:16 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-09 22:16 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-Jun-09 22:16 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-Jun-09 22:16 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-Jun-09 22:16 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-Jun-09 22:16 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-Jun-09 22:16 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-Jun-09 22:16 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-Jun-09 22:16 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-Jun-09 22:16 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jun-09 22:16 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-Jun-09 22:16 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-09 22:16 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-Jun-09 22:16 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26253 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17591 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    69783 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-09 22:16 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-09 22:16 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-Jun-09 22:16 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-09 22:16 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Jun-09 22:16 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    40790 b- defN 23-Jun-09 22:16 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Jun-09 22:16 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-Jun-09 22:16 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31056 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    39284 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-09 22:16 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jun-09 22:16 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-09 22:16 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-Jun-09 22:16 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-Jun-09 22:16 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-09 22:16 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-Jun-09 22:16 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-Jun-09 22:16 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-Jun-09 22:16 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-Jun-09 22:16 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-Jun-09 22:16 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Jun-09 22:16 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-Jun-09 22:16 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-Jun-09 22:16 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Jun-09 22:16 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx      987 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-Jun-09 22:16 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-09 22:16 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    19721 b- defN 23-Jun-09 22:16 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30756 b- defN 23-Jun-09 22:16 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36557 b- defN 23-Jun-09 22:16 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40177 b- defN 23-Jun-09 22:16 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34284 b- defN 23-Jun-09 22:16 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-09 22:16 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-Jun-09 22:16 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    43756 b- defN 23-Jun-09 22:16 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-Jun-09 22:16 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Jun-09 22:16 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-Jun-09 22:16 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-09 22:16 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    15797 b- defN 23-Jun-09 22:16 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Jun-09 22:16 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-Jun-09 22:16 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26321 b- defN 23-Jun-09 22:16 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Jun-09 22:16 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-09 22:16 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-09 22:16 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-Jun-09 22:16 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-Jun-09 22:16 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-09 22:16 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Jun-09 22:16 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-Jun-09 22:16 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-Jun-09 22:16 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-Jun-09 22:16 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-Jun-09 22:16 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-09 22:16 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-09 22:16 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-Jun-09 22:16 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-09 22:16 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-09 22:16 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-09 22:16 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Jun-09 22:16 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Jun-09 22:16 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-09 22:16 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5782 b- defN 23-Jun-09 22:16 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2502 b- defN 23-Jun-09 22:16 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-09 22:16 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7194 b- defN 23-Jun-09 22:16 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    34525 b- defN 23-Jun-09 22:16 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2748 b- defN 23-Jun-09 22:16 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     8196 b- defN 23-Jun-09 22:16 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-Jun-09 22:16 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6298 b- defN 23-Jun-09 22:16 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     4041 b- defN 23-Jun-09 22:16 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-09 22:19 sparseml-1.5.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21503 b- defN 23-Jun-09 22:19 sparseml-1.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Jun-09 22:19 sparseml-1.5.1.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-09 22:19 sparseml-1.5.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2377 b- defN 23-Jun-09 22:19 sparseml-1.5.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-09 22:19 sparseml-1.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    36457 b- defN 23-Jun-09 22:19 sparseml-1.5.1.dist-info/RECORD
+368 files, 3422861 bytes uncompressed, 886600 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1077,29 +1077,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml-1.5.0.dist-info/LICENSE
+Filename: sparseml-1.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml-1.5.0.dist-info/METADATA
+Filename: sparseml-1.5.1.dist-info/METADATA
 Comment: 
 
-Filename: sparseml-1.5.0.dist-info/NOTICE
+Filename: sparseml-1.5.1.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml-1.5.0.dist-info/WHEEL
+Filename: sparseml-1.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml-1.5.0.dist-info/entry_points.txt
+Filename: sparseml-1.5.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml-1.5.0.dist-info/top_level.txt
+Filename: sparseml-1.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml-1.5.0.dist-info/RECORD
+Filename: sparseml-1.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/version.py

```diff
@@ -15,15 +15,15 @@
 """
 Functionality for storing and setting the version info for SparseML
 """
 
 from datetime import date
 
 
-version_base = "1.5.0"
+version_base = "1.5.1"
 is_release = True  # change to True to set the generated version as a release version
 
 
 def _generate_version():
     return (
         version_base
         if is_release
```

## sparseml/yolov8/default.yaml

```diff
@@ -1,11 +1,12 @@
 # Default training settings and hyperparameters for medium-augmentation COCO training
 
 recipe: null
 recipe_args: null
+datasets_dir: null
 
 task: "detect" # choices=['detect', 'segment', 'classify', 'init'] # init is a special case. Specify task to run.
 mode: "train" # choices=['train', 'val', 'predict'] # mode to run task in.
 
 # Train settings -------------------------------------------------------------------------------------------------------
 model: "yolov8n.yaml" # i.e. yolov8n.pt, yolov8n.yaml. Path to model file
 data: "coco128.yaml" # i.e. coco128.yaml. Path to data file
```

## Comparing `sparseml-1.5.0.dist-info/LICENSE` & `sparseml-1.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml-1.5.0.dist-info/METADATA` & `sparseml-1.5.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml
-Version: 1.5.0
+Version: 1.5.1
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
```

## Comparing `sparseml-1.5.0.dist-info/NOTICE` & `sparseml-1.5.1.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml-1.5.0.dist-info/entry_points.txt` & `sparseml-1.5.1.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `sparseml-1.5.0.dist-info/RECORD` & `sparseml-1.5.1.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 sparseml/__init__.py,sha256=nxuiUykjTFTYiw28TB9H75wWbdzr6Y0j-2h4dabdp54,1413
 sparseml/analytics.py,sha256=WhXdKgK1-ll9sRzn2n8z-FAikQ02J8rUeWmceiX5S7E,898
 sparseml/base.py,sha256=oOPiaU2JhI0beFwp8Obe7hbt3kUuNvI5XD1wTBCtLnc,10284
 sparseml/log.py,sha256=K5E3goPRIPY7Uc14JcX-4oLXVWu7ecOPf1NYBGHc1r0,2483
-sparseml/version.py,sha256=UZJVzd8NwptR2hTgM4HQP2UR7hIZZO7BSRFwFYA0rNc,1510
+sparseml/version.py,sha256=Zx0jnyPm_JrvbK79HOskzzzT7KGIl1bLSX6cNUbw7qc,1510
 sparseml/benchmark/__init__.py,sha256=WynUhMzXq3-iQAhPwcmcMOj2_xCa9brLubs7gxq9T3U,758
 sparseml/benchmark/info.py,sha256=yRA5QgKQNKjOZhQH9uNvVuWlqL4eXDVikA8pL5Mzha4,17631
 sparseml/benchmark/serialization.py,sha256=FPpcC93x5H86Fqil9YbERUpltu7qhhIQjsyYaSlW_20,10778
 sparseml/deepsparse/__init__.py,sha256=o5ITzTEOlH--61_SXMISrmPcRk4ci91FGlR-aQxwOn4,863
 sparseml/deepsparse/base.py,sha256=nRjU6TSao0J2iWXcdHwj62X6dVT9vl6TQ2y4Bdn3KN0,3516
 sparseml/deepsparse/framework/__init__.py,sha256=ZHrXXM3AMH78zKcF8Y40IBuy38UFy4fLrvytozw_bNY,801
 sparseml/deepsparse/framework/info.py,sha256=HVDPHFXggFeDqbpM20PkByf1nBccwKnjpTWh0EfrVas,6032
@@ -345,24 +345,24 @@
 sparseml/yolact/__init__.py,sha256=5t9V0aePHnzJBik6z1r4W_3DsSn0lKpYjl3pIuZQft0,4020
 sparseml/yolact/scripts.py,sha256=7GE3xp_B8JJpa2H-Vum6rmiOJHcChyffuno4-yteUUw,1784
 sparseml/yolov5/__init__.py,sha256=LiVvIlHR1FF63Ixm2MabdDH1Ul8sFEUEIb3Sbs4awLI,1440
 sparseml/yolov5/helpers.py,sha256=jxzJrgKjsb0PHTeGevKICaL8iBOUzxwZXvPAyGyVE-c,4505
 sparseml/yolov5/scripts.py,sha256=rbVgQ3yNsBCk57BMVh5mKomDHql0S-PkHNGCy_qUfEg,1609
 sparseml/yolov5/yolov5.status.yaml,sha256=4GF6DClV65Qw_1b0J5Ul-B4YFHYQUj34vvqALX8sZFY,1220
 sparseml/yolov8/__init__.py,sha256=l6f1TkolWl2ejQQ63jN3VFft7mMpQDURpWDIeflVKGQ,1115
-sparseml/yolov8/default.yaml,sha256=dVDQ77Px58l5jLoVJOdiNGbW-cDn-SdUioHkpG19CXg,5763
+sparseml/yolov8/default.yaml,sha256=RoQ1eFWHEXcrojmuRsewJAvS9uNGCN5qmsof0goEjAA,5782
 sparseml/yolov8/export.py,sha256=BN4KFsrYYEfpU8e7icW4rQr4uR4lioNXlY3MII9ecKw,2502
 sparseml/yolov8/modules.py,sha256=j-8TGWMY5-pnEDt-uj1akERLt5zcjK11aN6Bnh1Clrg,2259
 sparseml/yolov8/train.py,sha256=DeZMrZ_moAc3fIojJloq3IvQqiPC_cgPgTjYFSOoG7E,7194
 sparseml/yolov8/trainers.py,sha256=-nCtUkmJNGOR48jMn_erjkV22ykd0lMp8PObI0v6Bzk,34525
 sparseml/yolov8/val.py,sha256=hlFImvknSpV1nONOxA3ivYgvzm64EmK0_Lh-JHLbOsw,2748
 sparseml/yolov8/validators.py,sha256=ytG7g_LOXvKFmxLPmQloT-wNf78convSoRRXVTYCR0Y,8196
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
 sparseml/yolov8/utils/export_samples.py,sha256=YbiV_0cv_W0xrhtZLg6ActLeSRYYikrOzHz0FqJ0LII,6298
 sparseml/yolov8/utils/helpers.py,sha256=8JZNaTT1zPKiZaOccmMtQu5mXCSMGkq8BDEgUqaPVIs,4041
-sparseml-1.5.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml-1.5.0.dist-info/METADATA,sha256=NNUqkAOG_hJCcHdVxNQw-1W3qWiE9iwF3l33wbPV1bs,21503
-sparseml-1.5.0.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml-1.5.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml-1.5.0.dist-info/entry_points.txt,sha256=KbSvJr3uXYQgZRF0Mzi5B89ijSwsiZalXMxinJRaass,2377
-sparseml-1.5.0.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml-1.5.0.dist-info/RECORD,,
+sparseml-1.5.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml-1.5.1.dist-info/METADATA,sha256=6toMRBz5TKEgHGMZMYsGGqmnJm52cNacQNWVAUN0svQ,21503
+sparseml-1.5.1.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml-1.5.1.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml-1.5.1.dist-info/entry_points.txt,sha256=KbSvJr3uXYQgZRF0Mzi5B89ijSwsiZalXMxinJRaass,2377
+sparseml-1.5.1.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml-1.5.1.dist-info/RECORD,,
```

