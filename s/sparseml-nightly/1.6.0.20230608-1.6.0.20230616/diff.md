# Comparing `tmp/sparseml_nightly-1.6.0.20230608-py3-none-any.whl.zip` & `tmp/sparseml_nightly-1.6.0.20230616-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,370 +1,374 @@
-Zip file size: 946842 bytes, number of entries: 368
--rw-rw-r--  2.0 unx     1413 b- defN 23-Jun-08 01:31 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-Jun-08 01:31 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-Jun-08 01:31 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-Jun-08 01:31 sparseml/log.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-08 01:31 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-Jun-08 01:31 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17631 b- defN 23-Jun-08 01:31 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-08 01:31 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jun-08 01:31 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-08 01:31 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jun-08 01:31 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-Jun-08 01:31 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jun-08 01:31 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-Jun-08 01:31 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-08 01:31 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-Jun-08 01:31 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     4783 b- defN 23-Jun-08 01:31 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2252 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     3866 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     4470 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4571 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      730 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx     8704 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jun-08 01:31 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-Jun-08 01:31 sparseml/framework/info.py
--rw-rw-r--  2.0 unx     1144 b- defN 23-Jun-08 01:31 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-Jun-08 01:31 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-Jun-08 01:31 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-Jun-08 01:31 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-Jun-08 01:31 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-Jun-08 01:31 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Jun-08 01:31 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-Jun-08 01:31 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-Jun-08 01:31 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-08 01:31 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-08 01:31 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-Jun-08 01:31 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-Jun-08 01:31 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-Jun-08 01:31 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-Jun-08 01:31 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-Jun-08 01:31 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-Jun-08 01:31 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-Jun-08 01:31 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-Jun-08 01:31 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-08 01:31 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-Jun-08 01:31 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-Jun-08 01:31 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-Jun-08 01:31 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-Jun-08 01:31 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-Jun-08 01:31 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-Jun-08 01:31 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-Jun-08 01:31 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-Jun-08 01:31 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1036 b- defN 23-Jun-08 01:31 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-Jun-08 01:31 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-Jun-08 01:31 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-Jun-08 01:31 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-Jun-08 01:31 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-08 01:31 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13285 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19639 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14532 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4552 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-Jun-08 01:31 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-Jun-08 01:31 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-08 01:31 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-Jun-08 01:31 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13013 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    16407 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    40230 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31591 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      931 b- defN 23-Jun-08 01:31 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3713 b- defN 23-Jun-08 01:31 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-Jun-08 01:31 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-Jun-08 01:31 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-Jun-08 01:31 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-Jun-08 01:31 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-Jun-08 01:31 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-Jun-08 01:31 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-Jun-08 01:31 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-Jun-08 01:31 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     1848 b- defN 23-Jun-08 01:31 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6173 b- defN 23-Jun-08 01:31 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Jun-08 01:31 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    10864 b- defN 23-Jun-08 01:31 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Jun-08 01:31 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-Jun-08 01:31 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      753 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    20912 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40800 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-08 01:31 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-Jun-08 01:31 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-Jun-08 01:31 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-Jun-08 01:31 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-08 01:31 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26838 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-Jun-08 01:31 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-Jun-08 01:31 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-08 01:31 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-Jun-08 01:31 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24121 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26778 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17905 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    70029 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    41409 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31098 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    39284 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8809 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-Jun-08 01:31 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-08 01:31 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-Jun-08 01:31 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-Jun-08 01:31 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-08 01:31 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-Jun-08 01:31 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-Jun-08 01:31 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-Jun-08 01:31 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-Jun-08 01:31 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-Jun-08 01:31 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-Jun-08 01:31 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-Jun-08 01:31 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-Jun-08 01:31 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-Jun-08 01:31 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx     1169 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-08 01:31 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    21274 b- defN 23-Jun-08 01:31 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30756 b- defN 23-Jun-08 01:31 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36557 b- defN 23-Jun-08 01:31 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40299 b- defN 23-Jun-08 01:31 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34350 b- defN 23-Jun-08 01:31 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jun-08 01:31 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-Jun-08 01:31 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    43772 b- defN 23-Jun-08 01:31 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-Jun-08 01:31 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-Jun-08 01:31 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-Jun-08 01:31 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-08 01:31 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    17072 b- defN 23-Jun-08 01:31 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-Jun-08 01:31 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-Jun-08 01:31 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26562 b- defN 23-Jun-08 01:31 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-Jun-08 01:31 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-08 01:31 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-08 01:31 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-Jun-08 01:31 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-08 01:31 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-08 01:31 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4020 b- defN 23-Jun-08 01:31 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-08 01:31 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-08 01:31 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-08 01:31 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Jun-08 01:31 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-Jun-08 01:31 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-08 01:31 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     5781 b- defN 23-Jun-08 01:31 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2502 b- defN 23-Jun-08 01:31 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-08 01:31 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     7194 b- defN 23-Jun-08 01:31 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    34788 b- defN 23-Jun-08 01:31 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2748 b- defN 23-Jun-08 01:31 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     8196 b- defN 23-Jun-08 01:31 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-Jun-08 01:31 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6288 b- defN 23-Jun-08 01:31 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     4041 b- defN 23-Jun-08 01:31 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/LICENSE
--rw-rw-r--  2.0 unx    21640 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2377 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    36578 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/RECORD
-368 files, 3427837 bytes uncompressed, 887634 bytes compressed:  74.1%
+Zip file size: 959278 bytes, number of entries: 372
+-rw-rw-r--  2.0 unx     1413 b- defN 23-Jun-16 12:34 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-Jun-16 12:34 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Jun-16 12:34 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-Jun-16 12:34 sparseml/log.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-16 12:34 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-Jun-16 12:34 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17631 b- defN 23-Jun-16 12:34 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-16 12:34 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Jun-16 12:34 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-16 12:34 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-16 12:34 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-Jun-16 12:34 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-16 12:34 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Jun-16 12:34 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-16 12:34 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Jun-16 12:34 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     6058 b- defN 23-Jun-16 12:34 sparseml/exporters/kv_cache_injector.py
+-rw-rw-r--  2.0 unx     4783 b- defN 23-Jun-16 12:34 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2276 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     3866 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     4866 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4681 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/kv_cache/__init__.py
+-rw-rw-r--  2.0 unx    20939 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
+-rw-rw-r--  2.0 unx     6763 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/kv_cache/position_embeddings_adjustment.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx    10570 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-16 12:34 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-Jun-16 12:34 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx     1144 b- defN 23-Jun-16 12:34 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-Jun-16 12:34 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-Jun-16 12:34 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-Jun-16 12:34 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jun-16 12:34 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-Jun-16 12:34 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jun-16 12:34 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-Jun-16 12:34 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-Jun-16 12:34 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-16 12:34 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-16 12:34 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-Jun-16 12:34 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-Jun-16 12:34 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-Jun-16 12:34 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-Jun-16 12:34 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Jun-16 12:34 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-Jun-16 12:34 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-Jun-16 12:34 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-Jun-16 12:34 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-16 12:34 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-Jun-16 12:34 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Jun-16 12:34 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-Jun-16 12:34 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-Jun-16 12:34 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Jun-16 12:34 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-Jun-16 12:34 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-Jun-16 12:34 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-Jun-16 12:34 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Jun-16 12:34 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-Jun-16 12:34 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-Jun-16 12:34 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-Jun-16 12:34 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Jun-16 12:34 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-16 12:34 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13285 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19639 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14532 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4552 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Jun-16 12:34 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-Jun-16 12:34 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-16 12:34 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Jun-16 12:34 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13013 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    16407 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    40230 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31591 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-Jun-16 12:34 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3713 b- defN 23-Jun-16 12:34 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-Jun-16 12:34 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-Jun-16 12:34 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-Jun-16 12:34 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-Jun-16 12:34 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-Jun-16 12:34 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-Jun-16 12:34 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-Jun-16 12:34 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-Jun-16 12:34 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     1848 b- defN 23-Jun-16 12:34 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6117 b- defN 23-Jun-16 12:34 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jun-16 12:34 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    10864 b- defN 23-Jun-16 12:34 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-Jun-16 12:34 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-Jun-16 12:34 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    20676 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-16 12:34 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-Jun-16 12:34 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-Jun-16 12:34 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-Jun-16 12:34 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-16 12:34 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jun-16 12:34 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-Jun-16 12:34 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-16 12:34 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-Jun-16 12:34 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26778 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17905 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    76796 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    41409 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31098 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    39284 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jun-16 12:34 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-16 12:34 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-Jun-16 12:34 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-Jun-16 12:34 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-16 12:34 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-Jun-16 12:34 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-Jun-16 12:34 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-Jun-16 12:34 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-Jun-16 12:34 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-Jun-16 12:34 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Jun-16 12:34 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-Jun-16 12:34 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-Jun-16 12:34 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Jun-16 12:34 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx     1169 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-16 12:34 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    21290 b- defN 23-Jun-16 12:34 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30756 b- defN 23-Jun-16 12:34 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36557 b- defN 23-Jun-16 12:34 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40299 b- defN 23-Jun-16 12:34 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34350 b- defN 23-Jun-16 12:34 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-16 12:34 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-Jun-16 12:34 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    43772 b- defN 23-Jun-16 12:34 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-Jun-16 12:34 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Jun-16 12:34 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-Jun-16 12:34 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-16 12:34 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    17072 b- defN 23-Jun-16 12:34 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Jun-16 12:34 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-Jun-16 12:34 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26562 b- defN 23-Jun-16 12:34 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Jun-16 12:34 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-16 12:34 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-16 12:34 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-Jun-16 12:34 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-16 12:34 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-16 12:34 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-Jun-16 12:34 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-16 12:34 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-16 12:34 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-16 12:34 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Jun-16 12:34 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Jun-16 12:34 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-16 12:34 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5781 b- defN 23-Jun-16 12:34 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2502 b- defN 23-Jun-16 12:34 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-16 12:34 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7194 b- defN 23-Jun-16 12:34 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    34788 b- defN 23-Jun-16 12:34 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2748 b- defN 23-Jun-16 12:34 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     8196 b- defN 23-Jun-16 12:34 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-Jun-16 12:34 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6288 b- defN 23-Jun-16 12:34 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     4041 b- defN 23-Jun-16 12:34 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21650 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2377 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    37031 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/RECORD
+372 files, 3471754 bytes uncompressed, 899318 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -42,14 +42,17 @@
 
 Filename: sparseml/exporters/__init__.py
 Comment: 
 
 Filename: sparseml/exporters/base_exporter.py
 Comment: 
 
