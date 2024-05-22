# Comparing `tmp/kimm-0.2.0.tar.gz` & `tmp/kimm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimm-0.2.0.tar", last modified: Thu May 16 09:29:44 2024, max compression
+gzip compressed data, was "kimm-0.2.1.tar", last modified: Wed May 22 03:28:56 2024, max compression
```

## Comparing `kimm-0.2.0.tar` & `kimm-0.2.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.044131 kimm-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 09:28:33.000000 kimm-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-16 09:29:44.044131 kimm-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-16 09:28:33.000000 kimm-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.028131 kimm-0.2.0/kimm/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.028131 kimm-0.2.0/kimm/_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.028131 kimm-0.2.0/kimm/_src/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/blocks/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/blocks/depthwise_separation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/blocks/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/blocks/squeeze_and_excitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/blocks/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.032132 kimm-0.2.0/kimm/_src/export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/export/export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/export/export_onnx_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/export/export_tflite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/export/export_tflite_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/kimm_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.032132 kimm-0.2.0/kimm/_src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/layer_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/layer_scale_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/learnable_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/learnable_affine_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/mobile_one_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/mobile_one_conv2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/position_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/rep_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/rep_conv2d_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.036131 kimm-0.2.0/kimm/_src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8660 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/convmixer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    29575 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/ghostnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    21491 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/hgnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/inception_next.py
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/mobileone.py
--rw-r--r--   0 runner    (1001) docker     (127)    26230 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/mobilevit.py
--rw-r--r--   0 runner    (1001) docker     (127)    19067 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/models_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18229 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/regnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/repvgg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/vgg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.036131 kimm-0.2.0/kimm/_src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/make_divisble.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/model_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/model_registry_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/model_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/timm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.036131 kimm-0.2.0/kimm/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.036131 kimm-0.2.0/kimm/export/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.036131 kimm-0.2.0/kimm/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.036131 kimm-0.2.0/kimm/models/
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/base_model/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/base_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/convmixer/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/convmixer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/ghostnet/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/ghostnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/hgnet/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/hgnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/inception_next/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/inception_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/mobileone/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/mobileone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/mobilevit/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/mobilevit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/regnet/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/regnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/repvgg/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/repvgg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/vgg/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/vgg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/vision_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/vision_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/timm_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/timm_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-16 09:29:44.000000 kimm-0.2.0/kimm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-16 09:29:44.000000 kimm-0.2.0/kimm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:29:44.000000 kimm-0.2.0/kimm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-16 09:29:44.000000 kimm-0.2.0/kimm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 09:29:44.000000 kimm-0.2.0/kimm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-16 09:28:33.000000 kimm-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:29:44.044131 kimm-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 03:27:34.000000 kimm-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-22 03:28:56.581305 kimm-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-22 03:27:34.000000 kimm-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.565304 kimm-0.2.1/kimm/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.565304 kimm-0.2.1/kimm/_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.569305 kimm-0.2.1/kimm/_src/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/blocks/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/blocks/depthwise_separation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/blocks/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/blocks/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.569305 kimm-0.2.1/kimm/_src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/export/export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/export/export_onnx_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/export/export_tflite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/export/export_tflite_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/kimm_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.569305 kimm-0.2.1/kimm/_src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/layer_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/layer_scale_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/learnable_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/learnable_affine_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/mobile_one_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/mobile_one_conv2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/position_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/rep_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/layers/rep_conv2d_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.573305 kimm-0.2.1/kimm/_src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/convmixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13058 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29473 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/ghostnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21389 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/hgnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10395 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/inception_next.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/mobileone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26900 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/mobilevit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22811 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18127 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/regnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/repvgg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/vgg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/models/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/_src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/make_divisble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/model_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/model_registry_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/model_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/utils/timm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/_src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/base_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/base_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/convmixer/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/convmixer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/ghostnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/ghostnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/hgnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/hgnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/inception_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/inception_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.577304 kimm-0.2.1/kimm/models/mobileone/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/mobileone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/mobilevit/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/mobilevit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/regnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/regnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/repvgg/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/repvgg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/vgg/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/vgg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/vision_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/vision_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/models/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/models/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/timm_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/timm_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-22 03:27:34.000000 kimm-0.2.1/kimm/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:28:56.581305 kimm-0.2.1/kimm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-22 03:28:56.000000 kimm-0.2.1/kimm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-22 03:28:56.000000 kimm-0.2.1/kimm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 03:28:56.000000 kimm-0.2.1/kimm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-22 03:28:56.000000 kimm-0.2.1/kimm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 03:28:56.000000 kimm-0.2.1/kimm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-22 03:27:34.000000 kimm-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 03:28:56.581305 kimm-0.2.1/setup.cfg
```

### Comparing `kimm-0.2.0/LICENSE` & `kimm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/PKG-INFO` & `kimm-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimm
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Keras model zoo with pretrained weights.
 Author-email: Hong-Yu Chiu <james77777778@gmail.com>
 Maintainer-email: Hong-Yu Chiu <james77777778@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/james77777778/keras-image-models
 Project-URL: Documentation, https://github.com/james77777778/keras-image-models
 Project-URL: Repository, https://github.com/james77777778/keras-image-models.git
```

### Comparing `kimm-0.2.0/README.md` & `kimm-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/blocks/conv2d.py` & `kimm-0.2.1/kimm/_src/blocks/conv2d.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/blocks/depthwise_separation.py` & `kimm-0.2.1/kimm/_src/blocks/depthwise_separation.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/blocks/inverted_residual.py` & `kimm-0.2.1/kimm/_src/blocks/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/blocks/squeeze_and_excitation.py` & `kimm-0.2.1/kimm/_src/blocks/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/blocks/transformer.py` & `kimm-0.2.1/kimm/_src/blocks/transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,40 +47,39 @@
 @kimm_export(parent_path=["kimm.blocks"])
 def apply_transformer_block(
     inputs,
     dim: int,
     num_heads: int,
     mlp_ratio: float = 4.0,
     use_qkv_bias: bool = False,
-    use_qk_norm: bool = False,
     projection_dropout_rate: float = 0.0,
     attention_dropout_rate: float = 0.0,
     activation: str = "gelu",
     name: str = "transformer_block",
 ):
+    # data_format must be "channels_last"
     x = inputs
     residual_1 = x
 
     x = layers.LayerNormalization(epsilon=1e-6, name=f"{name}_norm1")(x)
     x = Attention(
         dim,
         num_heads,
         use_qkv_bias,
-        use_qk_norm,
         attention_dropout_rate,
         projection_dropout_rate,
         name=f"{name}_attn",
     )(x)
     x = layers.Add()([residual_1, x])
 
     residual_2 = x
     x = layers.LayerNormalization(epsilon=1e-6, name=f"{name}_norm2")(x)
     x = apply_mlp_block(
         x,
         int(dim * mlp_ratio),
         activation=activation,
         dropout_rate=projection_dropout_rate,
-        data_format="channels_last",  # TODO: let backend decides
+        data_format="channels_last",
         name=f"{name}_mlp",
     )
     x = layers.Add()([residual_2, x])
     return x
```

### Comparing `kimm-0.2.0/kimm/_src/export/export_onnx.py` & `kimm-0.2.1/kimm/_src/export/export_onnx.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/export/export_onnx_test.py` & `kimm-0.2.1/kimm/_src/export/export_onnx_test.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/export/export_tflite.py` & `kimm-0.2.1/kimm/_src/export/export_tflite.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/export/export_tflite_test.py` & `kimm-0.2.1/kimm/_src/export/export_tflite_test.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/kimm_export.py` & `kimm-0.2.1/kimm/_src/kimm_export.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/layers/attention.py` & `kimm-0.2.1/kimm/_src/layers/attention.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,42 @@
 import keras
