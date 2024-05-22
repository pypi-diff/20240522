# Comparing `tmp/acetone_nnet-0.2.3.dev4.tar.gz` & `tmp/acetone_nnet-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone_nnet-0.2.3.dev4.tar", last modified: Thu May 16 14:43:28 2024, max compression
+gzip compressed data, was "acetone_nnet-0.3.tar", last modified: Wed May 22 06:47:28 2024, max compression
```

## Comparing `acetone_nnet-0.2.3.dev4.tar` & `acetone_nnet-0.3.tar`

### file list

```diff
@@ -1,148 +1,153 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.294291 acetone_nnet-0.2.3.dev4/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.2.3.dev4/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.2.3.dev4/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.2.3.dev4/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6684 2024-05-16 14:43:28.294291 acetone_nnet-0.2.3.dev4/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5294 2024-05-14 06:41:04.000000 acetone_nnet-0.2.3.dev4/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2070 2024-05-16 14:43:24.000000 acetone_nnet-0.2.3.dev4/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-16 14:43:28.294291 acetone_nnet-0.2.3.dev4/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.263291 acetone_nnet-0.2.3.dev4/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.269291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1801 2024-05-13 12:52:48.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.270290 acetone_nnet-0.2.3.dev4/src/acetone_nnet/bin/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/bin/bin_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2769 2024-05-15 12:06:29.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3921 2024-05-15 08:22:05.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.271291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4184 2024-05-16 06:28:50.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4946 2024-05-15 06:49:14.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.274291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3281 2024-05-16 12:23:11.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/AddBias.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4494 2024-05-16 12:12:33.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/BatchNormalization.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.276291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1708 2024-05-15 08:12:43.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1599 2024-05-15 08:12:34.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6103 2024-05-16 14:22:43.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1713 2024-05-15 08:12:54.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1592 2024-05-15 08:13:03.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1591 2024-05-15 08:13:08.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1724 2024-05-15 08:13:23.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1723 2024-05-15 08:13:39.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5069 2024-05-16 14:03:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.277291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5680 2024-05-16 14:40:47.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6263 2024-05-15 08:10:38.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4918 2024-05-15 14:39:50.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3541 2024-05-16 11:41:23.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4691 2024-05-15 07:06:26.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2859 2024-05-16 11:46:03.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4874 2024-05-16 11:34:22.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     9683 2024-05-16 08:45:22.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2934 2024-05-16 08:03:06.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3861 2024-05-16 07:57:35.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.278291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3503 2024-05-16 13:28:03.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.279291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1838 2024-05-15 07:56:30.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1721 2024-05-15 07:56:01.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6129 2024-05-16 14:39:59.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.280291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    12486 2024-05-16 12:52:50.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6895 2024-05-16 12:47:31.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6096 2024-05-15 07:37:55.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5476 2024-05-16 12:48:31.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2359 2024-05-16 08:00:32.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    29244 2024-05-16 14:36:20.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.280291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.281291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18659 2024-05-15 06:28:43.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.281291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7571 2024-05-14 15:19:20.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14558 2024-05-14 15:18:40.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.282291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3927 2024-05-14 15:17:50.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5379 2024-05-14 15:15:39.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.282291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    32109 2024-05-16 13:20:29.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4509 2024-05-14 14:54:21.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2754 2024-05-14 14:53:00.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.282291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5719 2024-05-15 08:15:19.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.284291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.287291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.289291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.290291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-05-13 08:47:21.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-05-13 08:47:14.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-05-13 13:12:23.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-05-13 08:47:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.291291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.292291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Dense.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Dot.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Gather.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.292291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/memory_layout/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.293291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/normalization/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_Makefile.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1034 2024-04-18 12:38:03.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1064 2024-04-18 12:38:21.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1137 2024-05-15 09:26:59.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_main_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1633 2024-05-16 07:42:59.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_source_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.293291 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6684 2024-05-16 14:43:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6926 2024-05-16 14:43:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-16 14:43:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-16 14:43:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-16 14:43:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-16 14:43:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.298191 acetone_nnet-0.3/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.3/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.3/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.3/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6677 2024-05-22 06:47:28.298191 acetone_nnet-0.3/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5294 2024-05-14 06:41:04.000000 acetone_nnet-0.3/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2063 2024-05-22 06:46:57.000000 acetone_nnet-0.3/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-22 06:47:28.298191 acetone_nnet-0.3/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.861186 acetone_nnet-0.3/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.917186 acetone_nnet-0.3/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2012 2024-05-22 06:40:35.000000 acetone_nnet-0.3/src/acetone_nnet/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.918186 acetone_nnet-0.3/src/acetone_nnet/bin/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.3/src/acetone_nnet/bin/bin_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2769 2024-05-15 12:06:29.000000 acetone_nnet-0.3/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3921 2024-05-15 08:22:05.000000 acetone_nnet-0.3/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.918186 acetone_nnet-0.3/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4184 2024-05-16 06:28:50.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4946 2024-05-15 06:49:14.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.920186 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3281 2024-05-16 12:23:11.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/AddBias.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4494 2024-05-16 12:12:33.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/BatchNormalization.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.921186 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1708 2024-05-15 08:12:43.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1599 2024-05-15 08:12:34.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6094 2024-05-21 06:29:34.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1713 2024-05-15 08:12:54.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1592 2024-05-15 08:13:03.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1591 2024-05-15 08:13:08.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1724 2024-05-15 08:13:23.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1723 2024-05-15 08:13:39.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5069 2024-05-16 14:03:28.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.923186 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5695 2024-05-17 07:53:15.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6263 2024-05-15 08:10:38.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4918 2024-05-15 14:39:50.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3541 2024-05-16 11:41:23.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4691 2024-05-15 07:06:26.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2863 2024-05-21 06:24:17.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4874 2024-05-16 11:34:22.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     9817 2024-05-17 11:33:03.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3045 2024-05-21 06:29:09.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3868 2024-05-21 12:26:03.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.924186 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3507 2024-05-17 06:51:32.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.944187 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1838 2024-05-15 07:56:30.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1721 2024-05-15 07:56:01.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6337 2024-05-21 10:14:37.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.945187 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    12359 2024-05-17 06:57:46.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6895 2024-05-16 12:47:31.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6096 2024-05-15 07:37:55.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5476 2024-05-16 12:48:31.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2359 2024-05-16 08:00:32.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    28977 2024-05-21 15:08:31.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.945187 acetone_nnet-0.3/src/acetone_nnet/debug_tools/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1393 2024-05-22 06:40:28.000000 acetone_nnet-0.3/src/acetone_nnet/debug_tools/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2725 2024-05-21 15:03:01.000000 acetone_nnet-0.3/src/acetone_nnet/debug_tools/debug_keras.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3646 2024-05-21 15:03:05.000000 acetone_nnet-0.3/src/acetone_nnet/debug_tools/debug_onnx.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3542 2024-05-22 06:38:47.000000 acetone_nnet-0.3/src/acetone_nnet/debug_tools/debug_tools.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.946187 acetone_nnet-0.3/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.946187 acetone_nnet-0.3/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18659 2024-05-15 06:28:43.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.946187 acetone_nnet-0.3/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7571 2024-05-14 15:19:20.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14558 2024-05-14 15:18:40.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.947187 acetone_nnet-0.3/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3927 2024-05-14 15:17:50.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5379 2024-05-14 15:15:39.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.947187 acetone_nnet-0.3/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    32768 2024-05-21 06:37:35.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4509 2024-05-14 14:54:21.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2754 2024-05-14 14:53:00.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.947187 acetone_nnet-0.3/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5719 2024-05-15 08:15:19.000000 acetone_nnet-0.3/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.042188 acetone_nnet-0.3/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.3/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.151189 acetone_nnet-0.3/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.198190 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.230190 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      847 2024-05-17 07:06:52.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-17 07:07:01.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      742 2024-05-17 07:07:09.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      724 2024-05-17 07:07:16.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.232190 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.262190 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1350 2024-05-21 10:14:20.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.275190 acetone_nnet-0.3/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.285190 acetone_nnet-0.3/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_Makefile.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1030 2024-05-21 10:01:05.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1060 2024-05-21 10:01:00.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1137 2024-05-15 09:26:59.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1633 2024-05-16 07:42:59.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.298191 acetone_nnet-0.3/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6677 2024-05-22 06:47:27.000000 acetone_nnet-0.3/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7098 2024-05-22 06:47:27.000000 acetone_nnet-0.3/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-22 06:47:27.000000 acetone_nnet-0.3/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-22 06:47:27.000000 acetone_nnet-0.3/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-22 06:47:27.000000 acetone_nnet-0.3/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-22 06:47:27.000000 acetone_nnet-0.3/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone_nnet-0.2.3.dev4/AUTHORS.md` & `acetone_nnet-0.3/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/COPYING` & `acetone_nnet-0.3/COPYING`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/LICENSE` & `acetone_nnet-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/PKG-INFO` & `acetone_nnet-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.2.3.dev4
+Version: 0.3
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.2.3.dev4/README.md` & `acetone_nnet-0.3/README.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/pyproject.toml` & `acetone_nnet-0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "acetone-nnet"
-version = "0.2.3.dev4"
+version = "0.3"
 requires-python = ">=3.10, <3.12"
 
 authors = [
     { name="Yanis AIT-AISSA", email="Yanis.AIT-AISSA@student.isae-supaero.fr"},
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/__init__.py` & `acetone_nnet-0.3/src/acetone_nnet/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,22 @@
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest,
     ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip, LeakyReLu
 )
 
+from . import debug_tools
+from .debug_tools import (
+    debug_onnx, run_model_onnx, 
+    debug_keras, run_model_keras, 
+    compare_result, extract_outputs_c, extract_outputs_python
+)
+
 from .cli_acetone import cli_acetone
 from .cli_compare import cli_compare
 
 __all__ = (
     "cli_acetone", "cli_compare",
-    code_generator.__all__
+    code_generator.__all__,
+    debug_tools.__all__
 )
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/bin/bin_acetone.py` & `acetone_nnet-0.3/src/acetone_nnet/bin/bin_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.3/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.3/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/BatchNormalization.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/BatchNormalization.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,24 +51,24 @@
         ### Checking argument type ###
         assert type(self.idx) == int
         assert type(self.size) == int
         assert type(self.output_channels) == int
         assert type(self.output_height) == int
         assert type(self.output_width) == int
         assert isinstance(self.activation_function, ActivationFunctions)
-        assert type(self.constant) == np.ndarray or type(self.constant) == None
+        assert type(self.constant) == np.ndarray or self.constant == None
 
         ### Checking value consistency ###
         assert self.size == self.output_channels*self.output_height*self.output_width
         assert all(shape[1] == 1 or shape[1]==self.output_channels for shape in self.input_shapes)
         assert all(shape[2] == 1 or shape[2]==self.output_height for shape in self.input_shapes)
         assert all(shape[3] == 1 or shape[3]==self.output_width for shape in self.input_shapes)
-        assert self.output_channels == np.max(self.input_shapes[:][1])
-        assert self.output_height == np.max(self.input_shapes[:][2])
-        assert self.output_width == np.max(self.input_shapes[:][3])
+        assert self.output_channels == np.max(self.input_shapes[:,1])
+        assert self.output_height == np.max(self.input_shapes[:,2])
+        assert self.output_width == np.max(self.input_shapes[:,3])
 
     #Go through all the indices and do the operation
     def generate_inference_code_layer(self):
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
         assert type(self.idx) == int
         assert type(self.size) == int
         assert type(conv_algorithm) == str
-        assert type(self.padding) == str or type(self.padding) == np.ndarray
+        assert type(self.padding) == str or all(type(pad) == int for pad in self.padding)
         assert type(self.strides) == int
         assert type(self.kernel_h) == int
         assert type(self.kernel_w) == int
         assert type(self.dilation_rate) == int
         assert type(self.nb_filters) == int
         assert type(self.input_channels) == int
         assert type(self.input_height) == int
@@ -77,16 +77,16 @@
         assert type(self.weights) == np.ndarray
         assert type(self.biases) == np.ndarray
 
         ### Checking value consistency ###
         assert self.size == self.output_channels*self.output_height*self.output_width
         assert self.weights.shape == (self.input_channels, self.kernel_h, self.kernel_w, self.nb_filters)
         assert len(self.biases.shape) == 1 and self.biases.shape[0] == self.nb_filters
-        assert self.output_height == math.ceil((self.input_height + self.pad_bottom + self.pad_top - self.kernel_h - (self.kernel_h - 1)*(self.dilation_rate - 1))/self.strides) + 1
-        assert self.output_width == math.ceil((self.input_width + self.pad_left + self.pad_right - self.kernel_w - (self.kernel_w - 1)*(self.dilation_rate - 1))/self.strides) + 1
+        assert self.output_height == math.floor((self.input_height + self.pad_bottom + self.pad_top - self.kernel_h - (self.kernel_h - 1)*(self.dilation_rate - 1))/self.strides) + 1
+        assert self.output_width == math.floor((self.input_width + self.pad_left + self.pad_right - self.kernel_w - (self.kernel_w - 1)*(self.dilation_rate - 1))/self.strides) + 1
         assert self.conv_algorithm in ['6loops',
                                        'indirect_gemm_nn','indirect_gemm_tn','indirect_gemm_nt','indirect_gemm_tt',
                                        'std_gemm_nn','std_gemm_tn','std_gemm_nt','std_gemm_']
 
     @abstractmethod
     def generate_inference_code_layer(self):
         pass
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.name = 'Flatten'
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
         assert type(self.idx) == int
         assert type(self.size) == int
-        assert all(type(shape) == int for shape in self.input_shape)
+        assert all(type(shape) == int for shape in self.input_shape[1:])
         assert self.data_format == 'channels_last' or self.data_format == 'channels_first'
 
         ### Checking value consistency ###
         assert self.size == self.input_shape[1]*self.input_shape[2]*self.input_shape[3]
 
     def generate_inference_code_layer(self):
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,23 @@
 class Gemm(Layer):
     def __init__(self, idx:int, size:int, alpha:float|int, beta:float|int, transA:bool|int, transB:bool|int, weights:np.ndarray, bias:np.ndarray, input_shape:list, output_shape:list, activation_function:ActivationFunctions):
         super().__init__() 
         self.name = 'Gemm'
         self.idx = idx
         self.size = size
         
-        self.alpha = [alpha]
-        self.beta =  [beta]
+        if alpha != 1:
+            self.alpha = [alpha]
+        else:
+            self.alpha = []
+        if beta != 1:
+            self.beta =  [beta]
+        else:
+            self.beta = []
+            
         self.transpo = (transA,transB)
         self.algo_gemm_mapping = {(0,0):self.write_gemm_nn,
                              (0,1):self.write_gemm_nt,
                              (1,1):self.write_gemm_tt,
                              (1,0):self.write_gemm_tn}
         
         self.output_height = output_shape[2]
@@ -58,31 +65,31 @@
         self.nb_biases = self.count_elements_array(self.biases)
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
         assert type(self.idx) == int
         assert type(self.size) == int
-        assert type(self.alpha) == float or type(self.alpha) == int
-        assert type(self.beta) == float or type(self.beta) == int
-        assert type(self.transpo) == tuple[int] or type(self.transpo) == tuple[bool]
+        assert type(self.alpha[0]) == float or type(self.alpha[0]) == int
+        assert type(self.beta[0]) == float or type(self.beta[0]) == int
+        assert all(type(self.transpo[i]) == int or type(self.transpo[i]) == bool for i in range(2))
         assert type(self.output_height) == int
         assert type(self.output_width) == int
         assert type(self.input_height) == int
         assert type(self.input_width) == int
         assert type(self.weights) == np.ndarray
         assert type(self.biases) == np.ndarray
         assert isinstance(self.activation_function,ActivationFunctions)
 
         ### Checking value consistency ###
         assert self.size == self.output_height*self.output_width
-        assert self.weights.shape[2 + self.transpo[1]] == self.input_height if self.transpo[0] else self.input_width
+        assert self.weights.shape[self.transpo[1]] == self.input_height if self.transpo[0] else self.input_width
         assert self.output_height == self.input_width if self.transpo[0] else self.input_height
-        assert self.output_width == self.weights.shape[3 - self.transpo[1]]
-        assert (self.biases.shape[0] == 1 or self.biases.shape[0] == self.output_height) and (self.biases.shape[1] == 1 or self.biases.shape[1] == self.output_width)
+        assert self.output_width == self.weights.shape[1-self.transpo[1]]
+        assert all(self.biases.shape[i] == 1 or self.biases.shape[i] == output_shape[3-i] for i in range(len(self.biases.shape)))
 
         
     #The various ways to compute the operation: 
     
     #None of the tensor ar transposed
     def write_gemm_nn(self, m, n, k, A, B):
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,65 +14,52 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import numpy as np
 from ..Layer import Layer
+import numpy as np
 import pystache
 
-class InputLayer(Layer):
+class Softmax(Layer):
 
-    def __init__(self, idx:int, size:int, input_shape:list, data_format:str):
-       
+    def __init__(self, idx:int, size:int):
+        
         super().__init__()
         self.idx = idx
         self.size = size
-        self.output_channels = input_shape[1]
-        self.output_height = input_shape[2]
-        self.output_width = input_shape[3]
-        self.data_format = data_format
-        self.name = 'Input_layer'
+        self.name = 'Softmax'
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
         assert type(self.idx) == int
         assert type(self.size) == int
-        assert type(self.output_channels) == int
-        assert type(self.output_height) == int
-        assert type(self.output_width) == int
-        assert self.data_format == 'channels_last' or self.data_format == 'channels_first'
-
-        ### Checking value consistency ###
-        assert self.size == self.output_channels*self.output_height*self.output_width
 
     def generate_inference_code_layer(self):
+        output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
+        mustach_hash['size'] = self.size
         mustach_hash['road'] = self.path
+        mustach_hash['output_str'] = output_str
 
-        if(self.data_format == 'channels_last' and len(self.input_shape) == 4):
-            mustach_hash['channels_last'] = True
-            mustach_hash['input_channels'] = self.output_channels
-            mustach_hash['input_height'] = self.output_height
-            mustach_hash['input_width'] = self.output_width
-        else:
-            mustach_hash['size'] = self.size
-
+        if (self.fused_layer):
+            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output_'+str(self.path)+'[j]', self.idx, 'j')
 
-
-
-        with open(self.template_path+'layers/template_Input_Layer.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_Softmax.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
-
+    
     def forward_path_layer(self, input:np.ndarray):
         
-        return input 
+        exp = np.exp(input, dtype=np.float)
+        output = exp/np.sum(exp)
+
+        return output
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.nb_weights = self.count_elements_array(self.weights)
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
         assert type(self.idx) == int
         assert type(self.size) == int
-        assert type(self.input_shape) == list[int]
+        assert all(type(shape) == int for shape in self.input_shape)
         assert type(self.weights) == np.ndarray
         assert type(side) == bool
         assert isinstance(self.activation_function, ActivationFunctions)
 
         ### Checking value consistency ###
         if self.side:
             assert self.weights.shape[-1] == self.input_shape[-2]
@@ -83,12 +83,12 @@
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
         
     def forward_path_layer(self, input):
         
-        input = input.reshape(self.previous_layer[0].size)
+        input = input.reshape(self.input_shape)
         if self.side:
             return self.activation_function.compute(np.matmul(self.weights,input))
         else:
             return self.activation_function.compute(np.matmul(input,self.weights))
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         assert type(self.idx) == int
         assert type(self.size) == int
         assert all(type(pad) == int for pad in self.pads)
         assert type(self.constant_value) == float or type(self.constant_value) == int
         assert type(self.output_channels) == int
         assert type(self.output_height) == int
         assert type(self.output_width) == int
-        assert all(type(shape) == int for shape in self.input_shape)
+        assert all(type(shape) == int for shape in self.input_shape[1:])
         assert isinstance(self.activation_function, ActivationFunctions)
 
 
         ### Checking value consistency ###
         assert self.size == self.output_channels*self.output_height*self.output_width
         assert all(0 <= axe and axe < 4 for axe in self.axes)
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,29 +55,30 @@
 
 
     ####### Checking the instantiation#######
 
         ### Checking argument type ###
         assert type(self.idx) == int
         assert type(self.size) == int
-        assert type(self.padding) == str or type(self.padding) == np.ndarray
+        assert type(self.padding) == str or all(type(pad) == int for pad in self.padding)
         assert type(self.strides) == int
         assert type(self.pool_size) == int
         assert type(self.input_channels) == int
         assert type(self.input_height) == int
         assert type(self.input_width) == int
         assert type(self.output_channels) == int
         assert type(self.output_height) == int
         assert type(self.output_width) == int
         assert isinstance(self.activation_function, ActivationFunctions)
 
         ### Checking value consistency ###
         assert self.size == self.output_channels*self.output_height*self.output_width
-        assert self.output_height == math.ceil((self.input_height - self.pool_size)/self.strides) + 1
-        assert self.output_width == math.ceil((self.input_width - self.pool_size)/self.strides) + 1
+        assert self.size == self.output_channels*self.output_height*self.output_width
+        assert self.output_height == math.floor((self.input_height + self.pad_bottom + self.pad_top - self.pool_size)/self.strides) + 1
+        assert self.output_width == math.floor((self.input_width + self.pad_left + self.pad_right - self.pool_size)/self.strides) + 1
     
     @abstractmethod    
     def specific_function(self, index:str, input_of_layer:str):
         pass
 
     @abstractmethod    
     def update_local_vars(self):
@@ -88,14 +89,15 @@
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['comment'] = self.activation_function.comment
         mustach_hash['road'] = self.path
+        mustach_hash['size'] = self.size
 
         mustach_hash['activation_function'] = self.activation_function.write_activation_str(self.output_var)
 
         mustach_hash['input_channels'] = self.input_channels
         mustach_hash['output_height'] = self.output_height
         mustach_hash['output_width'] = self.output_width
         mustach_hash['update_local_vars'] = self.update_local_vars()
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,29 +76,26 @@
         self.scale = [1.,0.,0.,0.]
         if (boolean_resize):
             self.scale = target_size
             self.output_channels = int(self.input_channels*target_size[1]) #should be equal to input_channels
             self.output_height = int(self.input_height*target_size[2])
             self.output_width = int(self.input_width*target_size[3])
         else:
-            self.output_channels = target_size[1] #should be equal to input_channels
-            self.output_height = target_size[2]
-            self.output_width = target_size[3]
+            self.output_channels = int(target_size[1]) #should be equal to input_channels
+            self.output_height = int(target_size[2])
+            self.output_width = int(target_size[3])
             self.scale[1] = self.output_channels / self.input_channels #should be 1
             self.scale[2] = self.output_height / self.input_height
             self.scale[3] = self.output_width / self.input_width
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
         assert type(self.idx) == int
         assert type(self.size) == int
-        assert type(self.output_channels) == int
-        assert type(self.output_height) == int
-        assert type(self.output_width) == int
         assert type(self.input_channels) == int
         assert type(self.input_height) == int
         assert type(self.input_width) == int
         assert type(self.coordinate_transformation_mode) == str
         assert type(axes) == np.ndarray or type(axes) == list
         assert type(self.exclude_outside) == int
         assert type(self.keep_aspect_ratio_policy) == str
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,52 +14,70 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from ..Layer import Layer
 import numpy as np
+from ..Layer import Layer
 import pystache
 
-class Softmax(Layer):
+class InputLayer(Layer):
 
-    def __init__(self, idx:int, size:int):
-        
+    def __init__(self, idx:int, size:int, input_shape:list, data_format:str):
+       
         super().__init__()
         self.idx = idx
         self.size = size
-        self.name = 'Softmax'
+        self.input_shape = input_shape
+        if len(self.input_shape) == 4:
+            self.output_channels = self.input_shape[1]
+            self.output_height = self.input_shape[2]
+            self.output_width = self.input_shape[3]
+        self.data_format = data_format
+        self.name = 'Input_layer'
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
         assert type(self.idx) == int
         assert type(self.size) == int
+        assert all(type(dim) == int for dim in self.input_shape[1:])
+        assert self.data_format == 'channels_last' or self.data_format == 'channels_first'
+
+        ### Checking value consistency ###
+        prod = 1
+        for shape in self.input_shape:
+            if shape != None and shape != 0:
+                prod *= shape
+
+        assert self.size == prod
 
     def generate_inference_code_layer(self):
-        output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
-        mustach_hash['size'] = self.size
         mustach_hash['road'] = self.path
-        mustach_hash['output_str'] = output_str
 
-        if (self.fused_layer):
-            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output_'+str(self.path)+'[j]', self.idx, 'j')
+        if(self.data_format == 'channels_last' and len(self.input_shape) == 4):
+            mustach_hash['channels_last'] = True
+            mustach_hash['input_channels'] = self.output_channels
+            mustach_hash['input_height'] = self.output_height
+            mustach_hash['input_width'] = self.output_width
+        else:
+            mustach_hash['size'] = self.size
 
-        with open(self.template_path+'layers/template_Softmax.c.tpl','r') as template_file:
+
+
+
+        with open(self.template_path+'layers/template_Input_Layer.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
-    
+
     def forward_path_layer(self, input:np.ndarray):
         
-        exp = np.exp(input, dtype=np.float)
-        output = exp/np.sum(exp)
-
-        return output
+        return input
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.3/src/acetone_nnet/code_generator/neural_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ResizeLinear, ResizeCubic, ResizeNearest, 
     Conv2D, Conv2D_6loops, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pooling2D, MaxPooling2D, AveragePooling2D
 )
 
 class CodeGenerator(ABC):
 
-    def __init__(self, file:str|onnx.ModelProto|Functional|Sequential, test_dataset:str|np.ndarray|None=None, function_name:str='inference', nb_tests:int|str=None, conv_algorithm:str='std_gemm_nn', normalize:bool|str=False, debug_mode:str|None=None, debug_target:list|None=None,**kwargs):
+    def __init__(self, file:str|onnx.ModelProto|Functional|Sequential, test_dataset:str|np.ndarray|None=None, function_name:str='inference', nb_tests:int|str=None, conv_algorithm:str='std_gemm_nn', normalize:bool|str=False, debug_mode:str|None=None,**kwargs):
 
         self.file = file
         self.function_name = function_name
         self.nb_tests = int(nb_tests)
         self.conv_algorithm = conv_algorithm
         self.normalize = bool(normalize)
         self.template_path = templates.__file__[:-11]
@@ -75,53 +75,49 @@
             self.test_dataset = ds
 
         self.files_to_gen = ['inference.c', 'inference.h', 'global_vars.c', 'main.c', 'Makefile', 'test_dataset.h', 'test_dataset.c']
         
         ##### Debug Mode #####
         self.debug_mode = debug_mode
         if self.debug_mode:
-            self.debug_target = self.load_debug_target(debug_mode, debug_target)
+            self.debug_target = self.load_debug_target(debug_mode)
         ##### Debug Mode #####
             
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
         assert type(self.file) == str or type(self.file) == onnx.ModelProto or type(self.file) == Functional or type(self.file) == Sequential
-        assert type(test_dataset) == str or type(test_dataset) == np.ndarray or type(test_dataset) == None
+        assert type(test_dataset) == str or type(test_dataset) == np.ndarray or test_dataset == None
         assert type(self.test_dataset) == np.ndarray
         assert type(self.function_name) == str
         assert type(self.conv_algorithm) == str
-        assert type(self.debug_mode) == None or type(self.debug_mode) == str
+        assert self.debug_mode == None or type(self.debug_mode) == str
         if self.debug_mode:
             assert type(self.debug_target) == list
 
         ### Checking value consistency ###
         assert self.conv_algorithm in ['6loops',
                                        'indirect_gemm_nn','indirect_gemm_tn','indirect_gemm_nt','indirect_gemm_tt',
                                        'std_gemm_nn','std_gemm_tn','std_gemm_nt','std_gemm_']
         ##### Debug Mode #####
         if self.debug_mode:
             assert self.debug_mode in ['keras','onnx']
             assert len(self.debug_target) <= len(self.layers)
             assert all(target <= len(self.layers) for target in self.debug_target)
         ##### Debug Mode #####
     
-    def load_debug_target(self, debug_mode:str|None, debug_target:list|None):
-        if debug_target == None:
-            return debug_target
-        
-        else:
-            targets = []
-            for layer in self.layers[1:]:
-                if debug_mode == 'keras' and layer.name == 'Softmax':
-                    targets[-1] = layer.idx
-                else:
-                    targets.append(layer.idx)
+    def load_debug_target(self, debug_mode:str|None):
+        targets = []
+        for layer in self.layers[1:]:
+            if debug_mode == 'keras' and layer.name == 'Softmax':
+                targets[-1] = layer.idx
+            else:
+                targets.append(layer.idx)
 
-            return targets
+        return targets
         
     def create_test_dataset(self):
         test_dataset = self.data_type_py(np.random.default_rng(seed=10).random((self.nb_tests,1,int(self.layers[0].size))))
         return test_dataset 
      
     def load_test_dataset(self):
         
@@ -150,14 +146,15 @@
     def compute_inference(self, c_files_directory:str):
         with open(os.path.join(c_files_directory, 'output_python.txt'), 'w+') as fi:
             for nn_input in self.test_dataset:
                 
                 ##### Debug Mode #####
                 if self.debug_mode:
                     debug_output = []
+                    targets = []
                 ##### Debug Mode #####
 
                 if((self.data_format == 'channels_last') and (len(self.layers[0].input_shape) == 4)): 
                     shape = (self.layers[0].input_shape[2],self.layers[0].input_shape[3],self.layers[0].input_shape[1])
                     nn_input = np.transpose(np.reshape(nn_input, shape), (2,0,1))
 
                 if (self.normalize): nn_input = self.Normalizer.pre_processing(nn_input)
@@ -215,16 +212,15 @@
                             if layer.idx in self.debug_target:
                                 debug_output.append(previous_layer_result[layer.path])
                                 if((self.data_format == 'channels_last') and hasattr(layer, 'output_channels')): debug_output[-1] = np.transpose(debug_output[-1], (1,2,0))
                                 debug_output[-1] = debug_output[-1].flatten()
 
                         # If all the targets are saved, the inference is stopped and the result is given
                         if len(debug_output) == len(self.debug_target):
-                            targets = [str(self.layers[k].name) + " " + str(self.layers[k].idx) for k in self.debug_target]
-                            return debug_output, targets
+                            targets.append(str(layer.name) + " " + str(layer.idx))
                     ##### Debug Mode #####
                         
                 nn_output = previous_layer_result[layer.path]
                 # print(nn_output) # write to file instead
                 
                 # Write results in text files to compare prediction.
                 if((self.data_format == 'channels_last') and hasattr(layer, 'output_channels')): nn_output = np.transpose(nn_output, (1,2,0))
@@ -238,15 +234,18 @@
                     # print(decimal.Decimal(nn_output[j]), end=' ', file=fi, flush=True)
                 print(" ",file=fi)
         
         fi.close()
 
         print("File output_python.txt generated.")
 
-        return nn_output
+        if self.debug_mode:
+            return debug_output, targets
+        else:
+            return nn_output
 
     def flatten_array_orderc(self, array:np.ndarray):
     
         flattened_aray = array.flatten(order='C')
         s = '\n        {'
         for i in range(flattened_aray.size):
             s += str(flattened_aray[i])+', '
@@ -502,15 +501,14 @@
             
         if (any(isinstance(layer, Concatenate) 
                 or any(isinstance(layer, Conv2D)) 
                 or any(isinstance(layer, Dense))
                 or any(issubclass(layer, Broadcast)) 
                 or any(isinstance(layer, Gather)) 
                 or any(isinstance(layer, Pad))) for layer in self.layers):
-            mustach_hash['tensor_temp'] = True
             mustach_hash['temp_size'] = max(self.l_size_max,self.patches_size_max)
  
         mustach_hash['layers'] = []
         for layer in self.layers:
             to_print = False
             layer_hash = {'name':layer.name, 'idx':"{:02d}".format(layer.idx)}
 
@@ -575,15 +573,14 @@
         
         if (any(isinstance(layer, Concatenate) 
                 or any(isinstance(layer, Conv2D)) 
                 or any(isinstance(layer, Dense))
                 or any(issubclass(layer, Broadcast)) 
                 or any(isinstance(layer, Gather)) 
                 or any(isinstance(layer, Pad))) for layer in self.layers):
-            mustach_hash['tensor_temp'] = True
             mustach_hash['temp_size'] = max(self.l_size_max,self.patches_size_max)
              
         if any(isinstance(layer, Conv2D_indirect_gemm) for layer in self.layers):
             mustach_hash['zero'] = True
         
         mustach_hash['layers'] = []
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/H5_importer/parser_h5.py` & `acetone_nnet-0.3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py` & `acetone_nnet-0.3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone_nnet-0.3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,19 +93,19 @@
             shape = [info.type.tensor_type.shape.dim[i].dim_value for i in range(len(info.type.tensor_type.shape.dim))]
     for input in model.graph.input:
         if(shape_name == input.name):
             shape = [input.type.tensor_type.shape.dim[i].dim_value for i in range(len(input.type.tensor_type.shape.dim))]
     for output in model.graph.output:
         if(shape_name == output.name):
             shape = [output.type.tensor_type.shape.dim[i].dim_value for i in range(len(output.type.tensor_type.shape.dim))]
-    if (shape and len(shape)<=4):
-        shape = [1 for i in range(4-len(shape))] + shape
     for i in range(len(shape)):
         if shape[i] == 0:
             shape[i] = 1
+    if (shape and len(shape)<=4):
+        shape = [1 for i in range(4-len(shape))] + shape
     return shape
 
 #Return the size of the layer when given the list output_shape
 def find_size(output_shape:list):
     size = 1
     for i in output_shape:
         if i != 0:
@@ -336,19 +336,28 @@
     dict_output[node.output[0]] = idx
     right_tensor = look_for_initializer(node.input[0],model)
     left_tensor = look_for_initializer(node.input[1],model)
     if(left_tensor or right_tensor):
         if(right_tensor and not left_tensor):
             #the weigth is the right tensor:  MatMul(W,T)
             side = True
+            input_shape = get_shape(node.input[1],model)
             weights = onnx.numpy_helper.to_array(right_tensor)
-            weights = np.reshape(weights, (get_shape(node.input[1],model)[-2],1,1,output_shape[-2]))
+            shape = get_shape(node.input[1],model)
+            count = 0
+            for i in shape:
+                if i == 1:
+                    count += 1
+            if count == 3 and input_shape[-1] != 1:
+                weights = np.reshape(weights, (get_shape(node.input[1],model)[-1],1,1,output_shape[-1]))
+                input_shape = [1,1,input_shape[-1],1]
+            else:
+                weights = np.reshape(weights, (get_shape(node.input[1],model)[-2],1,1,output_shape[-2]))
             weights = np.moveaxis(weights, 0,3)
             dict_input[idx] = [node.input[1]]
-            input_shape = get_shape(node.input[1],model)
         if(left_tensor and not right_tensor):
             #the weigth is the right tensor:  MatMul(W,T)
             side = False
             weights = onnx.numpy_helper.to_array(left_tensor)
             weights = np.reshape(weights, (1,1,get_shape(node.input[0],model)[-1],output_shape[-1]))
             dict_input[idx] = [node.input[0]]
             input_shape = get_shape(node.input[0],model)
@@ -456,15 +465,15 @@
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
     return AveragePooling2D(idx = idx,
                             size = size,
                             padding = [0,0,0,0],
-                            strides = 0,
+                            strides = 1,
                             pool_size = input_shape[2],
                             input_shape = input_shape,
                             output_shape = output_shape,
                             activation_function = Linear())
 
 ### Broadcats layers ###
 
@@ -505,25 +514,26 @@
     if(constant.any()):
         if (len(constant.shape)<4):
             for i in range(0,4-len(constant.shape)):
                 constant = np.expand_dims(constant,axis=0)
         input_shapes.append(constant.shape)
     else:
         constant = None
+    input_shapes = np.array(input_shapes)
     return Add(idx = idx,
                 size = size,
                 input_shapes = input_shapes,
                 output_shape = output_shape,
                 activation_function = Linear(),
                 constant = constant)
     
 #create a layer Div
 def create_Div(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shapes =[]
-    constant = 1
+    constant = np.ones(get_shape(node.input[0], model))
     dict_input[idx] = []
     for input in node.input:
         factor = look_for_initializer(input,model)
         if(factor):
             constant = constant / onnx.numpy_helper.to_array(factor)
         else:
             dict_input[idx].append(input)
@@ -534,26 +544,27 @@
     if((constant == np.ones(constant.shape)).all()):
         constant = None
     else:
         if (len(constant.shape)<4):
             for i in range(0,4-len(constant.shape)):
                 constant = np.expand_dims(constant,axis=0)
         input_shapes.append(constant.shape)
+    input_shapes = np.array(input_shapes)
     return Divide(idx=idx,
                     size=size,
                     input_shapes=input_shapes,
                     output_shape=output_shape,
                     activation_function= Linear(),
                     constant=constant)
 
 
 #create a layer Mul
 def create_Mul(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shapes =[]
-    constant = 1
+    constant = np.ones(get_shape(node.input[0], model))
     dict_input[idx] = []
     for input in node.input:
         factor = look_for_initializer(input,model)
         if(factor):
             constant = constant * onnx.numpy_helper.to_array(factor)
         else:
             dict_input[idx].append(input)
@@ -563,44 +574,46 @@
     dict_output[node.output[0]] = idx
     if((constant == np.ones(constant.shape)).all()):
         constant = None
     else:
         if (len(constant.shape)<4):
             for i in range(0,4-len(constant.shape)):
                 constant = np.expand_dims(constant,axis=0)
-        input_shapes.append(constant.shape)
+        input_shapes.append(list(constant.shape))
+    input_shapes = np.array(input_shapes)
     return Multiply(idx=idx,
                     size=size,
                     input_shapes=input_shapes,
                     output_shape=output_shape,
                     activation_function= Linear(),
                     constant=constant)
 
 #create a layer Sub
 def create_Sub(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shapes =[]
-    constant = 0
+    constant = np.zeros(get_shape(node.input[0], model))
     dict_input[idx] = []
     for input in node.input:
         factor = look_for_initializer(input,model)
         if(factor):
             constant = constant - onnx.numpy_helper.to_array(factor)
         else:
             dict_input[idx].append(input)
             input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_output[node.output[0]] = idx
-    if((constant == np.ones(constant.shape)).all()):
+    if(not constant.any()):
         constant = None
     else:
         if (len(constant.shape)<4):
             for i in range(0,4-len(constant.shape)):
                 constant = np.expand_dims(constant,axis=0)
         input_shapes.append(constant.shape)
+    input_shapes = np.array(input_shapes)
     return Subtract(idx=idx,
                     size=size,
                     input_shapes=input_shapes,
                     output_shape=output_shape,
                     activation_function= Linear(),
                     constant=constant)
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.3/src/acetone_nnet/format_importer/parser.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.3/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/__init__.py` & `acetone_nnet-0.3/src/acetone_nnet/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-        // gemm_nn
+    // gemm_nt
     for (i = 0; i < {{m}}; ++i)
     {
-        for (p = 0; p < {{k}}; ++p)
+        for (j = 0; j < {{n}}; ++j)
         {
-            register float weight = {{#alpha}}{{.}} * {{/alpha}}{{A}}[i*{{k}}+p];
-            for(j = 0; j < {{n}}; ++j)
+            register float output =0;
+            for (p = 0; p < {{k}}; ++p)
             {
-                tensor_temp[j*{{m}} + i] += weight * ({{B}}[j*{{k}} + p]);
+                output += {{#alpha}}{{.}}*{{/alpha}}{{A}}[p*{{m}}+i]*({{B}}[j*{{k}}+p]);
             }
-        }
-        for(j = 0; j<{{n}}; ++j)
-        {
-            register float output = tensor_temp[j*{{m}} + i];
-            output += {{#beta}}{{.}} * {{/beta}}biases_{{name}}_{{idx}}[i];
+            output += {{#beta}}{{.}}*{{/beta}}biases_{{name}}_{{idx}}[i];
         {{^fused_layer}}
-            tensor_temp[j*{{m}} + i] = {{{activation_function}}};
+            tensor_temp[j*{{m}}+i] = {{{activation_function}}};
         {{/fused_layer}}
         {{#fused_layer}}
             {{^linear}}
             output = {{{activation_function}}};
             {{/linear}}
-            tensor_temp[j*{{m}} + i] = {{{fused_layer}}};
+            tensor_temp[j*{{m}}+i] = {{{fused_layer}}};
         {{/fused_layer}}
         }
     }
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-    // gemm_nt
-    for (i = 0; i < {{m}}; ++i)
+    // gemm_tn
+    for (i = 0; i < {{m}}; i++)
     {
-        for (j = 0; j < {{n}}; ++j)
+        for(j = 0; j < {{n}}; ++j)
         {
-            register float output =0;
+            float register output = 0;
             for (p = 0; p < {{k}}; ++p)
             {
-                output += {{#alpha}}{{.}}{{/alpha}} * {{A}}[p*{{m}}+i] * ({{B}}[j*{{k}}+p]);
-            }
-            output += {{#beta}}{{.}}{{/beta}} * biases_{{name}}_{{idx}}[i];
+                output += {{#alpha}}{{.}}*{{/alpha}}{{A}}[i*{{k}}+p]*{{#direct}}*{{/direct}}({{B}}[p*{{n}}+j]);
+            }   
+            output += {{#beta}}{{.}}*{{/beta}}biases_{{name}}_{{idx}}[i];
         {{^fused_layer}}
-            tensor_temp[j*{{m}}+i] = {{{activation_function}}};
+            tensor_temp[j*{{m}} + i] = {{{activation_function}}};
         {{/fused_layer}}
         {{#fused_layer}}
             {{^linear}}
             output = {{{activation_function}}};
             {{/linear}}
-            tensor_temp[j*{{m}}+i] = {{{fused_layer}}};
+            tensor_temp[j*{{m}} + i] = {{{fused_layer}}};
         {{/fused_layer}}
+            
         }
     }
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-    // gemm_tn
-    for (i = 0; i < {{m}}; i++)
+        // gemm_nn
+    for (i = 0; i < {{m}}; ++i)
     {
-        for(j = 0; j < {{n}}; ++j)
+        for (p = 0; p < {{k}}; ++p)
         {
-            float register output = 0;
-            for (p = 0; p < {{k}}; ++p)
+            register float weight = {{#alpha}}{{.}}*{{/alpha}}{{A}}[i*{{k}}+p];
+            for(j = 0; j < {{n}}; ++j)
             {
-                output += {{#alpha}}{{.}}{{/alpha}} * {{A}}[i*{{k}}+p] * {{#direct}}*{{/direct}}({{B}}[p*{{n}}+j]);
-            }   
-            output += {{#beta}}{{.}}{{/beta}} * biases_{{name}}_{{idx}}[i];
+                tensor_temp[j*{{m}} + i] += weight*({{B}}[j*{{k}} + p]);
+            }
+        }
+        for(j = 0; j<{{n}}; ++j)
+        {
+            register float output = tensor_temp[j*{{m}} + i];
+            output += {{#beta}}{{.}}*{{/beta}}biases_{{name}}_{{idx}}[i];
         {{^fused_layer}}
             tensor_temp[j*{{m}} + i] = {{{activation_function}}};
         {{/fused_layer}}
         {{#fused_layer}}
             {{^linear}}
             output = {{{activation_function}}};
             {{/linear}}
             tensor_temp[j*{{m}} + i] = {{{fused_layer}}};
         {{/fused_layer}}
-            
         }
     }
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
     for (i = 0; i < {{m}}; ++i)
     {
         for (j = 0; j < {{n}}; ++j)
         {
             float register sum = 0;
             for (p = 0; p < {{k}}; ++p)
             {
-                sum += {{#alpha}}{{.}}{{/alpha}} * {{A}}[p*{{m}} +i]* {{#direct}}*{{/direct}}({{B}}[p*{{n}}+j]);
+                sum += {{#alpha}}{{.}}*{{/alpha}}{{A}}[p*{{m}} +i]*{{#direct}}*{{/direct}}({{B}}[p*{{n}}+j]);
             }
-            sum += {{#beta}}{{.}}{{/beta}} * biases_{{name}}_{{idx}}[i];
+            sum += {{#beta}}{{.}}*{{/beta}}biases_{{name}}_{{idx}}[i];
         {{^fused_layer}}
             tensor_temp[j*{{n}}+i] = {{{activation_function}}};
         {{/fused_layer}}
         {{#fused_layer}}
             {{^linear}}
             sum = {{{activation_function}}};
             {{/linear}}
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Dense.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Dense.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Dot.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Dot.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Flatten.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Gather.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Gather.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_MatMul.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl`

 * *Files 19% similar despite different names*