+Filename: sparseml/exporters/kv_cache_injector.py
+Comment: 
+
 Filename: sparseml/exporters/onnx_to_deepsparse.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/__init__.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/base_transform.py
@@ -120,14 +123,23 @@
 
 Filename: sparseml/exporters/transforms/skip_input_quantize.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/unwrap_batchnorms.py
 Comment: 
 
+Filename: sparseml/exporters/transforms/kv_cache/__init__.py
+Comment: 
+
+Filename: sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
+Comment: 
+
+Filename: sparseml/exporters/transforms/kv_cache/position_embeddings_adjustment.py
+Comment: 
+
 Filename: sparseml/exporters/transforms/utils/__init__.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/utils/helpers.py
@@ -1077,29 +1089,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230608.dist-info/LICENSE
+Filename: sparseml_nightly-1.6.0.20230616.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230608.dist-info/METADATA
+Filename: sparseml_nightly-1.6.0.20230616.dist-info/METADATA
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230608.dist-info/NOTICE
+Filename: sparseml_nightly-1.6.0.20230616.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230608.dist-info/WHEEL
+Filename: sparseml_nightly-1.6.0.20230616.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230608.dist-info/entry_points.txt
+Filename: sparseml_nightly-1.6.0.20230616.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230608.dist-info/top_level.txt
+Filename: sparseml_nightly-1.6.0.20230616.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230608.dist-info/RECORD
+Filename: sparseml_nightly-1.6.0.20230616.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/exporters/transforms/__init__.py

```diff
@@ -42,7 +42,8 @@
 from .matmul_to_matmulinteger_cast_mul import MatMulToMatMulIntegerCastMul
 from .propagate_embedding_quantization import PropagateEmbeddingQuantization
 from .quantize_qat_embedding import QuantizeQATEmbedding
 from .quantize_residuals import QuantizeResiduals
 from .remove_duplicate_qconv_weights import RemoveDuplicateQConvWeights
 from .remove_duplicate_quantize_ops import RemoveDuplicateQuantizeOps
 from .skip_input_quantize import SkipInputQuantize
+from .kv_cache import *
```

## sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py

```diff
@@ -31,35 +31,37 @@
 
 
 class MatMulAddToMatMulIntegerAddCastMul(OnnxTransform):
     """
     A transform for converting a MatMul with kernel and bias into a
     quantized representation
 
+    If add or bias initializer does not exist, the bias is skipped
+
     ```
     |     weight (initializer)
     |         |
     |         Q
     |         |
     | input   Dq
     |   |     |
     |  Q/Dq   optional Transpose
     |     |   |
-    |     MatMul  bias (initializer)
+    |     MatMul  bias (initializer) (optional)
     |         |   |
-    |         Add
+    |         Add (optional)
     ```
     (where `Q` is QuantizeLinear, and `Dq` is DequantizeLinear)
     into
     ```
     |   input
     |     |
     | MatMulInteger (with constant uint8 kernel)
     |     |
-    | Add (constant bias + zero point correction)
+    | Add (constant bias + zero point correction) (optional)
     |     |
     | Cast (INT32 -> FP32)
     |     |
     | Mul (Rescale from bias scale)
     ```
     """
 
@@ -74,24 +76,26 @@
                     # weight should be initializer
                     INITIALIZER_MATCH,
                     "QuantizeLinear",
                     "DequantizeLinear",
                     optional_node("Transpose"),
                 ],
             ],
-            children_ops=[["Add"]],
+            children_ops=[[optional_node("Add")]],
         )
         for match in matches:
-            # NOTE: bias could be either input 0 or 1 of add node
-            bias_init = graph.get_init_by_name(match.children[0][0].input[1])
-            if bias_init is None:
-                bias_init = graph.get_init_by_name(match.children[0][0].input[0])
+            add_node = match.children[0][0]
+            bias_init = None
+            if add_node:
+                # NOTE: bias could be either input 0 or 1 of add node
+                # if add does not have a bias initializer,
+                # still do conversion, but do not fold the bias add to rescale
+                bias_init = graph.get_init_by_name(match.children[0][0].input[1])
                 if bias_init is None:
-                    # bias initializer for add not present
-                    continue
+                    bias_init = graph.get_init_by_name(match.children[0][0].input[0])
             self.log_match(match)
             self._transform_match(graph, model, match, bias_init)
         return model
 
     def _transform_match(
         self,
         graph: ONNXGraph,
@@ -117,21 +121,23 @@
             model=model,
             node=matmul,
             input_quantize_node=input_quant,
             weight_quantize_node=weight_quant,
             input_quantize_params=input_quantize_params,
             weight_quantize_params=weight_quantize_params,
             bias_initializer=bias_init,
-            bias_add_name=add.name,
-            target_output=add.output[0],
+            bias_add_name=add.name if add else None,
+            target_output=add.output[0] if add and bias_init else None,
             transpose_weight=opt_transpose is not None,
         )
 
         # Clean up
         self.delete_node_deferred(weight_dequant)
         self.delete_node_deferred(weight_quant)
         if opt_transpose is not None:
             self.delete_node_deferred(opt_transpose)
         if len(graph.get_node_children(input_quant)) == 1:
             self.delete_node_deferred(input_quant)
         self.delete_node_deferred(matmul)
-        self.delete_node_deferred(add)
+        if bias_init is not None:
+            # add converted to quantized - delete previous add node
+            self.delete_node_deferred(add)
```

## sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py

```diff
@@ -72,17 +72,20 @@
             parent_ops=[
                 ["QuantizeLinear", "DequantizeLinear"],
                 ["QuantizeLinear", "DequantizeLinear"],
             ],
             op_type="MatMul",
         )
         for match in matches:
+            is_parameterized = False
             for quantize_linear_parent in [match.parents[0][0], match.parents[1][0]]:
                 if graph.get_init_by_name(quantize_linear_parent.input[0]):
-                    continue
+                    is_parameterized = True
+            if is_parameterized:
+                continue
             self.log_match(match)
             self._do_transform(model, match)
         return model
 
     def _do_transform(self, model: ModelProto, match: MatchResult):
         a_quant, a_dequant = match.parents[0]
         b_quant, b_dequant = match.parents[1]
```

## sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py

```diff
@@ -31,28 +31,35 @@
 def add_quantized_conv_matmul_add_ops(
     model: ModelProto,
     node: NodeProto,
     input_quantize_node: NodeProto,
     weight_quantize_node: NodeProto,
     input_quantize_params: QuantizationParams,
     weight_quantize_params: QuantizationParams,
-    bias_initializer: TensorProto,
+    bias_initializer: Optional[TensorProto],
     bias_add_name: str,
     target_output: str,
     transpose_weight: bool,
     output_quantize_node: Optional[NodeProto] = None,
     output_dequantize_node: Optional[NodeProto] = None,
 ) -> ModelProto:
     """
     Helper function for conversion of qat parameterized gemms, matmuls, or convs to
     conv/matmul integer add blocks.
 
     Adds new quantized ops to graph, does not perform any checks or deletions
     (should be called by the operator main conversion function)
     """
+    node_output_orig = node.output[0]
+    if not target_output and (
+        any(output.name == node_output_orig for output in model.graph.output)
+    ):
+        # original node output is a graph output, make that the quant block
+        # output target id
+        target_output = node_output_orig
 
     # Quantize weights and add to graph
     quantized_weight_initializer = _quantize_weight_initializer(
         node, weight_quantize_params, transpose_weight
     )
     model.graph.initializer.append(quantized_weight_initializer)
 
@@ -61,78 +68,107 @@
         node,
         input_quantize_node,
         weight_quantize_node,
         quantized_weight_initializer.name,
     )
     model.graph.node.append(integer_op_node)
 
-    # Add bias + zero point correction; quantize bias and add it to graph
-    (
-        quantized_bias_initializer,
-        quantized_bias_scale,
-        quantize_bias_zero_point,
-    ) = _quantize_bias(
-        node,
-        bias_initializer,
-        input_quantize_params,
-        weight_quantize_params,
-        bias_add_name,
-    )
-    model.graph.initializer.append(quantized_bias_initializer)
-    model.graph.initializer.append(quantized_bias_scale)
-    model.graph.initializer.append(quantize_bias_zero_point)
+    if bias_initializer is not None:
+        # Add bias + zero point correction; quantize bias and add it to graph
+        (
+            quantized_bias_initializer,
+            quantized_bias_scale,
+            quantize_bias_zero_point,
+        ) = _quantize_bias(
+            node,
+            bias_initializer,
+            input_quantize_params,
+            weight_quantize_params,
+            bias_add_name,
+        )
+        model.graph.initializer.append(quantized_bias_initializer)
+        model.graph.initializer.append(quantized_bias_scale)
+        model.graph.initializer.append(quantize_bias_zero_point)
+
+        # Create Quantized Bias Add node and add it to graph
+        qadd_node = _create_qadd_node(
+            node,
+            integer_op_output="{}_quant".format(node.output[0]),
+            quantized_bias_name=quantized_bias_initializer.name,
+            output_quantize_node=output_quantize_node,
+        )
+        model.graph.node.append(qadd_node)
 
-    # Create Quantized Bias Add node and add it to graph
-    qadd_node = _create_qadd_node(
-        node,
-        integer_op_output="{}_quant".format(node.output[0]),
-        quantized_bias_name=quantized_bias_initializer.name,
-        output_quantize_node=output_quantize_node,
-    )
-    model.graph.node.append(qadd_node)
+        # bias has same scale as future rescale op
+        rescale_scale = quantized_bias_scale
+        mul_input_node_name = qadd_node.name
+    else:
+        rescale_scale = _create_rescale_init(
+            node, input_quantize_params, weight_quantize_params
+        )
+        model.graph.initializer.append(rescale_scale)
+        # cast node should come directly after quantize op output instead of add
+        output_quantize_node = output_quantize_node or integer_op_node
+        mul_input_node_name = output_quantize_node.name
 
     # create Cast node and add it to graph
     cast_node = _create_cast_node(
         quant_add_name="{}_bias_add_quant".format(node.name),
         output_quantize_node=output_quantize_node,
     )
     model.graph.node.append(cast_node)
 
     # create Mul node for rescale
     mul_node = _create_mul_node(
         cast_node_output=cast_node.output[0],
-        quantized_bias_scale_name=quantized_bias_scale.name,
-        quant_add_name=qadd_node.name,
+        rescale_scale_name=rescale_scale.name,
+        input_node_name=mul_input_node_name,
         target_output=target_output,
+        model=model,
+        node_output_orig=node_output_orig,
     )
     model.graph.node.append(mul_node)
 
     return model
 
 
 def _create_mul_node(
     cast_node_output: str,
-    quantized_bias_scale_name: str,
-    quant_add_name: str,
+    rescale_scale_name: str,
+    input_node_name: str,
     target_output: str,
+    model: ModelProto,
+    node_output_orig: str,
 ) -> NodeProto:
     mul_node_inputs = [
         cast_node_output,  # a
-        quantized_bias_scale_name,  # b -> rescale factor
+        rescale_scale_name,  # b -> rescale factor
     ]
-    mul_node_name = "{}_rescale_mul".format(quant_add_name)
+    mul_node_name = "{}_rescale_mul".format(input_node_name)
+    if target_output is None:
+        target_output = mul_node_name
+        # since we skip the add conversion,
+        # update model to point all outputs of matmul/conv to the rescale mul
+        _update_model_input_id(model, node_output_orig, target_output)
     mul_node = onnx.helper.make_node(
         "Mul",
         mul_node_inputs,
         [target_output],
         mul_node_name,
     )
     return mul_node
 
 
+def _update_model_input_id(model: ModelProto, old_id: str, new_id: str):
+    for node in model.graph.node:
+        for idx, input_name in enumerate(node.input):
+            if input_name == old_id:
+                node.input[idx] = new_id
+
+
 def _create_cast_node(
     quant_add_name: str, output_quantize_node: Optional[NodeProto] = None
 ) -> NodeProto:
     quant_add_output = (
         output_quantize_node.output[0]
         if output_quantize_node
         else f"{quant_add_name}_output"
@@ -249,14 +285,23 @@
         numpy_helper.from_array(
             numpy.asarray(bias_zero_point, dtype=numpy.uint8),
             name=quantized_bias_zero_point_name,
         ),
     )
 
 
+def _create_rescale_init(
+    node, input_quantize_params, weight_quantize_params
+) -> TensorProto:
+    output_scale = input_quantize_params.scale * weight_quantize_params.scale
+    return numpy_helper.from_array(
+        numpy.asarray(output_scale), name=f"{node.name}_quant.rescale.scale"
+    )
+
+
 def _quantize_weight_initializer(
     node: NodeProto,
     weight_quantize_params: QuantizationParams,
     transpose_weight: bool = False,
 ) -> TensorProto:
     quantized_weight = quantize_array(
         weight_quantize_params.target,
```