+from keras import InputSpec
 from keras import layers
 from keras import ops
 
 from kimm._src.kimm_export import kimm_export
 
 
 @kimm_export(parent_path=["kimm.layers"])
 @keras.saving.register_keras_serializable(package="kimm")
 class Attention(layers.Layer):
     def __init__(
         self,
         hidden_dim: int,
         num_heads: int = 8,
         use_qkv_bias: bool = False,
-        use_qk_norm: bool = False,
         attention_dropout_rate: float = 0.0,
         projection_dropout_rate: float = 0.0,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.hidden_dim = hidden_dim
         self.num_heads = num_heads
         self.head_dim = hidden_dim // num_heads
         self.scale = self.head_dim ** (-0.5)
         self.use_qkv_bias = use_qkv_bias
-        self.use_qk_norm = use_qk_norm
         self.attention_dropout_rate = attention_dropout_rate
         self.projection_dropout_rate = projection_dropout_rate
 
         self.qkv = layers.Dense(
             hidden_dim * 3,
             use_bias=use_qkv_bias,
             dtype=self.dtype_policy,
             name=f"{self.name}_qkv",
         )
-        if use_qk_norm:
-            self.q_norm = layers.LayerNormalization(
-                dtype=self.dtype_policy, name=f"{self.name}_q_norm"
-            )
-            self.k_norm = layers.LayerNormalization(
-                dtype=self.dtype_policy, name=f"{self.name}_k_norm"
-            )
-        else:
-            self.q_norm = layers.Identity(dtype=self.dtype_policy)
-            self.k_norm = layers.Identity(dtype=self.dtype_policy)
 
         self.attention_dropout = layers.Dropout(
             attention_dropout_rate,
             dtype=self.dtype_policy,
             name=f"{self.name}_attn_drop",
         )
         self.projection = layers.Dense(
@@ -56,68 +45,84 @@
         self.projection_dropout = layers.Dropout(
             projection_dropout_rate,
             dtype=self.dtype_policy,
             name=f"{self.name}_proj_drop",
         )
 
     def build(self, input_shape):
+        self.input_spec = InputSpec(ndim=len(input_shape))
+        if self.input_spec.ndim not in (3, 4):
+            raise ValueError(
+                "The ndim of the inputs must be 3 or 4. "
+                f"Received: input_shape={input_shape}"
+            )
+
         self.qkv.build(input_shape)
         qkv_output_shape = list(input_shape)
         qkv_output_shape[-1] = qkv_output_shape[-1] * 3
-        self.q_norm.build(qkv_output_shape)
-        self.k_norm.build(qkv_output_shape)
         attention_input_shape = [
             input_shape[0],
             self.num_heads,
             input_shape[1],
             input_shape[1],
         ]
         self.attention_dropout.build(attention_input_shape)
         self.projection.build(input_shape)
         self.projection_dropout.build(input_shape)
         self.built = True
 
     def call(self, inputs, training=None, mask=None):
         input_shape = ops.shape(inputs)
         qkv = self.qkv(inputs)
-        qkv = ops.reshape(
-            qkv,
-            [
-                input_shape[0],
-                input_shape[1],
-                3,
-                self.num_heads,
-                self.head_dim,
-            ],
-        )
-        qkv = ops.transpose(qkv, [2, 0, 3, 1, 4])
-        q, k, v = ops.unstack(qkv, 3, axis=0)
-        q = self.q_norm(q)
-        k = self.k_norm(k)
+        if self.input_spec.ndim == 3:
+            qkv = ops.reshape(
+                qkv,
+                [
+                    input_shape[0],
+                    input_shape[1],
+                    3,
+                    self.num_heads,
+                    self.head_dim,
+                ],
+            )
+            qkv = ops.transpose(qkv, [0, 3, 2, 1, 4])
+            q, k, v = ops.unstack(qkv, 3, axis=2)
+        else:
+            # self.input_spec.ndim==4
+            qkv = ops.reshape(
+                qkv,
+                [
+                    input_shape[0],
+                    input_shape[1],
+                    input_shape[2],
+                    3,
+                    self.num_heads,
+                    self.head_dim,
+                ],
+            )
+            qkv = ops.transpose(qkv, [0, 1, 4, 3, 2, 5])
+            q, k, v = ops.unstack(qkv, 3, axis=3)
 
         # attention
         q = ops.multiply(q, self.scale)
         attn = ops.matmul(q, ops.swapaxes(k, -2, -1))
         attn = ops.softmax(attn)
         attn = self.attention_dropout(attn)
         x = ops.matmul(attn, v)
-
-        x = ops.swapaxes(x, 1, 2)
-        x = ops.reshape(x, input_shape)
+        x = ops.reshape(ops.swapaxes(x, -3, -2), input_shape)
         x = self.projection(x)
         x = self.projection_dropout(x)
         return x
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "hidden_dim": self.hidden_dim,
                 "num_heads": self.num_heads,
                 "use_qkv_bias": self.use_qkv_bias,
-                "use_qk_norm": self.use_qk_norm,
                 "attention_dropout_rate": self.attention_dropout_rate,
                 "projection_dropout_rate": self.projection_dropout_rate,
                 "name": self.name,
             }
         )
         return config
```

### Comparing `kimm-0.2.0/kimm/_src/layers/attention_test.py` & `kimm-0.2.1/kimm/_src/layers/layer_scale_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pytest
 from absl.testing import parameterized
 from keras.src import testing
 
-from kimm._src.layers.attention import Attention
+from kimm._src.layers.layer_scale import LayerScale
 
 
-class AttentionTest(testing.TestCase, parameterized.TestCase):
+class LayerScaleTest(testing.TestCase, parameterized.TestCase):
     @pytest.mark.requires_trainable_backend
-    def test_attention_basic(self):
+    def test_basic(self):
         self.run_layer_test(
-            Attention,
-            init_kwargs={"hidden_dim": 20, "num_heads": 2},
-            input_shape=(1, 10, 20),
-            expected_output_shape=(1, 10, 20),
-            expected_num_trainable_weights=3,
+            LayerScale,
+            init_kwargs={"axis": -1},
+            input_shape=(1, 10),
+            expected_output_shape=(1, 10),
+            expected_num_trainable_weights=1,
             expected_num_non_trainable_weights=0,
             expected_num_losses=0,
             supports_masking=False,
         )
```

### Comparing `kimm-0.2.0/kimm/_src/layers/layer_scale.py` & `kimm-0.2.1/kimm/_src/layers/layer_scale.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/layers/layer_scale_test.py` & `kimm-0.2.1/kimm/_src/layers/learnable_affine_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pytest
 from absl.testing import parameterized
 from keras.src import testing
 
-from kimm._src.layers.layer_scale import LayerScale
+from kimm._src.layers.learnable_affine import LearnableAffine
 
 
-class LayerScaleTest(testing.TestCase, parameterized.TestCase):
+class LearnableAffineTest(testing.TestCase, parameterized.TestCase):
     @pytest.mark.requires_trainable_backend
-    def test_layer_scale_basic(self):
+    def test_basic(self):
         self.run_layer_test(
-            LayerScale,
-            init_kwargs={"axis": -1},
+            LearnableAffine,
+            init_kwargs={"scale_value": 1.0, "bias_value": 0.0},
             input_shape=(1, 10),
             expected_output_shape=(1, 10),
-            expected_num_trainable_weights=1,
+            expected_num_trainable_weights=2,
             expected_num_non_trainable_weights=0,
             expected_num_losses=0,
             supports_masking=False,
         )
```

### Comparing `kimm-0.2.0/kimm/_src/layers/learnable_affine.py` & `kimm-0.2.1/kimm/_src/layers/learnable_affine.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/layers/mobile_one_conv2d.py` & `kimm-0.2.1/kimm/_src/layers/mobile_one_conv2d.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/layers/mobile_one_conv2d_test.py` & `kimm-0.2.1/kimm/_src/layers/mobile_one_conv2d_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     },
 ]
 
 
 class MobileOneConv2DTest(testing.TestCase, parameterized.TestCase):
     @parameterized.parameters(TEST_CASES)
     @pytest.mark.requires_trainable_backend