```diff
@@ -15,18 +15,23 @@
                         if (ii >= 0 && ii < {{input_height}} && jj >= 0 && jj < {{input_width}})
                         {
                             {{{specific_function}}}
                         }
                     }
                 }
                 {{^fused_layer}}
-                output_{{road}}[j + {{output_width}}*(i + {{output_height}}*f)] = {{{activation_function}}};
+                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{{activation_function}}};
                 {{/fused_layer}}
                 {{#fused_layer}}
                     {{^linear}}
                 {{local_var}} = {{{activation_function}}};
                     {{/linear}}
-                output_{{road}}[j + {{output_width}}*(i + {{output_height}}*f)] = {{{fused_layer}}};
+                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{{fused_layer}}};
                 {{/fused_layer}}
             }
         }
+    }
+
+    for (k = 0; k < {{size}}; ++k)
+    {
+        output_{{road}}[k] = tensor_temp[k];
     }
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_global_var_file.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/template_global_var_file.c.tpl`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 {{#cst}}
     {{#name}}
 {{data_type}} cst_{{name}}[{{size}}];
     {{/name}}
 {{/cst}}
 
-{{#tensor_temp}}
+{{#temp_size}}
 {{data_type}} tensor_temp[{{temp_size}}];
 
-{{/tensor_temp}}
+{{/temp_size}}
 {{#zero}}
 {{data_type}} zero = 0.0f;
 
 {{/zero}}
 {{#layers}}
     {{#nb_weights}}
 {{data_type}} weights_{{name}}_{{idx}}[{{nb_weights}}] = {{weights}};
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_header_file.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/template_header_file.c.tpl`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 {{#cst}}
     {{#name}}
 {{data_type}} cst_{{name}}[{{size}}];
     {{/name}}
 {{/cst}}
 
-{{#tensor_temp}}
+{{#temp_size}}
 {{data_type}} tensor_temp[{{temp_size}}];
 
-{{/tensor_temp}}
+{{/temp_size}}
 {{#layers}}
     {{#nb_weights}}
 extern {{data_type}} weights_{{name}}_{{idx}}[{{nb_weights}}];
     {{/nb_weights}}
     {{#nb_biases}}
 extern {{data_type}} biases_{{name}}_{{idx}}[{{nb_biases}}];
     {{/nb_biases}}
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_main_file.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/template_main_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_source_file.c.tpl` & `acetone_nnet-0.3/src/acetone_nnet/templates/template_source_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/PKG-INFO` & `acetone_nnet-0.3/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.2.3.dev4
+Version: 0.3
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone_nnet-0.3/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,18 @@
 src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
 src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
 src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
 src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+src/acetone_nnet/debug_tools/__init__.py
+src/acetone_nnet/debug_tools/debug_keras.py
+src/acetone_nnet/debug_tools/debug_onnx.py
+src/acetone_nnet/debug_tools/debug_tools.py
 src/acetone_nnet/format_importer/parser.py
 src/acetone_nnet/format_importer/H5_importer/parser_h5.py
 src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
 src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
 src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
 src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
 src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
```