## sparseml/pytorch/base.py

```diff
@@ -45,15 +45,15 @@
     "check_torchvision_install",
     "require_torch",
     "require_torchvision",
 ]
 
 
 _TORCH_MIN_VERSION = "1.0.0"
-_TORCH_MAX_VERSION = "1.13.100"  # set bug to 100 to support all future 1.9.X versions
+_TORCH_MAX_VERSION = "2.0.100"
 
 
 def check_torch_install(
     min_version: Optional[str] = _TORCH_MIN_VERSION,
     max_version: Optional[str] = _TORCH_MAX_VERSION,
     raise_on_error: bool = True,
 ) -> bool:
```

## sparseml/pytorch/image_classification/utils/helpers.py

```diff
@@ -15,15 +15,15 @@
 """
 Helper methods for image classification/detection based tasks
 """
 
 import logging
 import os
 import warnings
-from contextlib import contextmanager
+from contextlib import nullcontext
 from enum import Enum, auto, unique
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import torch
 from torch.nn import Module
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader, Dataset
@@ -258,15 +258,15 @@
     :param device: The device to use for the data loader. Required for ffcv
     :return: Tuple with the following format (dataset, dataloader)
     """
 
     download_context = (
         torch_distributed_zero_first(local_rank)  # only download once locally
         if training
-        else _nullcontext()
+        else nullcontext()
     )
     dataset_kwargs = dataset_kwargs or {}
 
     with download_context:
         dataset = DatasetRegistry.create(
             dataset_name,
             root=dataset_path,
@@ -616,16 +616,7 @@
             f" but got {recipe_stub} instead"
         )
 
     return download_framework_model_by_recipe_type(
         Model(recipe_stub),
         recipe_name=recipe_type,
     )
-
-
-@contextmanager
-def _nullcontext(enter_result=None):
-    """
-    A context manager that does nothing. For compatibility with Python 3.6
-    Update usages to use contextlib.nullcontext on Python 3.7+
-    """
-    yield enter_result
```

## sparseml/pytorch/sparsification/quantization/quantize_qat_export.py

```diff
@@ -564,18 +564,203 @@
         )
         model.graph.node.append(qmatmul_bias_add_node)
 
         # delete original Gemm node
         remove_node_and_params_from_graph(model, gemm_node)
 
 
-def _convert_quantizable_matmul(model: ModelProto):
+def _convert_quantizable_matmuls_with_nonquantized_outputs(model: ModelProto):
     """
-    A pass for converting a MatMul into a quantized representation
-    This MatMul is the result of quantizing native torch.matmul using QATMatMul
+    A pass for converting a MatMul with quantized inputs into
+    a MatMulInteger
+
+    | Starting with:
+    |          INPUT_0           INPUT_1
+    |            |               |
+    |     QuantizeLinear     QuantizeLinear
+    |            |               |
+    |     DequantizeLinear   DequantizeLinear
+    |                  |      |
+    |                   MatMul
+    |                     |
+    |                    Add (optional)
+    |                     |
+    |                  OUTPUT
+    | We end up converting to:
+    |          INPUT_0           INPUT_1
+    |            |               |
+    |     QuantizeLinear     QuantizeLinear
+    |                  |      |
+    |                  |      |
+    |                MatMulInteger
+    |                     |
+    |                    Add (Optional)
+    |                     |
+    |                    Cast (Int32 --> FP32)
+    |                     |
+    |                    Mul
+    |                     |
+    |                  OUTPUT
+    """
+
+    conversion_count = 0
+    matmul_nodes = [n for n in model.graph.node if n.op_type in ["MatMul"]]
+    graph = ONNXGraph(model)
+    for matmul_node in matmul_nodes:
+        #############
+        # Matching
+        #############
+
+        input_dequantize_nodes = [
+            graph.get_node_single_parent(matmul_node, i) for i in range(2)
+        ]
+
+        # Make sure these input nodes are DequantizeLinear
+        if numpy.any(
+            [
+                (node is None or node.op_type != "DequantizeLinear")
+                for node in input_dequantize_nodes
+            ]
+        ):
+            continue
+
+        # Make sure their parents are QuantizeLinear
+        parents = [
+            graph.get_node_single_parent(node, 0) for node in input_dequantize_nodes
+        ]
+        if numpy.any(
+            [
+                (parent is None or parent.op_type != "QuantizeLinear")
+                for parent in parents
+            ]
+        ):
+            continue
+
+        _LOGGER.debug(f"Matched quantizable MatMul: {matmul_node.name}")
+
+        # Create MatMulInteger node
+        node_0, node_1 = input_dequantize_nodes
+
+        input_nodes = [
+            node_0.input[0],  # a
+            node_1.input[0],  # b
+            node_0.input[2],  # a_zero_point
+            node_1.input[2],  # b_zero_point
+        ]
+
+        matmul_int_op_node = onnx.helper.make_node(
+            "MatMulInteger",
+            input_nodes,
+            [f"{matmul_node.name}_quant_out"],
+            f"{matmul_node.name}_quant",
+        )
+        model.graph.node.append(matmul_int_op_node)
+
+        node_0_parameters = get_quantization_params(model, node_0)
+        node_1_parameters = get_quantization_params(model, node_1)
+
+        output_scale = node_0_parameters.scale * node_1_parameters.scale
+
+        has_bias = False
+
+        # Check if is followed by Add node (bias)
+        bias_add_node = graph.get_node_single_child(matmul_node)
+        if bias_add_node is not None and bias_add_node.op_type == "Add":
+            bias_initializer = get_init_by_name(
+                model, bias_add_node.input[1]
+            ) or get_init_by_name(model, bias_add_node.input[0])
+            if bias_initializer is not None:
+                # check if bias is finite
+                bias_initializer = numpy_helper.to_array(bias_initializer)
+                if numpy.all(numpy.isfinite(bias_initializer)):
+                    # Create initializer for quantized bias
+                    quantized_bias_initializer_name = f"{bias_initializer.name}_quant"
+                    has_bias = True
+
+                    bias_zero_point = 0
+                    quantized_bias = _quantize_array(
+                        bias_initializer,
+                        output_scale,
+                        bias_zero_point,
+                        dtype=numpy.int32,
+                    )
+                    quantized_bias_initializer = numpy_helper.from_array(
+                        quantized_bias,
+                        name=quantized_bias_initializer_name,
+                    )
+                    model.graph.initializer.append(quantized_bias_initializer)
+
+                    # Create new Add node for quantized bias
+                    quantized_add_node_name = f"{bias_add_node.name}_quant"
+                    quantized_add_node = onnx.helper.make_node(
+                        "Add",
+                        [matmul_int_op_node.output[0], quantized_bias_initializer_name],
+                        [f"{quantized_add_node_name}_output"],
+                        quantized_add_node_name,
+                    )
+                    model.graph.node.append(quantized_add_node)
+
+        # Casting MatMulInteger INT32 output to FP32
+
+        cast_node_name = f"{matmul_node.name}_cast"
+        cast_node_input = (
+            quantized_add_node.output if has_bias else matmul_int_op_node.output
+        )
+        cast_node = onnx.helper.make_node(
+            "Cast",
+            cast_node_input,
+            [f"{cast_node_name}_output"],
+            cast_node_name,
+            to=getattr(onnx.TensorProto, "FLOAT"),  # get Float32 enum id
+        )
+        model.graph.node.append(cast_node)
+
+        output_scale_initializer_name = f"{matmul_node.name}.output_scale"
+        model.graph.initializer.append(
+            numpy_helper.from_array(
+                numpy.asarray(output_scale),
+                name=output_scale_initializer_name,
+            )
+        )
+
+        mul_node_output = bias_add_node.output if has_bias else matmul_node.output
+        mul_node = onnx.helper.make_node(
+            "Mul",
+            [cast_node.output[0], output_scale_initializer_name],
+            mul_node_output,
+            f"{matmul_node.name}_scale",
+        )
+        model.graph.node.append(mul_node)
+
+        for node in input_dequantize_nodes:
+            delete_quant_node(model, node)
+
+        # delete original MatMul node
+        remove_node_and_params_from_graph(model, matmul_node)
+
+        # delete original Add node
+        if has_bias:
+            remove_node_and_params_from_graph(model, bias_add_node)
+
+        conversion_count += 1
+
+    if matmul_nodes:
+        _LOGGER.info(
+            f"Converted {conversion_count} quantizable MatMul "
+            "(A8A8 inputs, FP output) ops to MatMulInteger"
+        )
+        graph = ONNXGraph(model)
+        graph.delete_unused_initializers()
+
+
+def _convert_quantizable_matmul_with_quantized_outputs(model: ModelProto):
+    """
+    A pass for converting a MatMul with quantized inputs and outputs into
+    a QLinearMatMul. This MatMul is the result of quantizing native
+    torch.matmul using QATMatMul
 
     | Starting with:
     |          INPUT_0           INPUT_1
     |            |               |
     |     QuantizeLinear     QuantizeLinear
     |            |               |
     |     DequantizeLinear   DequantizeLinear
@@ -728,17 +913,25 @@
         remove_node_and_params_from_graph(model, matmul_node)
 
         conversion_count += 1
         graph = ONNXGraph(model)
 
     if matmul_nodes:
         _LOGGER.info(
-            f"Converted {conversion_count} quantizable MatMul ops " "to QLinearMatMul"
+            f"Converted {conversion_count} quantizable MatMul with quantized outputs "
+            "to QLinearMatMul"
         )
 
+    return conversion_count
+
+
+def _convert_quantizable_matmul(model: ModelProto):
+    _convert_quantizable_matmul_with_quantized_outputs(model)
+    _convert_quantizable_matmuls_with_nonquantized_outputs(model)
+
 
 def _add_quantized_conv_matmul_add_ops(
     model: ModelProto,
     node: NodeProto,
     input_quantize_node: NodeProto,
     weight_quantize_node: NodeProto,
     input_quantize_params: QuantizationParams,
```