-    def test_mobile_one_conv2d_basic(
+    def test_basic(
         self,
         filters,
         kernel_size,
         has_skip,
         use_depthwise,
         branch_size,
         data_format,
@@ -109,15 +109,15 @@
             expected_num_trainable_weights=num_trainable_weights,
             expected_num_non_trainable_weights=num_non_trainable_weights,
             expected_num_losses=0,
             supports_masking=False,
         )
 
     @parameterized.parameters(TEST_CASES)
-    def test_mobile_one_conv2d_get_reparameterized_weights(
+    def test_get_reparameterized_weights(
         self,
         filters,
         kernel_size,
         has_skip,
         use_depthwise,
         branch_size,
         data_format,
```

### Comparing `kimm-0.2.0/kimm/_src/layers/rep_conv2d.py` & `kimm-0.2.1/kimm/_src/layers/rep_conv2d.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/layers/rep_conv2d_test.py` & `kimm-0.2.1/kimm/_src/layers/rep_conv2d_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     },
 ]
 
 
 class RepConv2DTest(testing.TestCase, parameterized.TestCase):
     @parameterized.parameters(TEST_CASES)
     @pytest.mark.requires_trainable_backend
-    def test_rep_conv2d_basic(
+    def test_basic(
         self,
         filters,
         kernel_size,
         has_skip,
         data_format,
         input_shape,
         output_shape,
@@ -85,15 +85,15 @@
             expected_num_trainable_weights=num_trainable_weights,
             expected_num_non_trainable_weights=num_non_trainable_weights,
             expected_num_losses=0,
             supports_masking=False,
         )
 
     @parameterized.parameters(TEST_CASES)
-    def test_rep_conv2d_get_reparameterized_weights(
+    def test_get_reparameterized_weights(
         self,
         filters,
         kernel_size,
         has_skip,
         data_format,
         input_shape,
         output_shape,
```

### Comparing `kimm-0.2.0/kimm/_src/models/__init__.py` & `kimm-0.2.1/kimm/_src/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/models/base_model.py` & `kimm-0.2.1/kimm/_src/models/base_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,94 +10,94 @@
 from keras.src.applications import imagenet_utils
 
 from kimm._src.kimm_export import kimm_export
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.base_model"])
 class BaseModel(models.Model):
-    default_origin = (
-        "https://github.com/james77777778/kimm/releases/download/0.1.0/"
-    )
+    default_origin = "https://github.com/james77777778/keras-image-models/releases/download/0.1.0/"
     available_feature_keys = []
     available_weights = []
 
     def __init__(
         self,
         inputs,
         outputs,
         features: typing.Optional[typing.Dict[str, KerasTensor]] = None,
         **kwargs,
     ):
+        self._check_feature_extractor_setting(features)
         _include_top = getattr(self, "_include_top", True)
-        if not hasattr(self, "_feature_extractor"):
+        if self._feature_extractor:
+            if self._feature_keys is None:
+                self._feature_keys = list(features.keys())
+            filtered_features = {}
+            for k in self._feature_keys:
+                filtered_features[k] = features[k]
+            # Add outputs
+            if _include_top and backend.is_keras_tensor(outputs):
+                filtered_features["TOP"] = outputs
+            super().__init__(inputs=inputs, outputs=filtered_features, **kwargs)
+        else:
             del features
             super().__init__(inputs=inputs, outputs=outputs, **kwargs)
-        else:
-            if not hasattr(self, "_feature_keys"):
-                raise AttributeError(
-                    "`self._feature_keys` must be set when initializing "
-                    "BaseModel"
+
+        if hasattr(self, "_weights"):
+            self.load_pretrained_weights(self._weights)
+
+    def _check_feature_extractor_setting(self, features):
+        if not hasattr(self, "_feature_keys"):
+            raise AttributeError(
+                "`self._feature_keys` must be set when initializing "
+                "BaseModel"
+            )
+        if self._feature_extractor:
+            if features is None:
+                raise ValueError(
+                    "`features` must be set when `feature_extractor=True`. "
+                    f"Received features={features}"
                 )
-            if self._feature_extractor:
-                if features is None:
-                    raise ValueError(
-                        "`features` must be set when `feature_extractor=True`. "
-                        f"Received features={features}"
+            _feature_keys = self._feature_keys
+            if _feature_keys is None:
+                _feature_keys = list(features.keys())
+            for k in _feature_keys:
+                if k not in features:
+                    raise KeyError(
+                        f"'{k}' is not a key of `features`. Available keys "
+                        f"are: {list(features.keys())}"
                     )
-                if self._feature_keys is None:
-                    self._feature_keys = list(features.keys())
-                filtered_features = {}
-                for k in self._feature_keys:
-                    if k not in features:
-                        raise KeyError(
-                            f"'{k}' is not a key of `features`. Available keys "
-                            f"are: {list(features.keys())}"
-                        )
-                    filtered_features[k] = features[k]
-                # Add outputs
-                if _include_top and backend.is_keras_tensor(outputs):
-                    filtered_features["TOP"] = outputs
-                super().__init__(
-                    inputs=inputs, outputs=filtered_features, **kwargs
-                )
-            else:
-                del features
-                super().__init__(inputs=inputs, outputs=outputs, **kwargs)
-
-        if hasattr(self, "_weights_url"):
-            self.load_pretrained_weights(self._weights_url)
 
     def set_properties(
         self, kwargs: typing.Dict[str, typing.Any], default_size: int = 224
     ):
         """Must be called in the initilization of the class.
 
         This method will add following common properties to the model object:
         - input_shape
         - include_preprocessing
         - include_top
         - pooling
         - dropout_rate
         - classes
         - classifier_activation
-        - _weights
-        - weights_url
+        - weights
         - default_size
+        - feature_extractor
+        - feature_keys
         """
         self._input_shape = kwargs.pop("input_shape", None)
         self._include_preprocessing = kwargs.pop("include_preprocessing", True)
         self._include_top = kwargs.pop("include_top", True)
         self._pooling = kwargs.pop("pooling", None)
         self._dropout_rate = kwargs.pop("dropout_rate", 0.0)
         self._classes = kwargs.pop("classes", 1000)
         self._classifier_activation = kwargs.pop(
             "classifier_activation", "softmax"
         )
-        self._weights = kwargs.pop("weights", None)
-        self._weights_url = kwargs.pop("weights_url", None)
+        self._weights = self.parse_weights(kwargs.pop("weights", None))
         self._default_size = kwargs.pop("default_size", default_size)
         # feature extractor
         self._feature_extractor = kwargs.pop("feature_extractor", False)
         self._feature_keys = kwargs.pop("feature_keys", None)
 
     def determine_input_tensor(
         self,
@@ -105,37 +105,64 @@
         input_shape: typing.Optional[typing.Sequence[int]] = None,
         default_size: int = 224,
         min_size: int = 32,
         require_flatten: bool = False,
         static_shape: bool = False,
     ):
         """Determine the input tensor by the arguments."""
-        input_shape = imagenet_utils.obtain_input_shape(
-            input_shape,
-            default_size=default_size,
-            min_size=min_size,
-            data_format=backend.image_data_format(),
-            require_flatten=require_flatten or static_shape,
-            weights=None,
-        )
-
+        try:
+            input_shape = imagenet_utils.obtain_input_shape(
+                input_shape,
+                default_size=default_size,
+                min_size=min_size,
+                data_format=backend.image_data_format(),
+                require_flatten=require_flatten or static_shape,
+                weights=None,
+            )
+        except ValueError as e:
+            # Override the error msg from `obtain_input_shape`
+            if "If `include_top` is True" in str(e):
+                raise ValueError(
+                    f"The inferred input_shape={input_shape} must be "
+                    f"static for {self.__class__.__name__} "
+                    f"(require_flatten={require_flatten}, "
+                    f"static_shape={static_shape})."
+                ) from None
         if input_tensor is None:
             x = layers.Input(shape=input_shape)
         else:
             if not backend.is_keras_tensor(input_tensor):
                 x = layers.Input(tensor=input_tensor, shape=input_shape)
             else:
-                x = utils.get_source_inputs(input_tensor)
+                x = utils.get_source_inputs(input_tensor)[0]
+        if static_shape:
+            if None in x.shape[1:]:
+                raise ValueError(
+                    f"The inferred input_shape={x.shape} must be "
+                    f"static for {self.__class__.__name__} "
+                    f"(require_flatten={require_flatten}, "
+                    f"static_shape={static_shape})."
+                )
         return x
 
     def build_preprocessing(
         self,
         inputs,
         mode: typing.Literal["imagenet", "0_1", "-1_1"] = "imagenet",
     ):
+        """Build the preprocessing pipeline.
+
+        Args:
+            inputs: A `KerasTensor` indicating the input.
+            mode: A `str` indicating the preprocessing mode. The available modes
+                are {"imagenet", "0_1", "-1_1"}. Defaults to "imagenet".
+
+        Returns:
+            A `KerasTensor`.
+        """
         if self._include_preprocessing is False:
             return inputs
         channels_axis = (
             -1 if backend.image_data_format() == "channels_last" else -3
         )
         if mode == "imagenet":
             # [0, 255] to [0, 1] and apply ImageNet mean and variance
@@ -184,20 +211,35 @@
         else:
             if self._pooling == "avg":
                 x = layers.GlobalAveragePooling2D(name="avg_pool")(x)
             elif self._pooling == "max":
                 x = layers.GlobalMaxPooling2D(name="max_pool")(x)
         return x
 
-    def load_pretrained_weights(self, weights_url: typing.Optional[str] = None):
-        if weights_url is not None:
-            result = urllib.parse.urlparse(weights_url)
+    def load_pretrained_weights(
+        self,
+        weights: typing.Union[pathlib.Path, str, None] = None,
+    ):
+        """Load the pretrained weights from `weights_url`.
+
+        This function prefers the following order:
+        1. Local file (a instance of pathlib.Path)
+        2. URL (a str starting with 'https://')
+        """
+        if weights is None:
+            return
+        # Check local files
+        if isinstance(weights, pathlib.Path):
+            self.load_weights(weights)
+        # Check URL
+        else:
+            result = urllib.parse.urlparse(weights)
             file_name = pathlib.Path(result.path).name
             weights_path = utils.get_file(
-                file_name, weights_url, cache_subdir="kimm_models"
+                file_name, weights, cache_subdir="kimm_models"
             )
             self.load_weights(weights_path)
 
     def get_config(self):
         # Don't chain to super here. The default `get_config()` for functional
         # models is nested and cannot be passed to BaseModel.
         config = {
@@ -209,33 +251,47 @@
             "include_preprocessing": self._include_preprocessing,
             "include_top": self._include_top,
             "pooling": self._pooling,
             "dropout_rate": self._dropout_rate,
             "classes": self._classes,
             "classifier_activation": self._classifier_activation,
             "weights": self._weights,
-            "weights_url": self._weights_url,
             # feature extractor
             "feature_extractor": self._feature_extractor,
             "feature_keys": self._feature_keys,
         }
         return config
 
     def fix_config(self, config: typing.Dict):
         return config
 
-    def get_weights_url(self, weights):
+    def parse_weights(self, weights: typing.Union[str, None]):
+        """Parse the path/URL if weights is specified.
+
+        This function prefers the following order:
+        1. Local file (a instance of pathlib.Path)
+        2. URL (a str starting with 'https://')
+        3. Available weights (mostly 'imagenet')
+        """
         if weights is None:
             return None
-
-        for _weights, _origin, _file_name in self.available_weights:
-            if weights == _weights:
-                return f"{_origin}{_file_name}"
+        # Check local files
+        elif pathlib.Path(weights).exists():
+            return pathlib.Path(weights)
+        # Check URL
+        elif str(weights).startswith(("http://", "https://")):
+            return str(weights)
+        # Check avaiable weights (a plain string)
+        else:
+            # Parse the string for available weights
+            for _weights, _origin, _file_name in self.available_weights:
+                if weights == _weights:
+                    return f"{_origin}{_file_name}"
 
         # Failed to find the weights
         _available_weights_name = [
-            _weights for _weights, _ in self.available_weights
+            _weights for _weights, _, _ in self.available_weights
         ]
         raise ValueError(
-            f"Available weights are {_available_weights_name}. "
-            f"Received weights={weights}"
+            f"If `weights` is a URL string, the available weights are "
+            f"{_available_weights_name}. Received: weights={weights}"
         )
```

### Comparing `kimm-0.2.0/kimm/_src/models/convmixer.py` & `kimm-0.2.1/kimm/_src/models/convmixer.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,18 +50,17 @@
     def __init__(
         self,
         depth: int = 32,
         hidden_channels: int = 768,
         patch_size: int = 7,
         kernel_size: int = 7,
         activation: str = "relu",
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs)
         channels_axis = (
             -1 if backend.image_data_format() == "channels_last" else -3
         )
 
         inputs = self.determine_input_tensor(
             input_tensor,
```

### Comparing `kimm-0.2.0/kimm/_src/models/convnext.py` & `kimm-0.2.1/kimm/_src/models/convnext.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,18 +139,17 @@
         self,
         depths: typing.Sequence[int] = [3, 3, 9, 3],
         hidden_channels: typing.Sequence[int] = [96, 192, 384, 768],
         patch_size: int = 4,
         kernel_size: int = 7,
         activation: str = "gelu",
         use_conv_mlp: bool = False,
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs)
         channels_axis = (
             -1 if backend.image_data_format() == "channels_last" else -3
         )
 
         inputs = self.determine_input_tensor(
             input_tensor,
@@ -454,15 +453,21 @@
     kernel_size = 7
     activation = "gelu"
     use_conv_mlp = False
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.convnext"])
 class ConvNeXtXLarge(ConvNeXtVariant):
-    available_weights = []
+    available_weights = [
+        (
+            "imagenet",
+            ConvNeXt.default_origin,
+            "convnextxlarge_convnext_xlarge.fb_in22k_ft_in1k.keras",
+        )
+    ]
 
     # Parameters
     depths = (3, 3, 27, 3)
     hidden_channels = (256, 512, 1024, 2048)
     patch_size = 4
     kernel_size = 7
     activation = "gelu"
@@ -473,8 +478,8 @@
 add_model_to_registry(ConvNeXtFemto, "imagenet")
 add_model_to_registry(ConvNeXtPico, "imagenet")
 add_model_to_registry(ConvNeXtNano, "imagenet")
 add_model_to_registry(ConvNeXtTiny, "imagenet")
 add_model_to_registry(ConvNeXtSmall, "imagenet")
 add_model_to_registry(ConvNeXtBase, "imagenet")
 add_model_to_registry(ConvNeXtLarge, "imagenet")
-add_model_to_registry(ConvNeXtXLarge)
+add_model_to_registry(ConvNeXtXLarge, "imagenet")
```

### Comparing `kimm-0.2.0/kimm/_src/models/densenet.py` & `kimm-0.2.1/kimm/_src/models/densenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,18 +79,17 @@
         *[f"BLOCK{i}_S{j}" for i, j in zip(range(4), [8, 16, 32, 32])],
     ]
 
     def __init__(
         self,
         growth_rate: float = 32,
         num_blocks: typing.Sequence[int] = [6, 12, 24, 16],
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs)
         channels_axis = (
             -1 if backend.image_data_format() == "channels_last" else -3
         )
 
         inputs = self.determine_input_tensor(
             input_tensor,
```

### Comparing `kimm-0.2.0/kimm/_src/models/efficientnet.py` & `kimm-0.2.1/kimm/_src/models/efficientnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,18 +146,17 @@
         depth: float = 1.0,
         stem_channels: int = 32,
         head_channels: int = 1280,
         fix_stem_and_head_channels: bool = False,
         fix_first_and_last_blocks: bool = False,
         activation="swish",
         config: str = "v1",
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
         _available_configs = [
             "v1",
             "v1_lite",
             "v2_s",
             "v2_m",
             "v2_l",
             "v2_xl",
@@ -186,15 +185,14 @@
         bn_epsilon = kwargs.pop("bn_epsilon", 1e-5)
         padding = kwargs.pop("padding", None)
         # EfficientNetV2Base config
         round_limit = kwargs.pop("round_limit", 0.9)
         # TinyNet config
         round_fn = kwargs.pop("round_fn", math.ceil)
 
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs)
         channels_axis = (
             -1 if backend.image_data_format() == "channels_last" else -3
         )
 
         inputs = self.determine_input_tensor(
             input_tensor,
```

### Comparing `kimm-0.2.0/kimm/_src/models/ghostnet.py` & `kimm-0.2.1/kimm/_src/models/ghostnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,17 +134,15 @@
         use_depthwise=True,
         name=f"{name}_cheap_operation",
     )
     out = layers.Concatenate(axis=channels_axis, name=f"{name}_concat")(
         [x1, x2]
     )
 
-    residual = layers.AveragePooling2D(
-        2, 2, data_format=backend.image_data_format(), name=f"{name}_avg_pool"
-    )(residual)
+    residual = layers.AveragePooling2D(2, 2, name=f"{name}_avg_pool")(residual)
     residual = apply_conv2d_block(
         residual,
         output_channels,
         kernel_size,
         strides,
         name=f"{name}_short_conv1",
     )
@@ -260,33 +258,31 @@
     ]
 
     def __init__(
         self,
         width: float = 1.0,
         config: typing.Union[str, typing.List] = "default",
         version: typing.Literal["v1", "v2"] = "v1",
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
         _available_configs = ["default"]
         if config == "default":
             _config = DEFAULT_CONFIG
         else:
             raise ValueError(
                 f"config must be one of {_available_configs} using string. "
                 f"Received: config={config}"
             )
         if version not in ("v1", "v2"):
             raise ValueError(
                 "`version` must be one of ('v1', 'v2'). "
                 f"Received version={version}"
             )
 
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs)
         inputs = self.determine_input_tensor(
             input_tensor,
             self._input_shape,
             self._default_size,
             require_flatten=self._include_top,
             static_shape=True if version == "v2" else False,
```

### Comparing `kimm-0.2.0/kimm/_src/models/hgnet.py` & `kimm-0.2.1/kimm/_src/models/hgnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,18 +389,17 @@
         "STEM_S4",
         *[f"BLOCK{i}_S{j}" for i, j in zip(range(4), [4, 8, 16, 32])],
     ]
 
     def __init__(
         self,
         config: str = "v1_tiny",
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
         _available_configs = ["v1_tiny", "v1_small", "v1_base"]
         if config == "v1_tiny":
             _config = DEFAULT_V1_TINY_CONFIG
         elif config == "v1_small":
             _config = DEFAULT_V1_SMALL_CONFIG
         elif config == "v1_base":
             _config = DEFAULT_V1_BASE_CONFIG
@@ -420,15 +419,14 @@
             _config = DEFAULT_V2_B6_CONFIG
         else:
             raise ValueError(
                 f"config must be one of {_available_configs} using string. "
                 f"Received: config={config}"
             )
 
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs)
         inputs = self.determine_input_tensor(
             input_tensor,
             self._input_shape,
             self._default_size,
         )
         x = inputs
```

### Comparing `kimm-0.2.0/kimm/_src/models/inception_next.py` & `kimm-0.2.1/kimm/_src/models/inception_next.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,19 +147,17 @@
 
     def __init__(
         self,
         depths: typing.Sequence[int] = [3, 3, 9, 3],
         hidden_channels: typing.Sequence[int] = [96, 192, 384, 768],
         mlp_ratios: typing.Sequence[float] = [4, 4, 4, 3],
         activation: str = "gelu",
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs, 224)
         channels_axis = (
             -1 if backend.image_data_format() == "channels_last" else -3
         )
 
         inputs = self.determine_input_tensor(
             input_tensor,
```

### Comparing `kimm-0.2.0/kimm/_src/models/inception_v3.py` & `kimm-0.2.1/kimm/_src/models/inception_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,18 +234,17 @@
 @keras.saving.register_keras_serializable(package="kimm")
 class InceptionV3Base(BaseModel):
     available_feature_keys = [
         "STEM_S2",
         *[f"BLOCK{i}_S{j}" for i, j in zip(range(4), [4, 8, 16, 32])],
     ]
 
-    def __init__(self, has_aux_logits: bool = False, **kwargs):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
-        input_tensor = kwargs.pop("input_tensor", None)
+    def __init__(
+        self, has_aux_logits: bool = False, input_tensor=None, **kwargs
+    ):
         self.set_properties(kwargs, 299)
         inputs = self.determine_input_tensor(
             input_tensor,
             self._input_shape,
             self._default_size,
             require_flatten=self._include_top,
         )
```

### Comparing `kimm-0.2.0/kimm/_src/models/mobilenet_v2.py` & `kimm-0.2.1/kimm/_src/models/mobilenet_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,28 +37,26 @@
 
     def __init__(
         self,
         width: float = 1.0,
         depth: float = 1.0,
         fix_stem_and_head_channels: bool = False,
         config: typing.Literal["default"] = "default",
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
         _available_configs = ["default"]
         if config == "default":
             _config = DEFAULT_CONFIG
         else:
             raise ValueError(
                 f"config must be one of {_available_configs} using string. "
                 f"Received: config={config}"
             )
 
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs)
         inputs = self.determine_input_tensor(
             input_tensor,
             self._input_shape,
             self._default_size,
         )
         x = inputs
```

### Comparing `kimm-0.2.0/kimm/_src/models/mobilenet_v3.py` & `kimm-0.2.1/kimm/_src/models/mobilenet_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,18 +88,17 @@
     def __init__(
         self,
         width: float = 1.0,
         depth: float = 1.0,
         fix_stem_and_head_channels: bool = False,
         config: typing.Literal["small", "large", "lcnet"] = "large",
         minimal: bool = False,
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
         _available_configs = ["small", "large", "lcnet"]
         if config == "small":
             _config = DEFAULT_SMALL_CONFIG
             conv_head_channels = 1024
         elif config == "large":
             _config = DEFAULT_LARGE_CONFIG
             conv_head_channels = 1280
@@ -119,15 +118,14 @@
             force_activation = None
             force_kernel_size = None
             no_se = False
         # TF default config
         bn_epsilon = kwargs.pop("bn_epsilon", 1e-5)
         padding = kwargs.pop("padding", None)
 
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs)
         inputs = self.determine_input_tensor(
             input_tensor,
             self._input_shape,
             self._default_size,
         )
         x = inputs
```

### Comparing `kimm-0.2.0/kimm/_src/models/mobileone.py` & `kimm-0.2.1/kimm/_src/models/mobileone.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,28 +19,26 @@
     def __init__(
         self,
         num_blocks: typing.Sequence[int],
         num_channels: typing.Sequence[int],
         stem_channels: int = 48,
         branch_size: int = 1,
         reparameterized: bool = False,
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-        if kwargs["weights_url"] is not None and reparameterized is True:
+        if kwargs["weights"] is not None and reparameterized is True:
             raise ValueError(
                 "Weights can only be loaded with `reparameterized=False`. "
                 "You can first initialize the model with "
                 "`reparameterized=False` then use "
                 "`get_reparameterized_model` to get the converted model. "
                 f"Received: weights={kwargs['weights']}, "
                 f"reparameterized={reparameterized}"
             )
-
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs)
         channels_axis = (
             -1 if backend.image_data_format() == "channels_last" else -3
         )
 
         inputs = self.determine_input_tensor(
             input_tensor,
```

### Comparing `kimm-0.2.0/kimm/_src/models/mobilevit.py` & `kimm-0.2.1/kimm/_src/models/mobilevit.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,50 +44,63 @@
     ["mobilevitv2", 1, 3, 256, 2, 2.0, 128, 2, 2],
     ["mobilevitv2", 1, 3, 384, 2, 2.0, 192, 4, 2],
     ["mobilevitv2", 1, 3, 512, 2, 2.0, 256, 3, 2],
 ]
 
 
 def unfold(inputs, patch_size):
-    # TODO: improve performance
     x = inputs
     h, w, c = x.shape[-3], x.shape[-2], x.shape[-1]
     new_h, new_w = (
         math.ceil(h / patch_size) * patch_size,
         math.ceil(w / patch_size) * patch_size,
     )
     num_patches_h = new_h // patch_size
     num_patches_w = new_w // patch_size
     num_patches = num_patches_h * num_patches_w
-    # [B, H, W, C] -> [B * P, N, C]
+
+    # Resize the feature map if needed
+    need_interpolation = False
+    if new_h != h or new_w != w:
+        x = ops.image.resize(
+            x, size=(new_h, new_w), data_format="channels_last"
+        )
+        need_interpolation = True
+
+    # [B, H, W, C] -> [B, P, N, C]
     x = ops.reshape(
         x, [-1, num_patches_h, patch_size, num_patches_w, patch_size, c]
     )
     x = ops.transpose(x, [0, 2, 4, 1, 3, 5])
-    x = ops.reshape(x, [-1, num_patches, c])
-    return x
+    x = ops.reshape(x, [-1, patch_size * patch_size, num_patches, c])
+    return x, need_interpolation
 
 
-def fold(inputs, h, w, c, patch_size):
-    # TODO: improve performance
+def fold(inputs, h, w, c, patch_size, need_interpolation=False):
     x = inputs
+
     new_h, new_w = (
         math.ceil(h / patch_size) * patch_size,
         math.ceil(w / patch_size) * patch_size,
     )
     num_patches_h = new_h // patch_size
     num_patches_w = new_w // patch_size
-    # [B * P, N, C] -> [B, P, N, C] -> [B, H, W, C]
+
+    # [B, P, N, C] -> [B, H, W, C]
     x = ops.reshape(
         x, [-1, patch_size, patch_size, num_patches_h, num_patches_w, c]
     )
     x = ops.transpose(x, [0, 3, 1, 4, 2, 5])
     x = ops.reshape(
         x, [-1, num_patches_h * patch_size, num_patches_w * patch_size, c]
     )
+
+    # Resize the feature map if needed
+    if need_interpolation:
+        x = ops.image.resize(x, size=(h, w), data_format="channels_last")
     return x
 
 
 def apply_mobilevit_block(
     inputs,
     output_channels: int,
     kernel_size: int = 3,
@@ -126,32 +139,31 @@
 
     # TODO: natively support channels_first
     # Unfold (feature map -> patches)
     if backend.image_data_format() == "channels_first":
         x = ops.transpose(x, [0, 2, 3, 1])
 
     h, w, c = x.shape[-3], x.shape[-2], x.shape[-1]
-    x = unfold(x, patch_size)
+    x, need_interpolation = unfold(x, patch_size)
 
     # Global representations
     for i in range(transformer_depth):
         x = apply_transformer_block(
             x,
             transformer_dim,
             num_heads,
             mlp_ratio,
             True,
-            False,
             activation=transformer_activation,
             name=f"{name}_transformer_{i}",
         )
     x = layers.LayerNormalization(axis=-1, epsilon=1e-6, name=f"{name}_norm")(x)
 
     # Fold (patch -> feature map)
-    x = fold(x, h, w, c, patch_size)
+    x = fold(x, h, w, c, patch_size, need_interpolation)
 
     # TODO: natively support channels_first
     if backend.image_data_format() == "channels_first":
         x = ops.transpose(x, [0, 3, 1, 2])
 
     x = apply_conv2d_block(
         x,
@@ -187,40 +199,49 @@
         math.ceil(h / patch_size) * patch_size,
         math.ceil(w / patch_size) * patch_size,
     )
     num_patches_h = new_h // patch_size
     num_patches_w = new_w // patch_size
     num_patches = num_patches_h * num_patches_w
 
+    # Resize feature map if needed
+    need_interpolation = False
+    if new_h != h or new_w != w:
+        x = ops.image.resize(
+            x, size=(new_h, new_w), data_format=backend.image_data_format()
+        )
+        need_interpolation = True
+
     if backend.image_data_format() == "channels_last":
         # [B, H, W, C] -> [B, P, N, C]
         x = ops.reshape(
             x, [-1, num_patches_h, patch_size, num_patches_w, patch_size, c]
         )
         x = ops.transpose(x, [0, 2, 4, 1, 3, 5])
         x = ops.reshape(x, [-1, patch_size * patch_size, num_patches, c])
     else:
         # [B, C, H, W] -> [B, C, P, N]
         x = ops.reshape(
             x, [-1, c, num_patches_h, patch_size, num_patches_w, patch_size]
         )
         x = ops.transpose(x, [0, 1, 3, 5, 2, 4])
         x = ops.reshape(x, [-1, c, patch_size * patch_size, num_patches])
-    return x
+    return x, need_interpolation
 
 
-def fold_v2(inputs, h, w, c, patch_size):
+def fold_v2(inputs, h, w, c, patch_size, need_interpolation=False):
     x = inputs
 
     new_h, new_w = (
         math.ceil(h / patch_size) * patch_size,
         math.ceil(w / patch_size) * patch_size,
     )
     num_patches_h = new_h // patch_size
     num_patches_w = new_w // patch_size
+
     if backend.image_data_format() == "channels_last":
         # [B, P, N, C] -> [B, H, W, C]
         x = ops.reshape(
             x, [-1, patch_size, patch_size, num_patches_h, num_patches_w, c]
         )
         x = ops.transpose(x, [0, 3, 1, 4, 2, 5])
         x = ops.reshape(
@@ -231,14 +252,18 @@
         x = ops.reshape(
             x, [-1, c, patch_size, patch_size, num_patches_h, num_patches_w]
         )
         x = ops.transpose(x, [0, 1, 4, 2, 5, 3])
         x = ops.reshape(
             x, [-1, c, num_patches_h * patch_size, num_patches_w * patch_size]
         )
+
+    # Resize the feature map if needed
+    if need_interpolation:
+        x = ops.image.resize(x, size=(h, w), data_format="channels_last")
     return x
 
 
 def apply_linear_self_attention_block(
     inputs, dim: int, use_bias=True, name="linear_self_attention_block"
 ):
     channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
@@ -348,15 +373,15 @@
     )(x)
 
     # Unfold (feature map -> patches)
     if backend.image_data_format() == "channels_last":
         h, w, c = x.shape[-3], x.shape[-2], x.shape[-1]
     else:
         c, h, w = x.shape[-3], x.shape[-2], x.shape[-1]
-    x = unfold_v2(x, patch_size)
+    x, need_interpolation = unfold_v2(x, patch_size)
 
     # Global representations:
     for i in range(transformer_depth):
         x = apply_linear_transformer_block(
             x,
             transformer_dim,
             mlp_ratio,
@@ -364,15 +389,15 @@
             name=f"{name}_transformer_{i}",
         )
     x = layers.GroupNormalization(
         1, axis=channels_axis, epsilon=1e-5, name=f"{name}_norm"
     )(x)
 
     # Fold (patch -> feature map)
-    x = fold_v2(x, h, w, c, patch_size)
+    x = fold_v2(x, h, w, c, patch_size, need_interpolation)
 
     x = apply_conv2d_block(
         x,
         output_channels,
         1,
         1,
         activation=None,
@@ -390,32 +415,30 @@
 
     def __init__(
         self,
         stem_channels: int = 16,
         head_channels: int = 640,
         activation: str = "swish",
         config: str = "v1_s",
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
         _available_configs = ["v1_s", "v1_xs", "v1_xss"]
         if config == "v1_s":
             _config = DEFAULT_V1_S_CONFIG
         elif config == "v1_xs":
             _config = DEFAULT_V1_XS_CONFIG
         elif config == "v1_xxs":
             _config = DEFAULT_V1_XXS_CONFIG
         else:
             raise ValueError(
                 f"config must be one of {_available_configs} using string. "
                 f"Received: config={config}"
             )
 
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs, 256)
 
         inputs = self.determine_input_tensor(
             input_tensor,
             self._input_shape,
             self._default_size,
             static_shape=True,
@@ -519,28 +542,26 @@
     ]
 
     def __init__(
         self,
         multiplier: float = 1.0,
         activation: str = "swish",
         config: str = "v2",
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
         _available_configs = ["v2"]
         if config == "v2":
             _config = DEFAULT_V2_CONFIG
         else:
             raise ValueError(
                 f"config must be one of {_available_configs} using string. "
                 f"Received: config={config}"
             )
 
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs, 256)
 
         inputs = self.determine_input_tensor(
             input_tensor,
             self._input_shape,
             self._default_size,
             static_shape=True,
```

### Comparing `kimm-0.2.0/kimm/_src/models/regnet.py` & `kimm-0.2.1/kimm/_src/models/regnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,21 +155,19 @@
         self,
         w0: int = 80,
         wa: float = 42.64,
         wm: float = 2.66,
         group_size: int = 24,
         depth: int = 21,
         se_ratio: float = 0.0,
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
         per_stage_config = _generate_regnet(w0, wa, wm, group_size, depth)
 
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs)
         inputs = self.determine_input_tensor(
             input_tensor,
             self._input_shape,
             self._default_size,
         )
         x = inputs
```

### Comparing `kimm-0.2.0/kimm/_src/models/repvgg.py` & `kimm-0.2.1/kimm/_src/models/repvgg.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,27 @@
 
     def __init__(
         self,
         num_blocks: typing.Sequence[int],
         num_channels: typing.Sequence[int],
         stem_channels: int = 48,
         reparameterized: bool = False,
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-        if kwargs["weights_url"] is not None and reparameterized is True:
+        if kwargs["weights"] is not None and reparameterized is True:
             raise ValueError(
                 "Weights can only be loaded with `reparameterized=False`. "
                 "You can first initialize the model with "
                 "`reparameterized=False` then use "
                 "`get_reparameterized_model` to get the converted model. "
                 f"Received: weights={kwargs['weights']}, "
                 f"reparameterized={reparameterized}"
             )
 
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs)
         channels_axis = (
             -1 if backend.image_data_format() == "channels_last" else -3
         )
 
         inputs = self.determine_input_tensor(
             input_tensor,
```

### Comparing `kimm-0.2.0/kimm/_src/models/resnet.py` & `kimm-0.2.1/kimm/_src/models/resnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,25 +114,23 @@
         *[f"BLOCK{i}_S{j}" for i, j in zip(range(4), [4, 8, 16, 32])],
     ]
 
     def __init__(
         self,
         block_fn: typing.Literal["basic", "bottleneck"],
         num_blocks: typing.Sequence[int],
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
         if block_fn not in ("basic", "bottleneck"):
             raise ValueError(
                 "`block_fn` must be one of ('basic', 'bottelneck'). "
                 f"Received: block_fn={block_fn}"
             )
 
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs)
         inputs = self.determine_input_tensor(
             input_tensor,
             self._input_shape,
             self._default_size,
         )
         x = inputs
```

### Comparing `kimm-0.2.0/kimm/_src/models/vgg.py` & `kimm-0.2.1/kimm/_src/models/vgg.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,17 +110,20 @@
 
 @keras.saving.register_keras_serializable(package="kimm")
 class VGG(BaseModel):
     available_feature_keys = [
         *[f"BLOCK{i}_S{j}" for i, j in zip(range(6), [1, 2, 4, 8, 16, 32])],
     ]
 
-    def __init__(self, config: typing.Union[str, typing.List], **kwargs):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
+    def __init__(
+        self,
+        config: typing.Union[str, typing.List],
+        input_tensor=None,
+        **kwargs,
+    ):
         _available_configs = ["vgg11", "vgg13", "vgg16", "vgg19"]
         if config == "vgg11":
             _config = DEFAULT_VGG11_CONFIG
         elif config == "vgg13":
             _config = DEFAULT_VGG13_CONFIG
         elif config == "vgg16":
             _config = DEFAULT_VGG16_CONFIG
@@ -128,15 +131,14 @@
             _config = DEFAULT_VGG19_CONFIG
         else:
             raise ValueError(
                 f"config must be one of {_available_configs} using string. "
                 f"Received: config={config}"
             )
 
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs)
         channels_axis = (
             -1 if backend.image_data_format() == "channels_last" else -3
         )
 
         inputs = self.determine_input_tensor(
             input_tensor,
```

### Comparing `kimm-0.2.0/kimm/_src/models/vision_transformer.py` & `kimm-0.2.1/kimm/_src/models/vision_transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 from kimm._src.layers.position_embedding import PositionEmbedding
 from kimm._src.models.base_model import BaseModel
 from kimm._src.utils.model_registry import add_model_to_registry
 
 
 @keras.saving.register_keras_serializable(package="kimm")
 class VisionTransformer(BaseModel):
+    # Updated weights: resizable position embedding
+    default_origin = "https://github.com/james77777778/keras-image-models/releases/download/0.1.2/"
+
     def __init__(
         self,
         patch_size: int,
         embed_dim: int,
         depth: int,
         num_heads: int,
         mlp_ratio: float = 4.0,
         use_qkv_bias: bool = True,
-        use_qk_norm: bool = False,
         pos_dropout_rate: float = 0.0,
+        input_tensor=None,
         **kwargs,
     ):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
-        input_tensor = kwargs.pop("input_tensor", None)
         self.set_properties(kwargs, 384)
         if self._pooling is not None:
             raise ValueError(
                 "`VisionTransformer` doesn't support `pooling`. "
                 f"Received: pooling={self._pooling}"
             )
         inputs = self.determine_input_tensor(
@@ -58,28 +58,30 @@
             use_bias=True,
             name="patch_embed_conv",
         )(x)
 
         # TODO: natively support channels_first
         if backend.image_data_format() == "channels_first":
             x = ops.transpose(x, [0, 2, 3, 1])
+        height, width = x.shape[-3], x.shape[-2]
 
         x = layers.Reshape((-1, embed_dim))(x)
-        x = PositionEmbedding(name="postition_embedding")(x)
+        x = PositionEmbedding(
+            height=height, width=width, name="postition_embedding"
+        )(x)
         features["EMBEDDING"] = x
         x = layers.Dropout(pos_dropout_rate, name="pos_dropout")(x)
 
         for i in range(depth):
             x = apply_transformer_block(
                 x,
                 embed_dim,
                 num_heads,
                 mlp_ratio,
                 use_qkv_bias,
-                use_qk_norm,
                 activation="gelu",
                 name=f"blocks_{i}",
             )
             features[f"BLOCK{i}"] = x
         x = layers.LayerNormalization(epsilon=1e-6, name="norm")(x)
 
         # Head
@@ -96,15 +98,14 @@
         # All references to `self` below this line
         self.patch_size = patch_size
         self.embed_dim = embed_dim
         self.depth = depth
         self.num_heads = num_heads
         self.mlp_ratio = mlp_ratio
         self.use_qkv_bias = use_qkv_bias
-        self.use_qk_norm = use_qk_norm
         self.pos_dropout_rate = pos_dropout_rate
 
     def build_top(self, inputs, classes, classifier_activation, dropout_rate):
         x = inputs[:, 0]  # class token
         x = layers.Dropout(dropout_rate, name="head_drop")(x)
         x = layers.Dense(
             classes, activation=classifier_activation, name="head"
@@ -117,29 +118,28 @@
             {
                 "patch_size": self.patch_size,
                 "embed_dim": self.embed_dim,
                 "depth": self.depth,
                 "num_heads": self.num_heads,
                 "mlp_ratio": self.mlp_ratio,
                 "use_qkv_bias": self.use_qkv_bias,
-                "use_qk_norm": self.use_qk_norm,
                 "pos_dropout_rate": self.pos_dropout_rate,
             }
         )
         return config
 
     def fix_config(self, config):
         unused_kwargs = [
             "patch_size",
             "embed_dim",
             "depth",
             "num_heads",
             "mlp_ratio",
             "use_qkv_bias",
-            "use_qk_norm",
+            "use_qk_norm",  # Deprecated
             "pos_dropout_rate",
         ]
         for k in unused_kwargs:
             config.pop(k, None)
         return config
 
 
@@ -150,15 +150,14 @@
     # Parameters
     patch_size = None
     embed_dim = None
     depth = None
     num_heads = None
     mlp_ratio = None
     use_qkv_bias = None
-    use_qk_norm = None
     pos_dropout_rate = None
 
     def __init__(
         self,
         input_tensor: keras.KerasTensor = None,
         input_shape: typing.Optional[typing.Sequence[int]] = None,
         include_preprocessing: bool = True,
@@ -186,15 +185,14 @@
         super().__init__(
             patch_size=self.patch_size,
             embed_dim=self.embed_dim,
             depth=self.depth,
             num_heads=self.num_heads,
             mlp_ratio=self.mlp_ratio,
             use_qkv_bias=self.use_qkv_bias,
-            use_qk_norm=self.use_qk_norm,
             pos_dropout_rate=self.pos_dropout_rate,
             input_tensor=input_tensor,
             input_shape=input_shape,
             include_preprocessing=include_preprocessing,
             include_top=include_top,
             pooling=pooling,
             dropout_rate=dropout_rate,
@@ -223,15 +221,14 @@
     # Parameters
     patch_size = 16
     embed_dim = 192
     depth = 12
     num_heads = 3
     mlp_ratio = 4.0
     use_qkv_bias = True
-    use_qk_norm = False
     pos_dropout_rate = 0.0
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.vision_transformer"])
 class VisionTransformerTiny32(VisionTransformerVariant):
     available_feature_keys = [
         "EMBEDDING",
@@ -242,15 +239,14 @@
     # Parameters
     patch_size = 32
     embed_dim = 192
     depth = 12
     num_heads = 3
     mlp_ratio = 4.0
     use_qkv_bias = True
-    use_qk_norm = False
     pos_dropout_rate = 0.0
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.vision_transformer"])
 class VisionTransformerSmall16(VisionTransformerVariant):
     available_feature_keys = [
         "EMBEDDING",
@@ -267,15 +263,14 @@
     # Parameters
     patch_size = 16
     embed_dim = 384
     depth = 12
     num_heads = 6
     mlp_ratio = 4.0
     use_qkv_bias = True
-    use_qk_norm = False
     pos_dropout_rate = 0.0
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.vision_transformer"])
 class VisionTransformerSmall32(VisionTransformerVariant):
     available_feature_keys = [
         "EMBEDDING",
@@ -292,15 +287,14 @@
     # Parameters
     patch_size = 32
     embed_dim = 384
     depth = 12
     num_heads = 6
     mlp_ratio = 4.0
     use_qkv_bias = True
-    use_qk_norm = False
     pos_dropout_rate = 0.0
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.vision_transformer"])
 class VisionTransformerBase16(VisionTransformerVariant):
     available_feature_keys = [
         "EMBEDDING",
@@ -317,15 +311,14 @@
     # Parameters
     patch_size = 16
     embed_dim = 768
     depth = 12
     num_heads = 12
     mlp_ratio = 4.0
     use_qkv_bias = True
-    use_qk_norm = False
     pos_dropout_rate = 0.0
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.vision_transformer"])
 class VisionTransformerBase32(VisionTransformerVariant):
     available_feature_keys = [
         "EMBEDDING",
@@ -342,57 +335,66 @@
     # Parameters
     patch_size = 32
     embed_dim = 768
     depth = 12
     num_heads = 12
     mlp_ratio = 4.0
     use_qkv_bias = True
-    use_qk_norm = False
     pos_dropout_rate = 0.0
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.vision_transformer"])
 class VisionTransformerLarge16(VisionTransformerVariant):
     available_feature_keys = [
         "EMBEDDING",
         *[f"BLOCK{i}" for i in range(24)],
     ]
-    available_weights = []
+    available_weights = [
+        (
+            "imagenet",
+            VisionTransformer.default_origin,
+            "visiontransformerlarge16_vit_large_patch16_384.keras",
+        )
+    ]
 
     # Parameters
     patch_size = 16
     embed_dim = 1024
     depth = 24
     num_heads = 16
     mlp_ratio = 4.0
     use_qkv_bias = True
-    use_qk_norm = False
     pos_dropout_rate = 0.0
 
 
 @kimm_export(parent_path=["kimm.models", "kimm.models.vision_transformer"])
 class VisionTransformerLarge32(VisionTransformerVariant):
     available_feature_keys = [
         "EMBEDDING",
         *[f"BLOCK{i}" for i in range(24)],
     ]
-    available_weights = []
+    available_weights = [
+        (
+            "imagenet",
+            VisionTransformer.default_origin,
+            "visiontransformerlarge32_vit_large_patch32_384.keras",
+        )
+    ]
 
     # Parameters
     patch_size = 32
     embed_dim = 1024
     depth = 24
     num_heads = 16
     mlp_ratio = 4.0
     use_qkv_bias = True
-    use_qk_norm = False
     pos_dropout_rate = 0.0
 
 
 add_model_to_registry(VisionTransformerTiny16, "imagenet")
 add_model_to_registry(VisionTransformerTiny32)
 add_model_to_registry(VisionTransformerSmall16, "imagenet")
 add_model_to_registry(VisionTransformerSmall32, "imagenet")
 add_model_to_registry(VisionTransformerBase16, "imagenet")
 add_model_to_registry(VisionTransformerBase32, "imagenet")
-add_model_to_registry(VisionTransformerLarge16)
-add_model_to_registry(VisionTransformerLarge32)
+add_model_to_registry(VisionTransformerLarge16, "imagenet")
+add_model_to_registry(VisionTransformerLarge32, "imagenet")
```

### Comparing `kimm-0.2.0/kimm/_src/models/xception.py` & `kimm-0.2.1/kimm/_src/models/xception.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,18 +71,15 @@
 @keras.saving.register_keras_serializable(package="kimm")
 class XceptionBase(BaseModel):
     available_feature_keys = [
         "STEM_S2",
         *[f"BLOCK{i}_S{j}" for i, j in zip(range(4), [4, 8, 16, 32])],
     ]
 
-    def __init__(self, **kwargs):
-        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
-
-        input_tensor = kwargs.pop("input_tensor", None)
+    def __init__(self, input_tensor=None, **kwargs):
         self.set_properties(kwargs)
         channels_axis = (
             -1 if backend.image_data_format() == "channels_last" else -3
         )
 
         inputs = self.determine_input_tensor(
             input_tensor,
```

### Comparing `kimm-0.2.0/kimm/_src/utils/model_registry.py` & `kimm-0.2.1/kimm/_src/utils/model_registry.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/utils/model_registry_test.py` & `kimm-0.2.1/kimm/_src/utils/model_registry_test.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/utils/model_utils.py` & `kimm-0.2.1/kimm/_src/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/utils/model_utils_test.py` & `kimm-0.2.1/kimm/_src/utils/model_utils_test.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/_src/utils/timm_utils.py` & `kimm-0.2.1/kimm/_src/utils/timm_utils.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/blocks/__init__.py` & `kimm-0.2.1/kimm/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/models/__init__.py` & `kimm-0.2.1/kimm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/models/convnext/__init__.py` & `kimm-0.2.1/kimm/models/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/models/efficientnet/__init__.py` & `kimm-0.2.1/kimm/models/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/models/hgnet/__init__.py` & `kimm-0.2.1/kimm/models/hgnet/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/models/mobilenet_v3/__init__.py` & `kimm-0.2.1/kimm/models/mobilenet_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/models/mobilevit/__init__.py` & `kimm-0.2.1/kimm/models/mobilevit/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/models/regnet/__init__.py` & `kimm-0.2.1/kimm/models/regnet/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm/models/vision_transformer/__init__.py` & `kimm-0.2.1/kimm/models/vision_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/kimm.egg-info/PKG-INFO` & `kimm-0.2.1/kimm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimm
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Keras model zoo with pretrained weights.
 Author-email: Hong-Yu Chiu <james77777778@gmail.com>
 Maintainer-email: Hong-Yu Chiu <james77777778@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/james77777778/keras-image-models
 Project-URL: Documentation, https://github.com/james77777778/keras-image-models
 Project-URL: Repository, https://github.com/james77777778/keras-image-models.git
```

### Comparing `kimm-0.2.0/kimm.egg-info/SOURCES.txt` & `kimm-0.2.1/kimm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kimm-0.2.0/pyproject.toml` & `kimm-0.2.1/pyproject.toml`

 * *Files identical despite different names*

