# Comparing `tmp/onediff-1.1.0.dev202405210127.tar.gz` & `tmp/onediff-1.1.0.dev202405220128.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediff-1.1.0.dev202405210127.tar", last modified: Tue May 21 01:27:57 2024, max compression
+gzip compressed data, was "onediff-1.1.0.dev202405220128.tar", last modified: Wed May 22 01:28:17 2024, max compression
```

## Comparing `onediff-1.1.0.dev202405210127.tar` & `onediff-1.1.0.dev202405220128.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.025021 onediff-1.1.0.dev202405210127/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-21 01:27:50.000000 onediff-1.1.0.dev202405210127/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-21 01:27:57.025021 onediff-1.1.0.dev202405210127/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-05-21 01:27:50.000000 onediff-1.1.0.dev202405210127/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 01:27:57.025021 onediff-1.1.0.dev202405210127/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.009021 onediff-1.1.0.dev202405210127/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.013021 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.013021 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77140 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.013021 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers_enterprise_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.013021 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_onediff_quant/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_onediff_quant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.013021 onediff-1.1.0.dev202405210127/src/onediff/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.017021 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.017021 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/backends/nexfort.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/backends/oneflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/backends/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.017021 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/core/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/core/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/core/with_onediff_compile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.017021 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/import_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/import_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/import_tools/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/import_tools/import_module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/import_tools/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.017021 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/nexfort/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/nexfort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/nexfort/deployable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.021021 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/oneflow/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/oneflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/oneflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/oneflow/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/oneflow/dual_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/oneflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/oneflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.021021 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15054 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/transform/builtin_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/transform/custom_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/transform/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/transform/patch_for_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.021021 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/args_tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/cost_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/graph_management_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/model_inplace_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/module_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/online_quantization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/param_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/patch_for_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/patch_for_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/version_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.025021 onediff-1.1.0.dev202405210127/src/onediff/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/optimization/attention_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/optimization/quant_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/optimization/rewrite_self_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.025021 onediff-1.1.0.dev202405210127/src/onediff/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/quantization/load_quantized_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/quantization/quant_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/quantization/quantize_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/quantization/quantize_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.025021 onediff-1.1.0.dev202405210127/src/onediff/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/src/onediff/schedulers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.025021 onediff-1.1.0.dev202405210127/src/onediff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-21 01:27:57.000000 onediff-1.1.0.dev202405210127/src/onediff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-21 01:27:57.000000 onediff-1.1.0.dev202405210127/src/onediff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 01:27:57.000000 onediff-1.1.0.dev202405210127/src/onediff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 01:27:57.000000 onediff-1.1.0.dev202405210127/src/onediff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 01:27:57.000000 onediff-1.1.0.dev202405210127/src/onediff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:27:57.025021 onediff-1.1.0.dev202405210127/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/tests/test_dual_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/tests/test_pipelines_oneflow_img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/tests/test_quantitative_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-21 01:27:51.000000 onediff-1.1.0.dev202405210127/tests/test_quantize_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.537298 onediff-1.1.0.dev202405220128/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-22 01:28:17.537298 onediff-1.1.0.dev202405220128/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:28:17.537298 onediff-1.1.0.dev202405220128/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.521298 onediff-1.1.0.dev202405220128/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.525297 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.525297 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77125 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24024 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61005 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24118 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.525297 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers_enterprise_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.525297 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_onediff_quant/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_onediff_quant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.525297 onediff-1.1.0.dev202405220128/src/onediff/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.529297 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.529297 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/deployable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.529297 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/nexfort/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/nexfort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/nexfort/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/nexfort/nexfort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.529297 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/dual_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/graph_management_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.533298 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/import_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/import_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/oneflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/param_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.533298 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/transform/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.533298 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.533298 onediff-1.1.0.dev202405220128/src/onediff/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/optimization/attention_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/optimization/quant_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/optimization/rewrite_self_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.533298 onediff-1.1.0.dev202405220128/src/onediff/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/quantization/load_quantized_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/quantization/quant_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/quantization/quantize_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/quantization/quantize_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.533298 onediff-1.1.0.dev202405220128/src/onediff/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/schedulers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.537298 onediff-1.1.0.dev202405220128/src/onediff/torch_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/torch_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/torch_utils/model_inplace_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/torch_utils/module_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.537298 onediff-1.1.0.dev202405220128/src/onediff/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/src/onediff/utils/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.537298 onediff-1.1.0.dev202405220128/src/onediff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-22 01:28:17.000000 onediff-1.1.0.dev202405220128/src/onediff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-22 01:28:17.000000 onediff-1.1.0.dev202405220128/src/onediff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:28:17.000000 onediff-1.1.0.dev202405220128/src/onediff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 01:28:17.000000 onediff-1.1.0.dev202405220128/src/onediff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-22 01:28:17.000000 onediff-1.1.0.dev202405220128/src/onediff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:28:17.537298 onediff-1.1.0.dev202405220128/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/tests/test_dual_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/tests/test_pipelines_oneflow_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/tests/test_quantitative_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-22 01:28:11.000000 onediff-1.1.0.dev202405220128/tests/test_quantize_custom_model.py
```

### Comparing `onediff-1.1.0.dev202405210127/LICENSE` & `onediff-1.1.0.dev202405220128/LICENSE`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405210127/PKG-INFO` & `onediff-1.1.0.dev202405220128/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.1.0.dev202405210127
+Version: 1.1.0.dev202405220128
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405210127 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405220128 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 contact@siliconflow.com License: Apache-2.0 Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `onediff-1.1.0.dev202405210127/README.md` & `onediff-1.1.0.dev202405220128/README.md`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405210127/setup.py` & `onediff-1.1.0.dev202405220128/setup.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/__init__.py` & `onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from onediff.infer_compiler.transform import register
+from onediff.infer_compiler.backends.oneflow.transform import register
 
 from packaging import version
 import importlib.metadata
 
 diffusers_version = version.parse(importlib.metadata.version("diffusers"))
 
 # register(package_names=["diffusers"])
@@ -11,48 +11,60 @@
     AttnProcessor,
     AttnProcessor2_0,
 )
 from diffusers.models.attention_processor import LoRAAttnProcessor2_0
 
 if diffusers_version < version.parse("0.26.00"):
     from diffusers.models.unet_2d_condition import UNet2DConditionModel
-    from diffusers.models.unet_2d_blocks import AttnUpBlock2D, CrossAttnUpBlock2D, UpBlock2D
+    from diffusers.models.unet_2d_blocks import (
+        AttnUpBlock2D,
+        CrossAttnUpBlock2D,
+        UpBlock2D,
+    )
     from diffusers.models.transformer_2d import Transformer2DModel
 else:
     from diffusers.models.unets.unet_2d_condition import UNet2DConditionModel
-    from diffusers.models.unets.unet_2d_blocks import AttnUpBlock2D, CrossAttnUpBlock2D, UpBlock2D
+    from diffusers.models.unets.unet_2d_blocks import (
+        AttnUpBlock2D,
+        CrossAttnUpBlock2D,
+        UpBlock2D,
+    )
     from diffusers.models.transformers.transformer_2d import Transformer2DModel
 
 if diffusers_version >= version.parse("0.25.00"):
     from diffusers.models.upsampling import Upsample2D
 else:
     from diffusers.models.resnet import Upsample2D
 if diffusers_version >= version.parse("0.24.00"):
     from diffusers.models.resnet import SpatioTemporalResBlock
     from diffusers.models.attention import TemporalBasicTransformerBlock
 
     if diffusers_version >= version.parse("0.26.00"):
         from diffusers.models.unets.unet_spatio_temporal_condition import (
             UNetSpatioTemporalConditionModel,
         )
-        from diffusers.models.transformers.transformer_temporal import TransformerSpatioTemporalModel
+        from diffusers.models.transformers.transformer_temporal import (
+            TransformerSpatioTemporalModel,
+        )
     else:
         from diffusers.models.transformer_temporal import TransformerSpatioTemporalModel
         from diffusers.models.unet_spatio_temporal_condition import (
             UNetSpatioTemporalConditionModel,
         )
 
     if diffusers_version >= version.parse("0.25.00"):
         from diffusers.models.autoencoders.autoencoder_kl_temporal_decoder import (
             TemporalDecoder,
         )
     else:
         from diffusers.models.autoencoder_kl_temporal_decoder import TemporalDecoder
-    
-    from .spatio_temporal_oflow import SpatioTemporalResBlock as SpatioTemporalResBlockOflow
+
+    from .spatio_temporal_oflow import (
+        SpatioTemporalResBlock as SpatioTemporalResBlockOflow,
+    )
     from .spatio_temporal_oflow import TemporalDecoder as TemporalDecoderOflow
     from .spatio_temporal_oflow import (
         TransformerSpatioTemporalModel as TransformerSpatioTemporalModelOflow,
     )
     from .spatio_temporal_oflow import (
         TemporalBasicTransformerBlock as TemporalBasicTransformerBlockOflow,
     )
```

### Comparing `onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py` & `onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import oneflow.nn.functional as F
 from oneflow import nn
 import os
 
 import diffusers
 from diffusers.utils import deprecate, logging
 