## sparseml/transformers/export.py

```diff
@@ -84,29 +84,29 @@
 from transformers.tokenization_utils_base import PaddingStrategy
 
 from sparseml.optim import parse_recipe_variables
 from sparseml.pytorch.optim import ScheduledModifierManager
 from sparseml.pytorch.utils import export_onnx
 from sparseml.transformers.sparsification import Trainer
 from sparseml.transformers.utils import SparseAutoModel
+from sparsezoo.utils.onnx import EXTERNAL_ONNX_DATA_NAME
 
 
 __all__ = ["export_transformer_to_onnx", "load_task_model"]
 
 MODEL_ONNX_NAME = "model.onnx"
 MANDATORY_DEPLOYMENT_FILES = [
     MODEL_ONNX_NAME,
     "tokenizer_config.json",
     "config.json",
 ]
-EXTERNAL_ONNX_DATA_NAME = ["model.data"]
 OPT_TOKENIZER_FILES = ["special_tokens_map.json", "vocab.json", "merges.txt"]
 
 OPTIONAL_DEPLOYMENT_FILES: List[str] = ["tokenizer.json"]
-OPTIONAL_DEPLOYMENT_FILES.extend(EXTERNAL_ONNX_DATA_NAME)
+OPTIONAL_DEPLOYMENT_FILES.append(EXTERNAL_ONNX_DATA_NAME)
 OPTIONAL_DEPLOYMENT_FILES.extend(OPT_TOKENIZER_FILES)
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 @dataclass
```

## Comparing `sparseml_nightly-1.6.0.20230608.dist-info/LICENSE` & `sparseml_nightly-1.6.0.20230616.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230608.dist-info/METADATA` & `sparseml_nightly-1.6.0.20230616.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml-nightly
-Version: 1.6.0.20230608
+Version: 1.6.0.20230616
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7.0,<3.11
+Requires-Python: >=3.8.0,<3.11
 Description-Content-Type: text/markdown
 Requires-Dist: sparsezoo-nightly (~=1.6.0)
 Requires-Dist: setuptools (<=59.5.0)
 Requires-Dist: jupyter (>=1.0.0)
 Requires-Dist: ipywidgets (>=7.0.0)
 Requires-Dist: pyyaml (>=5.0.0)
 Requires-Dist: progressbar2 (>=3.0.0)
@@ -87,40 +87,40 @@
 Requires-Dist: tensorboard (<2.0.0) ; extra == 'tf_v1'
 Requires-Dist: tf2onnx (<1.6,>=1.0.0) ; extra == 'tf_v1'
 Provides-Extra: tf_v1_gpu
 Requires-Dist: tensorflow-gpu (<2.0.0) ; extra == 'tf_v1_gpu'
 Requires-Dist: tensorboard (<2.0.0) ; extra == 'tf_v1_gpu'
 Requires-Dist: tf2onnx (<1.6,>=1.0.0) ; extra == 'tf_v1_gpu'
 Provides-Extra: torch
-Requires-Dist: torch (<1.14,>=1.7.0) ; extra == 'torch'
+Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'torch'
 Requires-Dist: gputils ; extra == 'torch'
 Provides-Extra: torch_all
-Requires-Dist: torch (<1.14,>=1.7.0) ; extra == 'torch_all'
+Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'torch_all'
 Requires-Dist: gputils ; extra == 'torch_all'
-Requires-Dist: torchvision (<0.15,>=0.3.0) ; extra == 'torch_all'
-Requires-Dist: torchaudio (<=0.13) ; extra == 'torch_all'
+Requires-Dist: torchvision (<=0.15.1,>=0.3.0) ; extra == 'torch_all'
+Requires-Dist: torchaudio (<=2.0.1) ; extra == 'torch_all'
 Provides-Extra: torchvision
-Requires-Dist: torch (<1.14,>=1.7.0) ; extra == 'torchvision'
+Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'torchvision'
 Requires-Dist: gputils ; extra == 'torchvision'
-Requires-Dist: torchvision (<0.15,>=0.3.0) ; extra == 'torchvision'
+Requires-Dist: torchvision (<=0.15.1,>=0.3.0) ; extra == 'torchvision'
 Requires-Dist: opencv-python (<=4.6.0.66) ; extra == 'torchvision'
 Provides-Extra: transformers
-Requires-Dist: torch (<1.14,>=1.7.0) ; extra == 'transformers'
+Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'transformers'
 Requires-Dist: gputils ; extra == 'transformers'
 Requires-Dist: nm-transformers-nightly (~=1.6.0) ; extra == 'transformers'
 Requires-Dist: datasets (<=1.18.4) ; extra == 'transformers'
 Requires-Dist: scikit-learn ; extra == 'transformers'
 Requires-Dist: seqeval ; extra == 'transformers'
 Provides-Extra: ultralytics
 Requires-Dist: ultralytics (==8.0.30) ; extra == 'ultralytics'
-Requires-Dist: torch (<1.14,>=1.7.0) ; extra == 'ultralytics'
+Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'ultralytics'
 Provides-Extra: yolov5
-Requires-Dist: torch (<1.14,>=1.7.0) ; extra == 'yolov5'
+Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'yolov5'
 Requires-Dist: gputils ; extra == 'yolov5'
-Requires-Dist: torchvision (<0.15,>=0.3.0) ; extra == 'yolov5'
+Requires-Dist: torchvision (<=0.15.1,>=0.3.0) ; extra == 'yolov5'
 Requires-Dist: opencv-python (<=4.6.0.66) ; extra == 'yolov5'
 Requires-Dist: nm-yolov5-nightly (~=1.6.0) ; extra == 'yolov5'
 
 <!--
 Copyright (c) 2021 - present / Neuralmagic, Inc. All Rights Reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -222,15 +222,15 @@
 
 - [PyTorch](integrations/torchvision#tutorials)
 - [Hugging Face Transformers](integrations/huggingface-transformers#tutorials)
 - [Ultralytics YOLOv5](integrations/ultralytics-yolov5#tutorials)
 
 ## Installation
 
-This repository is tested on Python 3.7-3.10, and Linux/Debian systems.
+This repository is tested on Python 3.8-3.10, and Linux/Debian systems.
 
 It is recommended to install in a [virtual environment](https://docs.python.org/3/library/venv.html) to keep your system in order.
 Currently supported ML Frameworks are the following: `torch>=1.1.0,<1.14`, `tensorflow>=1.8.0,<2.0.0`, `tensorflow.keras >= 2.2.0`.
 
 Install with pip using:
 
 ```bash
```

## Comparing `sparseml_nightly-1.6.0.20230608.dist-info/NOTICE` & `sparseml_nightly-1.6.0.20230616.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230608.dist-info/entry_points.txt` & `sparseml_nightly-1.6.0.20230616.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230608.dist-info/RECORD` & `sparseml_nightly-1.6.0.20230616.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -10,42 +10,46 @@
 sparseml/deepsparse/base.py,sha256=nRjU6TSao0J2iWXcdHwj62X6dVT9vl6TQ2y4Bdn3KN0,3516
 sparseml/deepsparse/framework/__init__.py,sha256=ZHrXXM3AMH78zKcF8Y40IBuy38UFy4fLrvytozw_bNY,801
 sparseml/deepsparse/framework/info.py,sha256=HVDPHFXggFeDqbpM20PkByf1nBccwKnjpTWh0EfrVas,6032
 sparseml/deepsparse/sparsification/__init__.py,sha256=re_2FtHWvO-iQQwRRJZDKz3l_pFZuwe266-4ZFxQqbY,813
 sparseml/deepsparse/sparsification/info.py,sha256=O5FJg5KMJvj-HcJn9W9iiKGZ6Z7_1SavOX-TstXRr6Q,1348
 sparseml/exporters/__init__.py,sha256=fH6rjBYAxuwrTzBTlTjTgCYNyh6TCvCqajCz4Im4YrA,617
 sparseml/exporters/base_exporter.py,sha256=M1HEe9GNf51uYx1z-qxWjIYo5iGZ_Ish8uZ3mj6OZR8,1477
+sparseml/exporters/kv_cache_injector.py,sha256=0SeVr1l_o3LZm_yFBv1s34Uz41sRXIezrN0uSUp-ZCw,6058
 sparseml/exporters/onnx_to_deepsparse.py,sha256=OO7WosKj8jtd-pSoh7RzaJh-ScWPHV7d-F75gOvJu08,4783
-sparseml/exporters/transforms/__init__.py,sha256=bitsfVa9RUFuZYVUD4oxEh_IqEyiQQuxIYaGA8rOt2w,2252
+sparseml/exporters/transforms/__init__.py,sha256=x0mpqLIbsRXjVVot0MH7ebFBmJwV_oZdOp7LhUEydI4,2276
 sparseml/exporters/transforms/base_transform.py,sha256=IpvdUdEADl2SfqHawcp6-lcNgz-R3L0zpS05WaWF5h8,2333
 sparseml/exporters/transforms/constants_to_initializers.py,sha256=_PX3y16OC-q85d-6DeOOVpKAAMNIU1m5BdYTZlFV_tk,1388
 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py,sha256=9z2HRqJAM68HPiSfu2RMyrn93dr8HCTpMcMrh_1-x2w,3866
 sparseml/exporters/transforms/conv_to_qlinearconv.py,sha256=CwCXtIBCOQ1qX5Z2JZhsdXSDk683wRCIBILF_1vd0GI,5838
 sparseml/exporters/transforms/delete_repeated_qdq.py,sha256=YiIOrvKqrxYboOA4A8YTbQIQ4s4MDdmqeLNYHPP4kjs,2440
 sparseml/exporters/transforms/delete_trivial_onnx_adds.py,sha256=St3-PQP8tPXYoyQTFn8fvJi7JF3LoX9Vb9nc-Zbx4Wg,1842
 sparseml/exporters/transforms/flatten_qparams.py,sha256=u0POagPJ_sqaS-DMe2x1Fd40RdlS9nYlLFZqHdsXx4Y,2181
 sparseml/exporters/transforms/fold_conv_div_bn.py,sha256=ckYdMKO2Z31NKRxQk4C4EbMWlVrsuhUDtyeMTMTErE4,3553
 sparseml/exporters/transforms/fold_identity_initializers.py,sha256=Yfv46MvL_vMxNGmUYSvlbucbrWIIDnjWnifmFCzyILA,1669
 sparseml/exporters/transforms/fold_relu_quants.py,sha256=qDGl-6aGmaQ8lAii3v0NvqkjbqtZB1UgHEkd3RzvjXQ,2070
 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py,sha256=r1oVnnu-U0mISkqBJrebXO1o-cmbkSMbo1X4xA0l-t4,4418
 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py,sha256=ccrB80ymufz6c9znwIGz0rxvM6U-vmKqiCa7l0vKYfE,7629
 sparseml/exporters/transforms/initializers_to_uint8.py,sha256=GxveAKe1xSNBZh1hjUx61veL6LTf9Msnx663Mrhvtxg,1645
-sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py,sha256=1YxX2xm2JC3IUj4AuRxRf2yXeOWj-esLLo-aoL_LtOo,4470
-sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py,sha256=l3JXoue_8Rs8DMGaH_MCNBR5RZRIzIhXiM5D_TRS81M,4571
+sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py,sha256=Fry6n_u6KMG6mwnrekP5nj5eHYL-T-SPFcjz6E6LUU4,4866
+sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py,sha256=5vPDFN9YHC5-0LYhv5_GI4ZBBRwYfPMhgv3MZEIUBqE,4681
 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py,sha256=Siii4mZ3LtqWY1blD1KT7ePVJud1oyLDrcr21YosU7E,4156
 sparseml/exporters/transforms/onnx_transform.py,sha256=vqlJJTjqZx9IUV3woHjKnWQMl2w-iurZK2eGABhYX9M,3724
 sparseml/exporters/transforms/propagate_embedding_quantization.py,sha256=XTEiUTX5nzLUtndGs_0t7nTgjIad-FyjuNc0O4f6Xro,3398
 sparseml/exporters/transforms/quantize_qat_embedding.py,sha256=_v1dEEt5vCSaMF6dJkg9fVGof145-_Lmo0DMjpXsnUE,4464
 sparseml/exporters/transforms/quantize_residuals.py,sha256=f3kNF930ymHI5CmCA0OmYW7vDKvEm9sYhN0UX0UC1EQ,3869
 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py,sha256=mod-7bnlkg20LjerZ7tKKmp_7XyO3FKo13BtIZkDsmM,3331
 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py,sha256=2FSXzaY3jdxOgj3xBaUOUqtk-hzg4kwhheELhoOKpS8,2545
 sparseml/exporters/transforms/skip_input_quantize.py,sha256=ANiYDwSos9gPW4960fMwmGubTDgpAcqFVSIHKf_ffYw,3210
 sparseml/exporters/transforms/unwrap_batchnorms.py,sha256=ly7GHCXN_2r8Gnk8PABWCqcoS-NL3GMfquEK0hRlFCs,1373
+sparseml/exporters/transforms/kv_cache/__init__.py,sha256=ykMEDNKJuV2jGlG1oydxopFrVD8U1h0AmSo22Um6vyk,807
+sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py,sha256=YYloawGYmaWfHe2Km5r86HahwTSksKlivt2R2qWvtlc,20939
+sparseml/exporters/transforms/kv_cache/position_embeddings_adjustment.py,sha256=pGThjU3jLGtgxXPAOxTC91oKerGhE6d1e0cSh--SSHw,6763
 sparseml/exporters/transforms/utils/__init__.py,sha256=tXSSUnzdyIc_H73xQ5dYhHb1Gj4Nb7GLLDVwJds8c_s,730
-sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py,sha256=lUutqioFTP3ZVa5IIA-Z5WbriNj_8m2mXut_QOyo_J0,8704
+sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py,sha256=I6kugQ0J9yHxCz7Yx3TlxQTUxcaAko4XkBDsQD7v5eo,10570
 sparseml/exporters/transforms/utils/helpers.py,sha256=vkEYL2Bdp_YNXlPg_TGd82Q2ef1EYEr11LVgmORQDiY,6457
 sparseml/exporters/transforms/utils/matching.py,sha256=CnVJLbJARBJwvFjoKh9vwYt6dLP4WXG3p7nCY5VUFaE,14429
 sparseml/framework/__init__.py,sha256=EcIX435yx552d7BkbxmAbQ_X3KAISInHVbD9X-AT1Uk,790
 sparseml/framework/info.py,sha256=TaZAMYdhBHcjl9Xyk3PWjJkDB6g3_f4vD3B6KmhgOl8,9479
 sparseml/keras/__init__.py,sha256=9D-eU-wi0UGuq55i2BTYDgS0mD6UJB10Gi8LQwh9KSk,1144
 sparseml/keras/base.py,sha256=yt1EO6KIeCkdg8rF37U5Y3FNGeAqOQLVGyxRANsyBy0,8054
 sparseml/keras/datasets/__init__.py,sha256=USLH-kFbXiubqgMW8IMkZfycVByQAOdAtzuPHzTok9I,943
@@ -115,15 +119,15 @@
 sparseml/optim/__init__.py,sha256=3oGQ4LY0MSrbTAwuyPHEOEyYiZ7JI7OX2BgWup5NPuw,882
 sparseml/optim/analyzer.py,sha256=LUYBYyvfVwaw_V1aAiOmaybUGJQk4vRK5RG3k3nD7pA,6302
 sparseml/optim/helpers.py,sha256=Zb7YPYe07vuVyYUhHJ-BlcMrZa-sxt1TUZ-Ec9Z6o_U,25563
 sparseml/optim/manager.py,sha256=KeDVHj9ea9EUaV908qfvq8ONwS8nUmAvQb1yXflOBWo,25984
 sparseml/optim/modifier.py,sha256=qYfVUL9thw94p4oEsNZgitUJ3y9izWYb8nUI3enyzOU,30708
 sparseml/optim/sensitivity.py,sha256=neMP_hTRqzDUV0MrATevC2-JQYnOIvNW_AlIf_y_ydw,26315
 sparseml/pytorch/__init__.py,sha256=3E40C1X1fjhlU0ZwdHZ-xhORHb-qDUtr7ALDv9xbzI0,1848
-sparseml/pytorch/base.py,sha256=-RvI-RM0ZynTCrsX0VaN_aoDPUdfCc1E1MeUY1VWFH8,6173
+sparseml/pytorch/base.py,sha256=C5ced9i5Y_fy-cnYkEFt6GuOGDHYu7fZ3pHrCm1W6mE,6117
 sparseml/pytorch/opset.py,sha256=-BsKarkkKfq09HYJLZfxt_AEHEfuENpRDZF_J2va1Ck,933
 sparseml/pytorch/torch_to_onnx_exporter.py,sha256=78Ft0yuGVKx3TMhPeG9e3o6dI2GC_432VwuiKokfZuc,10864
 sparseml/pytorch/datasets/__init__.py,sha256=2xoH_fCMojldFY1RCWSkt9pGfa8SzHAxU5em-_ZiwV8,998
 sparseml/pytorch/datasets/generic.py,sha256=nl-fFlpd7u5sNswe1AORZvQUne3sqrrPWnNgOUp6_Fc,4193
 sparseml/pytorch/datasets/registry.py,sha256=cEA3d5ju5EMft92f2StVLWARnAxlRpidKZaozujmFdE,2814
 sparseml/pytorch/datasets/classification/__init__.py,sha256=GMKhziJkRwSC7E_1Nox8FxnxhPFozZ6MxQWUWi1BN_Y,828
 sparseml/pytorch/datasets/classification/cifar.py,sha256=k32Z552YrrJv7IlshH8AWylaRKCOUC8KSrzRLLTHTag,4017
@@ -145,15 +149,15 @@
 sparseml/pytorch/image_classification/export.py,sha256=FG3TIe06X5PYlubyGmDjNKWBZHsX24wQ19gbqXMT3BQ,18265
 sparseml/pytorch/image_classification/lr_analysis.py,sha256=qweXU51KeWjW86RJknvsavKPPXMd3PGAO7bcGosjTqE,15494
 sparseml/pytorch/image_classification/pr_sensitivity.py,sha256=RA64lC4NOmFm2H11MO4HSuiw2ImtiRwvixtIw7Rol0o,14444
 sparseml/pytorch/image_classification/train.py,sha256=-My1yUclgRA5wQoV4B_jtoOMRO1nQj389WfDkebu3fs,29287
 sparseml/pytorch/image_classification/utils/__init__.py,sha256=ambjlzpSCaSZ7ZadPk2vMAB6kaZCm7f_hVqOVSWz8k8,682
 sparseml/pytorch/image_classification/utils/cli_helpers.py,sha256=qypcmjezy-fZn2Cjozv9vumZoB44_9PDe_WXnChbvLg,4278
 sparseml/pytorch/image_classification/utils/constants.py,sha256=k01fijyL2BicSWLL1EzhhdvG07WYMMXHZeFz-9fxecM,1257
-sparseml/pytorch/image_classification/utils/helpers.py,sha256=0VtpB5TFfPp8oNtSVlyAk70mTSOBmhbjnYCP49j-Jmg,20912
+sparseml/pytorch/image_classification/utils/helpers.py,sha256=_dfAcs5d1aftAB0cNnuA0lOqD_B3KxIv5m6prTQS3G8,20676
 sparseml/pytorch/image_classification/utils/trainer.py,sha256=2WOP42hSlowDG2_DyCZOu8T5yohhV38e192ZxeWXj_A,12056
 sparseml/pytorch/models/__init__.py,sha256=Lj1KLciXTQiZObA5HHgrPMHNQ1bGYswrsP776eizaUc,976
 sparseml/pytorch/models/registry.py,sha256=cJLPsK8zzhVyZPvcJ8_Kj9-Ru9lTOywv61xuE50LiC8,14753
 sparseml/pytorch/models/classification/__init__.py,sha256=opnCtf6WMl1kuQ_vRAZRLl1eFZefpG9GFc9o729HndQ,901
 sparseml/pytorch/models/classification/darknet.py,sha256=rR4XXQu7shLADU4Th0D-eodnv-Z3AmA6kj8tDgHmtxU,11658
 sparseml/pytorch/models/classification/efficientnet.py,sha256=Bs88xu2xX9P65TOZ_6rn_qO2CMa6oLsJm5xt-Y6gISI,40293
 sparseml/pytorch/models/classification/inception_v3.py,sha256=wxWU3ja6E0_ERhYniDlzcsnVWi-rvJVfgxmhsyrpuC4,16512
@@ -217,15 +221,15 @@
 sparseml/pytorch/sparsification/quantization/__init__.py,sha256=OjbeCzzhoeFJEJQvLmXZc89pghO83sLRhmvNF7_q_oQ,813
 sparseml/pytorch/sparsification/quantization/constants.py,sha256=sla-j0QwLFq92AbDZkHkNLxugpGrNEQJIuLWoWqV3Ks,2220
 sparseml/pytorch/sparsification/quantization/helpers.py,sha256=MmY5iOMlBUBEMrotPyj3H5drzpXhf13v4FJjb1N2aaw,32271
 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py,sha256=TToI4dGYZZEzB1q61m1YVg0THlvH7Ew1CZ2y-ajpTts,33626
 sparseml/pytorch/sparsification/quantization/modifier_quantization.py,sha256=LkHNB1IsiFlZugUecB4-LZMjWuoboFYf_PXPx6uPl1g,26778
 sparseml/pytorch/sparsification/quantization/quantization_scheme.py,sha256=10KNttNCHqUTNq706kPB6k7u6mvvfV0WTvx5D5Uqd-Y,12558
 sparseml/pytorch/sparsification/quantization/quantize.py,sha256=bqqH2qBEWYHfea5jzAHmz52uPddfRdmP3TFaCKgQqjM,17905
-sparseml/pytorch/sparsification/quantization/quantize_qat_export.py,sha256=9szHTgbPqgiZFw_dL3h_BXThUR2sklsSqiVQ4sQf-U0,70029
+sparseml/pytorch/sparsification/quantization/quantize_qat_export.py,sha256=6JLbd3NUy9J0_pygSypJZsPtfxLlY8ZFJfK7kJSRrSY,76796
 sparseml/pytorch/sparsification/training/__init__.py,sha256=4GGhQf6KVSOYwtr_WL9Xcvx4mR-k8yKMVI_zuTBHGO4,790
 sparseml/pytorch/sparsification/training/modifier_epoch.py,sha256=_5p1EZk2qbwTnWsMXbVan3vRj1IRyIM4wYYZdLGA5GE,1778
 sparseml/pytorch/sparsification/training/modifier_logging.py,sha256=K1NMqhea5EBPko6yim8CThShbiSJKN5P_ca_TCyZXto,2883
 sparseml/pytorch/sparsification/training/modifier_lr.py,sha256=m_tCydo_BHiXCHMUKZu6iqKLAP24acAT8-NLjH9RIlE,24287
 sparseml/pytorch/sparsification/training/modifier_params.py,sha256=G_0eVqu0Cup8WNLFhkfPmYnKtJlNrxcJt0FcOOdq9tA,21497
 sparseml/pytorch/sparsification/training/modifier_regularizer.py,sha256=ezHbcwI8ITgq4vwkzsWXgnq_ls6NONW_D8jEN-YR7u8,6690
 sparseml/pytorch/torchvision/__init__.py,sha256=fD0HjvgSO8WgfyPPSn7r_Fej6xWAelVJVbgWfI9ypY4,943
@@ -309,15 +313,15 @@
 sparseml/tensorflow_v1/utils/exporter.py,sha256=RqpSP-w21SrkA_ik9WoIWdIVAAui88AiBXxRWaDZJJs,10913
 sparseml/tensorflow_v1/utils/helpers.py,sha256=40eZgnejvIki_CdupK4V1gETAgGDE9rbEXEwuNg9ASA,996
 sparseml/tensorflow_v1/utils/loss.py,sha256=4AsXh70fjp1dDcxBUzgjjpLgndwVa1CBiMG1sYi5Was,1974
 sparseml/tensorflow_v1/utils/nets_utils.py,sha256=cOTKgw7PVPEjRVU-bvcsNLdBJGTi-A7djJaUaZQwsT4,8119
 sparseml/tensorflow_v1/utils/summary.py,sha256=A2ub7KDwzsaindIuCHa7N3cRpCU6d7QbD5uNHV-R6H8,1327
 sparseml/tensorflow_v1/utils/variable.py,sha256=6ziLaNOLnxQrSPWJ2RaINqg4w-4NK9reVJWH-weK3-k,12536
 sparseml/transformers/__init__.py,sha256=8J1vljjZiybTTdNXN9e9senxvZUmKXKHAB5-H4D_4nY,1511
-sparseml/transformers/export.py,sha256=SjYBxPPkuZAPEBqDeJNPZuDsmKAw_SzboUnAT1ClU64,21274
+sparseml/transformers/export.py,sha256=dcRG_1JeHCdym4zfyVUZQBDeG4aycBG7viEjQQojtZQ,21290
 sparseml/transformers/masked_language_modeling.py,sha256=xV1H7jyWCWMKTiow501cI498I5ouNC68nF7g-QNuzjw,30756
 sparseml/transformers/question_answering.py,sha256=E_Ljec9bNDrZ2KD3unTlbcRxEpyYU6C9asuEynhh4AQ,36557
 sparseml/transformers/text_classification.py,sha256=UYCpgSGTkmeGOeePQF5Idd8uY4GHQc-ShZK5SFOlP7E,40299
 sparseml/transformers/token_classification.py,sha256=6RUe1CmXQv7dHsE35aTg-xLW1g4BGakRp6pn0un2_mE,34350
 sparseml/transformers/sparsification/__init__.py,sha256=22XZNePvLFXNxp5NrcUIXzjgynCZm6jvQOErpRGlQNY,833
 sparseml/transformers/sparsification/question_answering.py,sha256=FAXhtQ8MW_2ar1dix2tQ1x1RXZuSWMLHZbVHToNWwmo,19529
 sparseml/transformers/sparsification/trainer.py,sha256=lylAxTy4WMmTqthB6ie4kUg1eIevSMIe11UcAO0WU9o,43772
@@ -355,14 +359,14 @@
 sparseml/yolov8/train.py,sha256=DeZMrZ_moAc3fIojJloq3IvQqiPC_cgPgTjYFSOoG7E,7194
 sparseml/yolov8/trainers.py,sha256=mzOuog5BmQg3tER3m35zqTcKRlxiw9IqCpgBy-Ep1sA,34788
 sparseml/yolov8/val.py,sha256=hlFImvknSpV1nONOxA3ivYgvzm64EmK0_Lh-JHLbOsw,2748
 sparseml/yolov8/validators.py,sha256=ytG7g_LOXvKFmxLPmQloT-wNf78convSoRRXVTYCR0Y,8196
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
 sparseml/yolov8/utils/export_samples.py,sha256=gn7et_J-OfnCTEYP0iLXx2W-HARgxqUnHqJWHBG72KM,6288
 sparseml/yolov8/utils/helpers.py,sha256=8JZNaTT1zPKiZaOccmMtQu5mXCSMGkq8BDEgUqaPVIs,4041
-sparseml_nightly-1.6.0.20230608.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml_nightly-1.6.0.20230608.dist-info/METADATA,sha256=EkTusfaRUQwBO-vLiYYRkox3Z5OIG2_ZofHVJl-Lw-8,21640
-sparseml_nightly-1.6.0.20230608.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml_nightly-1.6.0.20230608.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml_nightly-1.6.0.20230608.dist-info/entry_points.txt,sha256=KbSvJr3uXYQgZRF0Mzi5B89ijSwsiZalXMxinJRaass,2377
-sparseml_nightly-1.6.0.20230608.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml_nightly-1.6.0.20230608.dist-info/RECORD,,
+sparseml_nightly-1.6.0.20230616.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml_nightly-1.6.0.20230616.dist-info/METADATA,sha256=mbldDmE0rs01lQ8U9i7yYQQ1bq_cVkmu72tEVdd2lyo,21650
+sparseml_nightly-1.6.0.20230616.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml_nightly-1.6.0.20230616.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml_nightly-1.6.0.20230616.dist-info/entry_points.txt,sha256=KbSvJr3uXYQgZRF0Mzi5B89ijSwsiZalXMxinJRaass,2377
+sparseml_nightly-1.6.0.20230616.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml_nightly-1.6.0.20230616.dist-info/RECORD,,
```