-from onediff.infer_compiler.utils import parse_boolean_from_env, set_boolean_env_var
+from onediff.utils import parse_boolean_from_env, set_boolean_env_var
 
 
 def is_xformers_available():
     return False
 
 
 # from .lora import LoRALinearLayer
```

### Comparing `onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py` & `onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/resnet_oflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 import oneflow as torch
 import oneflow.nn as nn
 import oneflow.nn.functional as F
 from packaging import version
 import importlib.metadata
 
-from onediff.infer_compiler.transform import transform_mgr
+from onediff.infer_compiler.backends.oneflow.transform import transform_mgr
 
 transformed_diffusers = transform_mgr.transform_package("diffusers")
 
 diffusers_0210_v = version.parse("0.21.0")
 diffusers_0220_v = version.parse("0.22.0")
 diffusers_version = version.parse(importlib.metadata.version("diffusers"))
```

### Comparing `onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py` & `onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 diffusers_version = version.parse(importlib.metadata.version("diffusers"))
 
 diffusers_0240_v = version.parse("0.24.0")
 
 if diffusers_version >= diffusers_0240_v:
 
-    from onediff.infer_compiler.transform import transform_mgr
+    from onediff.infer_compiler.backends.oneflow.transform import transform_mgr
 
     transformed_diffusers = transform_mgr.transform_package("diffusers")
 
     diffusers_0260_v = version.parse("0.26.0")
 
     if diffusers_version >= diffusers_0260_v:
         DiffusersUNetSpatioTemporalConditionModel = (
```

### Comparing `onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py` & `onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, Optional
 from packaging import version
 import importlib.metadata
 
 import oneflow as torch
 import oneflow.nn.functional as F
 from oneflow import nn
-from onediff.infer_compiler.transform import transform_mgr
+from onediff.infer_compiler.backends.oneflow.transform import transform_mgr
 
 transformed_diffusers = transform_mgr.transform_package("diffusers")
 
 diffusers_0220_v = version.parse("0.22.0")
 diffusers_02499_v = version.parse("0.24.99")
 diffusers_0270_v = version.parse("0.27.0")
 diffusers_version = version.parse(importlib.metadata.version("diffusers"))
@@ -964,15 +964,17 @@
             Returns:
                 If `return_dict` is True, an [`~models.transformer_2d.Transformer2DModelOutput`] is returned, otherwise a
                 `tuple` where the first element is the sample tensor.
             """
             if diffusers_version >= diffusers_0270_v:
                 if cross_attention_kwargs is not None:
                     if cross_attention_kwargs.get("scale", None) is not None:
-                        logger.warning("Passing `scale` to `cross_attention_kwargs` is depcrecated. `scale` will be ignored.")
+                        logger.warning(
+                            "Passing `scale` to `cross_attention_kwargs` is depcrecated. `scale` will be ignored."
+                        )
             # ensure attention_mask is a bias, and give it a singleton query_tokens dimension.
             #   we may have done this conversion already, e.g. if we came here via UNet2DConditionModel#forward.
             #   we can tell by counting dims; if ndim == 2: it's a mask rather than a bias.
             # expects mask of shape:
             #   [batch, key_tokens]
             # adds singleton query_tokens dimension:
             #   [batch,                    1, key_tokens]
```

### Comparing `onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py` & `onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 from packaging import version
 import importlib.metadata
 import oneflow as torch
-from onediff.infer_compiler.transform import transform_mgr
+from onediff.infer_compiler.backends.oneflow.transform import transform_mgr
 
 diffusers_0210_v = version.parse("0.21.0")
 diffusers_version = version.parse(importlib.metadata.version("diffusers"))
 
 transformed_diffusers = transform_mgr.transform_package("diffusers")
 
 if diffusers_version < diffusers_0210_v:
@@ -66,15 +66,17 @@
                             else:
                                 return module(*inputs)
 
                         return custom_forward
 
                     ckpt_kwargs: Dict[str, Any] = {
                         "use_reentrant": False
-                    } if transformed_diffusers.utils.is_torch_version(">=", "1.11.0") else {}
+                    } if transformed_diffusers.utils.is_torch_version(
+                        ">=", "1.11.0"
+                    ) else {}
                     hidden_states = torch.utils.checkpoint.checkpoint(
                         create_custom_forward(resnet),
                         hidden_states,
                         temb,
                         **ckpt_kwargs,
                     )
                     hidden_states = attn(
@@ -232,15 +234,17 @@
                             else:
                                 return module(*inputs)
 
                         return custom_forward
 
                     ckpt_kwargs: Dict[str, Any] = {
                         "use_reentrant": False
-                    } if transformed_diffusers.utils.is_torch_version(">=", "1.11.0") else {}
+                    } if transformed_diffusers.utils.is_torch_version(
+                        ">=", "1.11.0"
+                    ) else {}
                     hidden_states = torch.utils.checkpoint.checkpoint(
                         create_custom_forward(resnet),
                         hidden_states,
                         temb,
                         **ckpt_kwargs,
                     )
                     hidden_states = attn(
```

### Comparing `onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py` & `onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 from packaging import version
 import importlib.metadata
 import oneflow as torch
-from onediff.infer_compiler.transform import transform_mgr
+from onediff.infer_compiler.backends.oneflow.transform import transform_mgr
 
 diffusers_0210_v = version.parse("0.21.0")
 diffusers_version = version.parse(importlib.metadata.version("diffusers"))
 
 transformed_diffusers = transform_mgr.transform_package("diffusers")
 UNet2DConditionOutput = (
     transformed_diffusers.models.unet_2d_condition.UNet2DConditionOutput
```

### Comparing `onediff-1.1.0.dev202405210127/src/infer_compiler_registry/register_onediff_quant/__init__.py` & `onediff-1.1.0.dev202405220128/src/infer_compiler_registry/register_onediff_quant/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from onediff.infer_compiler.transform import register
+from onediff.infer_compiler.backends.oneflow.transform import register
 
 import oneflow as flow
 import onediff_quant
 
 torch2oflow_class_map = {
     onediff_quant.FakeQuantModule: onediff_quant.OneFlowFakeQuantModule,
     onediff_quant.StaticQuantConvModule: onediff_quant.OneFlowStaticQuantConvModule,
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/backends/oneflow.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/oneflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import torch
-from .registry import register_backend
+
+from ..registry import register_backend
 
 
 @register_backend("oneflow")
 def compile(torch_module: torch.nn.Module, *, options=None):
     """
     Transform a torch nn.Module to oneflow.nn.Module, then optimize it with oneflow.nn.Graph.
     Args:
@@ -15,25 +16,26 @@
                      default True.
         - 'use_graph' whether to optimize with oneflow.nn.Graph, default True.
         - 'debug' which config the nn.Graph debug level, default -1(no debug info), max 3(max debug info).
         - 'size' which config the cache size when cache is enabled. Note that after onediff v0.12, cache is default disabled.
         - 'graph_file' (None) generates a compilation cache file. If the file exists, loading occurs; if not, the compilation result is saved after the first run.
         - 'graph_file_device' (None) sets the device for the graph file, default None.  If set, the compilation result will be converted to the specified device.
     """
-    from ..oneflow.deployable_module import OneflowDeployableModule
-    from ..oneflow.utils import get_mixed_deployable_module
-    from ..transform.custom_transform import set_default_registry
-    from ..utils import CompileOptions, set_oneflow_env_vars
-    from ..utils.param_utils import (
+    from .deployable_module import OneflowDeployableModule, get_mixed_deployable_module
+    from .env_var import set_oneflow_default_env_vars, set_oneflow_env_vars
+    from ..options import CompileOptions
+    from .param_utils import (
         state_update_hook,
         init_state_update_attr,
         forward_pre_check_and_update_state_hook,
         forward_generate_constant_folding_info_hook,
     )
+    from .transform.custom_transform import set_default_registry
 
+    set_oneflow_default_env_vars()
     set_default_registry()
 
     options = options if options is not None else CompileOptions()
     set_oneflow_env_vars(options.oneflow)
 
     def wrap_module(module):
         if isinstance(module, OneflowDeployableModule):
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/core/with_onediff_compile.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/compiler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import torch
+
 from .deployable_module import DeployableModule
 
 _DEFAULT_BACKEND = "oneflow"
 
+
 def compile(
     torch_module: torch.nn.Module, *, backend=_DEFAULT_BACKEND, options=None
 ) -> DeployableModule:
-    from ..backends.registry import lookup_backend
+    from .registry import lookup_backend
 
     backend = lookup_backend(backend)
     model = backend(torch_module, options=options)
     return model
 
 
 def oneflow_compile(torch_module: torch.nn.Module, *, options=None) -> DeployableModule:
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import importlib
 import inspect
 import os
 import torch
 from oneflow.mock_torch import enable
 from oneflow.mock_torch.mock_importer import _importer
 from .import_module_utils import import_module_from_path
-from ..utils.log_utils import logger
-from ..utils.patch_for_compiler import *
+from onediff.utils import logger
+from .patch_for_compiler import *
 
 __all__ = ["DynamicMockModule"]
 
 
 def _get_module(full_name: str):
     try:
         attrs = full_name.split(".")
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/import_tools/format_utils.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/import_tools/import_module_utils.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/import_tools/importer.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Optional, Union
 from functools import lru_cache
 from types import FunctionType, ModuleType
 from pathlib import Path
 from importlib.metadata import requires
 from .format_utils import MockEntityNameFormatter
 from .dyn_mock_mod import DynamicMockModule
-from ..utils.log_utils import logger
+from onediff.utils import logger
 
 __all__ = ["LazyMocker", "is_need_mock"]
 
 # Cache all imported modules (maxsize=None: no limit)
 @lru_cache(maxsize=None)
 def has_torch_dependency(main_pkg: str):
     try:
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/nexfort/deployable_module.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/nexfort/deployable_module.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import torch
-from ..core.deployable_module import DeployableModule
+
+from ..deployable_module import DeployableModule
 
 
 class NexfortDeployableModule(DeployableModule):
-    def __init__(self, torch_module):
+    def __init__(self, compiled_module, torch_module):
         torch.nn.Module.__init__(self)
-        object.__setattr__(self, "_deployable_module_model", torch_module)
-        object.__setattr__(self, "_modules", torch_module._modules)
+        object.__setattr__(self, "_deployable_module_model", compiled_module)
+        object.__setattr__(self, "_modules", compiled_module._modules)
         object.__setattr__(self, "_torch_module", torch_module)
 
     def __call__(self, *args, **kwargs):
         return self._deployable_module_model(*args, **kwargs)
 
     def __getattr__(self, name):
         return getattr(self._deployable_module_model, name)
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/oneflow/config.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/env_var.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,104 @@
+import dataclasses
 import os
+import torch
 from typing import Optional
-import dataclasses
-from ..utils import (
-    parse_boolean_from_env,
-    set_boolean_env_var,
-    parse_integer_from_env,
-    set_integer_env_var,
-)
+
+from onediff.utils import set_boolean_env_var, set_integer_env_var
+
+
+@dataclasses.dataclass
+class OneflowCompileOptions:
+    use_graph: bool = True
+    debug_level: int = -1
+    max_cached_graph_size: int = 9
+    graph_file: str = None
+    graph_file_device: torch.device = None
+
+    # Optimization related environment variables
+    run_graph_by_vm: bool = None
+    graph_delay_variable_op_execution: bool = None
+
+    conv_allow_half_precision_accumulation: bool = None
+    matmul_allow_half_precision_accumulation: bool = None
+    attention_allow_half_precision_accumulation: bool = None
+    attention_allow_half_precision_score_accumulation_max_m: int = None
+    attention_allow_quantization: bool = None
+
+    mlir_cse: bool = None
+    mlir_enable_inference_optimization: bool = None
+    mlir_enable_round_trip: bool = None
+    mlir_fuse_forward_ops: bool = None
+    mlir_fuse_ops_with_backward_impl: bool = None
+    mlir_group_matmul: bool = None
+    mlir_prefer_nhwc: bool = None
+    mlir_fuse_kernel_launch: bool = None
+
+    kernel_enable_cuda_graph: bool = None
+    kernel_enable_fused_conv_bias: bool = None
+    kernel_enable_fused_linear: bool = None
+    kernel_conv_cutlass_impl_enable_tuning_warmup: bool = None
+    kernel_enable_conv2d_tuning_warmup: bool = None
+    kernel_gemm_cutlass_impl_enable_tuning_warmup: bool = None
+    kernel_conv_enable_cutlass_impl: bool = None
+    kernel_gemm_enable_cutlass_impl: bool = None
+    kernel_glu_enable_dual_gemm_impl: bool = None
+    kernel_glu_enable_y_gemm_impl: bool = None
+    kernel_glu_quant_enable_dual_gemm_impl: bool = None
+
+
+def _set_env_vars(field2env_var, options):
+    for field in dataclasses.fields(options):
+        field_name = field.name
+        field_value = getattr(options, field_name)
+        if field_value is None or field_name not in field2env_var:
+            continue
+        env_var = field2env_var[field_name]
+        set_env_var = None
+        if field.type in (bool, Optional[bool]):
+            set_env_var = set_boolean_env_var
+        elif field.type in (int, Optional[int]):
+            set_env_var = set_integer_env_var
+        else:
+            raise ValueError(f"Unsupported type {field.type}")
+        set_env_var(env_var, field_value)
+
+
+def set_oneflow_env_vars(options):
+    field2env_var = {
+        "run_graph_by_vm": "ONEFLOW_RUN_GRAPH_BY_VM",
+        "graph_delay_variable_op_execution": "ONEFLOW_GRAPH_DELAY_VARIABLE_OP_EXECUTION",
+        "mlir_cse": "ONEFLOW_MLIR_CSE",
+        "mlir_enable_inference_optimization": "ONEFLOW_MLIR_ENABLE_INFERENCE_OPTIMIZATION",
+        "mlir_enable_round_trip": "ONEFLOW_MLIR_ENABLE_ROUND_TRIP",
+        "mlir_fuse_forward_ops": "ONEFLOW_MLIR_FUSE_FORWARD_OPS",
+        "mlir_fuse_ops_with_backward_impl": "ONEFLOW_MLIR_FUSE_OPS_WITH_BACKWARD_IMPL",
+        "mlir_group_matmul": "ONEFLOW_MLIR_GROUP_MATMUL",
+        "mlir_prefer_nhwc": "ONEFLOW_MLIR_PREFER_NHWC",
+        "mlir_fuse_kernel_launch": "ONEFLOW_MLIR_FUSE_KERNEL_LAUNCH",
+        "kernel_enable_cuda_graph": "ONEFLOW_KERNEL_ENABLE_CUDA_GRAPH",
+        "kernel_enable_fused_conv_bias": "ONEFLOW_KERNEL_ENABLE_FUSED_CONV_BIAS",
+        "kernel_enable_fused_linear": "ONEFLOW_KERNEL_ENABLE_FUSED_LINEAR",
+        "kernel_conv_cutlass_impl_enable_tuning_warmup": "ONEFLOW_KERNEL_CONV_CUTLASS_IMPL_ENABLE_TUNING_WARMUP",
+        "kernel_gemm_cutlass_impl_enable_tuning_warmup": "ONEFLOW_KERNEL_GEMM_CUTLASS_IMPL_ENABLE_TUNING_WARMUP",
+        "kernel_conv_enable_cutlass_impl": "ONEFLOW_KERNEL_CONV_ENABLE_CUTLASS_IMPL",
+        "kernel_enable_conv2d_tuning_warmup": "ONEFLOW_CONV2D_KERNEL_ENABLE_TUNING_WARMUP",
+        "kernel_gemm_enable_cutlass_impl": "ONEFLOW_KERNEL_GEMM_ENABLE_CUTLASS_IMPL",
+        "kernel_glu_enable_dual_gemm_impl": "ONEFLOW_KERNEL_GLU_ENABLE_DUAL_GEMM_IMPL",
+        "kernel_glu_enable_y_gemm_impl": "ONEFLOW_KERNEL_GLU_ENABLE_Y_GEMM_IMPL",
+        "kernel_glu_quant_enable_dual_gemm_impl": "ONEFLOW_KERNEL_GLU_QUANT_ENABLE_DUAL_GEMM_IMPL",
+        "conv_allow_half_precision_accumulation": "ONEFLOW_CONV_ALLOW_HALF_PRECISION_ACCUMULATION",
+        "matmul_allow_half_precision_accumulation": "ONEFLOW_MATMUL_ALLOW_HALF_PRECISION_ACCUMULATION",
+        "attention_allow_half_precision_accumulation": "ONEFLOW_ATTENTION_ALLOW_HALF_PRECISION_ACCUMULATION",
+        "attention_allow_half_precision_score_accumulation_max_m": "ONEFLOW_ATTENTION_ALLOW_HALF_PRECISION_SCORE_ACCUMULATION_MAX_M",
+    }
+    _set_env_vars(field2env_var, options)
 
 
-def init_default_env():
+def set_oneflow_default_env_vars():
     # ONEFLOW_RUN_GRAPH_BY_VM must set here to enable nn.Graph init with vm run
     os.environ.setdefault("ONEFLOW_RUN_GRAPH_BY_VM", "1")
     os.environ.setdefault("ONEFLOW_GRAPH_DELAY_VARIABLE_OP_EXECUTION", "1")
 
     os.environ.setdefault("ONEFLOW_MLIR_CSE", "1")
     os.environ.setdefault("ONEFLOW_MLIR_ENABLE_INFERENCE_OPTIMIZATION", "1")
     os.environ.setdefault("ONEFLOW_MLIR_ENABLE_ROUND_TRIP", "1")
@@ -38,111 +123,11 @@
     os.environ.setdefault("ONEFLOW_LINEAR_EMBEDDING_SKIP_INIT", "1")
     # os.environ.setdefault("ONEFLOW_ATTENTION_ALLOW_HALF_PRECISION_ACCUMULATION", "1")
     # os.environ.setdefault("ONEFLOW_ATTENTION_ALLOW_HALF_PRECISION_SCORE_ACCUMULATION_MAX_M", "-1")
     # os.environ.setdefault("ONEFLOW_ATTENTION_ALLOW_QUANTIZATION", "1")
 
     os.environ.setdefault("ONEFLOW_MLIR_GROUP_MATMUL_QUANT", "1")
     os.environ.setdefault("ONEFLOW_CONV2D_KERNEL_ENABLE_TUNING_WARMUP", "1")
+
     # TODO: enable this will cause the failure of multi resolution warmup
     # os.environ.setdefault("ONEFLOW_MLIR_FUSE_KERNEL_LAUNCH", "1")
     # os.environ.setdefault("ONEFLOW_KERNEL_ENABLE_CUDA_GRAPH", "1")
-
-
-@dataclasses.dataclass
-class OneFlowCompilerConfig:
-    run_graph_by_vm: Optional[bool] = None
-    graph_delay_variable_op_execution: Optional[bool] = None
-
-    mlir_cse: Optional[bool] = None
-    mlir_enable_inference_optimization: Optional[bool] = None
-    mlir_enable_round_trip: Optional[bool] = None
-    mlir_fuse_forward_ops: Optional[bool] = None
-    mlir_fuse_ops_with_backward_impl: Optional[bool] = None
-    mlir_group_matmul: Optional[bool] = None
-    mlir_prefer_nhwc: Optional[bool] = None
-    mlir_fuse_kernel_launch: Optional[bool] = None
-
-    kernel_enable_cuda_graph: Optional[bool] = None
-    kernel_enable_fused_conv_bias: Optional[bool] = None
-    kernel_enable_fused_linear: Optional[bool] = None
-    kernel_conv_cutlass_impl_enable_tuning_warmup: Optional[bool] = None
-    kernel_gemm_cutlass_impl_enable_tuning_warmup: Optional[bool] = None
-    kernel_conv_enable_cutlass_impl: Optional[bool] = None
-    kernel_gemm_enable_cutlass_impl: Optional[bool] = None
-    kernel_glu_enable_dual_gemm_impl: Optional[bool] = None
-    kernel_glu_enable_y_gemm_impl: Optional[bool] = None
-    kernel_glu_quant_enable_dual_gemm_impl: Optional[bool] = None
-
-    conv_allow_half_precision_accumulation: Optional[bool] = None
-    matmul_allow_half_precision_accumulation: Optional[bool] = None
-    linear_embedding_skip_init: Optional[bool] = None
-    attention_allow_half_precision_accumulation: Optional[bool] = None
-    attention_allow_half_precision_score_accumulation_max_m: Optional[int] = None
-    attention_allow_quantization: Optional[bool] = None
-    conv2d_kernel_enable_tuning_warmup: Optional[bool] = None
-
-    attr2env_var = {
-        "run_graph_by_vm": "ONEFLOW_RUN_GRAPH_BY_VM",
-        "graph_delay_variable_op_execution": "ONEFLOW_GRAPH_DELAY_VARIABLE_OP_EXECUTION",
-        "mlir_cse": "ONEFLOW_MLIR_CSE",
-        "mlir_enable_inference_optimization": "ONEFLOW_MLIR_ENABLE_INFERENCE_OPTIMIZATION",
-        "mlir_enable_round_trip": "ONEFLOW_MLIR_ENABLE_ROUND_TRIP",
-        "mlir_fuse_forward_ops": "ONEFLOW_MLIR_FUSE_FORWARD_OPS",
-        "mlir_fuse_ops_with_backward_impl": "ONEFLOW_MLIR_FUSE_OPS_WITH_BACKWARD_IMPL",
-        "mlir_group_matmul": "ONEFLOW_MLIR_GROUP_MATMUL",
-        "mlir_prefer_nhwc": "ONEFLOW_MLIR_PREFER_NHWC",
-        "mlir_fuse_kernel_launch": "ONEFLOW_MLIR_FUSE_KERNEL_LAUNCH",
-        "kernel_enable_cuda_graph": "ONEFLOW_KERNEL_ENABLE_CUDA_GRAPH",
-        "kernel_enable_fused_conv_bias": "ONEFLOW_KERNEL_ENABLE_FUSED_CONV_BIAS",
-        "kernel_enable_fused_linear": "ONEFLOW_KERNEL_ENABLE_FUSED_LINEAR",
-        "kernel_conv_cutlass_impl_enable_tuning_warmup": "ONEFLOW_KERNEL_CONV_CUTLASS_IMPL_ENABLE_TUNING_WARMUP",
-        "kernel_gemm_cutlass_impl_enable_tuning_warmup": "ONEFLOW_KERNEL_GEMM_CUTLASS_IMPL_ENABLE_TUNING_WARMUP",
-        "kernel_conv_enable_cutlass_impl": "ONEFLOW_KERNEL_CONV_ENABLE_CUTLASS_IMPL",
-        "kernel_gemm_enable_cutlass_impl": "ONEFLOW_KERNEL_GEMM_ENABLE_CUTLASS_IMPL",
-        "kernel_glu_enable_dual_gemm_impl": "ONEFLOW_KERNEL_GLU_ENABLE_DUAL_GEMM_IMPL",
-        "kernel_glu_enable_y_gemm_impl": "ONEFLOW_KERNEL_GLU_ENABLE_Y_GEMM_IMPL",
-        "kernel_glu_quant_enable_dual_gemm_impl": "ONEFLOW_KERNEL_GLU_QUANT_ENABLE_DUAL_GEMM_IMPL",
-        "conv_allow_half_precision_accumulation": "ONEFLOW_CONV_ALLOW_HALF_PRECISION_ACCUMULATION",
-        "matmul_allow_half_precision_accumulation": "ONEFLOW_MATMUL_ALLOW_HALF_PRECISION_ACCUMULATION",
-        "linear_embedding_skip_init": "ONEFLOW_LINEAR_EMBEDDING_SKIP_INIT",
-        "attention_allow_half_precision_accumulation": "ONEFLOW_ATTENTION_ALLOW_HALF_PRECISION_ACCUMULATION",
-        "attention_allow_half_precision_score_accumulation_max_m": "ONEFLOW_ATTENTION_ALLOW_HALF_PRECISION_SCORE_ACCUMULATION_MAX_M",
-        "conv2d_kernel_enable_tuning_warmup":'ONEFLOW_CONV2D_KERNEL_ENABLE_TUNING_WARMUP',
-    }
-
-    def __post_init__(self):
-        fields = dataclasses.fields(self)
-        fields = {field.name: field for field in fields}
-        for name in self.attr2env_var:
-            if fields[name].type in (bool, Optional[bool]):
-                super().__setattr__(
-                    name, parse_boolean_from_env(self.attr2env_var[name])
-                )
-            elif fields[name].type in (int, Optional[int]):
-                super().__setattr__(
-                    name, parse_integer_from_env(self.attr2env_var[name])
-                )
-            else:
-                raise ValueError(
-                    f"Unsupported type {dataclasses.fields(self)[name].type}"
-                )
-
-        super().__setattr__("_initialized", True)
-
-    def __setattr__(self, name, value):
-        super().__setattr__(name, value)
-        if getattr(self, "_initialized", False) and name in self.attr2env_var:
-            fields = dataclasses.fields(self)
-            fields = dataclasses.fields(self)
-            fields = {field.name: field for field in fields}
-            if fields[name].type in (bool, Optional[bool]):
-                set_boolean_env_var(self.attr2env_var[name], value)
-            elif fields[name].type in (int, Optional[int]):
-                set_integer_env_var(self.attr2env_var[name], value)
-            else:
-                raise ValueError(
-                    f"Unsupported type {dataclasses.fields(self)[name].type}"
-                )
-
-
-init_default_env()
-oneflow_compiler_config = OneFlowCompilerConfig()
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/oneflow/deployable_module.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/deployable_module.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,59 @@
 import types
 import torch
+from functools import wraps
+
 import oneflow as flow
 
-from ..core.deployable_module import DeployableModule
-from ..transform.manager import transform_mgr
-from ..utils.oneflow_exec_mode import oneflow_exec_mode, oneflow_exec_mode_enabled
-from ..utils.args_tree_util import input_output_processor
-from ..utils.log_utils import logger
-from ..utils.param_utils import parse_device, check_device, generate_constant_folding_info
-from ..utils.graph_management_utils import graph_file_management
-from ..utils.online_quantization_utils import quantize_and_deploy_wrapper
-from ..utils.options import OneflowCompileOptions
+from onediff.utils import logger
+
+from ..deployable_module import DeployableModule
+
+from .transform.manager import transform_mgr
+from .transform.builtin_transform import torch2oflow
+
+from .dual_module import DualModule, get_mixed_dual_module
+from .oneflow_exec_mode import oneflow_exec_mode, oneflow_exec_mode_enabled
+from .args_tree_util import input_output_processor
+from .param_utils import parse_device, check_device, generate_constant_folding_info
+from .graph_management_utils import graph_file_management
+from .online_quantization_utils import quantize_and_deploy_wrapper
+from .env_var import OneflowCompileOptions
 
-from .utils import handle_deployable_exception, get_mixed_dual_module, get_oneflow_graph
+
+@torch2oflow.register
+def _(mod: DualModule, verbose=False):
+    return torch2oflow(mod._torch_module, verbose)
+
+
+def handle_deployable_exception(func):
+    @wraps(func)
+    def wrapper(self, *args, **kwargs):
+        if transform_mgr.debug_mode:
+            return func(self, *args, **kwargs)
+        else:
+            try:
+                return func(self, *args, **kwargs)
+            except Exception as e:
+                logger.error(f"Exception in {func.__name__}: {e=}")
+                logger.warning("Recompile oneflow module ...")
+                del self._deployable_module_model.oneflow_module
+                self._deployable_module_dpl_graph = None
+                return func(self, *args, **kwargs)
+
+    return wrapper
+
+
+def get_oneflow_graph(model, size=9, dynamic_graph=True):
+    from .graph import OneflowGraph
+
+    g = OneflowGraph(model)
+    g._dynamic_input_graph_cache.set_cache_size(size)
+    g._dynamic_input_graph_cache.enable_shared(dynamic_graph)
+    return g
 
 
 class OneflowDeployableModule(DeployableModule):
     def __init__(
         self, torch_module, oneflow_module, dynamic=True, options=None,
     ):
         torch.nn.Module.__init__(self)
@@ -195,7 +232,33 @@
             ...     linear_mae_threshold=0.005,
             ...     conv_compute_density_threshold=300,
             ...     linear_compute_density_threshold=100,
             ...     cache_dir=args.cache_dir)
             >>> model.apply_online_quant(quant_config)
         """
         self._deployable_module_quant_config = quant_config
+
+
+def get_mixed_deployable_module(module_cls):
+    class MixedOneflowDeployableModule(OneflowDeployableModule, module_cls):
+        def __init__(self, torch_module, oneflow_module, dynamic=True, options=None):
+            OneflowDeployableModule.__init__(
+                self, torch_module, oneflow_module, dynamic, options
+            )
+            self._is_raw_deployable_module = False
+
+        @classmethod
+        def from_existing(cls, existing_module, dynamic=True, options=None):
+            torch_module = existing_module._deployable_module_model._torch_module
+            oneflow_module = existing_module._deployable_module_model._oneflow_module
+            instance = cls(torch_module, oneflow_module, dynamic, options)
+            instance._deployable_module_dpl_graph = None
+            if hasattr(existing_module, "_deployable_module_dpl_graph"):
+                instance._deployable_module_dpl_graph = (
+                    existing_module._deployable_module_dpl_graph
+                )
+            return instance
+
+        def _get_name(self):
+            return f"{self.__class__.__name__}(of {module_cls.__name__})"
+
+    return MixedOneflowDeployableModule
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/oneflow/dual_module.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/dual_module.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import Any
 from itertools import chain
 
 import torch
 import oneflow as flow
 from oneflow.utils.tensor import to_torch
 
-from ..transform.builtin_transform import torch2oflow
-from ..utils.oneflow_exec_mode import oneflow_exec_mode, oneflow_exec_mode_enabled
-from ..utils.log_utils import logger
+from onediff.utils import logger
+from .transform.builtin_transform import torch2oflow
+from .oneflow_exec_mode import oneflow_exec_mode, oneflow_exec_mode_enabled
 
 
 class DualModule(torch.nn.Module):
     def __init__(self, torch_module, oneflow_module):
         torch.nn.Module.__init__(self)
         object.__setattr__(self, "_torch_module", torch_module)
         object.__setattr__(self, "_oneflow_module", oneflow_module)
@@ -87,16 +87,14 @@
 
         if isinstance(torch_attr, torch.nn.ModuleList):
             if oneflow_attr is None:
                 oneflow_attr = flow.nn.ModuleList([None] * len(torch_attr))
             return DualModuleList(torch_attr, oneflow_attr)
 
         elif isinstance(torch_attr, torch.nn.Module):
-            from .utils import get_mixed_dual_module
-
             return get_mixed_dual_module(torch_attr.__class__)(torch_attr, oneflow_attr)
         else:
             return oneflow_attr if oneflow_exec_mode_enabled() else torch_attr
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name in ["_torch_module", "_oneflow_module"]:
             super().__setattr__(name, value)
@@ -116,15 +114,14 @@
 
 class DualModuleList(torch.nn.ModuleList):
     def __init__(self, torch_modules, oneflow_modules):
         super().__init__()
         assert len(torch_modules) == len(oneflow_modules)
         self._torch_modules = torch_modules
         self._oneflow_modules = oneflow_modules
-        from .utils import get_mixed_dual_module
 
         dual_modules = []
         for torch_module, oneflow_module in zip(
             self._torch_modules, self._oneflow_modules
         ):
             dual_modules.append(
                 get_mixed_dual_module(torch_module.__class__)(
@@ -148,7 +145,23 @@
             setattr(self._torch_modules, key, value._torch_module)
             setattr(self._oneflow_modules, key, value._oneflow_module)
         else:
             setattr(self._torch_modules, key, value)
             value = torch2oflow(value)
             setattr(self._oneflow_modules, key, value)
         return object.__setattr__(self, key, value)
+
+
+def get_mixed_dual_module(module_cls):
+    if issubclass(module_cls, DualModule) and "MixedDualModule" in module_cls.__name__:
+        return module_cls
+
+    class MixedDualModule(DualModule, module_cls):
+        def __init__(self, torch_module, oneflow_module):
+            while isinstance(torch_module, DualModule):
+                torch_module = torch_module._torch_module
+            DualModule.__init__(self, torch_module, oneflow_module)
+
+        def _get_name(self) -> str:
+            return f"{self.__class__.__name__}(of {module_cls.__name__})"
+
+    return MixedDualModule
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/oneflow/graph.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import oneflow as flow
 
-from ..transform.manager import transform_mgr
-from ..transform.builtin_transform import reverse_proxy_class
-from ..utils.log_utils import logger
-from ..utils.cost_util import cost_cnt
+from onediff.utils import logger
+from .transform.manager import transform_mgr
+from .transform.builtin_transform import reverse_proxy_class
+from .utils.cost_util import cost_cnt
 
 
 class OneflowGraph(flow.nn.Graph):
     @flow.nn.Graph.with_dynamic_input_shape()
     def __init__(self, model):
         super().__init__(enable_get_runtime_state_dict=True)
         self.model = model
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/transform/builtin_transform.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 from collections import OrderedDict
 from collections.abc import Iterable
 from typing import Union, Any
 import torch
 import oneflow as flow
 
 from .manager import transform_mgr
-from ..utils.log_utils import logger
-from ..utils.patch_for_diffusers import diffusers_checker
+from onediff.utils import logger
+from .patch_for_diffusers import diffusers_checker
 from ..import_tools.importer import is_need_mock
 
 from .patch_for_comfy import PatchForComfy
+
 __all__ = [
     "proxy_class",
     "ProxySubmodule",
     "map_args",
     "get_attr",
     "torch2oflow",
     "default_converter",
 ]
 
+
 def singledispatch_proxy(func):
     dispatcher = singledispatch(func)
     _warning_set = set()
 
     def wrapper(first_param, *args, **kwargs):
         nonlocal _warning_set
 
@@ -53,18 +55,20 @@
     wrapper.dispatch = dispatcher.dispatch
     return wrapper
 
 
 def proxy_class(cls: type):
     try:
         out = transform_mgr.transform_cls(cls)
-        return out 
+        return out
     except Exception as e:
         # If an exception occurs during transformation, print traceback for debugging
-        raise RuntimeError(f"An exception occurred during class transformation:\n{traceback.format_exc()}\nException: {e}")
+        raise RuntimeError(
+            f"An exception occurred during class transformation:\n{traceback.format_exc()}\nException: {e}"
+        )
 
 
 def reverse_proxy_class(cls: type):
     return transform_mgr.reverse_transform_cls(cls)
 
 
 class ProxySubmodule:
@@ -443,15 +447,15 @@
                 logger.warning(
                     f"warning when get {mod.__name__} in torch.nn.functional: {e}"
                 )
                 mod_name = mod.__module__.replace("torch", "oneflow")
         if mod_name is not None:
             m = importlib.import_module(mod_name)
             return getattr(m, mod.__name__)
-    
+
     return default_converter(mod, verbose)
 
 
 @torch2oflow.register
 def _(mod: torch.device, verbose=False):
     index = mod.index if mod.index is not None else 0
     return flow.device(mod.type, index)
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/transform/custom_transform.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import inspect
 import importlib.util
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Union
 from ..import_tools import import_module_from_path
 from .manager import transform_mgr
 from .builtin_transform import torch2oflow
-from ..utils.log_utils import logger
+from onediff.utils import logger
 
 __all__ = ["register"]
 
 
 def register_torch2oflow_class(cls: type, replacement: type, verbose=True):
     try:
         key = transform_mgr.get_transformed_entity_name(cls)
@@ -45,15 +45,15 @@
             return
         try:
             import_module_from_path(module_path)
         except Exception as e:
             logger.warning(f"Failed to import {module_name} from {module_path}. {e=}")
 
     # compiler_registry_path
-    registry_path = Path(__file__).parents[3] / "infer_compiler_registry"
+    registry_path = Path(__file__).parents[5] / "infer_compiler_registry"
 
     if importlib.util.find_spec("diffusers") is not None:
         import_module_safely(registry_path / "register_diffusers", "register_diffusers")
 
     if importlib.util.find_spec("onediff_quant") is not None:
         import_module_safely(
             registry_path / "register_onediff_quant", "register_onediff_quant"
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/transform/manager.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/transform/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import importlib
 import os
 import types
 import warnings
 import logging
 from typing import Dict, List, Union
 from pathlib import Path
-from ..utils.log_utils import logger
+from onediff.utils import logger
 from ..import_tools.importer import LazyMocker
 
 __all__ = ["transform_mgr"]
 
 
 class TransformManager:
     """TransformManager
@@ -113,18 +113,17 @@
 if not transform_mgr.debug_mode:
     warnings.simplefilter("ignore", category=UserWarning)
     warnings.simplefilter("ignore", category=FutureWarning)
 
 
 if importlib.util.find_spec("pydantic") is not None:
     import pydantic
+
     if pydantic.VERSION < "2.5.2":
         logger.warning(
             f"Pydantic version {pydantic.VERSION} is too low, please upgrade to 2.5.2 or higher."
         )
         from oneflow.mock_torch.mock_utils import MockEnableDisableMixin
 
         MockEnableDisableMixin.hazard_list.append(
             "huggingface_hub.inference._text_generation"
         )
-
-
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/transform/patch_for_comfy.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/args_tree_util.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import oneflow as flow
 from oneflow.framework.args_tree import ArgsTree
-from .log_utils import logger
+from onediff.utils import logger
 
 
 def input_output_processor(func):
     def process_input(*args, **kwargs):
         def input_fn(value):
             if isinstance(value, torch.Tensor):
                 # TODO: https://github.com/siliconflow/sd-team/issues/109
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/cost_util.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import wraps
 import oneflow as flow
 import time
 import inspect
-from .log_utils import logger
+from onediff.utils import logger
 
 __all__ = ["cost_cnt", "cost_time"]
 
 
 class cost_cnt:
     def __init__(self, debug=False, message="\t"):
         self.debug = debug
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/graph_management_utils.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/graph_management_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import os
 from typing import Dict
 import torch
 import oneflow as flow
 from pathlib import Path
 from functools import wraps
 from oneflow.framework.args_tree import ArgsTree
-from ..transform.builtin_transform import torch2oflow
-from ..transform.manager import transform_mgr
-from .log_utils import logger
-from .cost_util import cost_time
-from .options import OneflowCompileOptions
+from .transform.builtin_transform import torch2oflow
+from .transform.manager import transform_mgr
+from .utils.cost_util import cost_time
+from .env_var import OneflowCompileOptions
+from onediff.utils import logger
 
 
 def calculate_model_hash(model):
     return hashlib.sha256(f"{model}".encode("utf-8")).hexdigest()
 
 
 @cost_time(debug=transform_mgr.debug_mode, message="generate graph file name")
@@ -53,17 +53,20 @@
             graph_file = generate_graph_file_name(
                 graph_file, self, args=args, kwargs=kwargs
             )
             setattr(self, "_load_graph_first_run", False)
             # Avoid graph file conflicts
             if importlib.util.find_spec("register_comfy"):
                 from register_comfy import CrossAttntionStateDictPatch as state_patch
+
                 attn2_patch_sum = state_patch.attn2_patch_sum(input_kwargs=kwargs)
                 if attn2_patch_sum > 0:
-                    graph_file = graph_file.replace(".graph", f"_attn2_{attn2_patch_sum}.graph")
+                    graph_file = graph_file.replace(
+                        ".graph", f"_attn2_{attn2_patch_sum}.graph"
+                    )
 
         def process_state_dict_before_saving(state_dict: Dict):
             nonlocal self, args, kwargs, graph_file
             graph = self.get_graph()
             if importlib.util.find_spec("register_comfy"):
                 from register_comfy import CrossAttntionStateDictPatch as state_patch
 
@@ -94,15 +97,15 @@
             nonlocal graph_file, compile_options, is_first_load
             if not is_first_load:
                 return
             try:
                 parent_dir = os.path.dirname(graph_file)
                 if parent_dir != "":
                     os.makedirs(parent_dir, exist_ok=True)
-                
+
                 # Avoid graph file conflicts
                 if os.path.exists(graph_file):
                     raise FileExistsError(f"File {graph_file} exists!")
 
                 self.save_graph(
                     graph_file, process_state_dict=process_state_dict_before_saving
                 )
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/log_utils.py` & `onediff-1.1.0.dev202405220128/src/onediff/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/model_inplace_assign.py` & `onediff-1.1.0.dev202405220128/src/onediff/torch_utils/model_inplace_assign.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 _nested_counter = defaultdict(lambda: 0)
 
 
 class TensorInplaceAssign:
     r"""
     This class is used as a context manager, instantiated with either a `torch.nn.Module` or
-    `onediff.infer_compiler.deployable_module.DeployableModule` during initialization.
+    `onediff.infer_compiler.backends.deployable_module.DeployableModule` during initialization.
     Within the context manager, all Tensors associated with the provided module will be
     transformed into AutoInplaceCopyTensor. After transformed, assignments to Tensor.data are
     modified to in-place copying.
 
     The class is commonly used to ensure the stability of the data_ptr() for weights,
     particularly in scenarios involving the loading of LoRA weights.
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/module_operations.py` & `onediff-1.1.0.dev202405220128/src/onediff/torch_utils/module_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         sub_module_name (str): Dot-separated name of the submodule.
 
     Returns:
         nn.Module: The requested submodule.
     """
     if sub_module_name == "":
         return module
-    
+
     parts = sub_module_name.split(".")
     current_module = module
 
     for part in parts:
         try:
             if part.isdigit():
                 current_module = current_module[int(part)]
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/online_quantization_utils.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 def patch_input_adapter(in_args, in_kwargs):
     return in_args, in_kwargs
 
+
 def online_quantize_model(
-    model, input_args, input_kwargs,
-    seed=1, inplace=True,
+    model,
+    input_args,
+    input_kwargs,
+    seed=1,
+    inplace=True,
     module_selector=lambda x: x,
-    quant_config = None,
+    quant_config=None,
     calibration_info=None,
 ):
     """Optimize the quantization pipeline.
 
     Returns:
         tuple: A tuple containing the quantized model and the quantization
         status.
     """
 
     from onediff_quant.quantization import (
         OnlineQuantModule,
         create_quantization_calculator,
     )
+
     if getattr(quant_config, "quantization_calculator", None):
         calculator = quant_config.quantization_calculator
     else:
         calculator = create_quantization_calculator(
-            model, quant_config, module_selector, seed,
+            model,
+            quant_config,
+            module_selector,
+            seed,
             calibration_info=calibration_info,
         )
     module = OnlineQuantModule(calculator, False, inplace=inplace)
-    in_args , in_kwargs = patch_input_adapter(input_args, input_kwargs)
-    quantized_model,  info = module.quantize_with_calibration(
-        *in_args, **in_kwargs
-    )
+    in_args, in_kwargs = patch_input_adapter(input_args, input_kwargs)
+    quantized_model, info = module.quantize_with_calibration(*in_args, **in_kwargs)
     status = module.collect_quantization_status(model, info)
 
     return quantized_model, status
 
 
 def quantize_and_deploy_wrapper(func):
     def wrapper(self: "DeployableModule", *args, **kwargs):
         torch_model = self._torch_module
         quant_config = self._deployable_module_quant_config
         if quant_config:
             torch_model, _ = online_quantize_model(
-                torch_model, args, kwargs,
+                torch_model,
+                args,
+                kwargs,
                 module_selector=lambda x: x,
                 quant_config=quant_config,
                 inplace=True,
             )
-            self._deployable_module_quant_config = None 
+            self._deployable_module_quant_config = None
         output = func(self, *args, **kwargs)
         return output
-    return wrapper
 
-       
+    return wrapper
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/param_utils.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/param_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import torch
 import oneflow as flow
 from typing import List, Dict, Any, Union
 
-from .log_utils import logger
+from onediff.utils import logger
 
 
 def parse_device(args: List[Any], kwargs: Dict[str, Any]):
     if "device" in kwargs:
         return kwargs["device"]
     for x in args:
         if isinstance(x, (flow.device, torch.device)):
@@ -76,16 +76,16 @@
         )
         object.__setattr__(submodule, GRAPH_RELATED_TENSOR_ATTR, weight_tensor)
 
 
 def generate_constant_folding_info(
     deployable_module, torch_module: torch.nn.Module = None
 ) -> Dict[str, flow.Tensor]:
-    removeprefix = lambda ss, prefix: ss[len(prefix):] if ss.startswith(prefix) else ss
-    
+    removeprefix = lambda ss, prefix: ss[len(prefix) :] if ss.startswith(prefix) else ss
+
     # convert str like 'variable_transpose_model.input_blocks.10.0.in_layers.2.weight_239'
     # to 'input_blocks.10.0.in_layers.2.weight'
     def convert_var_name(s: str, prefix="variable_transpose_"):
         s = removeprefix(s, prefix)
         s = re.sub(r"_[0-9]+$", "", s)
         s = removeprefix(s, "model.")
         return s
@@ -182,12 +182,13 @@
     if constant_folding_info is None:
         return
 
     logger.info(f"state_dict updated, modify the related weight in graph")
     update_graph_with_constant_folding_info(module, constant_folding_info)
     setattr(module._torch_module, STATE_UPDATED_ATTR, False)
 
+
 def removesuffix(s: str, suffix: str) -> str:
     if s.endswith(suffix):
-        return s[:len(s) - len(suffix)]
+        return s[: len(s) - len(suffix)]
     else:
         return s
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/patch_for_compiler.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,17 +105,21 @@
 F.scaled_dot_product_attention = FakeCuda.scaled_dot_product_attention
 
 flow.cuda.memory_stats = torch.cuda.memory_stats
 flow.version = torch.version
 
 from oneflow import Tensor
 
+
 def oneflow_rfloordiv():
-    original_rfloordiv = Tensor.__rfloordiv__ 
+    original_rfloordiv = Tensor.__rfloordiv__
+
     def rfloordiv(self, other):
         if isinstance(other, int):
             other = flow.tensor(other)
-            
+
         return original_rfloordiv(self, other)
+
     return rfloordiv
 
-Tensor.__rfloordiv__ = oneflow_rfloordiv()
+
+Tensor.__rfloordiv__ = oneflow_rfloordiv()
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/patch_for_diffusers.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # TODO: remove this file to diffusers/src/infer_compiler_registry/register_diffusers
 from abc import ABC, abstractmethod
-from .log_utils import logger
+from onediff.utils import logger
 
 try:
     import diffusers
     from diffusers.models.attention_processor import Attention
 except ImportError:
     diffusers = None
     logger.warning("diffusers not found, some features will be disabled.")
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/infer_compiler/utils/version_util.py` & `onediff-1.1.0.dev202405220128/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from importlib_metadata import version
-from .log_utils import logger
+from onediff.utils import logger
 
 
 def get_support_message():
     message = f""" OneDiff Enterprise Edition features can't be used, please refer to here for help: https://github.com/siliconflow/onediff?tab=readme-ov-file#community--support """
     return message
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/optimization/attention_processor.py` & `onediff-1.1.0.dev202405220128/src/onediff/optimization/attention_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             key = attn.head_to_batch_dim(key)
             value = attn.head_to_batch_dim(value)
 
             attention_probs = attn.get_attention_scores(query, key, attention_mask)
             hidden_states = flow.bmm(attention_probs, value)
             hidden_states = attn.batch_to_head_dim(hidden_states)
         else:
-            from ..infer_compiler.utils import (
+            from onediff.utils import (
                 parse_boolean_from_env,
                 set_boolean_env_var,
             )
 
             if attn.upcast_attention and parse_boolean_from_env(
                 "ONEFLOW_ATTENTION_ALLOW_HALF_PRECISION_ACCUMULATION", True
             ):
@@ -119,17 +119,17 @@
 
         hidden_states = hidden_states / attn.rescale_output_factor
 
         return hidden_states
 
 
 try:
-    from onediff.infer_compiler.transform import register
+    from onediff.infer_compiler.backends.oneflow.transform import register
 
     def convert_fused_self_attn_processor(
         mod: FusedSelfAttnProcessor, verbose=True
     ) -> FusedSelfAttnProcessor:
         return mod
 
     register(torch2oflow_funcs=convert_fused_self_attn_processor)
 except:
-    print("Skip onediff.infer_compiler.transform.register")
+    print("Skip onediff.infer_compiler.backends.oneflow.transform.register")
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/optimization/quant_optimizer.py` & `onediff-1.1.0.dev202405220128/src/onediff/optimization/quant_optimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import time
 import torch
 import torch.nn as nn
 from copy import deepcopy
-from ..infer_compiler.utils.log_utils import logger
-from ..infer_compiler.utils.version_util import is_quantization_enabled
-from ..infer_compiler.utils.cost_util import cost_cnt
-from ..infer_compiler.utils.module_operations import modify_sub_module
-from ..infer_compiler.transform.manager import transform_mgr
+from onediff.utils import logger
+from onediff.infer_compiler.backends.oneflow.utils.version_util import is_quantization_enabled
+from onediff.infer_compiler.backends.oneflow.utils.cost_util import cost_cnt
+from onediff.infer_compiler.backends.oneflow.transform.manager import transform_mgr
+from onediff.torch_utils.module_operations import modify_sub_module
 
 
 __all__ = ["quantize_model", "varify_can_use_quantization"]
 
 
 def varify_can_use_quantization():
     if not is_quantization_enabled():
@@ -103,8 +103,7 @@
         f"Quantized model {type(model)} successfully! \n"
         + f"Quantized conv: {quantize_conv_cnt} \n"
         + f"Quantized linear: {quantize_linear_cnt} \n"
         + f"Time: {time.time() - start_time:.4f}s \n"
     )
 
     return model
-
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/optimization/rewrite_self_attention.py` & `onediff-1.1.0.dev202405220128/src/onediff/optimization/rewrite_self_attention.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/quantization/load_quantized_model.py` & `onediff-1.1.0.dev202405220128/src/onediff/quantization/load_quantized_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 from diffusers import AutoPipelineForText2Image
 from onediff.quantization.quantize_pipeline import QuantPipeline
-import argparse 
+import argparse
 import torch
 from onediff.infer_compiler import oneflow_compile
 
+
 def parse_args():
     parser = argparse.ArgumentParser()
-    parser.add_argument("--prompt", default="a photo of an astronaut riding a horse on mars")
-    parser.add_argument("--height", type= int,default=1024)
-    parser.add_argument("--width", type= int, default=1024)
+    parser.add_argument(
+        "--prompt", default="a photo of an astronaut riding a horse on mars"
+    )
+    parser.add_argument("--height", type=int, default=1024)
+    parser.add_argument("--width", type=int, default=1024)
     parser.add_argument("--num_inference_steps", type=int, default=30)
     parser.add_argument("--quantized_model", type=str, required=True)
     return parser.parse_args()
 
+
 args = parse_args()
 
 pipe = QuantPipeline.from_quantized(
-    AutoPipelineForText2Image, args.quantized_model, torch_dtype=torch.float16, variant="fp16", use_safetensors=True
+    AutoPipelineForText2Image,
+    args.quantized_model,
+    torch_dtype=torch.float16,
+    variant="fp16",
+    use_safetensors=True,
 )
 pipe = pipe.to("cuda")
 
 pipe_kwargs = dict(
     prompt=args.prompt,
     height=args.height,
     width=args.width,
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/quantization/quant_pipeline_test.py` & `onediff-1.1.0.dev202405220128/src/onediff/quantization/quant_pipeline_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 from diffusers import AutoPipelineForText2Image
 from onediff.quantization.quantize_pipeline import QuantPipeline
 import torch
-import argparse 
+import argparse
 
 
 def parse_args():
     parser = argparse.ArgumentParser()
-    parser.add_argument("--floatting_model_path", default="runwayml/stable-diffusion-v1-5")
-    parser.add_argument("--prompt", default="a photo of an astronaut riding a horse on mars")
-    parser.add_argument("--height",type=int, default=1024)
-    parser.add_argument("--width", type=int,default=1024)
+    parser.add_argument(
+        "--floatting_model_path", default="runwayml/stable-diffusion-v1-5"
+    )
+    parser.add_argument(
+        "--prompt", default="a photo of an astronaut riding a horse on mars"
+    )
+    parser.add_argument("--height", type=int, default=1024)
+    parser.add_argument("--width", type=int, default=1024)
     parser.add_argument("--num_inference_steps", type=int, default=30)
     parser.add_argument("--conv_compute_density_threshold", type=int, default=900)
     parser.add_argument("--linear_compute_density_threshold", type=int, default=300)
     parser.add_argument("--conv_ssim_threshold", type=float, default=0.985)
     parser.add_argument("--linear_ssim_threshold", type=float, default=0.991)
     parser.add_argument("--save_as_float", type=bool, default=False)
     parser.add_argument("--cache_dir", default="./run_sd-v1-5")
     parser.add_argument("--quantized_model", default="./quantized_model")
     return parser.parse_args()
 
+
 args = parse_args()
 
 pipe = QuantPipeline.from_pretrained(
-    AutoPipelineForText2Image, args.floatting_model_path, torch_dtype=torch.float16, variant="fp16", use_safetensors=True
+    AutoPipelineForText2Image,
+    args.floatting_model_path,
+    torch_dtype=torch.float16,
+    variant="fp16",
+    use_safetensors=True,
 )
 pipe.to("cuda")
 
 pipe_kwargs = dict(
     prompt=args.prompt,
     height=args.height,
     width=args.width,
     num_inference_steps=args.num_inference_steps,
 )
 
-pipe.quantize(**pipe_kwargs,
+pipe.quantize(
+    **pipe_kwargs,
     conv_compute_density_threshold=args.conv_compute_density_threshold,
     linear_compute_density_threshold=args.linear_compute_density_threshold,
     conv_ssim_threshold=args.conv_ssim_threshold,
     linear_ssim_threshold=args.linear_ssim_threshold,
     save_as_float=args.save_as_float,
     plot_calibrate_info=False,
-    cache_dir=args.cache_dir)
+    cache_dir=args.cache_dir
+)
 
 pipe.save_quantized(args.quantized_model, safe_serialization=True)
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/quantization/quantize_pipeline.py` & `onediff-1.1.0.dev202405220128/src/onediff/quantization/quantize_pipeline.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405210127/src/onediff/quantization/quantize_utils.py` & `onediff-1.1.0.dev202405220128/src/onediff/quantization/quantize_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 def load_calibration_and_quantize_pipeline(calibration_path, pipe):
     from onediff_quant.quantization import CalibrationStorage
     from onediff_quant.utils import replace_sub_module_with_quantizable_module
 
     store = CalibrationStorage()
     calibrate_info = store.load_from_file(file_path=calibration_path)
-    
+
     for sub_module_name, sub_calibrate_info in calibrate_info.items():
         replace_sub_module_with_quantizable_module(
             pipe.unet,
             sub_module_name,
             sub_calibrate_info,
             fake_quant=False,
             static=False,
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff.egg-info/PKG-INFO` & `onediff-1.1.0.dev202405220128/src/onediff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.1.0.dev202405210127
+Version: 1.1.0.dev202405220128
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405210127 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405220128 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 contact@siliconflow.com License: Apache-2.0 Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `onediff-1.1.0.dev202405210127/src/onediff.egg-info/SOURCES.txt` & `onediff-1.1.0.dev202405220128/src/onediff.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -16,60 +16,60 @@
 src/onediff.egg-info/PKG-INFO
 src/onediff.egg-info/SOURCES.txt
 src/onediff.egg-info/dependency_links.txt
 src/onediff.egg-info/requires.txt
 src/onediff.egg-info/top_level.txt
 src/onediff/infer_compiler/__init__.py
 src/onediff/infer_compiler/backends/__init__.py
-src/onediff/infer_compiler/backends/nexfort.py
-src/onediff/infer_compiler/backends/oneflow.py
+src/onediff/infer_compiler/backends/compiler.py
+src/onediff/infer_compiler/backends/deployable_module.py
+src/onediff/infer_compiler/backends/options.py
 src/onediff/infer_compiler/backends/registry.py
-src/onediff/infer_compiler/core/__init__.py
-src/onediff/infer_compiler/core/deployable_module.py
-src/onediff/infer_compiler/core/with_onediff_compile.py
-src/onediff/infer_compiler/import_tools/__init__.py
-src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
-src/onediff/infer_compiler/import_tools/format_utils.py
-src/onediff/infer_compiler/import_tools/import_module_utils.py
-src/onediff/infer_compiler/import_tools/importer.py
-src/onediff/infer_compiler/nexfort/__init__.py
-src/onediff/infer_compiler/nexfort/deployable_module.py
-src/onediff/infer_compiler/oneflow/__init__.py
-src/onediff/infer_compiler/oneflow/config.py
-src/onediff/infer_compiler/oneflow/deployable_module.py
-src/onediff/infer_compiler/oneflow/dual_module.py
-src/onediff/infer_compiler/oneflow/graph.py
-src/onediff/infer_compiler/oneflow/utils.py
-src/onediff/infer_compiler/transform/__init__.py
-src/onediff/infer_compiler/transform/builtin_transform.py
-src/onediff/infer_compiler/transform/custom_transform.py
-src/onediff/infer_compiler/transform/manager.py
-src/onediff/infer_compiler/transform/patch_for_comfy.py
-src/onediff/infer_compiler/utils/__init__.py
-src/onediff/infer_compiler/utils/args_tree_util.py
-src/onediff/infer_compiler/utils/cost_util.py
-src/onediff/infer_compiler/utils/env_var.py
-src/onediff/infer_compiler/utils/graph_management_utils.py
-src/onediff/infer_compiler/utils/log_utils.py
-src/onediff/infer_compiler/utils/model_inplace_assign.py
-src/onediff/infer_compiler/utils/module_operations.py
-src/onediff/infer_compiler/utils/oneflow_exec_mode.py
-src/onediff/infer_compiler/utils/online_quantization_utils.py
-src/onediff/infer_compiler/utils/options.py
-src/onediff/infer_compiler/utils/param_utils.py
-src/onediff/infer_compiler/utils/patch_for_compiler.py
-src/onediff/infer_compiler/utils/patch_for_diffusers.py
-src/onediff/infer_compiler/utils/version_util.py
+src/onediff/infer_compiler/backends/nexfort/__init__.py
+src/onediff/infer_compiler/backends/nexfort/deployable_module.py
+src/onediff/infer_compiler/backends/nexfort/nexfort.py
+src/onediff/infer_compiler/backends/oneflow/__init__.py
+src/onediff/infer_compiler/backends/oneflow/args_tree_util.py
+src/onediff/infer_compiler/backends/oneflow/deployable_module.py
+src/onediff/infer_compiler/backends/oneflow/dual_module.py
+src/onediff/infer_compiler/backends/oneflow/env_var.py
+src/onediff/infer_compiler/backends/oneflow/graph.py
+src/onediff/infer_compiler/backends/oneflow/graph_management_utils.py
+src/onediff/infer_compiler/backends/oneflow/oneflow.py
+src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py
+src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py
+src/onediff/infer_compiler/backends/oneflow/param_utils.py
+src/onediff/infer_compiler/backends/oneflow/import_tools/__init__.py
+src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py
+src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py
+src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py
+src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py
+src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py
+src/onediff/infer_compiler/backends/oneflow/transform/__init__.py
+src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py
+src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py
+src/onediff/infer_compiler/backends/oneflow/transform/manager.py
+src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py
+src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py
+src/onediff/infer_compiler/backends/oneflow/utils/__init__.py
+src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py
+src/onediff/infer_compiler/backends/oneflow/utils/version_util.py
 src/onediff/optimization/__init__.py
 src/onediff/optimization/attention_processor.py
 src/onediff/optimization/quant_optimizer.py
 src/onediff/optimization/rewrite_self_attention.py
 src/onediff/quantization/__init__.py
 src/onediff/quantization/load_quantized_model.py
 src/onediff/quantization/quant_pipeline_test.py
 src/onediff/quantization/quantize_pipeline.py
 src/onediff/quantization/quantize_utils.py
 src/onediff/schedulers/__init__.py
+src/onediff/torch_utils/__init__.py
+src/onediff/torch_utils/model_inplace_assign.py
+src/onediff/torch_utils/module_operations.py
+src/onediff/utils/__init__.py
+src/onediff/utils/env_var.py
+src/onediff/utils/log_utils.py
 tests/test_dual_module_list.py
 tests/test_pipelines_oneflow_img2img.py
 tests/test_quantitative_quality.py
 tests/test_quantize_custom_model.py
```

### Comparing `onediff-1.1.0.dev202405210127/tests/test_dual_module_list.py` & `onediff-1.1.0.dev202405220128/tests/test_dual_module_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from onediff.infer_compiler import oneflow_compile
-from onediff.infer_compiler.transform import register
+from onediff.infer_compiler.backends.oneflow.transform import register
 import torch
 import torch.nn as nn
 import oneflow as flow
 
 
 class MyModule(nn.Module):
     def __init__(self):
@@ -35,15 +35,15 @@
 y_torch = m(x)
 
 m = oneflow_compile(m)
 y_oneflow = m(x)
 
 assert np.allclose(y_torch.detach().cpu(), y_oneflow.detach().cpu(), 1e-03, 1e-03)
 
-from onediff.infer_compiler.oneflow.dual_module import DualModule, DualModuleList
+from onediff.infer_compiler.backends.oneflow.dual_module import DualModule, DualModuleList
 
 assert isinstance(m.linears, DualModuleList)
 
 x = getattr(m.linears, "1")
 assert isinstance(x, DualModule)
 
 x.bias = None
```

### Comparing `onediff-1.1.0.dev202405210127/tests/test_pipelines_oneflow_img2img.py` & `onediff-1.1.0.dev202405220128/tests/test_pipelines_oneflow_img2img.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405210127/tests/test_quantitative_quality.py` & `onediff-1.1.0.dev202405220128/tests/test_quantitative_quality.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405210127/tests/test_quantize_custom_model.py` & `onediff-1.1.0.dev202405220128/tests/test_quantize_custom_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import unittest
 
 import oneflow as flow
 import torch
 from torch import nn
 
 from onediff.infer_compiler import oneflow_compile
-from onediff.infer_compiler.transform import register
-from onediff.infer_compiler.utils import is_community_version
+from onediff.infer_compiler.backends.oneflow.transform import register
+from onediff.infer_compiler.backends.oneflow.utils.version_util import is_community_version
 
 is_community = is_community_version()
 onediff_quant_spec = importlib.util.find_spec("onediff_quant")
 if is_community or onediff_quant_spec is None:
     print(f"{is_community=} {onediff_quant_spec=}")
     exit(0)
```

